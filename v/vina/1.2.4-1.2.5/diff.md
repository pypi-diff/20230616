# Comparing `tmp/vina-1.2.4.tar.gz` & `tmp/vina-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vina-1.2.4.tar", last modified: Mon Jun 12 17:59:27 2023, max compression
+gzip compressed data, was "vina-1.2.5.tar", last modified: Fri Jun 16 06:09:26 2023, max compression
```

## Comparing `vina-1.2.4.tar` & `vina-1.2.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 17:58:58.318707 vina-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-12 17:59:27.886716 vina-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-12 17:58:58.318707 vina-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-12 17:58:58.318707 vina-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-12 17:58:58.318707 vina-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.882716 vina-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/src/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11024 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/ad4cache.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/ad4cache.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/array3d.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2098 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/atom.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/atom_base.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    12956 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/atom_constants.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2985 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/atom_type.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3951 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/bfgs.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/brick.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    12995 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/cache.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     2515 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/cache.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     9259 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/common.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    11290 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/conf.h
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/conf_independent.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/conf_independent.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/convert_substring.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/coords.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/coords.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/curl.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/file.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4083 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/grid.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     2288 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/grid.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/grid_dim.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/igrid.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/incrementable.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1025 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/int_pow.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1821 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/macros.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/matrix.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35551 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/model.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     9313 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/model.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/monte_carlo.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/monte_carlo.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2242 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/mutate.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      906 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/mutate.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     7027 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/non_cache.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/non_cache.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5325 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3001 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel_mc.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel_mc.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel_progress.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel_progress.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1373 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parse_error.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    25194 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parse_pdbqt.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1213 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parse_pdbqt.h
--rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/potentials.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     9027 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/precalculate.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/quasi_newton.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/quasi_newton.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4408 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/quaternion.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     3019 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/quaternion.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/random.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/random.h
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/scoring_function.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2796 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/szv_grid.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/szv_grid.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     8614 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/tree.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/triangular_matrix_index.h
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    36141 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/vina.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/vina.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-06-12 17:58:58.690706 vina-1.2.4/src/main/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/src/split/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-12 17:58:58.694706 vina-1.2.4/src/split/split.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/vina/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 17:58:58.318707 vina-1.2.4/vina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-12 17:58:58.318707 vina-1.2.4/vina/autodock_vina.i
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 17:58:58.318707 vina-1.2.4/vina/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 17:58:58.318707 vina-1.2.4/vina/vina.i
--rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-06-12 17:58:58.318707 vina-1.2.4/vina/vina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:09:26.326837 vina-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-16 06:08:54.649989 vina-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-16 06:09:26.326837 vina-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-16 06:08:54.649989 vina-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-16 06:08:54.649989 vina-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-16 06:08:54.649989 vina-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:09:26.322837 vina-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:09:26.326837 vina-1.2.5/src/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11024 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/ad4cache.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/ad4cache.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/array3d.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2098 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/atom.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/atom_base.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12956 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/atom_constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2985 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/atom_type.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3951 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/bfgs.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/brick.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12995 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/cache.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2515 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/cache.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9259 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/common.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11290 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/conf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/conf_independent.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/conf_independent.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/convert_substring.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/coords.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/coords.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/curl.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/file.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4083 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/grid.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2288 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/grid.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/grid_dim.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/igrid.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/incrementable.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1025 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/int_pow.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1821 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/macros.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/matrix.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35551 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/model.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9313 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/model.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/monte_carlo.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/monte_carlo.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2242 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/mutate.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      906 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/mutate.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7027 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/non_cache.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/non_cache.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5325 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/parallel.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3001 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/parallel_mc.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/parallel_mc.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/parallel_progress.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/parallel_progress.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1373 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/parse_error.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25194 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/parse_pdbqt.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1213 2023-06-16 06:08:54.985998 vina-1.2.5/src/lib/parse_pdbqt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/potentials.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9027 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/precalculate.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/quasi_newton.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/quasi_newton.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4408 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/quaternion.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3019 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/quaternion.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/random.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/scoring_function.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2796 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/szv_grid.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/szv_grid.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8614 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/tree.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/triangular_matrix_index.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36706 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/vina.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-16 06:08:54.989998 vina-1.2.5/src/lib/vina.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:09:26.326837 vina-1.2.5/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-06-16 06:08:54.989998 vina-1.2.5/src/main/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:09:26.326837 vina-1.2.5/src/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-16 06:08:54.989998 vina-1.2.5/src/split/split.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:09:26.326837 vina-1.2.5/vina/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 06:08:54.649989 vina-1.2.5/vina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-16 06:08:54.649989 vina-1.2.5/vina/autodock_vina.i
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-16 06:08:54.649989 vina-1.2.5/vina/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 06:08:54.649989 vina-1.2.5/vina/vina.i
+-rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-06-16 06:08:54.649989 vina-1.2.5/vina/vina.py
```

### Comparing `vina-1.2.4/LICENSE` & `vina-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/PKG-INFO` & `vina-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vina
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python interface to AutoDock Vina
 Home-page: https://ccsb.scripps.edu/
 Author: Diogo Santos Martins, Jerome Eberhardt, Andreas F. Tillack, Stefano Forli
 Author-email: forli@scripps.edu
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
```

### Comparing `vina-1.2.4/README.md` & `vina-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/setup.py` & `vina-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/ad4cache.cpp` & `vina-1.2.5/src/lib/ad4cache.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/ad4cache.h` & `vina-1.2.5/src/lib/ad4cache.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/array3d.h` & `vina-1.2.5/src/lib/array3d.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/atom.h` & `vina-1.2.5/src/lib/atom.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/atom_base.h` & `vina-1.2.5/src/lib/atom_base.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/atom_constants.h` & `vina-1.2.5/src/lib/atom_constants.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/atom_type.h` & `vina-1.2.5/src/lib/atom_type.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/bfgs.h` & `vina-1.2.5/src/lib/bfgs.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/brick.h` & `vina-1.2.5/src/lib/brick.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/cache.cpp` & `vina-1.2.5/src/lib/cache.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/cache.h` & `vina-1.2.5/src/lib/cache.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/common.h` & `vina-1.2.5/src/lib/common.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/conf.h` & `vina-1.2.5/src/lib/conf.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/conf_independent.cpp` & `vina-1.2.5/src/lib/conf_independent.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/conf_independent.h` & `vina-1.2.5/src/lib/conf_independent.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/convert_substring.h` & `vina-1.2.5/src/lib/convert_substring.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/coords.cpp` & `vina-1.2.5/src/lib/coords.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/coords.h` & `vina-1.2.5/src/lib/coords.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/curl.h` & `vina-1.2.5/src/lib/curl.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/file.h` & `vina-1.2.5/src/lib/file.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/grid.cpp` & `vina-1.2.5/src/lib/grid.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/grid.h` & `vina-1.2.5/src/lib/grid.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/grid_dim.h` & `vina-1.2.5/src/lib/grid_dim.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/igrid.h` & `vina-1.2.5/src/lib/igrid.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/incrementable.h` & `vina-1.2.5/src/lib/incrementable.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/int_pow.h` & `vina-1.2.5/src/lib/int_pow.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/macros.h` & `vina-1.2.5/src/lib/macros.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/matrix.h` & `vina-1.2.5/src/lib/matrix.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/model.cpp` & `vina-1.2.5/src/lib/model.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/model.h` & `vina-1.2.5/src/lib/model.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/monte_carlo.cpp` & `vina-1.2.5/src/lib/monte_carlo.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/monte_carlo.h` & `vina-1.2.5/src/lib/monte_carlo.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/mutate.cpp` & `vina-1.2.5/src/lib/mutate.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/mutate.h` & `vina-1.2.5/src/lib/mutate.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/non_cache.cpp` & `vina-1.2.5/src/lib/non_cache.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/non_cache.h` & `vina-1.2.5/src/lib/non_cache.h`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 struct non_cache : public igrid {
     non_cache() {}
 	non_cache(const model& m, const grid_dims& gd_, const precalculate* p_, fl slope_);
 	virtual fl eval      (const model& m, fl v) const; // needs m.coords // clean up
 	virtual fl eval_intra(      model& m, fl v) const;
 	virtual fl eval_deriv(      model& m, fl v) const; // needs m.coords, sets m.minus_forces // clean up
-	bool within(const model& m, fl margin = -0.0001) const; // negative margin ensures we stay inside (thanks Andreas!)
+	bool within(const model& m, fl margin = 0.0001) const;
 	fl slope;
 private:
 	szv_grid sgrid;
 	grid_dims gd;
 	const precalculate* p;
 };
```

