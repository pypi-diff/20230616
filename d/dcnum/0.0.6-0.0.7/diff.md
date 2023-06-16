# Comparing `tmp/dcnum-0.0.6.tar.gz` & `tmp/dcnum-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.0.6.tar", last modified: Thu Jun 15 21:46:04 2023, max compression
+gzip compressed data, was "dcnum-0.0.7.tar", last modified: Fri Jun 16 13:44:31 2023, max compression
```

## Comparing `dcnum-0.0.6.tar` & `dcnum-0.0.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.651131 dcnum-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-15 21:45:50.000000 dcnum-0.0.6/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-15 21:45:50.000000 dcnum-0.0.6/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-15 21:45:50.000000 dcnum-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-15 21:45:50.000000 dcnum-0.0.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 21:45:50.000000 dcnum-0.0.6/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-15 21:45:50.000000 dcnum-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-15 21:46:04.651131 dcnum-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-15 21:45:50.000000 dcnum-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/dcnum/feat/background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/feat/brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/brightness/bright_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/feat/haralick/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/haralick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/haralick/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/haralick/tex_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/feat/moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/segm/segmenter_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/write/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/write/writer_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-15 21:45:50.000000 dcnum-0.0.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-15 21:45:50.000000 dcnum-0.0.6/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-15 21:45:50.000000 dcnum-0.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 21:45:50.000000 dcnum-0.0.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-15 21:45:50.000000 dcnum-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:46:04.651131 dcnum-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.651131 dcnum-0.0.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_write_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_write_writer_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.934601 dcnum-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-16 13:44:19.000000 dcnum-0.0.7/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-16 13:44:19.000000 dcnum-0.0.7/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-16 13:44:19.000000 dcnum-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-16 13:44:19.000000 dcnum-0.0.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-16 13:44:19.000000 dcnum-0.0.7/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 13:44:19.000000 dcnum-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-16 13:44:31.942601 dcnum-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-16 13:44:19.000000 dcnum-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/brightness/bright_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/haralick/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/haralick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/haralick/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/haralick/tex_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/segm/segmenter_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/write/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/write/writer_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-16 13:44:19.000000 dcnum-0.0.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-16 13:44:19.000000 dcnum-0.0.7/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-16 13:44:19.000000 dcnum-0.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 13:44:19.000000 dcnum-0.0.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-16 13:44:19.000000 dcnum-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:44:31.942601 dcnum-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_write_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_write_writer_thread.py
```

### Comparing `dcnum-0.0.6/.github/workflows/check.yml` & `dcnum-0.0.7/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/.github/workflows/deploy_pypi.yml` & `dcnum-0.0.7/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/.gitignore` & `dcnum-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/CHANGELOG` & `dcnum-0.0.7/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+0.0.7
+ - enh: dataset keyword arguments and mode HDF5WriterThread
+ - enh: speed-up of brightness feature computation
 0.0.6
  - feat: add HDF5Writer and HDF5WriterThread classes in write submodule
  - feat: segmenters compute labeled images instead of masks
  - enh: introduce iter_chunks for cached image data
  - ref: do not filter for contour length
  - ref: rename feat.background.get_available_background_methods
  - ref: store PPID information in dataset metadata instead of "user" section
```

### Comparing `dcnum-0.0.6/LICENSE` & `dcnum-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/PKG-INFO` & `dcnum-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.6
+Version: 0.0.7
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.6/README.rst` & `dcnum-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/feat/background/base.py` & `dcnum-0.0.7/dcnum/feat/background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/feat/background/bg_roll_median.py` & `dcnum-0.0.7/dcnum/feat/background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/feat/background/bg_sparse_median.py` & `dcnum-0.0.7/dcnum/feat/background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/feat/haralick/tex_all.py` & `dcnum-0.0.7/dcnum/feat/haralick/tex_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from mahotas.features import haralick as mh_haralick
 import numpy as np
 
 from .common import haralick_names
 
 
-def haralick_texture_features(image, mask, image_bg=None):
-    if image_bg is not None:
-        # We have to perform background subtraction (casting required).
-        image_corr = np.array(image, dtype=int) - image_bg
-    else:
-        # Input is already background-corrected
-        image_corr = image
-
+def haralick_texture_features(image, mask, image_bg=None, image_corr=None):
     # make sure we have a boolean array
