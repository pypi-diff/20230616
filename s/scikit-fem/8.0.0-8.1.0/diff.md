# Comparing `tmp/scikit-fem-8.0.0.tar.gz` & `tmp/scikit-fem-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-fem-8.0.0.tar", last modified: Fri Dec 16 22:26:36 2022, max compression
+gzip compressed data, was "scikit-fem-8.1.0.tar", last modified: Fri Jun 16 20:23:38 2023, max compression
```

## Comparing `scikit-fem-8.0.0.tar` & `scikit-fem-8.1.0.tar`

### file list

```diff
@@ -1,162 +1,179 @@
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.962982 scikit-fem-8.0.0/
--rw-r--r--   0 tom       (1000) users      (100)     1469 2022-08-03 12:04:25.000000 scikit-fem-8.0.0/LICENSE
--rw-r--r--   0 tom       (1000) users      (100)    29172 2022-12-16 22:26:36.962982 scikit-fem-8.0.0/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (100)    28187 2022-12-16 21:51:10.000000 scikit-fem-8.0.0/README.md
--rw-r--r--   0 tom       (1000) users      (100)       93 2021-11-16 08:26:17.000000 scikit-fem-8.0.0/pyproject.toml
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.948982 scikit-fem-8.0.0/scikit_fem.egg-info/
--rw-r--r--   0 tom       (1000) users      (100)    29172 2022-12-16 22:26:36.000000 scikit-fem-8.0.0/scikit_fem.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (100)     4832 2022-12-16 22:26:36.000000 scikit-fem-8.0.0/scikit_fem.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) users      (100)        1 2022-12-16 22:26:36.000000 scikit-fem-8.0.0/scikit_fem.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) users      (100)       44 2022-12-16 22:26:36.000000 scikit-fem-8.0.0/scikit_fem.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) users      (100)        6 2022-12-16 22:26:36.000000 scikit-fem-8.0.0/scikit_fem.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) users      (100)     1116 2022-12-16 22:26:36.963982 scikit-fem-8.0.0/setup.cfg
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.949982 scikit-fem-8.0.0/skfem/
--rw-r--r--   0 tom       (1000) users      (100)      445 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/__about__.py
--rw-r--r--   0 tom       (1000) users      (100)      969 2022-11-03 07:35:24.000000 scikit-fem-8.0.0/skfem/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.949982 scikit-fem-8.0.0/skfem/assembly/
--rw-r--r--   0 tom       (1000) users      (100)     3005 2022-11-29 08:41:09.000000 scikit-fem-8.0.0/skfem/assembly/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.949982 scikit-fem-8.0.0/skfem/assembly/basis/
--rw-r--r--   0 tom       (1000) users      (100)      454 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/assembly/basis/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)    16202 2022-11-23 20:55:57.000000 scikit-fem-8.0.0/skfem/assembly/basis/abstract_basis.py
--rw-r--r--   0 tom       (1000) users      (100)    10180 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/assembly/basis/cell_basis.py
--rw-r--r--   0 tom       (1000) users      (100)     8196 2022-11-23 20:02:18.000000 scikit-fem-8.0.0/skfem/assembly/basis/facet_basis.py
--rw-r--r--   0 tom       (1000) users      (100)     1304 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/assembly/basis/interior_facet_basis.py
--rw-r--r--   0 tom       (1000) users      (100)     1860 2022-11-03 07:35:24.000000 scikit-fem-8.0.0/skfem/assembly/basis/mortar_facet_basis.py
--rw-r--r--   0 tom       (1000) users      (100)    14710 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/assembly/dofs.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.950982 scikit-fem-8.0.0/skfem/assembly/form/
--rw-r--r--   0 tom       (1000) users      (100)      216 2022-03-27 11:47:07.000000 scikit-fem-8.0.0/skfem/assembly/form/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     5412 2022-11-03 07:35:24.000000 scikit-fem-8.0.0/skfem/assembly/form/bilinear_form.py
--rw-r--r--   0 tom       (1000) users      (100)     5399 2022-11-29 08:41:09.000000 scikit-fem-8.0.0/skfem/assembly/form/coo_data.py
--rw-r--r--   0 tom       (1000) users      (100)     4171 2022-11-03 07:35:24.000000 scikit-fem-8.0.0/skfem/assembly/form/form.py
--rw-r--r--   0 tom       (1000) users      (100)     1841 2022-06-19 15:24:56.000000 scikit-fem-8.0.0/skfem/assembly/form/functional.py
--rw-r--r--   0 tom       (1000) users      (100)     1448 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/assembly/form/linear_form.py
--rw-r--r--   0 tom       (1000) users      (100)     2184 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/assembly/form/trilinear_form.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.952982 scikit-fem-8.0.0/skfem/element/
--rw-r--r--   0 tom       (1000) users      (100)     4524 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/element/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     3216 2022-05-02 07:08:33.000000 scikit-fem-8.0.0/skfem/element/discrete_field.py
--rw-r--r--   0 tom       (1000) users      (100)     4642 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/element/element.py
--rw-r--r--   0 tom       (1000) users      (100)     4126 2022-05-02 07:08:33.000000 scikit-fem-8.0.0/skfem/element/element_composite.py
--rw-r--r--   0 tom       (1000) users      (100)     1699 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/element/element_dg.py
--rw-r--r--   0 tom       (1000) users      (100)     6282 2021-09-17 13:48:17.000000 scikit-fem-8.0.0/skfem/element/element_global.py
--rw-r--r--   0 tom       (1000) users      (100)      898 2022-09-20 10:35:55.000000 scikit-fem-8.0.0/skfem/element/element_h1.py
--rw-r--r--   0 tom       (1000) users      (100)     2595 2022-11-23 20:02:18.000000 scikit-fem-8.0.0/skfem/element/element_hcurl.py
--rw-r--r--   0 tom       (1000) users      (100)     1767 2022-11-12 11:56:44.000000 scikit-fem-8.0.0/skfem/element/element_hdiv.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.953982 scikit-fem-8.0.0/skfem/element/element_hex/
--rw-r--r--   0 tom       (1000) users      (100)      253 2022-08-03 12:04:25.000000 scikit-fem-8.0.0/skfem/element/element_hex/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)      424 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_hex/element_hex0.py
--rw-r--r--   0 tom       (1000) users      (100)     2241 2021-08-31 06:59:29.000000 scikit-fem-8.0.0/skfem/element/element_hex/element_hex1.py
--rw-r--r--   0 tom       (1000) users      (100)    30688 2021-08-27 09:59:47.000000 scikit-fem-8.0.0/skfem/element/element_hex/element_hex2.py
--rw-r--r--   0 tom       (1000) users      (100)     1219 2022-08-03 12:04:25.000000 scikit-fem-8.0.0/skfem/element/element_hex/element_hex_rt1.py
--rw-r--r--   0 tom       (1000) users      (100)     2887 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_hex/element_hex_s2.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.953982 scikit-fem-8.0.0/skfem/element/element_line/
--rw-r--r--   0 tom       (1000) users      (100)      337 2021-08-31 06:59:29.000000 scikit-fem-8.0.0/skfem/element/element_line/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)      687 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_line/element_line_hermite.py
--rw-r--r--   0 tom       (1000) users      (100)      794 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_line/element_line_mini.py
--rw-r--r--   0 tom       (1000) users      (100)      404 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_line/element_line_p0.py
--rw-r--r--   0 tom       (1000) users      (100)      686 2021-08-31 06:59:29.000000 scikit-fem-8.0.0/skfem/element/element_line/element_line_p1.py
--rw-r--r--   0 tom       (1000) users      (100)      770 2021-08-25 18:15:40.000000 scikit-fem-8.0.0/skfem/element/element_line/element_line_p2.py
--rw-r--r--   0 tom       (1000) users      (100)     1647 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/element/element_line/element_line_pp.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.954982 scikit-fem-8.0.0/skfem/element/element_quad/
--rw-r--r--   0 tom       (1000) users      (100)      416 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/element/element_quad/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)      423 2021-11-27 21:19:08.000000 scikit-fem-8.0.0/skfem/element/element_quad/element_quad0.py
--rw-r--r--   0 tom       (1000) users      (100)      958 2021-11-27 21:19:08.000000 scikit-fem-8.0.0/skfem/element/element_quad/element_quad1.py
--rw-r--r--   0 tom       (1000) users      (100)     2501 2021-11-27 21:19:08.000000 scikit-fem-8.0.0/skfem/element/element_quad/element_quad2.py
--rw-r--r--   0 tom       (1000) users      (100)     1242 2021-11-27 21:19:08.000000 scikit-fem-8.0.0/skfem/element/element_quad/element_quad_bfs.py
--rw-r--r--   0 tom       (1000) users      (100)      931 2022-11-23 20:02:18.000000 scikit-fem-8.0.0/skfem/element/element_quad/element_quad_n1.py
--rw-r--r--   0 tom       (1000) users      (100)      755 2022-05-24 07:32:48.000000 scikit-fem-8.0.0/skfem/element/element_quad/element_quad_rt1.py
--rw-r--r--   0 tom       (1000) users      (100)     2044 2021-11-27 21:19:08.000000 scikit-fem-8.0.0/skfem/element/element_quad/element_quad_s2.py
--rw-r--r--   0 tom       (1000) users      (100)     2618 2022-09-23 19:10:47.000000 scikit-fem-8.0.0/skfem/element/element_quad/element_quadp.py
--rw-r--r--   0 tom       (1000) users      (100)     1120 2021-12-02 23:39:59.000000 scikit-fem-8.0.0/skfem/element/element_skeleton.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.955982 scikit-fem-8.0.0/skfem/element/element_tet/
--rw-r--r--   0 tom       (1000) users      (100)      466 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/element/element_tet/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     6214 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_ccr.py
--rw-r--r--   0 tom       (1000) users      (100)     1072 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_cr.py
--rw-r--r--   0 tom       (1000) users      (100)     1346 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_mini.py
--rw-r--r--   0 tom       (1000) users      (100)     1685 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_n1.py
--rw-r--r--   0 tom       (1000) users      (100)      409 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_p0.py
--rw-r--r--   0 tom       (1000) users      (100)     1117 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_p1.py
--rw-r--r--   0 tom       (1000) users      (100)     2799 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_p2.py
--rw-r--r--   0 tom       (1000) users      (100)     7285 2022-05-28 13:27:12.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_p3.py
--rw-r--r--   0 tom       (1000) users      (100)      901 2022-05-23 09:12:18.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_rt1.py
--rw-r--r--   0 tom       (1000) users      (100)      564 2022-10-16 09:12:53.000000 scikit-fem-8.0.0/skfem/element/element_tet/element_tet_skeleton_p0.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.958982 scikit-fem-8.0.0/skfem/element/element_tri/
--rw-r--r--   0 tom       (1000) users      (100)     1144 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/element/element_tri/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     1995 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_15param_plate.py
--rw-r--r--   0 tom       (1000) users      (100)     1961 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_argyris.py
--rw-r--r--   0 tom       (1000) users      (100)     2028 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_bdm1.py
--rw-r--r--   0 tom       (1000) users      (100)      789 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_cr.py
--rw-r--r--   0 tom       (1000) users      (100)     1184 2021-06-22 07:41:31.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_hermite.py
--rw-r--r--   0 tom       (1000) users      (100)     1102 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_morley.py
--rw-r--r--   0 tom       (1000) users      (100)      761 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_n1.py
--rw-r--r--   0 tom       (1000) users      (100)     1844 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_n2.py
--rw-r--r--   0 tom       (1000) users      (100)      405 2021-06-21 08:18:38.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p0.py
--rw-r--r--   0 tom       (1000) users      (100)      846 2021-11-27 21:19:08.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p1.py
--rw-r--r--   0 tom       (1000) users      (100)     1049 2022-05-02 07:08:33.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p1b.py
--rw-r--r--   0 tom       (1000) users      (100)      570 2022-05-02 07:08:33.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p1g.py
--rw-r--r--   0 tom       (1000) users      (100)     1399 2021-11-27 21:19:08.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p2.py
--rw-r--r--   0 tom       (1000) users      (100)     1692 2022-05-02 07:08:33.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p2b.py
--rw-r--r--   0 tom       (1000) users      (100)      854 2022-05-02 07:08:33.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p2g.py
--rw-r--r--   0 tom       (1000) users      (100)     3929 2021-11-27 21:19:08.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p3.py
--rw-r--r--   0 tom       (1000) users      (100)     8967 2021-09-19 11:47:40.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p4.py
--rw-r--r--   0 tom       (1000) users      (100)      744 2022-05-23 09:12:18.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_rt1.py
--rw-r--r--   0 tom       (1000) users      (100)     1695 2022-05-23 09:12:18.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_rt2.py
--rw-r--r--   0 tom       (1000) users      (100)      511 2022-09-30 20:03:42.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_skeleton_p0.py
--rw-r--r--   0 tom       (1000) users      (100)     1003 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/element/element_tri/element_tri_skeleton_p1.py
--rw-r--r--   0 tom       (1000) users      (100)     1653 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/element/element_vector.py
--rw-r--r--   0 tom       (1000) users      (100)     1532 2021-09-19 11:18:59.000000 scikit-fem-8.0.0/skfem/element/element_wedge_1.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.958982 scikit-fem-8.0.0/skfem/experimental/
--rw-r--r--   0 tom       (1000) users      (100)      203 2022-05-02 07:08:33.000000 scikit-fem-8.0.0/skfem/experimental/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.958982 scikit-fem-8.0.0/skfem/experimental/autodiff/
--rw-r--r--   0 tom       (1000) users      (100)     3107 2022-05-02 07:08:33.000000 scikit-fem-8.0.0/skfem/experimental/autodiff/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     1505 2022-10-16 09:12:53.000000 scikit-fem-8.0.0/skfem/experimental/autodiff/helpers.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.958982 scikit-fem-8.0.0/skfem/experimental/supermeshing/
--rw-r--r--   0 tom       (1000) users      (100)     2739 2022-11-29 08:41:09.000000 scikit-fem-8.0.0/skfem/experimental/supermeshing/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     1203 2022-11-03 07:35:24.000000 scikit-fem-8.0.0/skfem/generic_utils.py
--rw-r--r--   0 tom       (1000) users      (100)     6226 2022-11-11 11:47:21.000000 scikit-fem-8.0.0/skfem/helpers.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.958982 scikit-fem-8.0.0/skfem/io/
--rw-r--r--   0 tom       (1000) users      (100)       40 2020-06-04 12:37:26.000000 scikit-fem-8.0.0/skfem/io/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     2178 2021-08-31 06:59:29.000000 scikit-fem-8.0.0/skfem/io/json.py
--rw-r--r--   0 tom       (1000) users      (100)     8816 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/io/meshio.py
--rw-r--r--   0 tom       (1000) users      (100)     1611 2021-12-09 22:30:18.000000 scikit-fem-8.0.0/skfem/io/mfem.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.959982 scikit-fem-8.0.0/skfem/mapping/
--rw-r--r--   0 tom       (1000) users      (100)      418 2020-06-04 12:37:26.000000 scikit-fem-8.0.0/skfem/mapping/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     2882 2022-08-03 12:04:25.000000 scikit-fem-8.0.0/skfem/mapping/mapping.py
--rw-r--r--   0 tom       (1000) users      (100)     8056 2022-08-03 12:04:25.000000 scikit-fem-8.0.0/skfem/mapping/mapping_affine.py
--rw-r--r--   0 tom       (1000) users      (100)     8614 2022-08-03 12:04:25.000000 scikit-fem-8.0.0/skfem/mapping/mapping_isoparametric.py
--rw-r--r--   0 tom       (1000) users      (100)     7795 2022-11-07 19:18:05.000000 scikit-fem-8.0.0/skfem/mapping/mapping_mortar.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.961982 scikit-fem-8.0.0/skfem/mesh/
--rw-r--r--   0 tom       (1000) users      (100)     2701 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/mesh/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)    39526 2022-11-29 08:41:09.000000 scikit-fem-8.0.0/skfem/mesh/mesh.py
--rw-r--r--   0 tom       (1000) users      (100)      693 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/mesh/mesh_2d.py
--rw-r--r--   0 tom       (1000) users      (100)      367 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/mesh/mesh_2d_2.py
--rw-r--r--   0 tom       (1000) users      (100)     1823 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/mesh/mesh_3d.py
--rw-r--r--   0 tom       (1000) users      (100)     3606 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/mesh/mesh_dg.py
--rw-r--r--   0 tom       (1000) users      (100)     5486 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_hex_1.py
--rw-r--r--   0 tom       (1000) users      (100)      325 2021-08-31 06:59:29.000000 scikit-fem-8.0.0/skfem/mesh/mesh_hex_1_dg.py
--rw-r--r--   0 tom       (1000) users      (100)     1413 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_hex_2.py
--rw-r--r--   0 tom       (1000) users      (100)     2764 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_line_1.py
--rw-r--r--   0 tom       (1000) users      (100)      386 2021-08-31 06:59:29.000000 scikit-fem-8.0.0/skfem/mesh/mesh_line_1_dg.py
--rw-r--r--   0 tom       (1000) users      (100)     7163 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_quad_1.py
--rw-r--r--   0 tom       (1000) users      (100)      334 2021-12-29 21:34:09.000000 scikit-fem-8.0.0/skfem/mesh/mesh_quad_1_dg.py
--rw-r--r--   0 tom       (1000) users      (100)      864 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_quad_2.py
--rw-r--r--   0 tom       (1000) users      (100)      835 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/mesh/mesh_simplex.py
--rw-r--r--   0 tom       (1000) users      (100)    13604 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_tet_1.py
--rw-r--r--   0 tom       (1000) users      (100)     1923 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_tet_2.py
--rw-r--r--   0 tom       (1000) users      (100)    13355 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_tri_1.py
--rw-r--r--   0 tom       (1000) users      (100)      748 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_tri_1_dg.py
--rw-r--r--   0 tom       (1000) users      (100)     1587 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_tri_2.py
--rw-r--r--   0 tom       (1000) users      (100)     1363 2022-12-15 21:01:20.000000 scikit-fem-8.0.0/skfem/mesh/mesh_wedge_1.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.961982 scikit-fem-8.0.0/skfem/models/
--rw-r--r--   0 tom       (1000) users      (100)      152 2021-04-07 20:29:44.000000 scikit-fem-8.0.0/skfem/models/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     1129 2022-10-22 04:18:34.000000 scikit-fem-8.0.0/skfem/models/elasticity.py
--rw-r--r--   0 tom       (1000) users      (100)      432 2021-03-19 22:38:21.000000 scikit-fem-8.0.0/skfem/models/general.py
--rw-r--r--   0 tom       (1000) users      (100)      369 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/models/poisson.py
--rw-r--r--   0 tom       (1000) users      (100)   121022 2022-11-03 07:35:24.000000 scikit-fem-8.0.0/skfem/quadrature.py
--rw-r--r--   0 tom       (1000) users      (100)     6181 2022-10-16 09:12:53.000000 scikit-fem-8.0.0/skfem/refdom.py
--rw-r--r--   0 tom       (1000) users      (100)    21565 2022-11-29 08:41:09.000000 scikit-fem-8.0.0/skfem/utils.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-12-16 22:26:36.962982 scikit-fem-8.0.0/skfem/visuals/
--rw-r--r--   0 tom       (1000) users      (100)        7 2020-06-04 12:37:26.000000 scikit-fem-8.0.0/skfem/visuals/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)     1907 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/visuals/glvis.py
--rw-r--r--   0 tom       (1000) users      (100)    11818 2022-11-15 06:23:55.000000 scikit-fem-8.0.0/skfem/visuals/matplotlib.py
--rw-r--r--   0 tom       (1000) users      (100)     5232 2022-04-07 08:23:55.000000 scikit-fem-8.0.0/skfem/visuals/svg.py
--rw-r--r--   0 tom       (1000) users      (100)      690 2022-11-03 07:35:24.000000 scikit-fem-8.0.0/skfem/visuals/vedo.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.765991 scikit-fem-8.1.0/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1469 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/LICENSE
+-rw-r--r--   0 gustaft1   (502) staff       (20)    30140 2023-06-16 20:23:38.766137 scikit-fem-8.1.0/PKG-INFO
+-rw-r--r--   0 gustaft1   (502) staff       (20)    29155 2023-06-16 20:11:12.000000 scikit-fem-8.1.0/README.md
+-rw-r--r--   0 gustaft1   (502) staff       (20)       93 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/pyproject.toml
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.700847 scikit-fem-8.1.0/scikit_fem.egg-info/
+-rw-r--r--   0 gustaft1   (502) staff       (20)    30140 2023-06-16 20:23:38.000000 scikit-fem-8.1.0/scikit_fem.egg-info/PKG-INFO
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5287 2023-06-16 20:23:38.000000 scikit-fem-8.1.0/scikit_fem.egg-info/SOURCES.txt
+-rw-r--r--   0 gustaft1   (502) staff       (20)        1 2023-06-16 20:23:38.000000 scikit-fem-8.1.0/scikit_fem.egg-info/dependency_links.txt
+-rw-r--r--   0 gustaft1   (502) staff       (20)       44 2023-06-16 20:23:38.000000 scikit-fem-8.1.0/scikit_fem.egg-info/requires.txt
+-rw-r--r--   0 gustaft1   (502) staff       (20)        6 2023-06-16 20:23:38.000000 scikit-fem-8.1.0/scikit_fem.egg-info/top_level.txt
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1116 2023-06-16 20:23:38.766932 scikit-fem-8.1.0/setup.cfg
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.704088 scikit-fem-8.1.0/skfem/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      445 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/__about__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      980 2023-03-14 21:13:16.000000 scikit-fem-8.1.0/skfem/__init__.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.705539 scikit-fem-8.1.0/skfem/assembly/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3005 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/__init__.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.710065 scikit-fem-8.1.0/skfem/assembly/basis/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      454 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/basis/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    16699 2023-02-14 18:46:32.000000 scikit-fem-8.1.0/skfem/assembly/basis/abstract_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    10514 2023-06-04 15:41:44.000000 scikit-fem-8.1.0/skfem/assembly/basis/cell_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     8196 2023-01-19 20:25:59.000000 scikit-fem-8.1.0/skfem/assembly/basis/facet_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1304 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/basis/interior_facet_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1860 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/basis/mortar_facet_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    16525 2023-03-03 20:36:48.000000 scikit-fem-8.1.0/skfem/assembly/dofs.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.713578 scikit-fem-8.1.0/skfem/assembly/form/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      216 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/form/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5412 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/form/bilinear_form.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5399 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/form/coo_data.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4171 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/form/form.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1841 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/form/functional.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1448 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/form/linear_form.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2184 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/assembly/form/trilinear_form.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.718849 scikit-fem-8.1.0/skfem/element/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4734 2023-06-14 06:46:41.000000 scikit-fem-8.1.0/skfem/element/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3216 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/discrete_field.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4642 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4126 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_composite.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1699 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     6282 2023-06-14 06:46:41.000000 scikit-fem-8.1.0/skfem/element/element_global.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      898 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_h1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2595 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_hcurl.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1767 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_hdiv.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.721932 scikit-fem-8.1.0/skfem/element/element_hex/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      365 2023-06-14 06:46:41.000000 scikit-fem-8.1.0/skfem/element/element_hex/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      424 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_hex/element_hex0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2241 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_hex/element_hex1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    30688 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_hex/element_hex2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3523 2023-06-14 06:46:41.000000 scikit-fem-8.1.0/skfem/element/element_hex/element_hex_c1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1219 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_hex/element_hex_rt1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2887 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_hex/element_hex_s2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      653 2023-06-02 20:13:04.000000 scikit-fem-8.1.0/skfem/element/element_hex/element_hex_skeleton0.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.724979 scikit-fem-8.1.0/skfem/element/element_line/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      337 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_line/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      687 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_line/element_line_hermite.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      794 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_line/element_line_mini.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      404 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_line/element_line_p0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      686 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_line/element_line_p1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      770 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_line/element_line_p2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1647 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_line/element_line_pp.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      825 2023-04-19 14:25:14.000000 scikit-fem-8.1.0/skfem/element/element_matrix.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.728906 scikit-fem-8.1.0/skfem/element/element_quad/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      416 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      423 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/element_quad0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      958 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/element_quad1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2501 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/element_quad2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1242 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/element_quad_bfs.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      931 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/element_quad_n1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      755 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/element_quad_rt1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2044 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/element_quad_s2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2618 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_quad/element_quadp.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.733024 scikit-fem-8.1.0/skfem/element/element_tet/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      466 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     6214 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_ccr.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1072 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_cr.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1346 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_mini.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1685 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_n1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      409 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_p0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1117 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_p1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2799 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_p2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      901 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_rt1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      564 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tet/element_tet_skeleton_p0.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.742517 scikit-fem-8.1.0/skfem/element/element_tri/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1212 2023-04-19 14:25:14.000000 scikit-fem-8.1.0/skfem/element/element_tri/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1995 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_15param_plate.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1961 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_argyris.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2028 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_bdm1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1423 2023-04-15 15:49:59.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_bell.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      789 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_cr.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1184 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_hermite.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2562 2023-04-19 14:25:14.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_hhj.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1102 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_morley.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      761 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_n1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1844 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_n2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      405 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      846 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1049 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p1b.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      570 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p1g.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1399 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1692 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p2b.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      854 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p2g.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3929 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p3.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     8967 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p4.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      744 2023-02-14 20:19:31.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_rt1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1695 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_rt2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      511 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_skeleton_p0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1003 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_tri/element_tri_skeleton_p1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1653 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_vector.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1532 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/element/element_wedge_1.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.742876 scikit-fem-8.1.0/skfem/experimental/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      203 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/experimental/__init__.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.743614 scikit-fem-8.1.0/skfem/experimental/autodiff/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3172 2023-04-12 07:43:17.000000 scikit-fem-8.1.0/skfem/experimental/autodiff/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2006 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/experimental/autodiff/helpers.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.743936 scikit-fem-8.1.0/skfem/experimental/supermeshing/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2739 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/experimental/supermeshing/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1203 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/generic_utils.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     6226 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/helpers.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.745161 scikit-fem-8.1.0/skfem/io/
+-rw-r--r--   0 gustaft1   (502) staff       (20)       40 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/io/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2178 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/io/json.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     8834 2023-01-26 14:13:49.000000 scikit-fem-8.1.0/skfem/io/meshio.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.747211 scikit-fem-8.1.0/skfem/mapping/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      418 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mapping/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2882 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mapping/mapping.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     8056 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mapping/mapping_affine.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     8614 2023-06-04 15:41:44.000000 scikit-fem-8.1.0/skfem/mapping/mapping_isoparametric.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     7795 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mapping/mapping_mortar.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.754878 scikit-fem-8.1.0/skfem/mesh/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2701 2023-06-04 15:41:44.000000 scikit-fem-8.1.0/skfem/mesh/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    42111 2023-03-29 11:20:10.000000 scikit-fem-8.1.0/skfem/mesh/mesh.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      693 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_2d.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      367 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_2d_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1823 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_3d.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3606 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5486 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_hex_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      325 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_hex_1_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1413 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_hex_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2764 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_line_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      386 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_line_1_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     7163 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_quad_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      334 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_quad_1_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      864 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_quad_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      835 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_simplex.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    13604 2023-03-30 11:56:55.000000 scikit-fem-8.1.0/skfem/mesh/mesh_tet_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1923 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_tet_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    14811 2023-06-02 20:13:04.000000 scikit-fem-8.1.0/skfem/mesh/mesh_tri_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      748 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_tri_1_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1587 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_tri_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1363 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/mesh/mesh_wedge_1.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.756379 scikit-fem-8.1.0/skfem/models/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      152 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/models/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1129 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/models/elasticity.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      432 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/models/general.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      369 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/models/poisson.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)   121022 2023-06-04 15:41:44.000000 scikit-fem-8.1.0/skfem/quadrature.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     7610 2023-06-04 15:41:44.000000 scikit-fem-8.1.0/skfem/refdom.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    23201 2023-03-14 21:13:16.000000 scikit-fem-8.1.0/skfem/utils.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.758116 scikit-fem-8.1.0/skfem/visuals/
+-rw-r--r--   0 gustaft1   (502) staff       (20)        7 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/visuals/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1907 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/visuals/glvis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    11959 2023-05-11 04:57:40.000000 scikit-fem-8.1.0/skfem/visuals/matplotlib.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5232 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/visuals/svg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      690 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/skfem/visuals/vedo.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2023-06-16 20:23:38.765723 scikit-fem-8.1.0/tests/
+-rw-r--r--   0 gustaft1   (502) staff       (20)    19938 2023-01-19 20:25:59.000000 scikit-fem-8.1.0/tests/test_assembly.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    20769 2023-03-03 20:36:48.000000 scikit-fem-8.1.0/tests/test_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    14690 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/tests/test_convergence.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4077 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/tests/test_convergence_h2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     6407 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/tests/test_convergence_hdiv.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3249 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/tests/test_dofs.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    11550 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/tests/test_elements.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    10036 2023-04-19 14:25:14.000000 scikit-fem-8.1.0/tests/test_examples.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    12824 2023-01-19 20:25:59.000000 scikit-fem-8.1.0/tests/test_manufactured.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3785 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/tests/test_mapping.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    18974 2023-03-27 08:52:51.000000 scikit-fem-8.1.0/tests/test_mesh.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3219 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/tests/test_p_convergence.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4732 2023-02-14 18:46:32.000000 scikit-fem-8.1.0/tests/test_utils.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1950 2023-01-19 20:24:53.000000 scikit-fem-8.1.0/tests/test_visuals.py
```

### Comparing `scikit-fem-8.0.0/LICENSE` & `scikit-fem-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/PKG-INFO` & `scikit-fem-8.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-fem
-Version: 8.0.0
+Version: 8.1.0
 Summary: Simple finite element assemblers
 Home-page: https://github.com/kinnala/scikit-fem
 Author: Tom Gustafsson
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/kinnala/scikit-fem
 Project-URL: Issues, https://github.com/kinnala/scikit-fem/issues
 Classifier: Intended Audience :: Science/Research