### Comparing `vina-1.2.4/src/lib/parallel.h` & `vina-1.2.5/src/lib/parallel.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/parallel_mc.cpp` & `vina-1.2.5/src/lib/parallel_mc.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/parallel_mc.h` & `vina-1.2.5/src/lib/parallel_mc.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/parallel_progress.cpp` & `vina-1.2.5/src/lib/parallel_progress.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/parallel_progress.h` & `vina-1.2.5/src/lib/parallel_progress.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/parse_error.h` & `vina-1.2.5/src/lib/parse_error.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/parse_pdbqt.cpp` & `vina-1.2.5/src/lib/parse_pdbqt.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/parse_pdbqt.h` & `vina-1.2.5/src/lib/parse_pdbqt.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/potentials.h` & `vina-1.2.5/src/lib/potentials.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/precalculate.h` & `vina-1.2.5/src/lib/precalculate.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/quasi_newton.cpp` & `vina-1.2.5/src/lib/quasi_newton.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/quasi_newton.h` & `vina-1.2.5/src/lib/quasi_newton.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/quaternion.cpp` & `vina-1.2.5/src/lib/quaternion.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/quaternion.h` & `vina-1.2.5/src/lib/quaternion.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/random.cpp` & `vina-1.2.5/src/lib/random.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/random.h` & `vina-1.2.5/src/lib/random.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/scoring_function.h` & `vina-1.2.5/src/lib/scoring_function.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/szv_grid.cpp` & `vina-1.2.5/src/lib/szv_grid.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/szv_grid.h` & `vina-1.2.5/src/lib/szv_grid.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/tree.h` & `vina-1.2.5/src/lib/tree.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/triangular_matrix_index.h` & `vina-1.2.5/src/lib/triangular_matrix_index.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/utils.cpp` & `vina-1.2.5/src/lib/utils.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/utils.h` & `vina-1.2.5/src/lib/utils.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/lib/vina.cpp` & `vina-1.2.5/src/lib/vina.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -917,34 +917,39 @@
 		// For the Vina scoring function, we take the intramolecular energy from the best pose
 		// the order must not change because of non-decreasing g (see paper), but we'll re-sort in case g is non strictly increasing
 		if (m_sf_choice == SF_VINA || m_sf_choice == SF_VINARDO) {
 			// Refine poses if no_refine is false and got receptor
 			if (!m_no_refine & m_receptor_initialized) {
 				change g(m_model.get_size());
 				quasi_newton quasi_newton_par;
-				const vec authentic_v(1000, 1000, 1000);
 				//std::vector<double> energies_before_opt;
 				//std::vector<double> energies_after_opt;
 				int evalcount = 0;
 				const fl slope = 1e6;
 				m_non_cache.slope = slope;
 				quasi_newton_par.max_steps = unsigned((25 + m_model.num_movable_atoms()) / 3);
 
 				VINA_FOR_IN(i, poses){
-					const fl slope_orig = m_non_cache.slope;
 					VINA_FOR(p, 5){
 						m_non_cache.slope = 100 * std::pow(10.0, 2.0*p);
 						quasi_newton_par(m_model, m_precalculated_byatom, m_non_cache, poses[i], g, authentic_v, evalcount);
 						if(m_non_cache.within(m_model))
 							break;
 					}
 					poses[i].coords = m_model.get_heavy_atom_movable_coords();
-					if (!m_non_cache.within(m_model))
-						poses[i].e = max_fl;
 					m_non_cache.slope = slope;
+					// rescoring in case a ligand or flex sidechain atom is outside box
+					// ensuring poses will be sorted with the same slope (a.k.a. out of
+					// box penalty) that will be used to calculate final energies.
+					m_model.set(poses[i].c);
+					double all_grids = m_non_cache.eval(m_model, authentic_v[1]);
+					double inter_pairs = m_model.eval_inter(m_precalculated_byatom, authentic_v); // ligand -- flex
+					double intra_pairs = m_model.evalo(m_precalculated_byatom, authentic_v); // flex_i -- flex_i and flex_i -- flex_j
+					double lig_intra = m_model.evali(m_precalculated_byatom, authentic_v); // ligand_i -- ligand_i
+					poses[i].e = all_grids + inter_pairs + intra_pairs + lig_intra;
 				}
 			}
 
 			poses.sort(); // order often changes after non_cache refinement
 			m_model.set(poses[0].c);
 			if (m_no_refine || !m_receptor_initialized)
 				intramolecular_energy = m_model.eval_intramolecular(m_precalculated_byatom, m_grid, authentic_v);
@@ -1005,16 +1010,16 @@
 				std::cout << "  " << std::setw(9) << std::setprecision(4) << poses[i].ub << "\n";
 			}
 		}
 
 		// Clean up by putting back the best pose in model
 		m_model.set(poses[0].c);
 	} else {
-		std::cerr << "WARNING: Could not find any conformations completely within the search space.\n";
-		std::cerr << "WARNING: Check that it is large enough for all movable atoms, including those in the flexible side chains.\n";
+		std::cerr << "WARNING: Zero poses in output container after global search. This should not be happening and is likely a bug.\n";
+		std::cerr << "WARNING: If possible, please file a bug report with your input files and random seed on GitHub.\n";
 	}
 
 	// Store results in Vina object
 	m_poses = poses;
 }
 
 Vina::~Vina() {
```

### Comparing `vina-1.2.4/src/lib/vina.h` & `vina-1.2.5/src/lib/vina.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/main/main.cpp` & `vina-1.2.5/src/main/main.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/src/split/split.cpp` & `vina-1.2.5/src/split/split.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/vina/autodock_vina.i` & `vina-1.2.5/vina/autodock_vina.i`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/vina/utils.py` & `vina-1.2.5/vina/utils.py`

 * *Files identical despite different names*

### Comparing `vina-1.2.4/vina/vina.py` & `vina-1.2.5/vina/vina.py`

 * *Files identical despite different names*

