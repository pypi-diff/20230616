# Comparing `tmp/multipie-1.1.7.tar.gz` & `tmp/multipie-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multipie-1.1.7.tar", last modified: Mon Jun 12 14:22:42 2023, max compression
+gzip compressed data, was "multipie-1.1.8.tar", last modified: Fri Jun 16 02:53:50 2023, max compression
```

## Comparing `multipie-1.1.7.tar` & `multipie-1.1.8.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.048545 multipie-1.1.7/
--rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.1.7/LICENSE
--rw-------   0 hiro       (501) staff       (20)       81 2023-05-15 22:16:08.000000 multipie-1.1.7/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-12 14:22:42.048636 multipie-1.1.7/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1727 2023-05-25 21:40:12.000000 multipie-1.1.7/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:41.977510 multipie-1.1.7/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)     2299 2023-06-12 13:29:16.000000 multipie-1.1.7/multipie/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.013126 multipie-1.1.7/multipie/binary_data/
--rw-r--r--   0 hiro       (501) staff       (20)  5479250 2023-05-15 16:10:42.000000 multipie-1.1.7/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.1.7/multipie/binary_data/CharacterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-05-15 16:00:43.000000 multipie-1.1.7/multipie/binary_data/ClebschGordanPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-05-15 15:37:02.000000 multipie-1.1.7/multipie/binary_data/HarmonicsPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-05-15 16:01:10.000000 multipie-1.1.7/multipie/binary_data/ResponseTensorPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.1.7/multipie/binary_data/SymmetryOperationGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.1.7/multipie/binary_data/VirtualClusterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   380153 2023-05-15 15:37:10.000000 multipie-1.1.7/multipie/binary_data/WyckoffGSet.pkl
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.014444 multipie-1.1.7/multipie/character/
--rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/character/character_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/character/character_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.015068 multipie-1.1.7/multipie/clebsch_gordan/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/clebsch_gordan/clebsch_gordan_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
--rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.1.7/multipie/const.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.034652 multipie-1.1.7/multipie/data/
--rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_atomic_multipoles.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_cartesian_to_ch_harmoncis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_character_table.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_compatibility_relation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_harmonics_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_no_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_product_decomp.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_symmetry_operation_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_symmetry_operation_sg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      883 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_tag_harmonics_alias.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_tag_point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_tag_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1380 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_transform_matrix.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_virtual_cluster_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15108 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_wyckoff_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   157758 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/data/data_wyckoff_sg.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.035436 multipie-1.1.7/multipie/group/
--rwxr-xr-x   0 hiro       (501) staff       (20)    30142 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/group/point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    22542 2023-06-12 13:15:36.000000 multipie-1.1.7/multipie/group/space_group.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.038147 multipie-1.1.7/multipie/harmonics/
--rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/harmonics/harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/harmonics/harmonics_complex_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/harmonics/harmonics_complex_pg_set.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/harmonics/harmonics_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/harmonics/harmonics_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.038340 multipie-1.1.7/multipie/harmonics/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/harmonics/util/equivalent_operator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.039846 multipie-1.1.7/multipie/model/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2198 2023-06-06 22:09:12.000000 multipie-1.1.7/multipie/model/construct_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3459 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/model/create_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    31775 2023-06-12 01:30:37.000000 multipie-1.1.7/multipie/model/material_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/model/multipie_manager.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    17981 2023-06-07 14:42:34.000000 multipie-1.1.7/multipie/model/symmetry_adapted_model.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.040979 multipie-1.1.7/multipie/model/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/model/util/atomic_matrix_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    25780 2023-05-31 07:44:56.000000 multipie-1.1.7/multipie/model/util/create_pdf.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    25021 2023-06-07 14:42:34.000000 multipie-1.1.7/multipie/model/util/symmetry_adapted_model_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:41.975257 multipie-1.1.7/multipie/multipole/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.041456 multipie-1.1.7/multipie/multipole/base/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/multipole/base/base_atomic_multipole_dataset.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/multipole/base/base_atomic_multipole_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.043303 multipie-1.1.7/multipie/multipole/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    14715 2023-05-31 07:36:18.000000 multipie-1.1.7/multipie/multipole/util/atomic_orbital_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     6736 2023-06-01 08:23:27.000000 multipie-1.1.7/multipie/multipole/util/atomic_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/multipole/util/multipole_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/multipole/util/pauli.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/multipole/util/spin_orbital_basis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4751 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/multipole/util/structure_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/multipole/util/z_samb_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.043786 multipie-1.1.7/multipie/response_tensor/
--rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/response_tensor/response_tensor_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/response_tensor/response_tensor_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.043968 multipie-1.1.7/multipie/response_tensor/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/response_tensor/util/response_tensor_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.044591 multipie-1.1.7/multipie/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.1.7/multipie/scripts/create_binary.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1601 2023-06-04 14:31:58.000000 multipie-1.1.7/multipie/scripts/create_samb.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.045363 multipie-1.1.7/multipie/symmetry_operation/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/symmetry_operation/symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    14936 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/symmetry_operation/symmetry_operation_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/symmetry_operation/symmetry_operation_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.045583 multipie-1.1.7/multipie/symmetry_operation/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     5488 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/symmetry_operation/util/symmetry_operation_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.047241 multipie-1.1.7/multipie/tag/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/tag/tag.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/tag/tag_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/tag/tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/tag/tag_list.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/tag/tag_multipole.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/tag/tag_response_tensor.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/tag/tag_symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/tag/tag_wyckoff.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.047780 multipie-1.1.7/multipie/virtual_cluster/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/virtual_cluster/virtual_cluster_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/virtual_cluster/virtual_cluster_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:42.048290 multipie-1.1.7/multipie/wyckoff/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3252 2023-05-15 15:10:01.000000 multipie-1.1.7/multipie/wyckoff/wyckoff_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.1.7/multipie/wyckoff/wyckoff_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-12 14:22:41.978796 multipie-1.1.7/multipie.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-12 14:22:41.000000 multipie-1.1.7/multipie.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     3339 2023-06-12 14:22:41.000000 multipie-1.1.7/multipie.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-06-12 14:22:41.000000 multipie-1.1.7/multipie.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)      116 2023-06-12 14:22:41.000000 multipie-1.1.7/multipie.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-06-12 14:22:41.000000 multipie-1.1.7/multipie.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        9 2023-06-12 14:22:41.000000 multipie-1.1.7/multipie.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      888 2023-06-12 14:22:42.049053 multipie-1.1.7/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.1.7/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.404238 multipie-1.1.8/
+-rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.1.8/LICENSE
+-rw-------   0 hiro       (501) staff       (20)       81 2023-05-15 22:16:08.000000 multipie-1.1.8/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-16 02:53:50.404336 multipie-1.1.8/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1727 2023-05-25 21:40:12.000000 multipie-1.1.8/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.371873 multipie-1.1.8/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)     2299 2023-06-16 01:54:52.000000 multipie-1.1.8/multipie/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.387759 multipie-1.1.8/multipie/binary_data/
+-rw-r--r--   0 hiro       (501) staff       (20)  5479250 2023-05-15 16:10:42.000000 multipie-1.1.8/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.1.8/multipie/binary_data/CharacterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-05-15 16:00:43.000000 multipie-1.1.8/multipie/binary_data/ClebschGordanPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-05-15 15:37:02.000000 multipie-1.1.8/multipie/binary_data/HarmonicsPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-05-15 16:01:10.000000 multipie-1.1.8/multipie/binary_data/ResponseTensorPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.1.8/multipie/binary_data/SymmetryOperationGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.1.8/multipie/binary_data/VirtualClusterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   380153 2023-05-15 15:37:10.000000 multipie-1.1.8/multipie/binary_data/WyckoffGSet.pkl
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.388351 multipie-1.1.8/multipie/character/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/character/character_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/character/character_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.388661 multipie-1.1.8/multipie/clebsch_gordan/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/clebsch_gordan/clebsch_gordan_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.1.8/multipie/const.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.396946 multipie-1.1.8/multipie/data/
+-rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_atomic_multipoles.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_cartesian_to_ch_harmoncis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_character_table.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_compatibility_relation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_harmonics_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_no_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_product_decomp.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_symmetry_operation_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_symmetry_operation_sg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      883 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_tag_harmonics_alias.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_tag_point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_tag_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1380 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_transform_matrix.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_virtual_cluster_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15108 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_wyckoff_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   157758 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_wyckoff_sg.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.397450 multipie-1.1.8/multipie/group/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    30142 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/group/point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22542 2023-06-12 13:15:36.000000 multipie-1.1.8/multipie/group/space_group.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.398414 multipie-1.1.8/multipie/harmonics/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/harmonics/harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/harmonics/harmonics_complex_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/harmonics/harmonics_complex_pg_set.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/harmonics/harmonics_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/harmonics/harmonics_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.398553 multipie-1.1.8/multipie/harmonics/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/harmonics/util/equivalent_operator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.399239 multipie-1.1.8/multipie/model/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2198 2023-06-06 22:09:12.000000 multipie-1.1.8/multipie/model/construct_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3459 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/model/create_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    31907 2023-06-16 02:46:38.000000 multipie-1.1.8/multipie/model/material_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/model/multipie_manager.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    18219 2023-06-16 02:02:17.000000 multipie-1.1.8/multipie/model/symmetry_adapted_model.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.399686 multipie-1.1.8/multipie/model/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/model/util/atomic_matrix_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    26198 2023-06-16 02:40:39.000000 multipie-1.1.8/multipie/model/util/create_pdf.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    25021 2023-06-07 14:42:34.000000 multipie-1.1.8/multipie/model/util/symmetry_adapted_model_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.370377 multipie-1.1.8/multipie/multipole/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.400041 multipie-1.1.8/multipie/multipole/base/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/multipole/base/base_atomic_multipole_dataset.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/multipole/base/base_atomic_multipole_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.401106 multipie-1.1.8/multipie/multipole/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14715 2023-05-31 07:36:18.000000 multipie-1.1.8/multipie/multipole/util/atomic_orbital_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     6736 2023-06-01 08:23:27.000000 multipie-1.1.8/multipie/multipole/util/atomic_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/multipole/util/multipole_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/multipole/util/pauli.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/multipole/util/spin_orbital_basis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4751 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/multipole/util/structure_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/multipole/util/z_samb_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.401392 multipie-1.1.8/multipie/response_tensor/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/response_tensor/response_tensor_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/response_tensor/response_tensor_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.401539 multipie-1.1.8/multipie/response_tensor/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/response_tensor/util/response_tensor_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.401839 multipie-1.1.8/multipie/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.1.8/multipie/scripts/create_binary.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1601 2023-06-04 14:31:58.000000 multipie-1.1.8/multipie/scripts/create_samb.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.402268 multipie-1.1.8/multipie/symmetry_operation/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/symmetry_operation/symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14936 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/symmetry_operation/symmetry_operation_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/symmetry_operation/symmetry_operation_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.402424 multipie-1.1.8/multipie/symmetry_operation/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     5488 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/symmetry_operation/util/symmetry_operation_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.403559 multipie-1.1.8/multipie/tag/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_list.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_multipole.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_response_tensor.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_wyckoff.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.403834 multipie-1.1.8/multipie/virtual_cluster/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/virtual_cluster/virtual_cluster_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/virtual_cluster/virtual_cluster_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.404097 multipie-1.1.8/multipie/wyckoff/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3252 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/wyckoff/wyckoff_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/wyckoff/wyckoff_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.373060 multipie-1.1.8/multipie.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     3339 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      116 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        9 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      888 2023-06-16 02:53:50.405012 multipie-1.1.8/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.1.8/setup.py
```

### Comparing `multipie-1.1.7/LICENSE` & `multipie-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/PKG-INFO` & `multipie-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.1.7
+Version: 1.1.8
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.8
```

### Comparing `multipie-1.1.7/README.md` & `multipie-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/__init__.py` & `multipie-1.1.8/multipie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __top_dir__ = os.path.normpath(os.path.dirname(__file__) + "/../") + "/"
 __bin_dir__ = __top_dir__ + "multipie/binary_data/"
 
 
 # ==================================================
 from gcoreutils.string_util import class_name
 from gcoreutils.binary_manager import BinaryManager
