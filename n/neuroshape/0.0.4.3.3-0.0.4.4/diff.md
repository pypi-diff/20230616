# Comparing `tmp/neuroshape-0.0.4.3.3.tar.gz` & `tmp/neuroshape-0.0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.3.3.tar", last modified: Thu Jun 15 23:37:26 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.4.tar", last modified: Fri Jun 16 04:11:28 2023, max compression
```

## Comparing `neuroshape-0.0.4.3.3.tar` & `neuroshape-0.0.4.4.tar`

### file list

```diff
@@ -1,67 +1,63 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.224042 neuroshape-0.0.4.3.3/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.3.3/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-15 23:37:26.223693 neuroshape-0.0.4.3.3/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.3/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.207004 neuroshape-0.0.4.3.3/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.3.3/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/eigenmaps.py
--rw-r--r--   0 nik        (502) admin       (80)    22956 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.208404 neuroshape-0.0.4.3.3/neuroshape/nipype/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nipype/__init__.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.208595 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/__init__.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.209080 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/workbench/
--rw-r--r--   0 nik        (502) admin       (80)      269 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/workbench/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    13219 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/workbench/metric.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.211675 neuroshape-0.0.4.3.3/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    11949 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/spins.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.213503 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     4890 2023-06-13 05:36:45.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/eigenmode_replication.py
--rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 nik        (502) admin       (80)     4119 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)     5155 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/poly_eigenmaps.py
--rw-r--r--   0 nik        (502) admin       (80)    13885 2023-06-14 05:13:56.000000 neuroshape-0.0.4.3.3/neuroshape/recon.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/stats.py
--rw-r--r--   0 nik        (502) admin       (80)    11313 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/surface_eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.218494 neuroshape-0.0.4.3.3/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)    12044 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/utils/fetch_atlas.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)    30218 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/utils/normalize_data.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/zscore_avg_method.py
--rw-r--r--   0 nik        (502) admin       (80)     9467 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/volume_eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.208111 neuroshape-0.0.4.3.3/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-15 23:37:26.000000 neuroshape-0.0.4.3.3/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1672 2023-06-15 23:37:26.000000 neuroshape-0.0.4.3.3/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-15 23:37:26.000000 neuroshape-0.0.4.3.3/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-15 23:37:26.000000 neuroshape-0.0.4.3.3/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)      620 2023-06-15 23:36:52.000000 neuroshape-0.0.4.3.3/pyproject.toml
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-15 23:37:26.224138 neuroshape-0.0.4.3.3/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1048 2023-06-15 23:37:23.000000 neuroshape-0.0.4.3.3/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.219465 neuroshape-0.0.4.3.3/src/
--rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.3.3/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.3.3/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.3.3/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.338609 neuroshape-0.0.4.4/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.4/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-16 04:11:28.338269 neuroshape-0.0.4.4/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.4/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.227810 neuroshape-0.0.4.4/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.4/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)    22975 2023-06-16 04:08:55.000000 neuroshape-0.0.4.4/neuroshape/eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.229283 neuroshape-0.0.4.4/neuroshape/nipype/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nipype/__init__.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.229505 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/__init__.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.230006 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/workbench/
+-rw-r--r--   0 nik        (502) admin       (80)      269 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/workbench/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    13219 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/workbench/metric.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.248498 neuroshape-0.0.4.4/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.4/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.4/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    11949 2023-06-15 23:21:48.000000 neuroshape-0.0.4.4/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/spins.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.284392 neuroshape-0.0.4.4/neuroshape/nulls/tests/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     4890 2023-06-13 05:36:45.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 nik        (502) admin       (80)     4119 2023-06-15 23:21:48.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)    13885 2023-06-14 05:13:56.000000 neuroshape-0.0.4.4/neuroshape/recon.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/stats.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.289305 neuroshape-0.0.4.4/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.4/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)    12044 2023-06-15 23:21:48.000000 neuroshape-0.0.4.4/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.4/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)    30218 2023-06-16 03:21:06.000000 neuroshape-0.0.4.4/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.4/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/zscore_avg_method.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.228984 neuroshape-0.0.4.4/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-16 04:11:28.000000 neuroshape-0.0.4.4/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1554 2023-06-16 04:11:28.000000 neuroshape-0.0.4.4/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-16 04:11:28.000000 neuroshape-0.0.4.4/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-16 04:11:28.000000 neuroshape-0.0.4.4/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)      618 2023-06-16 04:11:22.000000 neuroshape-0.0.4.4/pyproject.toml
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-16 04:11:28.338698 neuroshape-0.0.4.4/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1046 2023-06-16 04:11:08.000000 neuroshape-0.0.4.4/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.317860 neuroshape-0.0.4.4/src/
+-rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.4/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.4/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.4/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.3.3/LICENSE` & `neuroshape-0.0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/README.rst` & `neuroshape-0.0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.4/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/eigenmodes.py` & `neuroshape-0.0.4.4/neuroshape/utils/fs_shapeDNA.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,32 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Calculate the Laplace-Beltrami operator of a surface
-
-     - Generates a surface if a volume nifti is given, uses Gmsh subroutines
-     - Calculates the LBO and returns a number of modes
-     
-     NOTE: use case for both T1 brain and native surface is shown in documentation
+#!/usr/bin/env python
+# -*- coding: latin-1 -*-
 
-@author: Nikitas C. Koussis, Systems Neuroscience Group Newcastle, 2023, based
-on fs_shapeDNA.py by Martin Reuter.
-"""
+#
+# fs_shapeDNA
+#
+# script to compute ShapeDNA of FreeSurfer structures
+#
+# Original Author: Martin Reuter
+# Date: Dec-16-2014
+#
 
-import nibabel as nib
-import numpy as np
-from argparse import ArgumentParser
-from neuroshape.utils.fetch_atlas import fetch_atlas
-from os.path import splitext
-from lapy import TriaMesh, TriaIO, Solver
-from neuroshape.utils.geometry import (
-    normalize_vtk,
-    make_tetra_file,
-    get_tkrvox2ras,
-    mri_mc,    
-    read_geometry,
-    read_label,
-    )
-import optparse
-import sys
+import warnings
 import os
+import sys
+import shlex
+import optparse
+import subprocess
 import tempfile
-import warnings
+import uuid
 import errno
 
 warnings.filterwarnings('ignore', '.*negative int.*')
 os.environ['OMP_NUM_THREADS'] = '1' # setenv OMP_NUM_THREADS 1
 
-image_types = [
-    '.nii',
-    '.nii.gz',
-    '.gii',
-    '.pial',
-    ]
-
-norm_types = [
-    'area',
-    'constant',
-    'number',
-    'volume',   
-    ]
-
-"""
-Description
------------
-Wraps the Laplace-Beltrami Operator as implemented in ShapeDNA, see:
-    https://en.wikipedia.org/wiki/Laplace%E2%80%93Beltrami_operator
-    and:
-    http://reuter.mit.edu/software/shapedna/
-    
-Runs the Laplace-Beltrami calculation in parallel (as implemented in
-.__call__() and ._call_method()) and outputs an np.ndarray of size (n,J,N) 
-of "eigenmodes" for J=200 as in Koussis et al. and where N is the number
-of vertices and n is the number of files given as input to `x`.
-
-Dependencies
-------------
-    'nibabel', 
-    'lapy', 
-    'nilearn', 
-    'numpy', 
-    'scipy', 
-    'scikit-sparse',
-    'neuromaps', 
-    'nipype'
-    
-"""
-
 def my_print(message):
     """
     print message, then flush stdout
     """
     print(message)
     sys.stdout.flush()
 
@@ -97,22 +44,47 @@
 --label   : a label file to cut out a surface patch (also pass --surf)
 --aparcid : an aparc id to cut out that cortical ROI (also pass --surf)
 
 If "meshfix" and "gmsh" are in the path, and shapeDNA-tetra is available
 in the $SHAPEDNA_HOME directory, it can also create and process
 tetrahedral meshes from closed surfaces, such as lh.white ( --dotet ).
 
+Note both FreeSurfer needs to be sourced and the environment variable
+$SHAPEDNA_HOME needs to be set to point to the shapeDNA executables
+and key file.
+
 REFERENCES
 ==========
 
+Always cite [1] as it describes the method. If you use topological
+features of eigenfunctions, also cite [2]. [3] compares different
+discretizations of Laplace-Beltrami operators and shows that the
+used FEM appraoch performs best. If you do statistical shape analysis
+you may also want to cite [4] as it discusses medical applications.
+
 [1] M. Reuter, F.-E. Wolter and N. Peinecke.
 Laplace-Beltrami spectra as "Shape-DNA" of surfaces and solids.
 Computer-Aided Design 38 (4), pp.342-366, 2006.
 http://dx.doi.org/10.1016/j.cad.2005.10.011
 
+[2] M. Reuter. Hierarchical Shape Segmentation and Registration
+via Topological Features of Laplace-Beltrami Eigenfunctions.
+International Journal of Computer Vision, 2009.
+http://dx.doi.org/10.1007/s11263-009-0278-1
+
+[3] M. Reuter, S. Biasotti, D. Giorgi, G. Patane, M. Spagnuolo.
+Discrete Laplace-Beltrami operators for shape analysis and
+segmentation. Computers & Graphics 33 (3), pp.381-390, 2009.
+http://dx.doi.org/10.1016/j.cag.2009.03.005
+
+[4] M. Reuter, F.-E. Wolter, M. Shenton, M. Niethammer.
+Laplace-Beltrami Eigenvalues and Topological Features of
+Eigenfunctions for Statistical Shape Analysis.
+Computer-Aided Design 41 (10), pp.739-755, 2009.
+http://dx.doi.org/10.1016/j.cad.2009.02.007
 """
 
 TMPTXT="""
 REQUIRED ARGUMENTS
 
 --sid <name>      Subject ID
 
@@ -151,21 +123,21 @@
 --ignorelq        Ignore low quality in input mesh
 
 --sparam "<str>"  Additional parameters for shapeDNA-tria
 """
 
 def split_callback(option, opt, value, parser):
   setattr(parser.values, option.dest, value.split(','))
-  
+
 def options_parse():
     """
     Command Line Options Parser:
     initiate the option parser and return the parsed object
     """