-    mask = np.asarray(mask, dtype=bool)
+    mask = np.array(mask, dtype=bool)
+
+    # compute features if necessary
+    if image_bg is not None or image_corr is not None:
+        # Background-corrected brightness values
+        if image_corr is None:
+            image_corr = np.array(image, dtype=np.int16) - image_bg
 
     size = image.shape[0]
 
     ds_dt = np.dtype({'names': haralick_names,
                       'formats': [float] * len(haralick_names)})
     rec_arr = np.recarray(size, dtype=ds_dt)
     nan_result = np.nan * np.zeros(26, dtype=float)
 
-    # This loop is parallelized with numba jit via `prange`.
     for ii in range(size):
         # Haralick texture features
         # https://gitlab.gwdg.de/blood_data_analysis/dcevent/-/issues/20
         # Preprocessing:
         # - create a copy of the array (don't edit `image_corr`)
         # - add grayscale values (negative values not supported)
         #   -> maximum value should be as small as possible
         # - set pixels outside contour to zero (ignored areas, see mahotas)
-        minval = (image_corr[ii][mask[ii]]).min()
-        imi = (image_corr[ii] - minval + 1) * mask[ii]
+        imcoi = image_corr[ii]
+        maski = mask[ii]
+        minval = imcoi[maski].min()
+        imi = np.array((imcoi - minval + 1) * maski, dtype=np.uint8)
         try:
             ret = mh_haralick(imi,
                               ignore_zeros=True,
                               return_mean_ptp=True)
         except ValueError:
             # The error message looks like this:
             #    ValueError: mahotas.haralick_features: the input is empty.
```

### Comparing `dcnum-0.0.6/dcnum/feat/moments/mt_legacy.py` & `dcnum-0.0.7/dcnum/feat/moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/meta/ppid.py` & `dcnum-0.0.7/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/read/cache.py` & `dcnum-0.0.7/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/read/hdf5_data.py` & `dcnum-0.0.7/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/segm/segm_thresh.py` & `dcnum-0.0.7/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/segm/segmenter.py` & `dcnum-0.0.7/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/segm/segmenter_cpu.py` & `dcnum-0.0.7/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/dcnum/write/writer_thread.py` & `dcnum-0.0.7/dcnum/write/writer_thread.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 from .writer import HDF5Writer
 
 
 class HDF5WriterThread(threading.Thread):
     def __init__(self,
                  path_out: pathlib.Path,
                  dq: collections.deque,
+                 ds_kwds: dict = None,
+                 mode: str = "a",
                  *args, **kwargs):
         """Convenience class for writing to data outside the main loop
 
         Parameters
         ----------
         path_out:
             Path to the output HDF5 file
         dq:
             `collections.deque` object from which data are taken
             using `popleft()`.
         """
         super(HDF5WriterThread, self).__init__(*args, **kwargs)
-        self.writer = HDF5Writer(path_out)
+        self.writer = HDF5Writer(path_out, mode=mode, ds_kwds=ds_kwds)
         self.dq = dq
         self.may_stop_loop = False
         self.must_stop_loop = False
 
     def abort_loop(self):
         """Force aborting the loop as soon as possible"""
         self.must_stop_loop = True
```

### Comparing `dcnum-0.0.6/dcnum.egg-info/PKG-INFO` & `dcnum-0.0.7/dcnum.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.6
+Version: 0.0.7
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.6/dcnum.egg-info/SOURCES.txt` & `dcnum-0.0.7/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/docs/conf.py` & `dcnum-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/docs/extensions/github_changelog.py` & `dcnum-0.0.7/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/pyproject.toml` & `dcnum-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.0.7/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.0.7/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/helper_methods.py` & `dcnum-0.0.7/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.0.7/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_feat_brightness.py` & `dcnum-0.0.7/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_feat_haralick.py` & `dcnum-0.0.7/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_feat_moments_based.py` & `dcnum-0.0.7/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_ppid.py` & `dcnum-0.0.7/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_read_concat_hdf5.py` & `dcnum-0.0.7/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_read_hdf5.py` & `dcnum-0.0.7/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_segm_thresh.py` & `dcnum-0.0.7/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_write_writer.py` & `dcnum-0.0.7/tests/test_write_writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.6/tests/test_write_writer_thread.py` & `dcnum-0.0.7/tests/test_write_writer_thread.py`

 * *Files identical despite different names*