```

### Comparing `multipie-1.1.7/multipie/binary_data/BaseAtomicMultipoleDataset.pkl` & `multipie-1.1.8/multipie/binary_data/BaseAtomicMultipoleDataset.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/binary_data/CharacterPGSet.pkl` & `multipie-1.1.8/multipie/binary_data/CharacterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/binary_data/ClebschGordanPGSet.pkl` & `multipie-1.1.8/multipie/binary_data/ClebschGordanPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/binary_data/HarmonicsPGSet.pkl` & `multipie-1.1.8/multipie/binary_data/HarmonicsPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/binary_data/ResponseTensorPGSet.pkl` & `multipie-1.1.8/multipie/binary_data/ResponseTensorPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/binary_data/SymmetryOperationGSet.pkl` & `multipie-1.1.8/multipie/binary_data/SymmetryOperationGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/binary_data/VirtualClusterPGSet.pkl` & `multipie-1.1.8/multipie/binary_data/VirtualClusterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/binary_data/WyckoffGSet.pkl` & `multipie-1.1.8/multipie/binary_data/WyckoffGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/character/character_pg.py` & `multipie-1.1.8/multipie/character/character_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/character/character_pg_set.py` & `multipie-1.1.8/multipie/character/character_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/clebsch_gordan/clebsch_gordan_pg.py` & `multipie-1.1.8/multipie/clebsch_gordan/clebsch_gordan_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/clebsch_gordan/clebsch_gordan_pg_set.py` & `multipie-1.1.8/multipie/clebsch_gordan/clebsch_gordan_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/const.py` & `multipie-1.1.8/multipie/const.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_atomic_multipoles.py` & `multipie-1.1.8/multipie/data/data_atomic_multipoles.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_cartesian_to_ch_harmoncis.py` & `multipie-1.1.8/multipie/data/data_cartesian_to_ch_harmoncis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_character_table.py` & `multipie-1.1.8/multipie/data/data_character_table.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_compatibility_relation.py` & `multipie-1.1.8/multipie/data/data_compatibility_relation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_harmonics.py` & `multipie-1.1.8/multipie/data/data_harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_harmonics_real.py` & `multipie-1.1.8/multipie/data/data_harmonics_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_no_space_group.py` & `multipie-1.1.8/multipie/data/data_no_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_product_decomp.py` & `multipie-1.1.8/multipie/data/data_product_decomp.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_symmetry_operation_pg.py` & `multipie-1.1.8/multipie/data/data_symmetry_operation_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_symmetry_operation_sg.py` & `multipie-1.1.8/multipie/data/data_symmetry_operation_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_tag_harmonics_alias.py` & `multipie-1.1.8/multipie/data/data_tag_harmonics_alias.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_tag_irrep.py` & `multipie-1.1.8/multipie/data/data_tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_tag_point_group.py` & `multipie-1.1.8/multipie/data/data_tag_point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_tag_space_group.py` & `multipie-1.1.8/multipie/data/data_tag_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_transform_matrix.py` & `multipie-1.1.8/multipie/data/data_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_virtual_cluster_real.py` & `multipie-1.1.8/multipie/data/data_virtual_cluster_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_wyckoff_pg.py` & `multipie-1.1.8/multipie/data/data_wyckoff_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/data/data_wyckoff_sg.py` & `multipie-1.1.8/multipie/data/data_wyckoff_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/group/point_group.py` & `multipie-1.1.8/multipie/group/point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/group/space_group.py` & `multipie-1.1.8/multipie/group/space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/harmonics/harmonics.py` & `multipie-1.1.8/multipie/harmonics/harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/harmonics/harmonics_complex_pg.py` & `multipie-1.1.8/multipie/harmonics/harmonics_complex_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/harmonics/harmonics_complex_pg_set.py` & `multipie-1.1.8/multipie/harmonics/harmonics_complex_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/harmonics/harmonics_pg.py` & `multipie-1.1.8/multipie/harmonics/harmonics_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/harmonics/harmonics_pg_set.py` & `multipie-1.1.8/multipie/harmonics/harmonics_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/harmonics/util/equivalent_operator.py` & `multipie-1.1.8/multipie/harmonics/util/equivalent_operator.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/model/construct_model.py` & `multipie-1.1.8/multipie/model/construct_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/model/create_model.py` & `multipie-1.1.8/multipie/model/create_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/model/material_model.py` & `multipie-1.1.8/multipie/model/material_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # ==================================================
 input_str = """
 === Input for SAMB construction (* optional [default]) ===
 - model : model name (str).
 - group : group name (Schoenflies notation) or group number (space group) (str/int).
 - site : site position, orbital info. (dict) { name: ("position", orbital or orbital list) }.
-- bond : bond (list) [ ("tail", "head", (list of) neighbors) ].
+- bond* : bond (list) [ ("tail", "head", (list of) neighbors) ], [[]].
 - spinful* : spinful basis ? (bool), [False].
 - cell* : unit-cell constants (dict) { "a", "b", "c", "alpha", "beta", "gamma" }, [a=b=c=1,alpha=beta=gamma=90].
 - option*
   - view* : view point (int list), [None].
   - view_mode* : mode for QtDraw file (str) ("standard"/"arrow"/"debug"), ["standard"].
   - output* : output folder (str), [model name].
   - minimal_samb* (bool) : minimal output in _samb.pdf ? [True].
@@ -820,14 +820,19 @@
         """
         # default setting.
         if "cell" not in d.keys():
             d["cell"] = None
 
         model = d["model"]
 