-    parser = optparse.OptionParser(version='$Id: eigenmodes, N Koussis $', usage=HELPTEXT)
+    parser = optparse.OptionParser(version='$Id: fs_shapeDNA,v 1.21 2013/05/17 15:14:08 mreuter Exp $', usage=HELPTEXT)
     
     # help text
     h_sid       = '(REQUIRED) subject ID (FS processed directory inside the subjects directory)'
     h_sdir      = 'FS subjects directory (or set environment $SUBJECTS_DIR)'
     
     h_asegid    = 'segmentation ID of structure in aseg.mgz (e.g. 17 is Left-Hippocampus), for ID\'s check <sid>/stats/aseg.stats or $FREESURFER_HOME/FreeSurferColorLUT.txt'
     h_surf      = 'surface name, e.g. lh.pial, rh.pial, lh.white, rh.white etc. to select a surface from the <sid>/surfs directory'
@@ -230,33 +202,65 @@
     group.add_option('--tsmooth',  dest='tsmooth',  help=h_tsmooth,  default=0,  type='int')   
     group.add_option('--gsmooth',  dest='gsmooth',  help=h_gsmooth,  default=0,  type='int')   
     group.add_option('--param2d',  dest='param2d',  help=h_param2d)
     parser.add_option_group(group)
     
                       
     (options, args) = parser.parse_args()
-    
+    #if len(args) == 0:
+    #    parser.print_help()
+    #    my_print('\n')
+    #    sys.exit(1)
+                
+    # WITHOUT FREESURFER DO NOTHING
+    fshome = os.getenv('FREESURFER_HOME')
+    if fshome is None:
+        parser.print_help()
+        my_print('\nERROR: Environment variable FREESURFER_HOME not set. \n')
+        my_print('       Make sure to source your FreeSurfer installation.\n')
+        sys.exit(1)
+
+    sdnahome = os.getenv('SHAPEDNA_HOME')
+    if sdnahome is None:
+        parser.print_help()
+        my_print('\nERROR: Environment variable SHAPEDNA_HOME not set.\n')
+        my_print('       Set SHAPEDNA_HOME to point to the shapeDNA-tria installation.\n')
+        sys.exit(1)
+
+    sdna = os.path.join(sdnahome,"shapeDNA-tria")
+    if not os.path.exists(sdna) and not options.dotet:
+        parser.print_help()
+        my_print('\nERROR: Cannot find shapeDNA-tria\n')
+        my_print('       Make sure that binary is at $SHAPEDNA_HOME \n')
+        sys.exit(1)
+
+    if which("shapeDNA-tetra") is None and options.dotet:
+        parser.print_help()
+        my_print('\nERROR: Cannot find shapeDNA-tetra\n')
+        my_print('       Make sure that binary is at $SHAPEDNA_HOME \n')
+        sys.exit(1)
+
     if options.sdir is None:
         options.sdir = os.getenv('SUBJECTS_DIR')
-        
+
     if options.sdir is None:
         parser.print_help()
         my_print('\nERROR: specify subjects directory via --sdir or $SUBJECTS_DIR\n')
         sys.exit(1)
         
     if options.sid is None:
         parser.print_help()
         my_print('\nERROR: Specify --sid\n')
         sys.exit(1)
-        
+            
     subjdir = os.path.join(options.sdir,options.sid)
     if not os.path.exists(subjdir):
         my_print('ERROR: cannot find sid in subjects directory\n')
         sys.exit(1)
-        
+    
     if options.label is not None and options.surf is None:
         parser.print_help()
         my_print('\nERROR: Specify --surf with --label\n')
         sys.exit(1)  
     if options.aparcid is not None and options.surf is None:
         parser.print_help()
         my_print('\nERROR: Specify --surf with --aparc\n')
@@ -270,15 +274,15 @@
     if options.asegid is not None and options.surf is not None:
         parser.print_help()
         my_print('\nERROR: Specify either --asegid or --surf (not both)\n')
         sys.exit(1)  
     
     # set default output dir (maybe this should be ./ ??)
     if options.outdir is None:
-        options.outdir = os.path.join(subjdir,'neuroshape')
+        options.outdir = os.path.join(subjdir,'brainprint')
     try:
         os.mkdir(options.outdir)
     except OSError as e:
         if e.errno != os.errno.EEXIST:
             raise e
         pass
 
@@ -336,258 +340,308 @@
             parser.print_help()
             my_print('\nERROR: Specified --label not found\n')
             sys.exit(1)  
                 
     # initialize outev 
     if options.outev is None:
         if options.dotet:
-            options.outev = options.outtet+'.txt'
+            options.outev = options.outtet+'.ev'
         else:
-            options.outev = options.outsurf+'.txt'
+            options.outev = options.outsurf+'.ev'
         
     return options
 
+def which(program):
+    def is_exe(fpath):
+        return os.path.isfile(fpath) and os.access(fpath, os.X_OK)
+
+    fpath, fname = os.path.split(program)
+    if fpath:
+        if is_exe(program):
+            return program
+    else:
+        for path in os.environ["PATH"].split(os.pathsep):
+            path = path.strip('"')
+            exe_file = os.path.join(path, program)
+            if is_exe(exe_file):
+                return exe_file
+        if is_exe(os.path.join(os.getenv('SHAPEDNA_HOME'),program)):
+            return os.path.join(os.getenv('SHAPEDNA_HOME'),program)
+        if is_exe(os.path.join('.',program)):
+            return os.path.join('.',program)
+
+    return None
+
+def run_cmd(cmd,err_msg):
+    """
+    execute the comand
+    """
+    clist = cmd.split()
+    progname=which(clist[0])
+    if (progname) is None:
+        my_print('ERROR: '+ clist[0] +' not found in path!')
+        sys.exit(1)
+    clist[0]=progname
+    cmd = ' '.join(clist)
+    my_print('#@# Command: ' + cmd+'\n')
+
+    args = shlex.split(cmd)
+    try:
+        subprocess.check_call(args)
+    except subprocess.CalledProcessError as e:
+        my_print('ERROR: '+err_msg)
+        #sys.exit(1)
+        raise
+    my_print('\n')
+
 # Gets global path to surface input (if it is a FS surf)
-def get_path_surf(sdir,sid,surf):
+def get_surf_surf(sdir,sid,surf):
     return os.path.join(sdir,sid,'surf',surf)
 
+
 # creates tria surface from label (and specified surface)
 # maps the label first if source is different from sid
-def make_surf(sdir,sid,surf,outdir):
+def get_label_surf(sdir,sid,label,surf,source,outsurf):
+    subjdir  = os.path.join(sdir,sid)
+    outdir   = os.path.dirname( outsurf )
+    stlsurf  = os.path.join(outdir,'label'+str(uuid.uuid4())+'.stl')
+
     # get hemi from surf
     splitsurf = surf.split(".",1)
     hemi = splitsurf[0]
     surf = splitsurf[1]
     # map label if necessary
-    coords, faces = read_geometry(get_path_surf(surf))
-    
-    outsurf = os.path.join(outdir, hemi, surf, '.vtk')
-    
-    # save tria mesh to outsurf
-    tria = TriaMesh(coords, faces)
-    
-    TriaIO.export_vtk(tria, outsurf)
-    
+    mappedlabel = label
+    if (source != sid):
+        mappedlabel = os.path.join(outdir,os.path.basename(label)+'.'+str(uuid.uuid4())+'.label')
+        cmd = 'mri_label2label --sd '+sdir+' --srclabel '+label+' --srcsubject '+ source+' --trgsubject '+sid+' --trglabel '+mappedlabel+' --hemi '+hemi+' --regmethod surface'
+        run_cmd(cmd,'mri_label2label failed?')     
+    # make surface path (make sure output is stl, this currently needs fsdev, will probably be in 6.0)
+    cmd = 'label2patch -writesurf -sdir '+sdir+' -surf '+ surf + ' ' +sid+' '+hemi+' '+mappedlabel+' '+stlsurf
+    run_cmd(cmd,'label2patch failed?')     
+    cmd = 'mris_convert '+stlsurf+' '+outsurf
+    run_cmd(cmd,'mris_convert failed.')
+    
+    # cleanup map label if necessary
+    if (source != sid):
+        cmd ='rm '+mappedlabel
+        run_cmd(cmd,'rm mapped label '+mappedlabel+' failed.')     
+    cmd = 'rm '+stlsurf
+    run_cmd(cmd,'rm stlsurf failed.')
     # return surf name
     return outsurf
 
-# creates tria surface from label (and specified surface)
-# maps the label first if source is different from sid
-# def get_label_surf(sdir,sid,label,surf,source,outsurf):
-#     subjdir  = os.path.join(sdir,sid)
-#     outdir   = os.path.dirname( outsurf )
-#     stlsurf  = os.path.join(outdir,'label'+str(uuid.uuid4())+'.stl')
-
-#     # get hemi from surf
-#     splitsurf = surf.split(".",1)
-#     hemi = splitsurf[0]
-#     surf = splitsurf[1]
-#     # map label if necessary
-#     mappedlabel = label
-#     if (source != sid):
-#         mappedlabel = os.path.join(outdir,os.path.basename(label)+'.'+str(uuid.uuid4())+'.label')
-#         cmd = 'mri_label2label --sd '+sdir+' --srclabel '+label+' --srcsubject '+ source+' --trgsubject '+sid+' --trglabel '+mappedlabel+' --hemi '+hemi+' --regmethod surface'
-#         run_cmd(cmd,'mri_label2label failed?')     
-#     # make surface path (make sure output is stl, this currently needs fsdev, will probably be in 6.0)
-#     cmd = 'label2patch -writesurf -sdir '+sdir+' -surf '+ surf + ' ' +sid+' '+hemi+' '+mappedlabel+' '+stlsurf
-#     run_cmd(cmd,'label2patch failed?')     
-#     cmd = 'mris_convert '+stlsurf+' '+outsurf
-#     run_cmd(cmd,'mris_convert failed.')
-    
-#     # cleanup map label if necessary
-#     if (source != sid):
-#         cmd ='rm '+mappedlabel
-#         run_cmd(cmd,'rm mapped label '+mappedlabel+' failed.')     
-#     cmd = 'rm '+stlsurf
-#     run_cmd(cmd,'rm stlsurf failed.')
-#     # return surf name
-#     return outsurf
 
 # Creates a surface from the aseg and label info
 # and writes it to the outdir