@@ -233,14 +233,31 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
 with respect to documented and/or tested features.
 
 ### Unreleased
 
+## [8.1.0] - 2023-06-16
+
+- Added: `ElementTriHHJ0` and `ElementTriHHJ1` matrix finite elements
+  for implementing the Hellan-Hermann-Johnson mixed method (see [`ex48.py`](https://github.com/kinnala/scikit-fem/blob/master/docs/examples/ex48.py))
+- Added: `ElementHexSkeleton0`, piecewise constant element on the skeleton
+  of a hexahedral mesh
+- Added: `ElementHexC1`, C1-continuous hexahedral element
+- Added: `Mesh.restrict` now preserves subdomains and boundaries
+- Added: `skfem.utils.mpc` for setting multipoint constraints
+- Added: `Basis.get_dofs` now supports fetching DOFs at specific nodes
+  through kwarg `nodes`
+- Added: `DofsView.sort` for sorting a set of DOFs returned by
+  `Basis.get_dofs`
+- Added: `CellBasis.with_elements` as a shortcut for initiating a new Basis with subset of elements
+- Added: `Mesh.refined` now preserves subdomains in adaptive mesh refinement
+- Fixed: `Mesh.refined` used to modify the element connectivity of the original mesh
+
 ## [8.0.0] - 2022-12-16
 
 - Removed: The deprecated `Basis.find_dofs` method, see `Basis.get_dofs` for a
   replacement
 - Added: Renamed `ElementTetN0` to `ElementTriN1` and added alias for backwards
   compatibility
 - Added: `ElementQuadN1`, first order H(curl) conforming quadrilateral element
```

### Comparing `scikit-fem-8.0.0/README.md` & `scikit-fem-8.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,31 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
 with respect to documented and/or tested features.
 
 ### Unreleased
 
+## [8.1.0] - 2023-06-16
+
+- Added: `ElementTriHHJ0` and `ElementTriHHJ1` matrix finite elements
+  for implementing the Hellan-Hermann-Johnson mixed method (see [`ex48.py`](https://github.com/kinnala/scikit-fem/blob/master/docs/examples/ex48.py))
+- Added: `ElementHexSkeleton0`, piecewise constant element on the skeleton
+  of a hexahedral mesh
+- Added: `ElementHexC1`, C1-continuous hexahedral element
+- Added: `Mesh.restrict` now preserves subdomains and boundaries
+- Added: `skfem.utils.mpc` for setting multipoint constraints
+- Added: `Basis.get_dofs` now supports fetching DOFs at specific nodes
+  through kwarg `nodes`
+- Added: `DofsView.sort` for sorting a set of DOFs returned by
+  `Basis.get_dofs`
+- Added: `CellBasis.with_elements` as a shortcut for initiating a new Basis with subset of elements
+- Added: `Mesh.refined` now preserves subdomains in adaptive mesh refinement
+- Fixed: `Mesh.refined` used to modify the element connectivity of the original mesh
+
 ## [8.0.0] - 2022-12-16
 
 - Removed: The deprecated `Basis.find_dofs` method, see `Basis.get_dofs` for a
   replacement
 - Added: Renamed `ElementTetN0` to `ElementTriN1` and added alias for backwards
   compatibility
 - Added: `ElementQuadN1`, first order H(curl) conforming quadrilateral element
```

### Comparing `scikit-fem-8.0.0/scikit_fem.egg-info/PKG-INFO` & `scikit-fem-8.1.0/scikit_fem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-fem
-Version: 8.0.0
+Version: 8.1.0
 Summary: Simple finite element assemblers
 Home-page: https://github.com/kinnala/scikit-fem
 Author: Tom Gustafsson
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/kinnala/scikit-fem
 Project-URL: Issues, https://github.com/kinnala/scikit-fem/issues
 Classifier: Intended Audience :: Science/Research
@@ -233,14 +233,31 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
 with respect to documented and/or tested features.
 
 ### Unreleased
 
+## [8.1.0] - 2023-06-16
+
+- Added: `ElementTriHHJ0` and `ElementTriHHJ1` matrix finite elements
+  for implementing the Hellan-Hermann-Johnson mixed method (see [`ex48.py`](https://github.com/kinnala/scikit-fem/blob/master/docs/examples/ex48.py))
+- Added: `ElementHexSkeleton0`, piecewise constant element on the skeleton
+  of a hexahedral mesh
+- Added: `ElementHexC1`, C1-continuous hexahedral element
+- Added: `Mesh.restrict` now preserves subdomains and boundaries
+- Added: `skfem.utils.mpc` for setting multipoint constraints
+- Added: `Basis.get_dofs` now supports fetching DOFs at specific nodes
+  through kwarg `nodes`
+- Added: `DofsView.sort` for sorting a set of DOFs returned by
+  `Basis.get_dofs`
+- Added: `CellBasis.with_elements` as a shortcut for initiating a new Basis with subset of elements
+- Added: `Mesh.refined` now preserves subdomains in adaptive mesh refinement
+- Fixed: `Mesh.refined` used to modify the element connectivity of the original mesh
+
 ## [8.0.0] - 2022-12-16
 
 - Removed: The deprecated `Basis.find_dofs` method, see `Basis.get_dofs` for a
   replacement
 - Added: Renamed `ElementTetN0` to `ElementTriN1` and added alias for backwards
   compatibility
 - Added: `ElementQuadN1`, first order H(curl) conforming quadrilateral element
```

### Comparing `scikit-fem-8.0.0/scikit_fem.egg-info/SOURCES.txt` & `scikit-fem-8.1.0/scikit_fem.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -34,23 +34,25 @@
 skfem/element/element.py
 skfem/element/element_composite.py
 skfem/element/element_dg.py
 skfem/element/element_global.py
 skfem/element/element_h1.py
 skfem/element/element_hcurl.py
 skfem/element/element_hdiv.py
-skfem/element/element_skeleton.py
+skfem/element/element_matrix.py
 skfem/element/element_vector.py
 skfem/element/element_wedge_1.py
 skfem/element/element_hex/__init__.py
 skfem/element/element_hex/element_hex0.py
 skfem/element/element_hex/element_hex1.py
 skfem/element/element_hex/element_hex2.py
+skfem/element/element_hex/element_hex_c1.py
 skfem/element/element_hex/element_hex_rt1.py
 skfem/element/element_hex/element_hex_s2.py
+skfem/element/element_hex/element_hex_skeleton0.py
 skfem/element/element_line/__init__.py
 skfem/element/element_line/element_line_hermite.py
 skfem/element/element_line/element_line_mini.py
 skfem/element/element_line/element_line_p0.py
 skfem/element/element_line/element_line_p1.py
 skfem/element/element_line/element_line_p2.py
 skfem/element/element_line/element_line_pp.py
@@ -67,23 +69,24 @@
 skfem/element/element_tet/element_tet_ccr.py
 skfem/element/element_tet/element_tet_cr.py
 skfem/element/element_tet/element_tet_mini.py
 skfem/element/element_tet/element_tet_n1.py
 skfem/element/element_tet/element_tet_p0.py
 skfem/element/element_tet/element_tet_p1.py
 skfem/element/element_tet/element_tet_p2.py
-skfem/element/element_tet/element_tet_p3.py
 skfem/element/element_tet/element_tet_rt1.py
 skfem/element/element_tet/element_tet_skeleton_p0.py
 skfem/element/element_tri/__init__.py
 skfem/element/element_tri/element_tri_15param_plate.py
 skfem/element/element_tri/element_tri_argyris.py
 skfem/element/element_tri/element_tri_bdm1.py
+skfem/element/element_tri/element_tri_bell.py
 skfem/element/element_tri/element_tri_cr.py
 skfem/element/element_tri/element_tri_hermite.py
+skfem/element/element_tri/element_tri_hhj.py
 skfem/element/element_tri/element_tri_morley.py
 skfem/element/element_tri/element_tri_n1.py
 skfem/element/element_tri/element_tri_n2.py
 skfem/element/element_tri/element_tri_p0.py
 skfem/element/element_tri/element_tri_p1.py
 skfem/element/element_tri/element_tri_p1b.py
 skfem/element/element_tri/element_tri_p1g.py
@@ -99,15 +102,14 @@
 skfem/experimental/__init__.py
 skfem/experimental/autodiff/__init__.py
 skfem/experimental/autodiff/helpers.py
 skfem/experimental/supermeshing/__init__.py
 skfem/io/__init__.py
 skfem/io/json.py
 skfem/io/meshio.py
-skfem/io/mfem.py
 skfem/mapping/__init__.py
 skfem/mapping/mapping.py
 skfem/mapping/mapping_affine.py
 skfem/mapping/mapping_isoparametric.py
 skfem/mapping/mapping_mortar.py
 skfem/mesh/__init__.py
 skfem/mesh/mesh.py
@@ -134,8 +136,22 @@
 skfem/models/elasticity.py
 skfem/models/general.py
 skfem/models/poisson.py
 skfem/visuals/__init__.py
 skfem/visuals/glvis.py
 skfem/visuals/matplotlib.py
 skfem/visuals/svg.py
-skfem/visuals/vedo.py
+skfem/visuals/vedo.py
+tests/test_assembly.py
+tests/test_basis.py
+tests/test_convergence.py
+tests/test_convergence_h2.py
+tests/test_convergence_hdiv.py
+tests/test_dofs.py
+tests/test_elements.py
+tests/test_examples.py
+tests/test_manufactured.py
+tests/test_mapping.py
+tests/test_mesh.py
+tests/test_p_convergence.py
+tests/test_utils.py
+tests/test_visuals.py
```

### Comparing `scikit-fem-8.0.0/setup.cfg` & `scikit-fem-8.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-fem
-version = 8.0.0
+version = 8.1.0
 author = Tom Gustafsson
 description = Simple finite element assemblers
 url = https://github.com/kinnala/scikit-fem
 project_urls = 
 	Code=https://github.com/kinnala/scikit-fem
 	Issues=https://github.com/kinnala/scikit-fem/issues
 long_description = file: README.md
```

### Comparing `scikit-fem-8.0.0/skfem/__init__.py` & `scikit-fem-8.1.0/skfem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     'condense',
     'enforce',
     'penalize',
     'project',  # TODO remove due to deprecation
     'projection',  # TODO remove due to deprecation
     'solve',
     'bmat',
+    'mpc',
     'solver_direct_scipy',
     'solver_eigen_scipy',
     'solver_eigen_scipy_sym',
     'solver_iter_pcg',
     'solver_iter_krylov',
     'solver_iter_cg',
     '__version__',
```

### Comparing `scikit-fem-8.0.0/skfem/assembly/__init__.py` & `scikit-fem-8.1.0/skfem/assembly/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/basis/abstract_basis.py` & `scikit-fem-8.1.0/skfem/assembly/basis/abstract_basis.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,15 @@
             # if a dict of Dofs objects are given, flatten all
             D = tuple(D[0][key].all() for key in D[0])
         return np.setdiff1d(np.arange(self.N), np.concatenate(D))
 
     def get_dofs(self,
                  facets: Optional[Any] = None,
                  elements: Optional[Any] = None,
+                 nodes: Optional[Any] = None,
                  skip: Optional[List[str]] = None) -> Any:
         """Find global DOF numbers.
 
         Accepts an array of facet/element indices.  However, various argument
         types can be turned into an array of facet/element indices.
 
         Get all boundary DOFs:
@@ -204,14 +205,16 @@
             An array of facet indices.  If ``None``, find facets by
             ``self.mesh.boundary_facets()``.  If callable, call
             ``self.mesh.facets_satisfying(facets)`` to get the facets.  If
             string, use ``self.mesh.boundaries[facets]`` to get the facets.
             If list, tuple or set, use the combined facet indices.
         elements
             An array of element indices.  See above.
+        nodes
+            An array of node indices.
         skip
             List of dofnames to skip.
 
         """
         if isinstance(facets, dict):
             warn("Passing dict to get_dofs is deprecated.", DeprecationWarning)
 
@@ -220,23 +223,29 @@
                     return self.mesh.facets_satisfying(f)
                 return f
 
             return {k: self.dofs.get_facet_dofs(to_indices(facets[k]),
                                                 skip_dofnames=skip)
                     for k in facets}
 
-        if elements is not None and facets is not None:
-            raise ValueError
-
         if elements is not None:
             elements = self.mesh.normalize_elements(elements)
-            return self.dofs.get_element_dofs(elements, skip_dofnames=skip)
+            return self.dofs.get_element_dofs(elements,
+                                              skip_dofnames=skip,
+                                              doflocs=self.doflocs)
+        elif nodes is not None:
+            nodes = self.mesh.normalize_nodes(nodes)
+            return self.dofs.get_vertex_dofs(nodes,
+                                             skip_dofnames=skip,
+                                             doflocs=self.doflocs)
 
         facets = self.mesh.normalize_facets(facets)
-        return self.dofs.get_facet_dofs(facets, skip_dofnames=skip)
+        return self.dofs.get_facet_dofs(facets,
+                                        skip_dofnames=skip,
+                                        doflocs=self.doflocs)
 
     def __repr__(self):
         size = sum([sum([y.size if hasattr(y, 'size') else 0
                          for y in x.astuple])
                     for x in self.basis[0]]) * 8 * len(self.basis)
         rep = ""
         rep += "<skfem {}({}, {}) object>\n".format(type(self).__name__,
```

### Comparing `scikit-fem-8.0.0/skfem/assembly/basis/cell_basis.py` & `scikit-fem-8.1.0/skfem/assembly/basis/cell_basis.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,24 @@
             self.mesh,
             elem,
             mapping=self.mapping,
             quadrature=self.quadrature,
             elements=self.tind,
         )
 
+    def with_elements(self, elements: Optional[Any] = None) -> 'CellBasis':
+        """Return a similar basis on a subset of element indices."""
+        return type(self)(
+            self.mesh,
+            self.elem,
+            mapping=self.mapping,
+            quadrature=self.quadrature,
+            elements=elements,
+        )
+
     def boundary(self,
                  facets: Optional[Any] = None,
                  intorder: Optional[int] = None,
                  quadrature: Optional[Tuple[ndarray, ndarray]] = None):
         """Return corresponding :class:`~skfem.assembly.basis.FacetBasis`.
 
         Parameters
```

### Comparing `scikit-fem-8.0.0/skfem/assembly/basis/facet_basis.py` & `scikit-fem-8.1.0/skfem/assembly/basis/facet_basis.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/basis/interior_facet_basis.py` & `scikit-fem-8.1.0/skfem/assembly/basis/interior_facet_basis.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/basis/mortar_facet_basis.py` & `scikit-fem-8.1.0/skfem/assembly/basis/mortar_facet_basis.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/dofs.py` & `scikit-fem-8.1.0/skfem/assembly/dofs.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         default_factory=lambda: slice(None))
     facet_rows: Union[ndarray, slice] = field(
         default_factory=lambda: slice(None))
     edge_rows: Union[ndarray, slice] = field(
         default_factory=lambda: slice(None))
     interior_rows: Union[ndarray, slice] = field(
         default_factory=lambda: slice(None))
+    doflocs: Any = None
 
     def __repr__(self):
         nnodal = len(np.unique(
             self.obj.nodal_dofs[self.nodal_rows][:, self.nodal_ix]
         ))
         nfacet = len(np.unique(
             self.obj.facet_dofs[self.facet_rows][:, self.facet_ix]
@@ -74,14 +75,17 @@
                           + self.obj.edge_dofs.shape[0]):][self.interior_rows],
             )
         return rep
 
     def __str__(self):
         return self.__repr__()
 
+    def __len__(self):
+        return len(self.flatten())
+
     def flatten(self) -> ndarray:
         """Return all DOF indices as a single array."""
         return np.unique(
             np.concatenate((
                 (self.obj
                  .nodal_dofs[self.nodal_rows][:, self.nodal_ix]
                  .flatten()),
@@ -93,14 +97,32 @@
                  .flatten()),
                 (self.obj
                  .interior_dofs[self.interior_rows][:, self.interior_ix]
                  .flatten())
             ))
         )
 
+    def sort(self, sorting=None) -> ndarray:
+        """Sort a set of DOFs based on output value of a given function.
+
+        Parameters
+        ----------
+        sorting
+            Optionally, specify a function which takes in a set of DOF
+            locations and outputs a number.  Used for sorting the
+            DOFs.  By default, the function "sum(x)" is used.
+
+        """
+        if sorting is None:
+            def sorting(x):
+                return sum(x)
+        dofs = self.flatten()
+        ix = np.argsort(sorting(self.doflocs[:, dofs]))
+        return dofs[ix]
+
     def _intersect(self, a, b):
         if isinstance(a, slice):
             if a.start == 0:
                 return a
             return b
         if isinstance(b, slice):
             if b.start == 0:
@@ -300,18 +322,54 @@
         # interior dofs
         self.element_dofs = np.vstack((self.element_dofs,
                                        self.interior_dofs))
 
         # total dofs
         self.N = np.max(self.element_dofs) + 1
 
+    def get_vertex_dofs(
+            self,
+            nodes: ndarray,
+            skip_dofnames: Optional[List[str]] = None,
+            doflocs: Optional[ndarray] = None
+    ) -> DofsView:
+        """Return a subset of DOFs corresponding to the given nodes.
+
+        Parameters
+        ----------
+        nodes
+            An array of vertex indices.
+        skip_dofnames
+            An array of dofnames to skip.
+
+        """
+        if skip_dofnames is None:
+            skip_dofnames = []
+
+        r1, r2, r3, r4 = self._dofnames_to_rows(skip_dofnames, skip=True)
+
+        return DofsView(
+            self,
+            nodes,
+            np.empty((0,), dtype=np.int64),
+            np.empty((0,), dtype=np.int64),
+            np.empty((0,), dtype=np.int64),
+            r1,
+            r2,
+            r3,
+            r4,
+            doflocs
+        )
+
     def get_element_dofs(
             self,
             elements: ndarray,
-            skip_dofnames: Optional[List[str]] = None) -> DofsView:
+            skip_dofnames: Optional[List[str]] = None,
+            doflocs: Optional[ndarray] = None
+    ) -> DofsView:
         """Return a subset of DOFs corresponding to the given elements.
 
         Parameters
         ----------
         elements
             An array of element indices.
         skip_dofnames
@@ -328,26 +386,35 @@
                     if self.element.facet_dofs == 0
                     else np.unique(self.topo.t2f[:, elements]))
         interior_ix = elements
 
         if skip_dofnames is None:
             skip_dofnames = []
 
+        r1, r2, r3, r4 = self._dofnames_to_rows(skip_dofnames, skip=True)
+
         return DofsView(
             self,
             nodal_ix,
             facet_ix,
             edge_ix,
             interior_ix,
-            *self._dofnames_to_rows(skip_dofnames, skip=True)
+            r1,
+            r2,
+            r3,
+            r4,
+            doflocs
         )
 
-    def get_facet_dofs(self,
-                       facets: ndarray,
-                       skip_dofnames: Optional[List[str]] = None) -> DofsView:
+    def get_facet_dofs(
+            self,
+            facets: ndarray,
+            skip_dofnames: Optional[List[str]] = None,
+            doflocs: Optional[ndarray] = None
+    ) -> DofsView:
         """Return a subset of DOFs corresponding to the given facets.
 
         Parameters
         ----------
         facets
             An array of facet indices.
         skip_dofnames
@@ -366,21 +433,27 @@
         facet_ix = (np.empty((0,), dtype=np.int64)
                     if self.element.facet_dofs == 0
                     else facets)
 
         if skip_dofnames is None:
             skip_dofnames = []
 
+        r1, r2, r3, r4 = self._dofnames_to_rows(skip_dofnames, skip=True)
+
         return DofsView(
             self,
             nodal_ix,
             facet_ix,
             edge_ix,
-            np.empty((0,), dtype=np.int64),
-            *self._dofnames_to_rows(skip_dofnames, skip=True)
+            np.empty((0,), dtype=np.uint64),
+            r1,
+            r2,
+            r3,
+            r4,
+            doflocs
         )
 
     def _by_name(self,
                  dofs: ndarray,
                  off: int = 0,
                  ix: Optional[ndarray] = None,
                  rows: Optional[Union[List[int], ndarray]] = None):
```

### Comparing `scikit-fem-8.0.0/skfem/assembly/form/bilinear_form.py` & `scikit-fem-8.1.0/skfem/assembly/form/bilinear_form.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/form/coo_data.py` & `scikit-fem-8.1.0/skfem/assembly/form/coo_data.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/form/form.py` & `scikit-fem-8.1.0/skfem/assembly/form/form.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/form/functional.py` & `scikit-fem-8.1.0/skfem/assembly/form/functional.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/form/linear_form.py` & `scikit-fem-8.1.0/skfem/assembly/form/linear_form.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/assembly/form/trilinear_form.py` & `scikit-fem-8.1.0/skfem/assembly/form/trilinear_form.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/__init__.py` & `scikit-fem-8.1.0/skfem/element/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 from .element_tri import (ElementTriP1, ElementTriP2, ElementTriP0,
                           ElementTriRT1, ElementTriMorley, ElementTriArgyris,
                           ElementTriP1B, ElementTriCR, ElementTriHermite,
                           ElementTriP1DG, ElementTriSkeletonP0,
                           ElementTriSkeletonP1, ElementTriP3, ElementTriP4,
                           ElementTri15ParamPlate, ElementTriBDM1,
                           ElementTriP1G, ElementTriP2G, ElementTriP2B,
-                          ElementTriRT2, ElementTriN1, ElementTriN2)  # noqa
+                          ElementTriRT2, ElementTriN1, ElementTriN2,
+                          ElementTriHHJ0, ElementTriHHJ1)  # noqa
 from .element_quad import (ElementQuad0, ElementQuad1, ElementQuad2,  # noqa
                            ElementQuadS2, ElementQuadP,
                            ElementQuadBFS, ElementQuadRT1, ElementQuad1DG,
                            ElementQuadN1)
 from .element_tet import (ElementTetP0, ElementTetP1, ElementTetP2,  # noqa
                           ElementTetRT1, ElementTetN1, ElementTetMini,
                           ElementTetCR, ElementTetCCR, ElementTetSkeletonP0)
 from .element_hex import (ElementHex0, ElementHex1, ElementHex2,  # noqa
-                          ElementHexS2, ElementHex1DG, ElementHexRT1)
+                          ElementHexS2, ElementHex1DG, ElementHexRT1,
+                          ElementHexSkeleton0, ElementHexC1)
 from .element_line import (ElementLineP0, ElementLineP1, ElementLineP2,  # noqa
                            ElementLinePp, ElementLineHermite,
                            ElementLineMini, ElementLineP1DG)
 from .element_wedge_1 import ElementWedge1
 from .element_composite import ElementComposite  # noqa
 from .element_dg import ElementDG
 
@@ -102,14 +104,16 @@
     "ElementTriBDM1",
     "ElementTriP1G",
     "ElementTriP2G",
     "ElementTriP1B",
     "ElementTriP2B",
     "ElementTriN1",
     "ElementTriN2",
+    "ElementTriHHJ0",
+    "ElementTriHHJ1",
     "ElementQuad0",
     "ElementQuad1",
     "ElementQuad2",
     "ElementQuadS2",
     "ElementQuadDG",
     "ElementQuadP",
     "ElementQuadBFS",
@@ -132,16 +136,18 @@
     "ElementHex0",
     "ElementHex1",
     "ElementHex2",
     "ElementHexS2",
     "ElementHex1DG",
     "ElementHexDG",
     "ElementHexRT1",
+    "ElementHexSkeleton0",
     "ElementLineP0",
     "ElementLineP1",
     "ElementLineP1DG",
     "ElementLineP2",
     "ElementLinePp",
     "ElementLineHermite",
     "ElementLineMini",
     "ElementWedge1",
+    "ElementHexC1",
 ]
```

### Comparing `scikit-fem-8.0.0/skfem/element/discrete_field.py` & `scikit-fem-8.1.0/skfem/element/discrete_field.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element.py` & `scikit-fem-8.1.0/skfem/element/element.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_composite.py` & `scikit-fem-8.1.0/skfem/element/element_composite.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_dg.py` & `scikit-fem-8.1.0/skfem/element/element_dg.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_global.py` & `scikit-fem-8.1.0/skfem/element/element_global.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,16 @@
             maxdeg = int(maxdeg / 2)
         self._pbasis = {}
         for k in range(Ndiff + 1):
             diffs = list(itertools.product(*((list(range(dim)),) * k)))
             for diff in diffs:
                 #  desc = ''.join([str(d) for d in diff])
                 dx = sum([1 for d in diff if d == 0])
-                dy = sum([1 for d in diff if d == 1]) if dim == 2 else None
-                dz = sum([1 for d in diff if d == 2]) if dim == 3 else None
+                dy = sum([1 for d in diff if d == 1]) if dim >= 2 else None
+                dz = sum([1 for d in diff if d == 2]) if dim >= 3 else None
                 if dim == 1:
                     self._pbasis[diff] = [
                         self._pbasis_create(i=i, dx=dx)
                         for i in range(maxdeg + 1)
                         if i <= maxdeg
                     ]
                 elif dim == 2:
@@ -147,15 +147,15 @@
 
         N = len(self._pbasis[()])
         V = np.zeros((len(tind), N, N))
         w = {
             'v': np.array([mesh.p[:, mesh.t[itr, tind]]
                            for itr in range(mesh.t.shape[0])]),
         }
-        if mesh.p.shape[0] >= 2:
+        if mesh.p.shape[0] == 2:
             w['e'] = np.array([
                 .5 * (w['v'][itr] + w['v'][(itr + 1) % mesh.t.shape[0]])
                 for itr in range(mesh.t.shape[0])
             ])
             w['n'] = np.array([
                 w['v'][itr] - w['v'][(itr + 1) % mesh.t.shape[0]]
                 for itr in range(mesh.t.shape[0])
```

### Comparing `scikit-fem-8.0.0/skfem/element/element_h1.py` & `scikit-fem-8.1.0/skfem/element/element_h1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_hcurl.py` & `scikit-fem-8.1.0/skfem/element/element_hcurl.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_hdiv.py` & `scikit-fem-8.1.0/skfem/element/element_hdiv.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_hex/element_hex1.py` & `scikit-fem-8.1.0/skfem/element/element_hex/element_hex1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_hex/element_hex2.py` & `scikit-fem-8.1.0/skfem/element/element_hex/element_hex2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_hex/element_hex_rt1.py` & `scikit-fem-8.1.0/skfem/element/element_hex/element_hex_rt1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_hex/element_hex_s2.py` & `scikit-fem-8.1.0/skfem/element/element_hex/element_hex_s2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_line/element_line_hermite.py` & `scikit-fem-8.1.0/skfem/element/element_line/element_line_hermite.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_line/element_line_mini.py` & `scikit-fem-8.1.0/skfem/element/element_line/element_line_mini.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_line/element_line_p1.py` & `scikit-fem-8.1.0/skfem/element/element_line/element_line_p1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_line/element_line_p2.py` & `scikit-fem-8.1.0/skfem/element/element_line/element_line_p2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_line/element_line_pp.py` & `scikit-fem-8.1.0/skfem/element/element_line/element_line_pp.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_quad/element_quad1.py` & `scikit-fem-8.1.0/skfem/element/element_quad/element_quad1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_quad/element_quad2.py` & `scikit-fem-8.1.0/skfem/element/element_quad/element_quad2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_quad/element_quad_bfs.py` & `scikit-fem-8.1.0/skfem/element/element_quad/element_quad_bfs.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_quad/element_quad_n1.py` & `scikit-fem-8.1.0/skfem/element/element_quad/element_quad_n1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_quad/element_quad_rt1.py` & `scikit-fem-8.1.0/skfem/element/element_quad/element_quad_rt1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_quad/element_quad_s2.py` & `scikit-fem-8.1.0/skfem/element/element_quad/element_quad_s2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_quad/element_quadp.py` & `scikit-fem-8.1.0/skfem/element/element_quad/element_quadp.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_skeleton.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_wedge_1.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,54 @@
+from dataclasses import dataclass, field
+from typing import Type
+
 import numpy as np
+from numpy import ndarray
+
+from ..element import Element, ElementWedge1
+from .mesh_3d import Mesh3D
+from .mesh_tet_1 import MeshTet1
+
+
+@dataclass(repr=False)
+class MeshWedge1(Mesh3D):
+
+    doflocs: ndarray = field(
+        default_factory=lambda: np.array(
+            [
+                [0.0, 0.0, 0.0],
+                [0.0, 0.0, 1.0],
+                [0.0, 1.0, 0.0],
+                [1.0, 0.0, 0.0],
+                [0.0, 1.0, 1.0],
+                [1.0, 0.0, 1.0],
+                [1.0, 1.0, 0.0],
+                [1.0, 1.0, 1.0],
+            ],
+            dtype=np.float64,
+        ).T
+    )
+    t: ndarray = field(
+        default_factory=lambda: np.array(
+            [[0, 2, 3, 1, 4, 5], [2, 3, 6, 4, 5, 7]], dtype=np.int64
+        ).T
+    )
+    elem: Type[Element] = ElementWedge1
+
+    def to_meshtet(self):
+
+        t = np.hstack((
+            self.t[[0, 1, 2, 3]],
+            self.t[[1, 2, 3, 4]],
+            self.t[[2, 3, 4, 5]],
+        ))
+
+        return MeshTet1(self.doflocs, t)
+
+    def element_finder(self, mapping=None):
+        """Transform to :class:`skfem.MeshTet` and return its finder."""
+        tet_finder = self.to_meshtet().element_finder()
+
+        def finder(*args):
+            return tet_finder(*args) % self.t.shape[1]
 
-from .element_h1 import ElementH1
-from .element_dg import ElementDG
-from .element_line import ElementLinePp
-
-class ElementSkeleton(ElementH1):
-
-    def __init__(self, refdom, p):
-        self.refdom = refdom
-        self.elem = ElementDG(ElementLinePp(p))
-        self.facet_dofs = self.elem.interior_dofs
-        self.dofnames = ['u', 'u']
-        self.doflocs = np.array([[.0, .0],
-                                 [1., .0],
-                                 [1., .0],
-                                 [.0, 1.],
-                                 [.0, .0],
-                                 [.0, 1.]])
-
-    def lbasis(self, X, i):
-        if i in range(self.refdom.nfacets * self.facet_dofs):
-            facet_ix = int(i / self.facet_dofs)
-            if facet_ix == 0:
-                coord = slice(0, 1)
-            else:
-                coord = slice(1, 2)
-            basis_ix = i % self.facet_dofs
-            return (
-                (self.elem.lbasis(X[coord], basis_ix)[0]
-                 * self.refdom.on_facet(facet_ix, X)),
-                0. * X
-            )
-        self._index_error()
+        return finder
```

### Comparing `scikit-fem-8.0.0/skfem/element/element_tet/element_tet_ccr.py` & `scikit-fem-8.1.0/skfem/element/element_tet/element_tet_ccr.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tet/element_tet_cr.py` & `scikit-fem-8.1.0/skfem/element/element_tet/element_tet_cr.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tet/element_tet_mini.py` & `scikit-fem-8.1.0/skfem/element/element_tet/element_tet_mini.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tet/element_tet_n1.py` & `scikit-fem-8.1.0/skfem/element/element_tet/element_tet_n1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tet/element_tet_p1.py` & `scikit-fem-8.1.0/skfem/element/element_tet/element_tet_p1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tet/element_tet_p2.py` & `scikit-fem-8.1.0/skfem/element/element_tet/element_tet_p2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tet/element_tet_rt1.py` & `scikit-fem-8.1.0/skfem/element/element_tet/element_tet_rt1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tet/element_tet_skeleton_p0.py` & `scikit-fem-8.1.0/skfem/element/element_tet/element_tet_skeleton_p0.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/__init__.py` & `scikit-fem-8.1.0/skfem/element/element_tri/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 from .element_tri_skeleton_p0 import ElementTriSkeletonP0  # noqa
 from .element_tri_skeleton_p1 import ElementTriSkeletonP1  # noqa
 from .element_tri_p1g import ElementTriP1G  # noqa
 from .element_tri_p2g import ElementTriP2G  # noqa
 from .element_tri_p2b import ElementTriP2B  # noqa
 from .element_tri_n1 import ElementTriN1  # noqa
 from .element_tri_n2 import ElementTriN2  # noqa
+from .element_tri_hhj import ElementTriHHJ0, ElementTriHHJ1  # noqa
```

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_15param_plate.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_15param_plate.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_argyris.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_argyris.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_bdm1.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_bdm1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_cr.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_cr.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_hermite.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_hermite.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_morley.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_morley.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_n1.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_n1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_n2.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_n2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p1.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p1b.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p1b.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p1g.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p1g.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p2.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p2b.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p2b.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p2g.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p2g.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p3.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p3.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_p4.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_p4.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_rt1.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_rt1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_rt2.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_rt2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_tri/element_tri_skeleton_p1.py` & `scikit-fem-8.1.0/skfem/element/element_tri/element_tri_skeleton_p1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_vector.py` & `scikit-fem-8.1.0/skfem/element/element_vector.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/element/element_wedge_1.py` & `scikit-fem-8.1.0/skfem/element/element_wedge_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/experimental/autodiff/__init__.py` & `scikit-fem-8.1.0/skfem/experimental/autodiff/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,33 +4,35 @@
 import numpy as np
 
 from autograd import make_jvp
 
 
 class NonlinearForm(Form):
 
-    def assemble(self, u0, basis, **kwargs):
+    def assemble(self, basis, x=None, **kwargs):
         """Assemble the Jacobian and the right-hand side.
 
         Parameters
         ----------
-        u0
-            The point at which the form is linearized.
         basis
             The basis used for all variables.
+        x
+            Optional point at which the form is linearized, default is zero.
 
         """
         # interpolate and cast to tuple
-        # make u0 compatible with u in forms
-        if isinstance(u0, ndarray):
-            u0 = basis.interpolate(u0)
-            if isinstance(u0, tuple):
-                u0 = tuple(c.astuple for c in u0)
+        # make x compatible with u in forms
+        if x is None:
+            x = basis.zeros()
+        if isinstance(x, ndarray):
+            x = basis.interpolate(x)
+            if isinstance(x, tuple):
+                x = tuple(c.astuple for c in x)
             else:
-                u0 = (u0.astuple,)
+                x = (x.astuple,)
 
         nt = basis.nelems
         dx = basis.dx
         w = FormExtraParams({
             **basis.default_parameters(),
             **self._normalize_asm_kwargs(kwargs, basis),
         })
@@ -44,25 +46,25 @@
         sz1 = basis.Nbfun * nt
         data1 = np.zeros(sz1, dtype=self.dtype)
         rows1 = np.zeros(sz1, dtype=np.int64)
 
         def _make_jacobian(V):
             if 'hessian' in self.params:
                 F = make_jvp(lambda U: self.form(*U, w))
-                return make_jvp(lambda W: F(W)(V)[1])(u0)
-            return make_jvp(lambda U: self.form(*U, *V, w))(u0)
+                return make_jvp(lambda W: F(W)(V)[1])(x)
+            return make_jvp(lambda U: self.form(*U, *V, w))(x)
 
         # # JAX version
         # def _make_jacobian(V):
         #     if 'hessian' in self.params:
         #         return linearize(
         #             lambda W: jvp(lambda U: self.form(*U, w), (W,), (V,))[1],
-        #             u0
+        #             x
         #         )
-        #     return linearize(lambda U: self.form(*U, *V, w), u0)
+        #     return linearize(lambda U: self.form(*U, *V, w), x)
 
         # loop over the indices of local stiffness matrix
         for i in range(basis.Nbfun):
             DF = _make_jacobian(tuple(c.astuple for c in basis.basis[i]))
             for j in range(basis.Nbfun):
                 y, DFU = DF(tuple(c.astuple for c in basis.basis[j]))
                 # Jacobian
@@ -83,12 +85,12 @@
                 np.array([rows, cols]),
                 data,
                 (basis.N, basis.N),
                 (basis.Nbfun, basis.Nbfun),
             ),
             COOData(
                 np.array([rows1]),
-                data1,
+                -data1,
                 (basis.N,),
                 (basis.Nbfun,)
             ).todefault()
         )
```

### Comparing `scikit-fem-8.0.0/skfem/experimental/autodiff/helpers.py` & `scikit-fem-8.1.0/skfem/experimental/autodiff/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 import autograd.numpy as np
+from autograd.builtins import isinstance
 
 from skfem import DiscreteField
 
 
 def dot(u, v):
+    if isinstance(u, tuple):
+        u = u[0]
+    if isinstance(v, tuple):
+        v = v[0]
     return np.einsum('i...,i...', u, v)
 
 
 def ddot(u, v):
+    if isinstance(u, tuple):
+        u = u[0]
+    if isinstance(v, tuple):
+        v = v[0]
     return np.einsum('ij...,ij...', u, v)
 
 
 def dddot(u, v):
+    if isinstance(u, tuple):
+        u = u[0]
+    if isinstance(v, tuple):
+        v = v[0]
     return np.einsum('ijk...,ijk...', u, v)
 
 
 def grad(u):
     if isinstance(u, DiscreteField):
         return u.grad
     return u[1]
@@ -36,24 +49,32 @@
 def dd(u):
     if isinstance(u, DiscreteField):
         return u.hess
     return u[4]
 
 
 def transpose(T):
+    if isinstance(T, tuple):
+        T = T[0]
     return np.einsum('ij...->ji...', T)
 
 
 def mul(A, B):
+    if isinstance(A, tuple):
+        A = A[0]
+    if isinstance(B, tuple):
+        B = B[0]
     if len(A.shape) == len(B.shape):
         return np.einsum('ij...,jk...->ik...', A, B)
     return np.einsum('ij...,j...->i...', A, B)
 
 
 def trace(T):
+    if isinstance(T, tuple):
+        T = T[0]
     return np.einsum('ii...', T)
 
 
 def eye(w, size):
     return np.array([[w if i == j else 0. * w for i in range(size)]
                      for j in range(size)])
```

### Comparing `scikit-fem-8.0.0/skfem/experimental/supermeshing/__init__.py` & `scikit-fem-8.1.0/skfem/experimental/supermeshing/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/generic_utils.py` & `scikit-fem-8.1.0/skfem/generic_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/helpers.py` & `scikit-fem-8.1.0/skfem/helpers.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/io/json.py` & `scikit-fem-8.1.0/skfem/io/json.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/io/meshio.py` & `scikit-fem-8.1.0/skfem/io/meshio.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         m.int_data_to_sets()
 
     subdomains = {}
     boundaries = {}
 
     # parse any subdomains from cell_sets
     if m.cell_sets:
-        subdomains = {k: v[meshio_type]
+        subdomains = {k: v[meshio_type].astype(np.uint64)
                       for k, v in m.cell_sets_dict.items()
                       if meshio_type in v}
 
     # create temporary mesh for matching boundary elements
     mtmp = mesh_type(p, t, validate=False)
     bnd_type = BOUNDARY_TYPE_MAPPING[meshio_type]
```

### Comparing `scikit-fem-8.0.0/skfem/mapping/mapping.py` & `scikit-fem-8.1.0/skfem/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mapping/mapping_affine.py` & `scikit-fem-8.1.0/skfem/mapping/mapping_affine.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mapping/mapping_isoparametric.py` & `scikit-fem-8.1.0/skfem/mapping/mapping_isoparametric.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mapping/mapping_mortar.py` & `scikit-fem-8.1.0/skfem/mapping/mapping_mortar.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/__init__.py` & `scikit-fem-8.1.0/skfem/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh.py` & `scikit-fem-8.1.0/skfem/mesh/mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,15 +190,16 @@
             subdomain.
 
         """
         return replace(
             self,
             _subdomains={
                 **({} if self._subdomains is None else self._subdomains),
-                **{name: self.elements_satisfying(test)
+                **{name: (self.elements_satisfying(test)
+                          if callable(test) else test)
                    for name, test in subdomains.items()},
             },
         )
 
     def _encode_point_data(self) -> Dict[str, List[ndarray]]:
 
         subdomains = {} if self._subdomains is None else self._subdomains
@@ -385,15 +386,15 @@
         ----------
         test
             A function which returns ``True`` for the element midpoints that
             are to be included in the return set.
 
         """
         midp = self.p[:, self.t].mean(axis=1)
-        return np.nonzero(test(midp))[0]
+        return np.nonzero(test(midp))[0].astype(np.uint64)
 
     def _expand_facets(self, ix: ndarray) -> Tuple[ndarray, ndarray]:
         """Return vertices and edges corresponding to given facet indices.
 
         Parameters
         ----------
         ix
@@ -747,25 +748,41 @@
         times_or_ix
             Either an integer giving the number of uniform refinements or an
             array of element indices for adaptive refinement.
 
         """
         m = self
         has_boundaries = self.boundaries is not None
-        if self.subdomains is not None:
-            logger.warning("Named subdomains invalidated by a call to "
-                           "Mesh.refined()")
+        has_subdomains = self.subdomains is not None
         if isinstance(times_or_ix, int):
             for _ in range(times_or_ix):
-                m = m._uniform()
+                mtmp = m._uniform()
+                # fix subdomains for all mesh types
+                if m._subdomains is not None:
+                    N = int(mtmp.t.shape[1] / m.t.shape[1])
+                    new_t = np.zeros((N, m.t.shape[1]), dtype=np.int64)
+                    new_t[0] = np.arange(m.t.shape[1], dtype=np.int64)
+                    for itr in range(N - 1):
+                        new_t[itr + 1] = new_t[itr] + m.t.shape[1]
+                    mtmp = replace(
+                        mtmp,
+                        _subdomains={
+                            name: np.sort(new_t[:, ixs].flatten())
+                            for name, ixs in m._subdomains.items()
+                        },
+                    )
+                m = mtmp
         else:
             m = m._adaptive(times_or_ix)
         if has_boundaries and m.boundaries is None:
             logger.warning("Named boundaries invalidated by a call to "
                            "Mesh.refined()")
+        if has_subdomains and self.subdomains is None:
+            logger.warning("Named subdomains invalidated by a call to "
+                           "Mesh.refined()")
         return m
 
     def scaled(self, factors):
         """Return a new mesh with scaled dimensions.
 
         Parameters
         ----------
@@ -1003,21 +1020,31 @@
         ----------
         elements
             Criteria of which elements to include.  This input is normalized
             using ``self.normalize_elements``.
 
         """
         elements = self.normalize_elements(elements)
-        p, t, _ = self._reix(self.t[:, elements])
+        p, t, ix = self._reix(self.t[:, elements])
+        newt = np.zeros(self.t.shape[1], dtype=np.int64) - 1
+        newt[elements] = np.arange(len(elements), dtype=np.int64)
+        newf = np.zeros(self.facets.shape[1], dtype=np.int64) - 1
+        facets = np.unique(self.t2f[:, elements])
+        newf[facets] = np.arange(len(facets), dtype=np.int64)
         return replace(
             self,
             doflocs=p,
             t=t,
-            _boundaries=None,
-            _subdomains=None,
+            _boundaries=({k: np.extract(newf[self.boundaries[k]] >= 0,
+                                        newf[self.boundaries[k]])
+                          for k in self.boundaries}
+                         if self.boundaries is not None else None),
+            _subdomains=({k: newt[np.intersect1d(self.subdomains[k], elements)]
+                          for k in self.subdomains}
+                         if self.subdomains is not None else None),
         )
 
     def remove_elements(self, element_indices: ndarray):
         """Construct a new mesh by removing elements.
 
         Parameters
         ----------
@@ -1055,20 +1082,49 @@
     def plot(self, x, visuals='matplotlib', **kwargs):
         """Convenience wrapper for skfem.visuals."""
         if not isinstance(visuals, str):
             logger.warning("Second argument, 'visuals', must be a string.")
         mod = importlib.import_module('skfem.visuals.{}'.format(visuals))
         return mod.plot(self, x, **kwargs)
 
+    def normalize_nodes(self, nodes) -> ndarray:
+        """Generate an array of node indices.
+
+        Parameters
+        ----------
+        nodes
+            Criteria of which nodes to include.  Function has different
+            behavior based on the type of this parameter.
+
+        """
+        if isinstance(nodes, tuple):
+            return self.normalize_nodes(
+                lambda x: np.linalg.norm(x - np.array(list(nodes))[:, None],
+                                         axis=0) < 1e-12
+            )
+        if isinstance(nodes, ndarray):
+            # assumed an array of nodes
+            return nodes
+        elif isinstance(nodes, (list, set)):
+            # Recurse over the list, building an array of all matching elements
+            return np.unique(
+                np.concatenate(
+                    [self.normalize_nodes(n) for n in nodes]
+                )
+            )
+        elif callable(nodes):
+            return self.nodes_satisfying(nodes)
+        raise NotImplementedError
+
     def normalize_facets(self, facets) -> ndarray:
         """Generate an array of facet indices.
 
         Parameters
         ----------
-        elements
+        facets
             Criteria of which facets to include.  Function has different
             behavior based on the type of this parameter.
 
         """
         if isinstance(facets, int):
             # Make  normalize_facets([1,2,3]) have the same behavior as
             # normalize_facets(np.array([1,2,3]))
```

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_2d.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_2d.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_3d.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_3d.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_dg.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_dg.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_hex_1.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_hex_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_hex_2.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_hex_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_line_1.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_line_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_quad_1.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_quad_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_quad_2.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_quad_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_simplex.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_simplex.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_tet_1.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_tet_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_tet_2.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_tet_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_tri_1.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_tri_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -258,14 +258,16 @@
         l12 = np.sqrt(np.sum((p[:, t[1]] - p[:, t[2]]) ** 2, axis=0))
         l02 = np.sqrt(np.sum((p[:, t[0]] - p[:, t[2]]) ** 2, axis=0))
 
         ix01 = (l01 > l02) * (l01 > l12)
         ix12 = (l12 > l01) * (l12 > l02)
 
         # row swaps
+        t = t.copy()
+
         tmp = t[2, ix01]
         t[2, ix01] = t[1, ix01]
         t[1, ix01] = tmp
 
         tmp = t[0, ix12]
         t[0, ix12] = t[1, ix12]
         t[1, ix12] = tmp
@@ -284,15 +286,15 @@
             t2facets = facets[m.t2f]
             t2facets[2, t2facets[0] + t2facets[1] > 0] = 1
             facets[m.t2f[t2facets == 1]] = 1
 
         return facets
 
     @staticmethod
-    def _adaptive_split_elements(m, facets):
+    def _adaptive_split_elements(m, facets, subdomains):
         """Define new elements."""
         ix = (-1) * np.ones(m.facets.shape[1], dtype=np.int64)
         ix[facets == 1] = (np.arange(np.count_nonzero(facets))
                            + m.p.shape[1])
         ix = ix[m.t2f]
 
         red = (ix[0] >= 0) * (ix[1] >= 0) * (ix[2] >= 0)
@@ -328,35 +330,68 @@
             np.vstack((m.t[2, green], ix[2, green], m.t[1, green])),
         ))
 
         # new nodes
         p = .5 * (m.p[:, m.facets[0, facets == 1]] +
                   m.p[:, m.facets[1, facets == 1]])
 
+        if subdomains is not None:
+            new_t = np.zeros((4, m.t.shape[1]), dtype=np.int64) - 1
+            nred = np.sum(red)
+            nblue1 = np.sum(blue1)
+            nblue2 = np.sum(blue2)
+            ngreen = np.sum(green)
+            offset = np.sum(rest)
+            new_t[0, rest] = np.arange(offset, dtype=np.int64)
+            new_t[:, red] = np.arange(offset,
+                                      offset + 4 * nred,
+                                      dtype=np.int64).reshape(4, -1)
+            offset += 4 * nred
+            new_t[:3, blue1] = np.arange(offset,
+                                         offset + 3 * nblue1,
+                                         dtype=np.int64).reshape(3, -1)
+            offset += 3 * nblue1
+            new_t[:3, blue2] = np.arange(offset,
+                                         offset + 3 * nblue2,
+                                         dtype=np.int64).reshape(3, -1)
+            offset += 3 * nblue2
+            new_t[:2, green] = np.arange(offset,
+                                         offset + 2 * ngreen,
+                                         dtype=np.int64).reshape(2, -1)
+            subdomains = {
+                name: np.setdiff1d(np.unique(new_t[:, ixs]), [-1])
+                for name, ixs in subdomains.items()
+            }
+
         return (
             np.hstack((m.p, p)),
             np.hstack((m.t[:, rest], t_red, t_blue1, t_blue2, t_green)),
+            subdomains,
         )
 
     def _adaptive(self, marked):
 
         sorted_mesh = replace(
             self,
             t=self._adaptive_sort_mesh(self.p, self.t),
             sort_t=False,
         )
         facets = self._adaptive_find_facets(sorted_mesh, marked)
-        doflocs, t = self._adaptive_split_elements(sorted_mesh, facets)
+        doflocs, t, subdomains = self._adaptive_split_elements(
+            sorted_mesh,
+            facets,
+            self._subdomains,
+        )
 
         return replace(
             self,
             doflocs=doflocs,
             t=t,
             _boundaries=None,
-            _subdomains=None,
+            _subdomains=subdomains,
         )
 
     def __mul__(self, other):
 
         from .mesh_wedge_1 import MeshWedge1
         from .mesh_line_1 import MeshLine1
```

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_tri_1_dg.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_tri_1_dg.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/mesh/mesh_tri_2.py` & `scikit-fem-8.1.0/skfem/mesh/mesh_tri_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/models/elasticity.py` & `scikit-fem-8.1.0/skfem/models/elasticity.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/quadrature.py` & `scikit-fem-8.1.0/skfem/quadrature.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/utils.py` & `scikit-fem-8.1.0/skfem/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,15 +206,18 @@
 
     if solver is None:
         solver = solver_eigen_scipy(**kwargs)
 
     if x is not None and I is not None:
         L, X = solver(A, M, **kwargs)
         y = np.tile(x.copy()[:, None], (1, X.shape[1]))
-        y[I] = X
+        if isinstance(I, tuple):
+            np.add.at(y, I[0], np.array([I[1](x) for x in X.T]).T)
+        else:
+            y[I] = X
         return L, y
     return solver(A, M, **kwargs)
 
 
 def solve_linear(A: spmatrix,
                  b: ndarray,
                  x: Optional[ndarray] = None,
@@ -223,15 +226,18 @@
                  **kwargs) -> ndarray:
 
     if solver is None:
         solver = solver_direct_scipy(**kwargs)
 
     if x is not None and I is not None:
         y = x.copy()
-        y[I] = solver(A, b, **kwargs)
+        if isinstance(I, tuple):
+            np.add.at(y, I[0], I[1](solver(A, b, **kwargs)))
+        else:
+            y[I] = solver(A, b, **kwargs)
         return y
     return solver(A, b, **kwargs)
 
 
 def solve(A: spmatrix,
           b: Union[ndarray, spmatrix],
           x: Optional[ndarray] = None,
@@ -574,33 +580,92 @@
 
     """
     b, x, I, D = _init_bc(A, b, x, I, D)
 
     ret_value: CondensedSystem = (None,)
 
     if b is None:
-        ret_value = (A[I].T[I].T,)
+        ret_value = (A[I][:, I],)
     else:
         if isinstance(b, spmatrix):
             # generalized eigenvalue problem: don't modify rhs
-            Aout = A[I].T[I].T
-            bout = b[I].T[I].T
+            Aout = A[I][:, I]
+            bout = b[I][:, I]
         elif isinstance(b, ndarray):
-            Aout = A[I].T[I].T
-            bout = b[I] - A[I].T[D].T @ x[D]
+            Aout = A[I][:, I]
+            bout = b[I] - A[I][:, D] @ x[D]
         else:
             raise Exception("Type of second arg not supported.")
         ret_value = (Aout, bout)
 
     if expand:
         ret_value += (x, I)
 
     return ret_value if len(ret_value) > 1 else ret_value[0]
 
 
+def mpc(A: spmatrix,
+        b: ndarray,
+        S: Optional[ndarray] = None,
+        M: Optional[ndarray] = None,
+        T: Optional[spmatrix] = None,
+        g: Optional[ndarray] = None) -> CondensedSystem:
+    """Apply a multipoint constraint on the linear system.
+
+    Parameters
+    ----------
+    A
+    b
+        The linear system to constrain.
+    S
+    M
+    T
+    g
+        The constraint is of the form `x[S] = T @ x[M] + g`.
+
+    """
+    if M is None:
+        M = np.array([], dtype=np.int64)
+    if S is None:
+        S = np.array([], dtype=np.int64)
+
+    U = np.setdiff1d(np.arange(A.shape[0], dtype=np.int64),
+                     np.concatenate((M, S)))
+
+    if T is None:
+        T = sp.eye(len(S), len(M))
+    if g is None:
+        g = np.zeros(len(S))
+
+    if T.shape[0] != len(S) or T.shape[1] != len(M) or len(g) != len(S):
+        raise ValueError("Inputs to mpc have incompatible shapes.")
+
+    B = bmat([
+        [
+            A[U][:, U],
+            A[U][:, M] + A[U][:, S] @ T,
+        ],
+        [
+            A[M][:, U],
+            A[M][:, M] + A[M][:, S] @ T,
+        ]], 'csr')
+    y = np.concatenate((b[U] - A[U][:, S] @ g,
+                        b[M] - A[M][:, S] @ g))
+
+    return (
+        B,
+        y,
+        np.zeros_like(b, dtype=B.dtype),
+        (
+            np.concatenate((U, M, S)),
+            lambda x: np.concatenate((x, T @ x[len(U):] + g)),
+        )
+    )
+
+
 # additional utilities
 
 
 def bmat(blocks, *args, **kwargs):
     """A variant of scipy bmat which adds block indices to out.blocks."""
     m = len(blocks)
     n = len(blocks[0])
```

### Comparing `scikit-fem-8.0.0/skfem/visuals/glvis.py` & `scikit-fem-8.1.0/skfem/visuals/glvis.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/visuals/matplotlib.py` & `scikit-fem-8.1.0/skfem/visuals/matplotlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,19 @@
         ys.append(None)
     ax.plot(xs,
             ys,
             kwargs['color'] if 'color' in kwargs else 'k',
             linewidth=kwargs['linewidth'] if 'linewidth' in kwargs else .5,
             **plot_kwargs)
 
+    if "subdomain" in kwargs:
+        y = np.zeros(m.t.shape[1])
+        y[m.subdomains[kwargs['subdomain']]] = 1
+        plot(m, y, ax=ax)
+
     if "boundaries" in kwargs:
         cm = plt.get_cmap('gist_rainbow')
         colors = [cm(1.*i/len(m.boundaries)) for i in range(len(m.boundaries))]
         for i, k in enumerate(m.boundaries):
             facets = m.facets[:, m.boundaries[k]]
             xs = []
             ys = []
```

### Comparing `scikit-fem-8.0.0/skfem/visuals/svg.py` & `scikit-fem-8.1.0/skfem/visuals/svg.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-8.0.0/skfem/visuals/vedo.py` & `scikit-fem-8.1.0/skfem/visuals/vedo.py`

 * *Files identical despite different names*