+        if "site" not in d.keys():
+            d["site"] = {}
+        if "bond" not in d.keys():
+            d["bond"] = []
+
         if "option" not in d.keys():
             d["option"] = {"view": None, "view_mode": "standard", "output": model, "minimal_samb": True}
         else:
             if "view" not in d["option"].keys():
                 d["option"]["view"] = None
             if "view_mode" not in d["option"].keys():
                 d["option"]["view_mode"] = "standard"
```

### Comparing `multipie-1.1.7/multipie/model/multipie_manager.py` & `multipie-1.1.8/multipie/model/multipie_manager.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/model/symmetry_adapted_model.py` & `multipie-1.1.8/multipie/model/symmetry_adapted_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,33 +185,40 @@
 
             func = create_zk_samb_set
             args = [z_data, bc_samb_set, u_samb_set, k_samb_set, cluster_bond, bond, dim, self._parallel]
             zk_data = _run("Zk", mpm, func, *args)
 
         # delete unused samb and redefine the serial number of multipoles.
         if model["info"]["option"]["minimal_samb"]:
-            atomic_info_, atomic_data_, z_data = redefine_index(atomic_info, atomic_data, z_data, molecule=molecule)
-            site_cluster_info, site_cluster_data, z_data = redefine_index(
-                site_cluster_info, site_cluster_data, z_data, molecule=molecule
-            )
+            if len(site_cluster_data) > 0:
+                site_cluster_info, site_cluster_data, z_data = redefine_index(
+                    site_cluster_info, site_cluster_data, z_data, molecule=molecule
+                )
             if len(site_cluster_info) > 0:
                 init_idx = int(list(site_cluster_info.values())[-1][-1].split("_")[1]) + 1
             else:
                 init_idx = 1