-# def get_aseg_surf(sdir,sid,asegid,outsurf):
-#     astring2 = ' '.join(asegid)
-#     subjdir  = os.path.join(sdir,sid)
-#     aseg     = os.path.join(subjdir,'mri','aseg.mgz')
-#     norm     = os.path.join(subjdir,'mri','norm.mgz')  
-#     outdir   = os.path.dirname( outsurf )    
-#     tmpname  = 'aseg.'+str(uuid.uuid4())
-#     segf     = os.path.join(outdir,tmpname+'.mgz')
-#     segsurf  = os.path.join(outdir,tmpname+'.surf')
-#     # binarize on selected labels (creates temp segf)
-#     ptinput = aseg
-#     ptlabel = str(asegid[0])
-#     #if len(asegid) > 1:
-#     # always binarize first, otherwise pretess may scale aseg if labels are larger than 255 (e.g. aseg+aparc, bug in mri_pretess?)
-#     cmd ='mri_binarize --i '+aseg+' --match '+astring2+' --o '+segf
-#     run_cmd(cmd,'mri_binarize failed.') 
-#     ptinput = segf
-#     ptlabel = '1'
-#     # if norm exist, fix label (pretess)
-#     if os.path.isfile(norm):
-#         cmd ='mri_pretess '+ptinput+' '+ptlabel+' '+norm+' '+segf
-#         run_cmd(cmd,'mri_pretess failed.') 
-#     else:
-#         if not os.path.isfile(segf):
-#             # cp segf if not exist yet
-#             # (it exists already if we combined labels above)
-#             cmd = 'cp '+ptinput+' '+segf
-#             run_cmd(cmd,'cp segmentation file failed.') 
-#     # runs marching cube to extract surface
-#     cmd ='mri_mc '+segf+' '+ptlabel+' '+segsurf
-#     run_cmd(cmd,'mri_mc failed?') 
-#     # convert to stl
-#     cmd ='mris_convert '+segsurf+' '+outsurf
-#     run_cmd(cmd,'mris_convert failed.')
-#     # cleanup temp files
-#     cmd ='rm '+segf
-#     run_cmd(cmd,'rm temp segf failed.') 
-#     cmd ='rm '+segsurf
-#     run_cmd(cmd,'rm temp segsurf failed.') 
-#     # return surf name
-#     return outsurf
-
-# # Creates a surface from the aparc and label number
-# # and writes it to the outdir
-# def get_aparc_surf(sdir,sid,surf,aparcid,outsurf):
-#     astring2 = ' '.join(aparcid)
-#     subjdir  = os.path.join(sdir,sid)
-#     outdir   = os.path.dirname( outsurf )    
-#     rndname = str(uuid.uuid4()) 
-#     # get hemi from surf
-#     hemi = surf.split(".",1)[0]
-#     # convert annotation id to label:
-#     alllabels = ''
-#     for aid in aparcid:
-#         # create label of this id
-#         outlabelpre = os.path.join(outdir,hemi+'.aparc.'+rndname)
-#         cmd = 'mri_annotation2label --sd '+sdir+' --subject '+sid+' --hemi '+hemi+' --label '+str(aid)+' --labelbase '+outlabelpre 
-#         run_cmd(cmd,'mri_annotation2label failed?') 
-#         alllabels = alllabels+'-i '+outlabelpre+"-%03d.label" % int(aid)+' ' 
-#     # merge labels (if more than 1)
-#     mergedlabel = outlabelpre+"-%03d.label" % int(aid)
-#     if len(aparcid) > 1:
-#         mergedlabel = os.path.join(outdir,hemi+'.aparc.all.'+rndname+'.label')
-#         cmd = 'mri_mergelabels '+alllabels+' -o '+mergedlabel
-#         run_cmd(cmd,'mri_mergelabels failed?') 
-#     # make to surface (call subfunction above)
-#     get_label_surf(sdir,sid,mergedlabel,surf,sid,outsurf)
-#     # cleanup
-#     if len(aparcid) > 1:
-#         cmd ='rm '+mergedlabel
-#         run_cmd(cmd,'rm '+mergedlabel+' failed?')
-#     for aid in aparcid:
-#         outlabelpre = os.path.join(outdir,hemi+'.aparc.'+rndname+"-%03d.label" % int(aid))
-#         cmd ='rm '+outlabelpre
-#         run_cmd(cmd,'rm '+outlabelpre+' failed?')
-#     # return surf name
-#     return outsurf
-
-# def get_tetmesh(surf,outtet,fixiter):
-#     surfbase  = os.path.basename(surf)
-#     outdir    = os.path.dirname( outtet )    
-#     surftemp_stl = os.path.join(outdir,surfbase+'.temp.stl')
-    
-#     # massage surface mesh (rm handles, 60000 vertices, uniform)
-#     cmd='mris_convert '+surf+' '+surftemp_stl
-#     run_cmd(cmd,'mris_convert (to STLs) failed')
-# #    cmd='meshfix '+surftemp_stl+' -a 2.0 --remove-handles -q --stl -o '+surftemp_stl
-# #    run_cmd(cmd,'meshfix (remove-handles) failed, is it in your path?') 
-#     cmd='meshfix '+surftemp_stl+' -a 2.0 -u 5 --vertices 60000 -q --stl -o '+surftemp_stl
-#     run_cmd(cmd,'meshfix (downsample) failed?') 
-#     for num in range(0,fixiter):
-#         cmd='meshfix '+surftemp_stl+' -a 2.0 -u 1 -q --stl -o '+surftemp_stl
-#         run_cmd(cmd,'meshfix failed ('+str(num)+'a)?')      
-#         cmd='meshfix '+surftemp_stl+' -a 2.0 -q --stl -o '+surftemp_stl
-#         run_cmd(cmd,'meshfix failed ('+str(num)+'b)?') 
+def get_aseg_surf(sdir,sid,asegid,outsurf):
+    astring2 = ' '.join(asegid)
+    subjdir  = os.path.join(sdir,sid)
+    aseg     = os.path.join(subjdir,'mri','aseg.mgz')
+    norm     = os.path.join(subjdir,'mri','norm.mgz')  
+    outdir   = os.path.dirname( outsurf )    
+    tmpname  = 'aseg.'+str(uuid.uuid4())
+    segf     = os.path.join(outdir,tmpname+'.mgz')
+    segsurf  = os.path.join(outdir,tmpname+'.surf')
+    # binarize on selected labels (creates temp segf)
+    ptinput = aseg
+    ptlabel = str(asegid[0])
+    #if len(asegid) > 1:
+    # always binarize first, otherwise pretess may scale aseg if labels are larger than 255 (e.g. aseg+aparc, bug in mri_pretess?)
+    cmd ='mri_binarize --i '+aseg+' --match '+astring2+' --o '+segf
+    run_cmd(cmd,'mri_binarize failed.') 
+    ptinput = segf
+    ptlabel = '1'
+    # if norm exist, fix label (pretess)
+    if os.path.isfile(norm):
+        cmd ='mri_pretess '+ptinput+' '+ptlabel+' '+norm+' '+segf
+        run_cmd(cmd,'mri_pretess failed.') 
+    else:
+        if not os.path.isfile(segf):
+            # cp segf if not exist yet
+            # (it exists already if we combined labels above)
+            cmd = 'cp '+ptinput+' '+segf
+            run_cmd(cmd,'cp segmentation file failed.') 
+    # runs marching cube to extract surface
+    cmd ='mri_mc '+segf+' '+ptlabel+' '+segsurf
+    run_cmd(cmd,'mri_mc failed?') 
+    # convert to stl
+    cmd ='mris_convert '+segsurf+' '+outsurf
+    run_cmd(cmd,'mris_convert failed.')
+    # cleanup temp files
+    cmd ='rm '+segf
+    run_cmd(cmd,'rm temp segf failed.') 
+    cmd ='rm '+segsurf
+    run_cmd(cmd,'rm temp segsurf failed.') 
+    # return surf name
+    return outsurf
+
+
+# Creates a surface from the aparc and label number
+# and writes it to the outdir
+def get_aparc_surf(sdir,sid,surf,aparcid,outsurf):
+    astring2 = ' '.join(aparcid)
+    subjdir  = os.path.join(sdir,sid)
+    outdir   = os.path.dirname( outsurf )    
+    rndname = str(uuid.uuid4()) 
+    # get hemi from surf
+    hemi = surf.split(".",1)[0]
+    # convert annotation id to label:
+    alllabels = ''
+    for aid in aparcid:
+        # create label of this id
+        outlabelpre = os.path.join(outdir,hemi+'.aparc.'+rndname)
+        cmd = 'mri_annotation2label --sd '+sdir+' --subject '+sid+' --hemi '+hemi+' --label '+str(aid)+' --labelbase '+outlabelpre 
+        run_cmd(cmd,'mri_annotation2label failed?') 
+        alllabels = alllabels+'-i '+outlabelpre+"-%03d.label" % int(aid)+' ' 
+    # merge labels (if more than 1)
+    mergedlabel = outlabelpre+"-%03d.label" % int(aid)
+    if len(aparcid) > 1:
+        mergedlabel = os.path.join(outdir,hemi+'.aparc.all.'+rndname+'.label')
+        cmd = 'mri_mergelabels '+alllabels+' -o '+mergedlabel
+        run_cmd(cmd,'mri_mergelabels failed?') 
+    # make to surface (call subfunction above)
+    get_label_surf(sdir,sid,mergedlabel,surf,sid,outsurf)
+    # cleanup
+    if len(aparcid) > 1:
+        cmd ='rm '+mergedlabel
+        run_cmd(cmd,'rm '+mergedlabel+' failed?')
+    for aid in aparcid:
+        outlabelpre = os.path.join(outdir,hemi+'.aparc.'+rndname+"-%03d.label" % int(aid))
+        cmd ='rm '+outlabelpre
+        run_cmd(cmd,'rm '+outlabelpre+' failed?')
+    # return surf name
+    return outsurf
+
+def get_tetmesh(surf,outtet,fixiter):
+    surfbase  = os.path.basename(surf)
+    outdir    = os.path.dirname( outtet )    
+    surftemp_stl = os.path.join(outdir,surfbase+'.temp.stl')
+    
+    # massage surface mesh (rm handles, 60000 vertices, uniform)
+    cmd='mris_convert '+surf+' '+surftemp_stl
+    run_cmd(cmd,'mris_convert (to STLs) failed')
+#    cmd='meshfix '+surftemp_stl+' -a 2.0 --remove-handles -q --stl -o '+surftemp_stl
+#    run_cmd(cmd,'meshfix (remove-handles) failed, is it in your path?') 
+    cmd='meshfix '+surftemp_stl+' -a 2.0 -u 5 --vertices 60000 -q --stl -o '+surftemp_stl
+    run_cmd(cmd,'meshfix (downsample) failed?') 
+    for num in range(0,fixiter):
+        cmd='meshfix '+surftemp_stl+' -a 2.0 -u 1 -q --stl -o '+surftemp_stl
+        run_cmd(cmd,'meshfix failed ('+str(num)+'a)?')      
+        cmd='meshfix '+surftemp_stl+' -a 2.0 -q --stl -o '+surftemp_stl
+        run_cmd(cmd,'meshfix failed ('+str(num)+'b)?') 
         
-# # replacing meshfix never worked:
-# #    sdnahome = os.getenv('SHAPEDNA_HOME')
-# #    triaio = os.path.join(sdnahome,"triaIO")  
-# #    cmd=triaio+' --infile '+surf+' --outfile '+surftemp_stl' --contractedges --remeshbk 1'
-# #    run_cmd(cmd,'triaIO remeshing failed?')
+# replacing meshfix never worked:
+#    sdnahome = os.getenv('SHAPEDNA_HOME')
+#    triaio = os.path.join(sdnahome,"triaIO")  
+#    cmd=triaio+' --infile '+surf+' --outfile '+surftemp_stl' --contractedges --remeshbk 1'
+#    run_cmd(cmd,'triaIO remeshing failed?')
       
-#     # write gmsh geofile
-#     geofile  = os.path.join(outdir,'gmsh.'+str(uuid.uuid4())+'.geo')
-#     g = open(geofile, 'w')
-#     g.write("Mesh.Algorithm3D=4;\n")
-#     g.write("Mesh.Optimize=1;\n")
-#     g.write("Mesh.OptimizeNetgen=1;\n")
-#     g.write("Merge \"" + surfbase+'.temp.stl' + "\";\n")
-#     g.write("Surface Loop(1) = {1};\n")
-#     g.write("Volume(1) = {1};\n")
-#     g.write("Physical Volume(1) = {1};\n")
-#     g.close()
-#     # use gmsh to create tet mesh
-#     cmd = 'gmsh -3 -o '+outtet+' '+geofile
-#     run_cmd(cmd,'gmsh failed, is it in your path?') 
-    
-#     # cleanup
-#     cmd ='rm '+geofile
-#     run_cmd(cmd,'rm temp geofile failed?') 
-#     cmd='rm '+surftemp_stl
-#     run_cmd(cmd,'rm temp stl surface failed?') 
-
-#     # return tetmesh filename
-#     return outtet
-
-# calculate the eigenmodes
-def eigenmodes(sdir, sid, surf, outev, outdir, num_modes):
-    fem = Solver(surf)
-    ev = fem(k=num_modes)
-    
-    evals = ev['Eigenvalues']
-    emodes = ev['Eigenvectors']
-    
-    # remove the medial wall
-    medial_wall = find_medial_wall(sdir, sid)
-    emodes[medial_wall] = np.nan
-    
-    outev = os.path.join(outdir, outev)
-    
-    np.savetxt(outev, emodes)
-
-# remove the medial wall
-def find_medial_wall(sdir, sid):
-    label = os.path.join(sdir, sid, 'label', 'lh.aparc.a2009s.annot')
-    labels = read_label(label)
+    # write gmsh geofile
+    geofile  = os.path.join(outdir,'gmsh.'+str(uuid.uuid4())+'.geo')
+    g = open(geofile, 'w')
+    g.write("Mesh.Algorithm3D=4;\n")
+    g.write("Mesh.Optimize=1;\n")
+    g.write("Mesh.OptimizeNetgen=1;\n")
+    g.write("Merge \"" + surfbase+'.temp.stl' + "\";\n")
+    g.write("Surface Loop(1) = {1};\n")
+    g.write("Volume(1) = {1};\n")
+    g.write("Physical Volume(1) = {1};\n")
+    g.close()
+    # use gmsh to create tet mesh
+    cmd = 'gmsh -3 -o '+outtet+' '+geofile
+    run_cmd(cmd,'gmsh failed, is it in your path?') 
+    
+    # cleanup
+    cmd ='rm '+geofile
+    run_cmd(cmd,'rm temp geofile failed?') 
+    cmd='rm '+surftemp_stl
+    run_cmd(cmd,'rm temp stl surface failed?') 
+
+    # return tetmesh filename
+    return outtet
+
+def run_shapeDNAtetra(tetmesh,outev,options):
+    sdnahome = os.getenv('SHAPEDNA_HOME')
+    sdna = os.path.join(sdnahome,"shapeDNA-tetra")
+    # mesh refine degree num bcond ouput ev
+    num = 50
+    if options.num is not None:       
+        num = options.num
+    degree = 1
+    if options.degree is not None:
+        degree = options.degree
+    dirichlet = ""
+    if options.bcond == 0:
+        dirichlet = " --dirichlet"
+    cmd =sdna+' --mesh '+tetmesh+' --num '+str(options.num)+' --outfile '+outev+' --degree '+str(options.degree)+dirichlet
+    if options.evec:
+        cmd = cmd+' --evec'
+    run_cmd(cmd,'shapeDNA-tetra failed?') 
+
+
+def run_shapeDNAtria(surf,outev,outsurf,options):
+ # options : num, degree, evec, ignorelq, refmin, tsmooth, gsmooth, param2d
+    sdnahome = os.getenv('SHAPEDNA_HOME')
+    sdna = os.path.join(sdnahome,"shapeDNA-tria") 
+    num = 50
+    if options.num is not None:       
+        num = options.num
+    degree = 1
+    if options.degree is not None:
+        degree = options.degree
+    dirichlet = ""
+    if options.bcond == 0:
+        dirichlet = " --dirichlet"
+    cmd =sdna+' --mesh '+surf+' --num '+str(options.num)+' --outfile '+outev+' --degree '+str(options.degree)+dirichlet
+    if options.evec:
+        cmd = cmd+' --evec'
+    if options.ignorelq:
+        cmd = cmd+' --ignorelq'
+    if options.refmin > 0:
+        cmd = cmd+' --refmin '+str(options.refmin)
+    if options.tsmooth > 0:
+        cmd = cmd+' --tsmooth '+str(options.tsmooth)
+    if options.gsmooth > 0:
+        cmd = cmd+' --gsmooth '+str(options.gsmooth)
+    if options.param2d is not None:
+        cmd = cmd+' '+options.param2d
+    if not outsurf == "":
+        cmd = cmd+' --outmesh '+outsurf
+    run_cmd(cmd,'shapeDNA-tria failed?') 
 
-    indices = np.where(labels==1644825) # fs medial wall labels
-    
-    return indices
 
 if __name__=="__main__":
     # Command Line options and error checking done here
     options = options_parse()
 
     my_print(options.label)
     my_print(options.surf)
 
-    # if options.asegid is not None:
-    #     surf = get_aseg_surf(options.sdir,options.sid,options.asegid,options.outsurf)
-    #     outsurf = surf
-    # elif options.label is not None:
-    #     surf = get_label_surf(options.sdir,options.sid,options.label,options.surf,options.source,options.outsurf)
-    #     outsurf = surf
-    # elif options.aparcid is not None:
-    #     surf = get_aparc_surf(options.sdir,options.sid,options.surf,options.aparcid,options.outsurf)    
-    #     outsurf = surf
-    if options.surf is not None:
-        surf = make_surf(options.sdir,options.sid,options.surf)
+    if options.asegid is not None:
+        surf = get_aseg_surf(options.sdir,options.sid,options.asegid,options.outsurf)
+        outsurf = surf
+    elif options.label is not None:
+        surf = get_label_surf(options.sdir,options.sid,options.label,options.surf,options.source,options.outsurf)
+        outsurf = surf
+    elif options.aparcid is not None:
+        surf = get_aparc_surf(options.sdir,options.sid,options.surf,options.aparcid,options.outsurf)    
+        outsurf = surf
+    elif options.surf is not None:
+        surf = get_surf_surf(options.sdir,options.sid,options.surf)
         outsurf = options.outsurf
     #my_print(surf)
     #sys.exit(0)
     if surf is None:
         my_print('ERROR: no surface was created/selected?')
         sys.exit(1)
 
-    # if options.dotet:
-    #     #convert to tetmesh
-    #     get_tetmesh(surf,options.outtet,options.fixiter)
-    #     #run shapedna tetra
-    #     calc_eigenmodes(options.outtet,options.outev,options)
-    
-    eigenmodes(options.sdir, options.sid, surf,options.outev,options.outdir, options.num)
+    if options.dotet:
+        #convert to tetmesh
+        get_tetmesh(surf,options.outtet,options.fixiter)
+        #run shapedna tetra
+        run_shapeDNAtetra(options.outtet,options.outev,options)
+    else:
+        run_shapeDNAtria(surf,options.outev,outsurf,options)
 
     # always exit with 0 exit code
     sys.exit(0)