-            bond_cluster_info, bond_cluster_data, z_data = redefine_index(
-                bond_cluster_info, bond_cluster_data, z_data, molecule=molecule, init_idx=init_idx
-            )
-            uniform_info_, uniform_data_, z_data = redefine_index(uniform_info, uniform_data, z_data, molecule=molecule)
+            if len(bond_cluster_data) > 0:
+                bond_cluster_info, bond_cluster_data, z_data = redefine_index(
+                    bond_cluster_info, bond_cluster_data, z_data, molecule=molecule, init_idx=init_idx
+                )
             if molecule:
-                atomic_info, atomic_data = atomic_info_, atomic_data_
-                uniform_info, uniform_data = uniform_info_, uniform_data_
+                if len(atomic_data) > 0:
+                    atomic_info, atomic_data, z_data = redefine_index(atomic_info, atomic_data, z_data, molecule=True)
+                if len(uniform_data) > 0:
+                    uniform_info, uniform_data, z_data = redefine_index(
+                        uniform_info, uniform_data, z_data, molecule=True
+                    )
             if not molecule:
-                atomic_info, atomic_data, zk_data = redefine_index(atomic_info, atomic_data, zk_data)
-                uniform_info, uniform_data, zk_data = redefine_index(uniform_info, uniform_data, zk_data)
-                structure_info, structure_data, zk_data = redefine_index(structure_info, structure_data, zk_data)
+                if len(atomic_data) > 0:
+                    atomic_info, atomic_data, zk_data = redefine_index(atomic_info, atomic_data, zk_data)
+                if len(uniform_data) > 0:
+                    uniform_info, uniform_data, zk_data = redefine_index(uniform_info, uniform_data, zk_data)
+                if len(structure_data) > 0:
+                    structure_info, structure_data, zk_data = redefine_index(structure_info, structure_data, zk_data)
 
         # harmonics
         head_list = ["Q", "G", "M", "T"]
         harmonics_info = {"Q": [], "G": []}
         for X in head_list:
             data = atomic_data | site_cluster_data | bond_cluster_data | uniform_data
             if not molecule:
```

### Comparing `multipie-1.1.7/multipie/model/util/create_pdf.py` & `multipie-1.1.8/multipie/model/util/create_pdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,19 +71,16 @@
         pdf.text(r"\begin{itemize}")
         self.information(pdf, info, name, data)
         self.hr(pdf)
         if not info["molecule"]:
             self.lattice_info(pdf, info, name, data)
             self.hr(pdf)
         self.ket_space(pdf, info, name, data)
-        self.hr(pdf)
         self.basis_info(pdf, info, data, samb_dict)
-        self.hr(pdf)
         self.harmonics_info(pdf, info, samb_dict)
-        self.hr(pdf)
         self.group_info(pdf, info, name, data)
         pdf.text(r"\end{itemize}")
 
         # postscript.
         mpm.log(f"  * wrote '{filename}.tex.'", None)
         mpm.log(f"  * wrote '{filename}.pdf.'", None)
 
@@ -116,14 +113,17 @@
         pdf.text(r"\quad - time-reversal type: \texttt{" + info["generate"]["time_reversal_type"] + "}\n")
         pdf.text(r"\quad - irrep: \texttt{[" + ", ".join(info["generate"]["irrep"]) + "]}\n")
         spinful_str = "spinful" if info["spinful"] else "spinless"
         pdf.text(r"\quad - \texttt{" + spinful_str + "}\n")
 
     # ==================================================
     def ket_space(self, pdf, info, name, data):
+        if not info["site"]:  # no sites.
+            return
+
         self.comment(pdf, "ket hilbert space.")
         pdf.text(r"\item Kets: dimension = " + str(len(info["ket"])))
         orb = to_latex([i.split("@")[0] for i in info["ket"]], info["spinful"], info["crystal"])
         s = [i.split("@")[1] for i in info["ket"]]
         ket = [i + "@" + j for i, j in zip(orb, s)]
         ket = [
             "$"
@@ -173,14 +173,17 @@
             cpos="cc|c|l",
             caption="Site-clusters.",
             stretch=1.3,
             long=True,
             hl=True,
         )
 
+        if not info["bond"]:  # no bonds.
+            return
+
         pdf.text()
         self.comment(pdf, "bonds in unit cell.")
         pdf.text(r"\item Bonds in (primitive) unit cell:")
         row = []
         tbl = []
         for cluster, lst in data["cluster_bond"].items():
             cluster_name = self.ubar_name(cluster)
@@ -212,17 +215,21 @@
             ["bond", "tail", "head", "$n$", "\#", r"$\bm{b}@\bm{c}$", "mapping"],
             caption="Bond-clusters.",
             cpos="cc|cc|c|c|c|l",
             stretch=1.3,
             long=True,
             hl=True,
         )
+        self.hr(pdf)
 
     # ==================================================
     def basis_info(self, pdf, info, data, samb):
+        if not samb["info"]["Z"]:  # no SAMBs.
+            return
+
         # SAMB.
         self.comment(pdf, "SAMB.")
         pdf.text(r"\item SAMB:" + "\n")
 
         Zinfo = {}
         for k, v in samb["info"]["Z"].items():
             for z_tag in v:
@@ -443,14 +450,16 @@
             stretch=1.3,
             long=True,
             rmath=True,
             hl=hl[1:],
         )
 
         if not info["molecule"]:
+            if not samb["info"]["structure"]:  # no structure SAMBs.
+                return
             # structure SAMB.
             self.comment(pdf, "structure SAMB.")
             row = []
             tbl = []
             hl_no = -1
             hl = []
             for c_group, s_lst in samb["info"]["structure"].items():
@@ -473,17 +482,21 @@
                 caption="Structure SAMB.",
                 cpos="c|c|c|c",
                 stretch=1.3,
                 long=True,
                 rmath=True,
                 hl=hl[1:],
             )
+        self.hr(pdf)
 
     # ==================================================
     def harmonics_info(self, pdf, info, samb):
+        if len(samb["info"]["harmonics"]["Q"]) == 0 and len(samb["info"]["harmonics"]["G"]) == 0:  # no harmonics.
+            return
+
         self.comment(pdf, "harmonics.")
         group = self._mpm.point_group
 
         polar = TagList.from_str(TagMultipole, samb["info"]["harmonics"]["Q"])
         axial = TagList.from_str(TagMultipole, samb["info"]["harmonics"]["G"])
 
         for hset, name in [(polar, "Polar"), (axial, "Axial")]:
@@ -521,14 +534,15 @@
                 caption=f"{name} harmonics.",
                 stretch=1.3,
                 rmath=True,
                 tmath=True,
                 long=True,
                 hl=hl[1:],
             )
+        self.hr(pdf)
 
     # ==================================================
     def lattice_info(self, pdf, info, name, data):
         self.comment(pdf, "unit cell.")
         pdf.text(r"\item Unit cell:" + "\n")
         cell = info["cell"]
         a, b, c, alpha, beta, gamma = (
```

### Comparing `multipie-1.1.7/multipie/model/util/symmetry_adapted_model_util.py` & `multipie-1.1.8/multipie/model/util/symmetry_adapted_model_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/base/base_atomic_multipole_dataset.py` & `multipie-1.1.8/multipie/multipole/base/base_atomic_multipole_dataset.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/base/base_atomic_multipole_set.py` & `multipie-1.1.8/multipie/multipole/base/base_atomic_multipole_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/util/atomic_orbital_util.py` & `multipie-1.1.8/multipie/multipole/util/atomic_orbital_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/util/atomic_samb_util.py` & `multipie-1.1.8/multipie/multipole/util/atomic_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/util/multipole_util.py` & `multipie-1.1.8/multipie/multipole/util/multipole_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/util/pauli.py` & `multipie-1.1.8/multipie/multipole/util/pauli.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/util/spin_orbital_basis.py` & `multipie-1.1.8/multipie/multipole/util/spin_orbital_basis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/util/structure_samb_util.py` & `multipie-1.1.8/multipie/multipole/util/structure_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/multipole/util/z_samb_util.py` & `multipie-1.1.8/multipie/multipole/util/z_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/response_tensor/response_tensor_pg.py` & `multipie-1.1.8/multipie/response_tensor/response_tensor_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/response_tensor/response_tensor_pg_set.py` & `multipie-1.1.8/multipie/response_tensor/response_tensor_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/response_tensor/util/response_tensor_util.py` & `multipie-1.1.8/multipie/response_tensor/util/response_tensor_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/scripts/create_binary.py` & `multipie-1.1.8/multipie/scripts/create_binary.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/scripts/create_samb.py` & `multipie-1.1.8/multipie/scripts/create_samb.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/symmetry_operation/symmetry_operation.py` & `multipie-1.1.8/multipie/symmetry_operation/symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/symmetry_operation/symmetry_operation_g.py` & `multipie-1.1.8/multipie/symmetry_operation/symmetry_operation_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/symmetry_operation/symmetry_operation_g_set.py` & `multipie-1.1.8/multipie/symmetry_operation/symmetry_operation_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/symmetry_operation/util/symmetry_operation_util.py` & `multipie-1.1.8/multipie/symmetry_operation/util/symmetry_operation_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/tag/tag.py` & `multipie-1.1.8/multipie/tag/tag.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/tag/tag_group.py` & `multipie-1.1.8/multipie/tag/tag_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/tag/tag_irrep.py` & `multipie-1.1.8/multipie/tag/tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/tag/tag_list.py` & `multipie-1.1.8/multipie/tag/tag_list.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/tag/tag_multipole.py` & `multipie-1.1.8/multipie/tag/tag_multipole.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/tag/tag_response_tensor.py` & `multipie-1.1.8/multipie/tag/tag_response_tensor.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/tag/tag_symmetry_operation.py` & `multipie-1.1.8/multipie/tag/tag_symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/tag/tag_wyckoff.py` & `multipie-1.1.8/multipie/tag/tag_wyckoff.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/virtual_cluster/virtual_cluster_pg.py` & `multipie-1.1.8/multipie/virtual_cluster/virtual_cluster_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/virtual_cluster/virtual_cluster_pg_set.py` & `multipie-1.1.8/multipie/virtual_cluster/virtual_cluster_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/wyckoff/wyckoff_g.py` & `multipie-1.1.8/multipie/wyckoff/wyckoff_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie/wyckoff/wyckoff_g_set.py` & `multipie-1.1.8/multipie/wyckoff/wyckoff_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/multipie.egg-info/PKG-INFO` & `multipie-1.1.8/multipie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.1.7
+Version: 1.1.8
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.8
```

### Comparing `multipie-1.1.7/multipie.egg-info/SOURCES.txt` & `multipie-1.1.8/multipie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multipie-1.1.7/setup.cfg` & `multipie-1.1.8/setup.cfg`

 * *Files identical despite different names*