-
```

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/workbench/metric.py` & `neuroshape-0.0.4.4/neuroshape/nipype/interfaces/workbench/metric.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.4/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.4/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.4/neuroshape/nulls/eigensphere.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.4/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.4/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/eigenmode_replication.py` & `neuroshape-0.0.4.4/neuroshape/nulls/tests/eigenmode_replication.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.4/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.4/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.4/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.4/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.4/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/permutation.py` & `neuroshape-0.0.4.4/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/recon.py` & `neuroshape-0.0.4.4/neuroshape/recon.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/stats.py` & `neuroshape-0.0.4.4/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.4/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.4/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/checks.py` & `neuroshape-0.0.4.4/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.4/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.4/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.4/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.4/neuroshape/utils/eigen.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/fetch_atlas.py` & `neuroshape-0.0.4.4/neuroshape/utils/fetch_atlas.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.4/neuroshape/eigenmodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,61 @@
-#!/usr/bin/env python
-# -*- coding: latin-1 -*-
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Calculate the Laplace-Beltrami operator of a surface
 
-#
-# fs_shapeDNA
-#
-# script to compute ShapeDNA of FreeSurfer structures
-#
-# Original Author: Martin Reuter
-# Date: Dec-16-2014
-#
+     - Generates a surface if a volume nifti is given, uses Gmsh subroutines
+     - Calculates the LBO and returns a number of modes
+     
+     NOTE: use case for both T1 brain and native surface is shown in documentation
 
-import warnings
-import os
-import sys
-import shlex
+@author: Nikitas C. Koussis, Systems Neuroscience Group Newcastle, 2023, based
+on fs_shapeDNA.py by Martin Reuter.
+"""
+
+import nibabel as nib
+import numpy as np
+from neuroshape.utils.fetch_atlas import fetch_atlas
+from os.path import splitext
+from lapy import TriaMesh, TriaIO, TetIO, TetMesh, Solver
+from neuroshape.utils.geometry import (
+    normalize_vtk,
+    make_tetra_file,
+    get_tkrvox2ras,
+    mri_mc,    
+    read_geometry,
+    read_annot,
+    )
 import optparse
-import subprocess
+import sys
+import os
 import tempfile
-import uuid
+import warnings
 import errno
+import subprocess
+import uuid
 
 warnings.filterwarnings('ignore', '.*negative int.*')
 os.environ['OMP_NUM_THREADS'] = '1' # setenv OMP_NUM_THREADS 1
 
-def my_print(message):
+image_types = [
+    '.nii',
+    '.nii.gz',
+    '.gii',
+    '.pial',
+    ]
+
+norm_types = [
+    'area',
+    'constant',
+    'number',
+    'volume',   
+    ]
+
+def m_print(message):
     """
     print message, then flush stdout
     """
     print(message)
     sys.stdout.flush()
 
 HELPTEXT = """
@@ -40,51 +68,25 @@
 
 Input can be one of the following:
 --asegid  : an aseg label id to construct a surface of that ROI
 --surf    : a surface, e.g. lh.white
 --label   : a label file to cut out a surface patch (also pass --surf)
 --aparcid : an aparc id to cut out that cortical ROI (also pass --surf)
 
-If "meshfix" and "gmsh" are in the path, and shapeDNA-tetra is available
-in the $SHAPEDNA_HOME directory, it can also create and process
+If "gmsh" is in the path, it can also create and process
 tetrahedral meshes from closed surfaces, such as lh.white ( --dotet ).
 
-Note both FreeSurfer needs to be sourced and the environment variable
-$SHAPEDNA_HOME needs to be set to point to the shapeDNA executables
-and key file.
-
 REFERENCES
 ==========
 
-Always cite [1] as it describes the method. If you use topological
-features of eigenfunctions, also cite [2]. [3] compares different
-discretizations of Laplace-Beltrami operators and shows that the
-used FEM appraoch performs best. If you do statistical shape analysis
-you may also want to cite [4] as it discusses medical applications.
-
 [1] M. Reuter, F.-E. Wolter and N. Peinecke.
 Laplace-Beltrami spectra as "Shape-DNA" of surfaces and solids.
 Computer-Aided Design 38 (4), pp.342-366, 2006.
 http://dx.doi.org/10.1016/j.cad.2005.10.011
 
-[2] M. Reuter. Hierarchical Shape Segmentation and Registration
-via Topological Features of Laplace-Beltrami Eigenfunctions.
-International Journal of Computer Vision, 2009.
-http://dx.doi.org/10.1007/s11263-009-0278-1
-
-[3] M. Reuter, S. Biasotti, D. Giorgi, G. Patane, M. Spagnuolo.
-Discrete Laplace-Beltrami operators for shape analysis and
-segmentation. Computers & Graphics 33 (3), pp.381-390, 2009.
-http://dx.doi.org/10.1016/j.cag.2009.03.005
-
-[4] M. Reuter, F.-E. Wolter, M. Shenton, M. Niethammer.
-Laplace-Beltrami Eigenvalues and Topological Features of
-Eigenfunctions for Statistical Shape Analysis.
-Computer-Aided Design 41 (10), pp.739-755, 2009.
-http://dx.doi.org/10.1016/j.cad.2009.02.007
 """
 
 TMPTXT="""
 REQUIRED ARGUMENTS
 
 --sid <name>      Subject ID
 
@@ -103,18 +105,24 @@
 --sdir <name>     Subjects directory (or set via environment $SUBJECTS_DIR)
 
 --outdir <name>   Output directory (default: <sdir>/<sid>/brainprint/ )
 
 --outsurf <name>  Name for surface output (with --asegid)
                   (default: aseg.<asegid>.surf )
 
---outev <name>    Name for eigenvalue output
-                  (default: <(out)surf>.<shapedna_parametrs>.ev )
+--outevec <name>    Name for eigenmodes output
+                  (default: <(out)surf>.<shapedna_parameters>.txt )
+                  
+--savegii <name>  Name for gifti output if input is surface
 
-ShapeDNA parameters (see shapeDNA-tria --help for details):
+--label <name>    Label to create surface patch if input is surface
+
+--savenii <name>  Name for nifti output (modes are projected to new volume in freesurfer space)
+
+ShapeDNA parameters (see shapeDNA --help for details):
 
 --num <int>       Number of eigenvalues/vectors to compute (default: 50)
 
 --degree <int>    FEM degree (default 1)
 
 --bcond <int>     Boundary condition (0=Dirichlet, 1=Neumann default)
 
@@ -123,21 +131,21 @@
 --ignorelq        Ignore low quality in input mesh
 
 --sparam "<str>"  Additional parameters for shapeDNA-tria
 """
 
 def split_callback(option, opt, value, parser):
   setattr(parser.values, option.dest, value.split(','))
-
+  
 def options_parse():
     """
     Command Line Options Parser:
     initiate the option parser and return the parsed object
     """
-    parser = optparse.OptionParser(version='$Id: fs_shapeDNA,v 1.21 2013/05/17 15:14:08 mreuter Exp $', usage=HELPTEXT)
+    parser = optparse.OptionParser(version='$Id: eigenmodes, N Koussis $', usage=HELPTEXT)
     
     # help text
     h_sid       = '(REQUIRED) subject ID (FS processed directory inside the subjects directory)'
     h_sdir      = 'FS subjects directory (or set environment $SUBJECTS_DIR)'
     
     h_asegid    = 'segmentation ID of structure in aseg.mgz (e.g. 17 is Left-Hippocampus), for ID\'s check <sid>/stats/aseg.stats or $FREESURFER_HOME/FreeSurferColorLUT.txt'
     h_surf      = 'surface name, e.g. lh.pial, rh.pial, lh.white, rh.white etc. to select a surface from the <sid>/surfs directory'
@@ -147,15 +155,15 @@
 
     h_dotet     = 'construct a tetrahedra volume mesh and compute spectra of solid'
     h_fixiter   = 'iterations of meshfix (default=4), only with --dotet'
     
     h_outdir    = 'Output directory (default: <sdir>/<sid>/brainprint/ )'
     h_outsurf   = 'Full path for surface output in VTK format (with --asegid default: <outdir>/aseg.<asegid>.vtk )'
     h_outtet    = 'Full path for tet output (with --dotet) (default: <outdir>/<(out)surf>.msh )'
-    h_outev     = 'Full path for eigenvalue output (default: <outdir>/<(out)surf or outtet>.ev )'
+    h_outevec     = 'Full path for eigenvalue output (default: <outdir>/<(out)surf or outtet>.ev )'
     
     h_num       = 'number of eigenvalues/vectors to compute (default: 50)'
     h_degree    = 'degree for FEM computation (1=linear default, 3=cubic)'
     h_bcond     = 'boundary condition (1=Neumann default, 0=Dirichlet )'
     h_evec      = 'bool to switch on eigenvector computation'
     h_ignorelq  = 'ignore low quality in input mesh'
     h_refmin    = 'mesh refinement so that DOF is at least <int>'
@@ -184,15 +192,15 @@
     parser.add_option_group(group)
 
     #output switches
     group = optparse.OptionGroup(parser, "Output Parameters" )
     group.add_option('--outdir',  dest='outdir',   help=h_outdir)
     group.add_option('--outsurf', dest='outsurf',  help=h_outsurf)
     group.add_option('--outtet',  dest='outtet',   help=h_outtet)
-    group.add_option('--outev',   dest='outev',    help=h_outev)
+    group.add_option('--outevec',   dest='outevec',    help=h_outevec)
     parser.add_option_group(group)
 
     #shapedna switches
     group = optparse.OptionGroup(parser, "ShapeDNA Parameters","See shapeDNA-tria --help for details")
     group.add_option('--num' ,     dest='num',      help=h_num,      default=50, type='int')
     group.add_option('--degree' ,  dest='degree',   help=h_degree,   default=1,  type='int')
     group.add_option('--bcond' ,   dest='bcond',    help=h_bcond,    default=1,  type='int')
@@ -202,87 +210,55 @@
     group.add_option('--tsmooth',  dest='tsmooth',  help=h_tsmooth,  default=0,  type='int')   
     group.add_option('--gsmooth',  dest='gsmooth',  help=h_gsmooth,  default=0,  type='int')   
     group.add_option('--param2d',  dest='param2d',  help=h_param2d)
     parser.add_option_group(group)
     
                       
     (options, args) = parser.parse_args()
-    #if len(args) == 0:
-    #    parser.print_help()
-    #    my_print('\n')
-    #    sys.exit(1)
-                
-    # WITHOUT FREESURFER DO NOTHING
-    fshome = os.getenv('FREESURFER_HOME')
-    if fshome is None:
-        parser.print_help()
-        my_print('\nERROR: Environment variable FREESURFER_HOME not set. \n')
-        my_print('       Make sure to source your FreeSurfer installation.\n')
-        sys.exit(1)
-
-    sdnahome = os.getenv('SHAPEDNA_HOME')
-    if sdnahome is None:
-        parser.print_help()
-        my_print('\nERROR: Environment variable SHAPEDNA_HOME not set.\n')
-        my_print('       Set SHAPEDNA_HOME to point to the shapeDNA-tria installation.\n')
-        sys.exit(1)
-
-    sdna = os.path.join(sdnahome,"shapeDNA-tria")
-    if not os.path.exists(sdna) and not options.dotet:
-        parser.print_help()
-        my_print('\nERROR: Cannot find shapeDNA-tria\n')
-        my_print('       Make sure that binary is at $SHAPEDNA_HOME \n')
-        sys.exit(1)
-
-    if which("shapeDNA-tetra") is None and options.dotet:
-        parser.print_help()
-        my_print('\nERROR: Cannot find shapeDNA-tetra\n')
-        my_print('       Make sure that binary is at $SHAPEDNA_HOME \n')
-        sys.exit(1)
-
+    
     if options.sdir is None:
         options.sdir = os.getenv('SUBJECTS_DIR')
-
+        
     if options.sdir is None:
         parser.print_help()
-        my_print('\nERROR: specify subjects directory via --sdir or $SUBJECTS_DIR\n')
+        m_print('\nERROR: specify subjects directory via --sdir or $SUBJECTS_DIR\n')
         sys.exit(1)
         
     if options.sid is None:
         parser.print_help()
-        my_print('\nERROR: Specify --sid\n')
+        m_print('\nERROR: Specify --sid\n')
         sys.exit(1)
-            
-    subjdir = os.path.join(options.sdir,options.sid)
+        
+    subjdir = os.path.join(options.sdir, options.sid)
     if not os.path.exists(subjdir):
-        my_print('ERROR: cannot find sid in subjects directory\n')
+        m_print('ERROR: cannot find sid in subjects directory\n')
         sys.exit(1)
-    
+        
     if options.label is not None and options.surf is None:
         parser.print_help()
-        my_print('\nERROR: Specify --surf with --label\n')
+        m_print('\nERROR: Specify --surf with --label\n')
         sys.exit(1)  
     if options.aparcid is not None and options.surf is None:
         parser.print_help()
-        my_print('\nERROR: Specify --surf with --aparc\n')
+        m_print('\nERROR: Specify --surf with --aparc\n')
         sys.exit(1)  
     # input needs to be either a surf or aseg label(s)
     if options.asegid is None and options.surf is None:
         parser.print_help()
-        my_print('\nERROR: Specify either --asegid or --surf\n')
+        m_print('\nERROR: Specify either --asegid or --surf\n')
         sys.exit(1)
     # and it cannot be both
     if options.asegid is not None and options.surf is not None:
         parser.print_help()
-        my_print('\nERROR: Specify either --asegid or --surf (not both)\n')
+        m_print('\nERROR: Specify either --asegid or --surf (not both)\n')
         sys.exit(1)  
     
     # set default output dir (maybe this should be ./ ??)
     if options.outdir is None:
-        options.outdir = os.path.join(subjdir,'brainprint')
+        options.outdir = os.path.join(subjdir, 'eigenmodes')
     try:
         os.mkdir(options.outdir)
     except OSError as e:
         if e.errno != os.errno.EEXIST:
             raise e
         pass
 
@@ -290,358 +266,360 @@
     try:
         testfile = tempfile.TemporaryFile(dir = options.outdir)
         testfile.close()
     except OSError as e:
         if e.errno != errno.EACCES:  # 13
             e.filename = options.outdir
             raise
-        my_print('\nERROR: '+options.outdir+' not writeable (check access)!\n')
+        m_print('\nERROR: '+options.outdir+' not writeable (check access)!\n')
         sys.exit(1)
     
     # initialize outsurf
     if options.outsurf is None:
         # for aseg stuff, we need to create a surface (and we'll keep it around)
         if options.asegid is not None:
             astring  = '_'.join(options.asegid)
             #surfname = 'aseg.'+astring+'.surf'
-            surfname = 'aseg.'+astring+'.vtk'
+            surfname = 'aseg.' + astring + '.vtk'
             options.outsurf = os.path.join(options.outdir,surfname)    
         elif options.label is not None:
-            surfname = os.path.basename(options.surf)+'.'+os.path.basename(options.label)+'.vtk'
-            options.outsurf = os.path.join(options.outdir,surfname)
+            surfname = os.path.basename(options.surf) + '.' + os.path.basename(options.label) + '.vtk'
+            options.outsurf = os.path.join(options.outdir, surfname)
         elif options.aparcid is not None:
             astring  = '_'.join(options.aparcid)
-            surfname = os.path.basename(options.surf)+'.aparc.'+astring+'.vtk'
-            options.outsurf = os.path.join(options.outdir,surfname)          
+            surfname = os.path.basename(options.surf) + '.aparc.' + astring + '.vtk'
+            options.outsurf = os.path.join(options.outdir, surfname)          
         else:
             # for surfaces, a refined/smoothed version could be written
-            surfname = os.path.basename(options.surf)+'.vtk'
-            options.outsurf = os.path.join(options.outdir,surfname)
+            surfname = os.path.basename(options.surf) +' .vtk'
+            options.outsurf = os.path.join(options.outdir, surfname)
     else:
         # make sure it is vtk ending
         if (os.path.splitext(options.outsurf)[1]).upper() != '.VTK':
-            my_print('ERROR: outsurf needs vtk extension (VTK format)')
+            m_print('ERROR: outsurf needs vtk extension (VTK format)')
             sys.exit(1)
     
     # for 3d processing, initialize outtet:
     if options.dotet and options.outtet is None:
         surfname = os.path.basename(options.outsurf)
-        options.outtet = os.path.join(options.outdir,surfname+'.msh')    
+        options.outtet = os.path.join(options.outdir, surfname+ '.msh')    
     
     # set source to sid if empty
     if options.source is None:
         options.source = options.sid
         
     # if label does not exist, search in subject label dir
     if options.label is not None and not os.path.isfile(options.label):
-        ltemp = os.path.join(options.sdir,options.source,'label',options.label)
+        ltemp = os.path.join(options.sdir, options.source, 'label', options.label)
         if os.path.isfile(ltemp):
             options.label = ltemp
         else:
             parser.print_help()
-            my_print('\nERROR: Specified --label not found\n')
+            m_print('\nERROR: Specified --label not found\n')
             sys.exit(1)  
                 
-    # initialize outev 
-    if options.outev is None:
+    # initialize outevec 
+    if options.outevec is None:
         if options.dotet:
-            options.outev = options.outtet+'.ev'
+            options.outevec = options.outtet + '.txt'
         else:
-            options.outev = options.outsurf+'.ev'
+            options.outevec = options.outsurf + '.txt'
         
     return options
 
-def which(program):
-    def is_exe(fpath):
-        return os.path.isfile(fpath) and os.access(fpath, os.X_OK)
-
-    fpath, fname = os.path.split(program)
-    if fpath:
-        if is_exe(program):
-            return program
-    else:
-        for path in os.environ["PATH"].split(os.pathsep):
-            path = path.strip('"')
-            exe_file = os.path.join(path, program)
-            if is_exe(exe_file):
-                return exe_file
-        if is_exe(os.path.join(os.getenv('SHAPEDNA_HOME'),program)):
-            return os.path.join(os.getenv('SHAPEDNA_HOME'),program)
-        if is_exe(os.path.join('.',program)):
-            return os.path.join('.',program)
-
-    return None
-
-def run_cmd(cmd,err_msg):
-    """
-    execute the comand
-    """
-    clist = cmd.split()
-    progname=which(clist[0])
-    if (progname) is None:
-        my_print('ERROR: '+ clist[0] +' not found in path!')
-        sys.exit(1)
-    clist[0]=progname
-    cmd = ' '.join(clist)
-    my_print('#@# Command: ' + cmd+'\n')
-
-    args = shlex.split(cmd)
-    try:
-        subprocess.check_call(args)
-    except subprocess.CalledProcessError as e:
-        my_print('ERROR: '+err_msg)
-        #sys.exit(1)
-        raise
-    my_print('\n')
-
 # Gets global path to surface input (if it is a FS surf)
-def get_surf_surf(sdir,sid,surf):
-    return os.path.join(sdir,sid,'surf',surf)
+def get_path_surf(sdir, sid, surf):
+    return os.path.join(sdir, sid, 'surf', surf)
+
+def make_surf(sdir, sid, surf, outdir, outsurf=None):
+    """
+    creates surface from freesurfer
+    """    
+    coords, faces = read_geometry(get_path_surf(sdir, sid, surf))
+    
+    # get hemi from surf
+    splitsurf = surf.split(".", 1)
+    hemi = splitsurf[0]
+    surf = splitsurf[1]
+    
+    if outsurf is None: # base case
+        outsurf = os.path.join(outdir, hemi + '.' + surf + '.vtk')
+    
+    # save tria mesh to outsurf
+    tria = TriaMesh(coords, faces)
+    TriaIO.export_vtk(tria, outsurf)
+    
+    # return surf name
+    return outsurf
 
 
-# creates tria surface from label (and specified surface)
-# maps the label first if source is different from sid
-def get_label_surf(sdir,sid,label,surf,source,outsurf):
-    subjdir  = os.path.join(sdir,sid)
-    outdir   = os.path.dirname( outsurf )
-    stlsurf  = os.path.join(outdir,'label'+str(uuid.uuid4())+'.stl')
+def get_label_surf(sdir, sid, label, surf, source, outsurf):
+    """
+    creates tria surface from label (and specified surface)
+    maps the label first if source is different from sid
+    """
+    subjdir  = os.path.join(sdir, sid)
+    outdir   = os.path.dirname(outsurf)
+    stlsurf  = os.path.join(outdir, 'label' + str(uuid.uuid4()) + '.stl')
 
     # get hemi from surf
     splitsurf = surf.split(".",1)
     hemi = splitsurf[0]
     surf = splitsurf[1]
     # map label if necessary
     mappedlabel = label
     if (source != sid):
-        mappedlabel = os.path.join(outdir,os.path.basename(label)+'.'+str(uuid.uuid4())+'.label')
-        cmd = 'mri_label2label --sd '+sdir+' --srclabel '+label+' --srcsubject '+ source+' --trgsubject '+sid+' --trglabel '+mappedlabel+' --hemi '+hemi+' --regmethod surface'
-        run_cmd(cmd,'mri_label2label failed?')     
+        mappedlabel = os.path.join(outdir, os.path.basename(label) + '.' + str(uuid.uuid4()) + '.label')
+        cmd = 'mri_label2label --sd ' + sdir + ' --srclabel ' + label + ' --srcsubject ' + source + ' --trgsubject ' + sid + ' --trglabel ' + mappedlabel + ' --hemi ' + hemi + ' --regmethod surface'
+        subprocess.run(cmd)     
     # make surface path (make sure output is stl, this currently needs fsdev, will probably be in 6.0)
-    cmd = 'label2patch -writesurf -sdir '+sdir+' -surf '+ surf + ' ' +sid+' '+hemi+' '+mappedlabel+' '+stlsurf
-    run_cmd(cmd,'label2patch failed?')     
-    cmd = 'mris_convert '+stlsurf+' '+outsurf
-    run_cmd(cmd,'mris_convert failed.')
+    cmd = 'label2patch -writesurf -sdir ' + sdir + ' -surf ' + surf + ' ' + sid + ' ' + hemi + ' ' + mappedlabel + ' ' + stlsurf
+    subprocess.run(cmd)     
+    cmd = 'mris_convert ' + stlsurf + ' ' + outsurf
+    subprocess.run(cmd)
     
     # cleanup map label if necessary
     if (source != sid):
-        cmd ='rm '+mappedlabel
-        run_cmd(cmd,'rm mapped label '+mappedlabel+' failed.')     
-    cmd = 'rm '+stlsurf
-    run_cmd(cmd,'rm stlsurf failed.')
+        cmd ='rm ' + mappedlabel
+        subprocess.run(cmd)     
+    cmd = 'rm ' + stlsurf
+    subprocess.run(cmd)
+    
+    # make and write surface
+    outsurf = make_surf(sdir, sid, surf, outdir, outsurf)
+    
     # return surf name
     return outsurf
 
 
-# Creates a surface from the aseg and label info
-# and writes it to the outdir
-def get_aseg_surf(sdir,sid,asegid,outsurf):
+def get_aseg_surf(sdir, sid, asegid, outsurf):
+    """
+    Creates a surface from the aseg and label info
+    and writes it to the outdir
+    """
     astring2 = ' '.join(asegid)
-    subjdir  = os.path.join(sdir,sid)
-    aseg     = os.path.join(subjdir,'mri','aseg.mgz')
-    norm     = os.path.join(subjdir,'mri','norm.mgz')  
-    outdir   = os.path.dirname( outsurf )    
-    tmpname  = 'aseg.'+str(uuid.uuid4())
-    segf     = os.path.join(outdir,tmpname+'.mgz')
-    segsurf  = os.path.join(outdir,tmpname+'.surf')
+    subjdir  = os.path.join(sdir, sid)
+    aseg     = os.path.join(subjdir, 'mri', 'aseg.mgz')
+    norm     = os.path.join(subjdir, 'mri', 'norm.mgz')  
+    outdir   = os.path.dirname(outsurf)    
+    tmpname  = 'aseg.' + str(uuid.uuid4())
+    segf     = os.path.join(outdir, tmpname + '.mgz')
+    segsurf  = os.path.join(outdir, tmpname + '.vtk')
     # binarize on selected labels (creates temp segf)
     ptinput = aseg
     ptlabel = str(asegid[0])
     #if len(asegid) > 1:
     # always binarize first, otherwise pretess may scale aseg if labels are larger than 255 (e.g. aseg+aparc, bug in mri_pretess?)
-    cmd ='mri_binarize --i '+aseg+' --match '+astring2+' --o '+segf
-    run_cmd(cmd,'mri_binarize failed.') 
+    cmd ='mri_binarize --i ' + aseg + ' --match ' + astring2 + ' --o ' + segf
+    subprocess.run(cmd) 
     ptinput = segf
     ptlabel = '1'
     # if norm exist, fix label (pretess)
     if os.path.isfile(norm):
-        cmd ='mri_pretess '+ptinput+' '+ptlabel+' '+norm+' '+segf
-        run_cmd(cmd,'mri_pretess failed.') 
+        cmd ='mri_pretess ' + ptinput + ' ' + ptlabel + ' ' + norm + ' ' + segf
+        subprocess.run(cmd) 
     else:
         if not os.path.isfile(segf):
             # cp segf if not exist yet
             # (it exists already if we combined labels above)
-            cmd = 'cp '+ptinput+' '+segf
-            run_cmd(cmd,'cp segmentation file failed.') 
+            cmd = 'cp ' + ptinput + ' ' + segf
+            subprocess.run(cmd) 
     # runs marching cube to extract surface
-    cmd ='mri_mc '+segf+' '+ptlabel+' '+segsurf
-    run_cmd(cmd,'mri_mc failed?') 
+    cmd ='mri_mc ' + segf + ' ' + ptlabel + ' ' + segsurf
+    subprocess.run(cmd) 
     # convert to stl
-    cmd ='mris_convert '+segsurf+' '+outsurf
-    run_cmd(cmd,'mris_convert failed.')
+    cmd ='mris_convert ' + segsurf + ' ' + outsurf
+    subprocess.run(cmd)
     # cleanup temp files
-    cmd ='rm '+segf
-    run_cmd(cmd,'rm temp segf failed.') 
-    cmd ='rm '+segsurf
-    run_cmd(cmd,'rm temp segsurf failed.') 
+    cmd ='rm ' + segf
+    subprocess.run(cmd) 
+    cmd ='rm ' + segsurf
+    subprocess.run(cmd)
+    
+    
     # return surf name
     return outsurf
 
 
-# Creates a surface from the aparc and label number
-# and writes it to the outdir
-def get_aparc_surf(sdir,sid,surf,aparcid,outsurf):
+def get_aparc_surf(sdir, sid, surf, aparcid, outsurf):
+    """
+    Creates a surface from the aparc and label number
+    and writes it to the outdir
+    """
     astring2 = ' '.join(aparcid)
-    subjdir  = os.path.join(sdir,sid)
-    outdir   = os.path.dirname( outsurf )    
+    subjdir  = os.path.join(sdir, sid)
+    outdir   = os.path.dirname(outsurf)    
     rndname = str(uuid.uuid4()) 
     # get hemi from surf
-    hemi = surf.split(".",1)[0]
+    hemi = surf.split(".", 1)[0]
     # convert annotation id to label:
     alllabels = ''
     for aid in aparcid:
         # create label of this id
-        outlabelpre = os.path.join(outdir,hemi+'.aparc.'+rndname)
-        cmd = 'mri_annotation2label --sd '+sdir+' --subject '+sid+' --hemi '+hemi+' --label '+str(aid)+' --labelbase '+outlabelpre 
-        run_cmd(cmd,'mri_annotation2label failed?') 
-        alllabels = alllabels+'-i '+outlabelpre+"-%03d.label" % int(aid)+' ' 
+        outlabelpre = os.path.join(outdir, hemi + '.aparc.' + rndname)
+        cmd = 'mri_annotation2label --sd ' + sdir + ' --subject ' + sid + ' --hemi ' + hemi + ' --label ' + str(aid) + ' --labelbase ' + outlabelpre 
+        subprocess.run(cmd) 
+        alllabels = alllabels + '-i ' + outlabelpre + "-%03d.label" % int(aid) + ' ' 
     # merge labels (if more than 1)
-    mergedlabel = outlabelpre+"-%03d.label" % int(aid)
+    mergedlabel = outlabelpre + "-%03d.label" % int(aid)
     if len(aparcid) > 1:
-        mergedlabel = os.path.join(outdir,hemi+'.aparc.all.'+rndname+'.label')
-        cmd = 'mri_mergelabels '+alllabels+' -o '+mergedlabel
-        run_cmd(cmd,'mri_mergelabels failed?') 
+        mergedlabel = os.path.join(outdir, hemi + '.aparc.all.' + rndname + '.label')
+        cmd = 'mri_mergelabels ' + alllabels + ' -o ' + mergedlabel
+        subprocess.run(cmd) 
     # make to surface (call subfunction above)
-    get_label_surf(sdir,sid,mergedlabel,surf,sid,outsurf)
+    get_label_surf(sdir, sid, mergedlabel, surf, sid, outsurf)
     # cleanup
     if len(aparcid) > 1:
-        cmd ='rm '+mergedlabel
-        run_cmd(cmd,'rm '+mergedlabel+' failed?')
+        cmd ='rm ' + mergedlabel
+        subprocess.run(cmd)
     for aid in aparcid:
-        outlabelpre = os.path.join(outdir,hemi+'.aparc.'+rndname+"-%03d.label" % int(aid))
-        cmd ='rm '+outlabelpre
-        run_cmd(cmd,'rm '+outlabelpre+' failed?')
+        outlabelpre = os.path.join(outdir, hemi + '.aparc.' + rndname + "-%03d.label" % int(aid))
+        cmd ='rm ' + outlabelpre
+        subprocess.run(cmd)
     # return surf name
     return outsurf
 
-def get_tetmesh(surf,outtet,fixiter):
+def get_tetmesh(sdir, sid, surf, outtet, norm_type, norm_factor=1):
+    # TODO FIX nonfunctional for now 
     surfbase  = os.path.basename(surf)
-    outdir    = os.path.dirname( outtet )    
-    surftemp_stl = os.path.join(outdir,surfbase+'.temp.stl')
+    outdir    = os.path.dirname(outtet)    
+    surftemp_stl = os.path.join(outdir, surfbase + '.temp.stl')
     
-    # massage surface mesh (rm handles, 60000 vertices, uniform)
-    cmd='mris_convert '+surf+' '+surftemp_stl
-    run_cmd(cmd,'mris_convert (to STLs) failed')
-#    cmd='meshfix '+surftemp_stl+' -a 2.0 --remove-handles -q --stl -o '+surftemp_stl
-#    run_cmd(cmd,'meshfix (remove-handles) failed, is it in your path?') 
-    cmd='meshfix '+surftemp_stl+' -a 2.0 -u 5 --vertices 60000 -q --stl -o '+surftemp_stl
-    run_cmd(cmd,'meshfix (downsample) failed?') 
-    for num in range(0,fixiter):
-        cmd='meshfix '+surftemp_stl+' -a 2.0 -u 1 -q --stl -o '+surftemp_stl
-        run_cmd(cmd,'meshfix failed ('+str(num)+'a)?')      
-        cmd='meshfix '+surftemp_stl+' -a 2.0 -q --stl -o '+surftemp_stl
-        run_cmd(cmd,'meshfix failed ('+str(num)+'b)?') 
-        
-# replacing meshfix never worked:
-#    sdnahome = os.getenv('SHAPEDNA_HOME')
-#    triaio = os.path.join(sdnahome,"triaIO")  
-#    cmd=triaio+' --infile '+surf+' --outfile '+surftemp_stl' --contractedges --remeshbk 1'
-#    run_cmd(cmd,'triaIO remeshing failed?')
+    # make surface mesh
+    cmd = 'mris_convert ' + surf + ' ' + surftemp_stl
+    subprocess.run(cmd)
+    
+    # marching cubes
+    tria_file = 'tmp_surface.vtk'
+    cmd = 'mri_mc ' + surftemp_stl + ' 1 ' + outdir + '/' + tria_file
+    subprocess.run(cmd)
       
     # write gmsh geofile
     geofile  = os.path.join(outdir,'gmsh.'+str(uuid.uuid4())+'.geo')
-    g = open(geofile, 'w')
-    g.write("Mesh.Algorithm3D=4;\n")
-    g.write("Mesh.Optimize=1;\n")
-    g.write("Mesh.OptimizeNetgen=1;\n")
-    g.write("Merge \"" + surfbase+'.temp.stl' + "\";\n")
-    g.write("Surface Loop(1) = {1};\n")
-    g.write("Volume(1) = {1};\n")
-    g.write("Physical Volume(1) = {1};\n")
-    g.close()
+    
+    with open(geofile, 'w') as g:
+        g.write("Mesh.Algorithm3D=4;\n")
+        g.write("Mesh.Optimize=1;\n")
+        g.write("Mesh.OptimizeNetgen=1;\n")
+        g.write("Merge \""+surfbase+'.temp.stl'+"\";\n")
+        g.write("Surface Loop(1) = {1};\n")
+        g.write("Volume(1) = {1};\n")
+        g.write("Physical Volume(1) = {1};\n")
+        
     # use gmsh to create tet mesh
-    cmd = 'gmsh -3 -o '+outtet+' '+geofile
-    run_cmd(cmd,'gmsh failed, is it in your path?') 
+    cmd = 'gmsh -3 -o ' + outtet + ' ' + geofile
+    subprocess.run(cmd)
+    
+    cmd = "sed 's/double/float/g;s/UNSTRUCTURED_GRID/POLYDATA/g;s/CELLS/POLYGONS/g;/CELL_TYPES/,$d' " + outtet + " > " + outtet + "'_fixed'"
+    subprocess.run(cmd)
+    
+    # get volume and number of non-zero voxels in ROI
+    brainmask_path = os.path.join(sdir, sid, 'mri', 'brainmask.mgz')
+    
+    # normalize surface
+    tet = TetIO.import_gmsh(outtet)
+    tet_norm = tet
+    
+    
+    coords, faces = read_geometry(surf, read_metadata=True) # only want the faces
+    #number, volume = 
+    
+    # if norm_type == 'number':
+    #     tet_norm.v = tet.v/(number ** (1/3))
+    # elif norm_type == 'volume':
+    #     tet_norm.v = tet.v/(volume ** (1/3))
+    # elif norm_type == 'constant':
+    #     tet_norm.v = tet.v/(norm_factor ** (1/3))
+    
+    
     
     # cleanup
-    cmd ='rm '+geofile
-    run_cmd(cmd,'rm temp geofile failed?') 
-    cmd='rm '+surftemp_stl
-    run_cmd(cmd,'rm temp stl surface failed?') 
+    cmd ='rm ' + geofile
+    subprocess.run(cmd) 
+    cmd='rm ' + surftemp_stl
+    subprocess.run(cmd)
+    cmd = 'rm '+ '/tmp_surface.vtk'
+    subprocess.run(cmd)
 
     # return tetmesh filename
     return outtet
 
-def run_shapeDNAtetra(tetmesh,outev,options):
-    sdnahome = os.getenv('SHAPEDNA_HOME')
-    sdna = os.path.join(sdnahome,"shapeDNA-tetra")
-    # mesh refine degree num bcond ouput ev
-    num = 50
-    if options.num is not None:       
-        num = options.num
-    degree = 1
-    if options.degree is not None:
-        degree = options.degree
-    dirichlet = ""
-    if options.bcond == 0:
-        dirichlet = " --dirichlet"
-    cmd =sdna+' --mesh '+tetmesh+' --num '+str(options.num)+' --outfile '+outev+' --degree '+str(options.degree)+dirichlet
-    if options.evec:
-        cmd = cmd+' --evec'
-    run_cmd(cmd,'shapeDNA-tetra failed?') 
-
-
-def run_shapeDNAtria(surf,outev,outsurf,options):
- # options : num, degree, evec, ignorelq, refmin, tsmooth, gsmooth, param2d
-    sdnahome = os.getenv('SHAPEDNA_HOME')
-    sdna = os.path.join(sdnahome,"shapeDNA-tria") 
-    num = 50
-    if options.num is not None:       
-        num = options.num
-    degree = 1
-    if options.degree is not None:
-        degree = options.degree
-    dirichlet = ""
-    if options.bcond == 0:
-        dirichlet = " --dirichlet"
-    cmd =sdna+' --mesh '+surf+' --num '+str(options.num)+' --outfile '+outev+' --degree '+str(options.degree)+dirichlet
-    if options.evec:
-        cmd = cmd+' --evec'
-    if options.ignorelq:
-        cmd = cmd+' --ignorelq'
-    if options.refmin > 0:
-        cmd = cmd+' --refmin '+str(options.refmin)
-    if options.tsmooth > 0:
-        cmd = cmd+' --tsmooth '+str(options.tsmooth)
-    if options.gsmooth > 0:
-        cmd = cmd+' --gsmooth '+str(options.gsmooth)
-    if options.param2d is not None:
-        cmd = cmd+' '+options.param2d
-    if not outsurf == "":
-        cmd = cmd+' --outmesh '+outsurf
-    run_cmd(cmd,'shapeDNA-tria failed?') 
+def calc_eigenmodes(sdir, sid, surf_file, outdir, outevec=None, num_modes=2):
+    """
+    Calculate the eigenmodes of a mesh
+    """
+    # check if tet mesh
+    if '.msh' in surf_file:
+        surface = TriaIO.import_gmsh(surf_file)
+        ext = '.msh'
+        
+    else:
+        surface = TriaIO.import_vtk(surf_file)
+        ext = '.vtk'
+    
+    try:
+        import sksparse.cholmod
+        cholmod = True
+        print("Found scikit-sparse libraries, using cholesky decomposition")
+    except:
+        raise ImportWarning("Could not find cholmod library. using (slower) LU decomposition")
+        cholmod = False
+        
+    fem = Solver(surface, use_cholmod=cholmod)
+    evals, emodes = fem.eigs(k=num_modes)
+    
+    # standardize modes
+    emodes = (emodes - np.mean(emodes, axis=0))/np.std(emodes, axis=0)
+    
+    # remove the medial wall
+    medial_wall = find_medial_wall(sdir, sid).reshape(-1,)
+    emodes[medial_wall] = np.nan
+    
+    if not outevec:
+        outevec = surf_file.replace(ext, '') + '_outevecs_' + str(num_modes) + '.txt'
+    
+    outevec = os.path.join(outdir, outevec)
+    
+    np.savetxt(outevec, emodes)
+    
+    return outevec
+
+# remove the medial wall
+def find_medial_wall(sdir, sid):
+    label = os.path.join(sdir, sid, 'label', 'lh.aparc.a2009s.annot')
+    labels, ctab, names = read_annot(label)
 
+    indices = np.argwhere(labels==-1) # fs medial wall labels
+    
+    return indices
 
 if __name__=="__main__":
     # Command Line options and error checking done here
     options = options_parse()
+    
+    if options.surf is None:
+        m_print('ERROR: no surface was created/selected?')
+        sys.exit(1)
 
-    my_print(options.label)
-    my_print(options.surf)
+    m_print(options.label)
+    m_print(options.surf)
 
     if options.asegid is not None:
-        surf = get_aseg_surf(options.sdir,options.sid,options.asegid,options.outsurf)
-        outsurf = surf
+        outsurf = get_aseg_surf(options.sdir, options.sid, options.asegid, options.outsurf)
     elif options.label is not None:
-        surf = get_label_surf(options.sdir,options.sid,options.label,options.surf,options.source,options.outsurf)
-        outsurf = surf
+        outsurf = get_label_surf(options.sdir, options.sid, options.label, options.surf, options.source, options.outsurf)
     elif options.aparcid is not None:
-        surf = get_aparc_surf(options.sdir,options.sid,options.surf,options.aparcid,options.outsurf)    
-        outsurf = surf
-    elif options.surf is not None:
-        surf = get_surf_surf(options.sdir,options.sid,options.surf)
-        outsurf = options.outsurf
-    #my_print(surf)
+        outsurf = get_aparc_surf(options.sdir, options.sid, options.surf, options.aparcid, options.outsurf)    
+    else: # make surface out of --surf
+        outsurf = make_surf(options.sdir, options.sid, options.surf)
+    #m_print(surf)
     #sys.exit(0)
-    if surf is None:
-        my_print('ERROR: no surface was created/selected?')
-        sys.exit(1)
-
+    
     if options.dotet:
         #convert to tetmesh
-        get_tetmesh(surf,options.outtet,options.fixiter)
-        #run shapedna tetra
-        run_shapeDNAtetra(options.outtet,options.outev,options)
-    else:
-        run_shapeDNAtria(surf,options.outev,outsurf,options)
+        get_tetmesh(outsurf,options.outtet,options.fixiter)
+        
+    calc_eigenmodes(options.sdir, options.sid, outsurf, options.outdir, options.outevec, options.num)
 
     # always exit with 0 exit code
     sys.exit(0)
+
```

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.4/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.4/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.4/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.4/neuroshape.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.py
 neuroshape/__init__.py
 neuroshape/connectopic_laplacian.py
-neuroshape/eigenmaps.py
 neuroshape/eigenmodes.py
 neuroshape/permutation.py
-neuroshape/poly_eigenmaps.py
 neuroshape/recon.py
 neuroshape/stats.py
-neuroshape/surface_eigenmodes.py
-neuroshape/volume_eigenmodes.py
 neuroshape.egg-info/PKG-INFO
 neuroshape.egg-info/SOURCES.txt
 neuroshape.egg-info/dependency_links.txt
 neuroshape.egg-info/top_level.txt
 neuroshape/nipype/__init__.py
 neuroshape/nipype/interfaces/__init__.py
 neuroshape/nipype/interfaces/workbench/__init__.py
```

### Comparing `neuroshape-0.0.4.3.3/pyproject.toml` & `neuroshape-0.0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuroshape"
-version = "0.0.4.3.3"
+version = "0.0.4.4"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.3.3/setup.py` & `neuroshape-0.0.4.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 #                   include_dirs=[numpy.get_include()])
 
 #euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
 #                  include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.3.3',
+      version='0.0.4.4',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages())
       #ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.3.3/src/eta_squared.c` & `neuroshape-0.0.4.4/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/src/euler_threshold.c` & `neuroshape-0.0.4.4/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.3/src/glmfit.c` & `neuroshape-0.0.4.4/src/glmfit.c`

 * *Files identical despite different names*

