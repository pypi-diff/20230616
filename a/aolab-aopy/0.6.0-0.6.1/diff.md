# Comparing `tmp/aolab-aopy-0.6.0.tar.gz` & `tmp/aolab-aopy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aolab-aopy-0.6.0.tar", last modified: Fri Jun 16 16:23:21 2023, max compression
+gzip compressed data, was "aolab-aopy-0.6.1.tar", last modified: Fri Jun 16 17:00:19 2023, max compression
```

## Comparing `aolab-aopy-0.6.0.tar` & `aolab-aopy-0.6.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.969025 aolab-aopy-0.6.0/
--rw-r--r--   0 leoscholl   (501) staff       (20)     1106 2023-06-16 16:22:43.000000 aolab-aopy-0.6.0/LICENSE
--rw-r--r--   0 leoscholl   (501) staff       (20)      749 2023-06-16 16:23:21.968856 aolab-aopy-0.6.0/PKG-INFO
--rw-r--r--   0 leoscholl   (501) staff       (20)      203 2023-03-20 22:49:31.000000 aolab-aopy-0.6.0/README.md
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.961252 aolab-aopy-0.6.0/aolab_aopy.egg-info/
--rw-r--r--   0 leoscholl   (501) staff       (20)      749 2023-06-16 16:23:21.000000 aolab-aopy-0.6.0/aolab_aopy.egg-info/PKG-INFO
--rw-r--r--   0 leoscholl   (501) staff       (20)     1397 2023-06-16 16:23:21.000000 aolab-aopy-0.6.0/aolab_aopy.egg-info/SOURCES.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)        1 2023-06-16 16:23:21.000000 aolab-aopy-0.6.0/aolab_aopy.egg-info/dependency_links.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)      164 2023-06-16 16:23:21.000000 aolab-aopy-0.6.0/aolab_aopy.egg-info/requires.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)        5 2023-06-16 16:23:21.000000 aolab-aopy-0.6.0/aolab_aopy.egg-info/top_level.txt
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.961711 aolab-aopy-0.6.0/aopy/
--rw-r--r--   0 leoscholl   (501) staff       (20)      241 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/__init__.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.962708 aolab-aopy-0.6.0/aopy/analysis/
--rw-r--r--   0 leoscholl   (501) staff       (20)      271 2022-11-29 17:21:22.000000 aolab-aopy-0.6.0/aopy/analysis/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    28781 2023-06-06 22:20:50.000000 aolab-aopy-0.6.0/aopy/analysis/accllr.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    48803 2023-06-06 22:20:50.000000 aolab-aopy-0.6.0/aopy/analysis/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    13768 2023-06-06 22:20:50.000000 aolab-aopy-0.6.0/aopy/analysis/behavior.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     7187 2022-11-29 17:21:22.000000 aolab-aopy-0.6.0/aopy/analysis/celltype.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8263 2022-11-29 17:21:22.000000 aolab-aopy-0.6.0/aopy/analysis/kfdecoder.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4897 2022-11-29 17:21:22.000000 aolab-aopy-0.6.0/aopy/analysis/tuning.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.963657 aolab-aopy-0.6.0/aopy/data/
--rw-r--r--   0 leoscholl   (501) staff       (20)       84 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/data/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    32887 2023-03-23 20:22:25.000000 aolab-aopy-0.6.0/aopy/data/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    35700 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/data/bmi3d.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3717 2023-03-23 20:22:25.000000 aolab-aopy-0.6.0/aopy/data/eye.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     9471 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/data/neuropixel.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5284 2022-12-19 23:14:32.000000 aolab-aopy-0.6.0/aopy/data/optitrack.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    13116 2022-07-26 16:06:37.000000 aolab-aopy-0.6.0/aopy/data/peslab.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.963905 aolab-aopy-0.6.0/aopy/postproc/
--rw-r--r--   0 leoscholl   (501) staff       (20)       19 2022-12-19 23:14:32.000000 aolab-aopy-0.6.0/aopy/postproc/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    28672 2023-06-06 22:20:50.000000 aolab-aopy-0.6.0/aopy/postproc/base.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.964330 aolab-aopy-0.6.0/aopy/precondition/
--rw-r--r--   0 leoscholl   (501) staff       (20)       39 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/precondition/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    32825 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/precondition/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8200 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/precondition/eye.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.965797 aolab-aopy-0.6.0/aopy/preproc/
--rw-r--r--   0 leoscholl   (501) staff       (20)       69 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/preproc/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    33372 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/preproc/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    33999 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/preproc/bmi3d.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2577 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/preproc/neuropixel.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     7060 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/preproc/oculomatic.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3817 2022-12-19 23:14:32.000000 aolab-aopy-0.6.0/aopy/preproc/optitrack.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     9620 2022-11-29 17:21:22.000000 aolab-aopy-0.6.0/aopy/preproc/quality.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    17132 2023-03-23 20:22:25.000000 aolab-aopy-0.6.0/aopy/preproc/wrappers.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2998 2022-07-26 16:06:37.000000 aolab-aopy-0.6.0/aopy/torch.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3759 2022-07-26 16:06:37.000000 aolab-aopy-0.6.0/aopy/tutorial_functions.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.966292 aolab-aopy-0.6.0/aopy/utils/
--rw-r--r--   0 leoscholl   (501) staff       (20)       41 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/utils/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    27126 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/utils/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2775 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/aopy/utils/memory.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.966683 aolab-aopy-0.6.0/aopy/visualization/
--rw-r--r--   0 leoscholl   (501) staff       (20)       44 2023-06-05 22:34:46.000000 aolab-aopy-0.6.0/aopy/visualization/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8138 2023-06-05 22:34:46.000000 aolab-aopy-0.6.0/aopy/visualization/animation.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    45663 2023-06-06 22:20:50.000000 aolab-aopy-0.6.0/aopy/visualization/base.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.967222 aolab-aopy-0.6.0/aopy/whitematter/
--rw-r--r--   0 leoscholl   (501) staff       (20)       62 2022-07-26 16:06:37.000000 aolab-aopy-0.6.0/aopy/whitematter/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      365 2022-07-26 16:06:37.000000 aolab-aopy-0.6.0/aopy/whitematter/arraymethods.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    15382 2022-07-26 16:06:37.000000 aolab-aopy-0.6.0/aopy/whitematter/dataset.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5220 2022-07-26 16:06:37.000000 aolab-aopy-0.6.0/aopy/whitematter/stream.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      556 2023-06-16 16:15:44.000000 aolab-aopy-0.6.0/pyproject.toml
--rw-r--r--   0 leoscholl   (501) staff       (20)       38 2023-06-16 16:23:21.969084 aolab-aopy-0.6.0/setup.cfg
--rw-r--r--   0 leoscholl   (501) staff       (20)      897 2023-06-05 23:06:59.000000 aolab-aopy-0.6.0/setup.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 16:23:21.968593 aolab-aopy-0.6.0/tests/
--rw-r--r--   0 leoscholl   (501) staff       (20)    51536 2023-06-06 22:20:50.000000 aolab-aopy-0.6.0/tests/test_analysis.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    39331 2023-06-05 23:07:00.000000 aolab-aopy-0.6.0/tests/test_data.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    10364 2023-06-06 22:20:50.000000 aolab-aopy-0.6.0/tests/test_postproc.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    25303 2023-06-05 23:07:00.000000 aolab-aopy-0.6.0/tests/test_precondition.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    62987 2023-06-05 23:07:00.000000 aolab-aopy-0.6.0/tests/test_preproc.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      819 2022-07-26 16:06:39.000000 aolab-aopy-0.6.0/tests/test_torch.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2037 2022-07-26 16:06:39.000000 aolab-aopy-0.6.0/tests/test_tutorial_functions.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    17660 2023-06-05 23:07:00.000000 aolab-aopy-0.6.0/tests/test_utils.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    19118 2023-06-05 22:34:47.000000 aolab-aopy-0.6.0/tests/test_visualization.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.352901 aolab-aopy-0.6.1/
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1106 2023-06-16 16:22:43.000000 aolab-aopy-0.6.1/LICENSE
+-rw-r--r--   0 leoscholl   (501) staff       (20)      749 2023-06-16 17:00:19.352747 aolab-aopy-0.6.1/PKG-INFO
+-rw-r--r--   0 leoscholl   (501) staff       (20)      203 2023-03-20 22:49:31.000000 aolab-aopy-0.6.1/README.md
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.343555 aolab-aopy-0.6.1/aolab_aopy.egg-info/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      749 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/PKG-INFO
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1397 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/SOURCES.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)        1 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/dependency_links.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)      164 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/requires.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)        5 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/top_level.txt
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.344153 aolab-aopy-0.6.1/aopy/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      241 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/__init__.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.345136 aolab-aopy-0.6.1/aopy/analysis/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      271 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/analysis/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    28781 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/analysis/accllr.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    48803 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/analysis/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    13768 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/analysis/behavior.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     7187 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/analysis/celltype.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8263 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/analysis/kfdecoder.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4897 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/analysis/tuning.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.346273 aolab-aopy-0.6.1/aopy/data/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       84 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/data/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    32990 2023-06-16 16:58:07.000000 aolab-aopy-0.6.1/aopy/data/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    35802 2023-06-16 16:58:45.000000 aolab-aopy-0.6.1/aopy/data/bmi3d.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3717 2023-03-23 20:22:25.000000 aolab-aopy-0.6.1/aopy/data/eye.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9471 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/data/neuropixel.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5284 2022-12-19 23:14:32.000000 aolab-aopy-0.6.1/aopy/data/optitrack.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    13116 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/data/peslab.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.346539 aolab-aopy-0.6.1/aopy/postproc/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       19 2022-12-19 23:14:32.000000 aolab-aopy-0.6.1/aopy/postproc/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    28672 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/postproc/base.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.346961 aolab-aopy-0.6.1/aopy/precondition/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       39 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/precondition/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    32825 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/precondition/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8200 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/precondition/eye.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.348341 aolab-aopy-0.6.1/aopy/preproc/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       69 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    33372 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    33999 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/bmi3d.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2577 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/neuropixel.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     7060 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/oculomatic.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3817 2022-12-19 23:14:32.000000 aolab-aopy-0.6.1/aopy/preproc/optitrack.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9620 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/preproc/quality.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    17132 2023-03-23 20:22:25.000000 aolab-aopy-0.6.1/aopy/preproc/wrappers.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2998 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/torch.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3759 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/tutorial_functions.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.349004 aolab-aopy-0.6.1/aopy/utils/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       41 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/utils/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    27126 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/utils/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2775 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/utils/memory.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.349453 aolab-aopy-0.6.1/aopy/visualization/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       44 2023-06-05 22:34:46.000000 aolab-aopy-0.6.1/aopy/visualization/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8138 2023-06-05 22:34:46.000000 aolab-aopy-0.6.1/aopy/visualization/animation.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    45663 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/visualization/base.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.350530 aolab-aopy-0.6.1/aopy/whitematter/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       62 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/whitematter/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      365 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/whitematter/arraymethods.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    15382 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/whitematter/dataset.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5220 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/whitematter/stream.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      556 2023-06-16 17:00:09.000000 aolab-aopy-0.6.1/pyproject.toml
+-rw-r--r--   0 leoscholl   (501) staff       (20)       38 2023-06-16 17:00:19.352945 aolab-aopy-0.6.1/setup.cfg
+-rw-r--r--   0 leoscholl   (501) staff       (20)      897 2023-06-16 16:59:58.000000 aolab-aopy-0.6.1/setup.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.352527 aolab-aopy-0.6.1/tests/
+-rw-r--r--   0 leoscholl   (501) staff       (20)    51536 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/tests/test_analysis.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    39331 2023-06-05 23:07:00.000000 aolab-aopy-0.6.1/tests/test_data.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    10364 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/tests/test_postproc.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    25303 2023-06-05 23:07:00.000000 aolab-aopy-0.6.1/tests/test_precondition.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    62987 2023-06-05 23:07:00.000000 aolab-aopy-0.6.1/tests/test_preproc.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      819 2022-07-26 16:06:39.000000 aolab-aopy-0.6.1/tests/test_torch.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2037 2022-07-26 16:06:39.000000 aolab-aopy-0.6.1/tests/test_tutorial_functions.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    17660 2023-06-05 23:07:00.000000 aolab-aopy-0.6.1/tests/test_utils.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    19118 2023-06-05 22:34:47.000000 aolab-aopy-0.6.1/tests/test_visualization.py
```

### Comparing `aolab-aopy-0.6.0/LICENSE` & `aolab-aopy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/PKG-INFO` & `aolab-aopy-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aolab-aopy
-Version: 0.6.0
+Version: 0.6.1
 Summary: Neural data analysis
 Home-page: https://github.com/aolabNeuro/analyze
 Author: aoLab
 Author-email: aolab <aolab.uw@gmail.com>
 Project-URL: Homepage, https://github.com/aolabNeuro/aopy
 Project-URL: Bug Tracker, https://github.com/aolabNeuro/aopy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aolab-aopy-0.6.0/aolab_aopy.egg-info/PKG-INFO` & `aolab-aopy-0.6.1/aolab_aopy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aolab-aopy
-Version: 0.6.0
+Version: 0.6.1
 Summary: Neural data analysis
 Home-page: https://github.com/aolabNeuro/analyze
 Author: aoLab
 Author-email: aolab <aolab.uw@gmail.com>
 Project-URL: Homepage, https://github.com/aolabNeuro/aopy
 Project-URL: Bug Tracker, https://github.com/aolabNeuro/aopy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aolab-aopy-0.6.0/aolab_aopy.egg-info/SOURCES.txt` & `aolab-aopy-0.6.1/aolab_aopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/analysis/accllr.py` & `aolab-aopy-0.6.1/aopy/analysis/accllr.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/analysis/base.py` & `aolab-aopy-0.6.1/aopy/analysis/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/analysis/behavior.py` & `aolab-aopy-0.6.1/aopy/analysis/behavior.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/analysis/celltype.py` & `aolab-aopy-0.6.1/aopy/analysis/celltype.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/analysis/kfdecoder.py` & `aolab-aopy-0.6.1/aopy/analysis/kfdecoder.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/analysis/tuning.py` & `aolab-aopy-0.6.1/aopy/analysis/tuning.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/data/base.py` & `aolab-aopy-0.6.1/aopy/data/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import warnings
 import pickle as pkl
 import numpy as np
 from pandas import read_excel
 import warnings
 import yaml
 import pandas as pd
-
-config_dir = os.path.join(os.path.dirname(__file__), '../config')
+from importlib.resources import files, as_file
 
 ###############################################################################
 # Loading preprocessed data
 ###############################################################################
 def get_filenames_in_dir(base_dir, te):
     '''
     Gets the filenames for available systems in a given task entry. Requires that
@@ -629,24 +628,28 @@
     Returns:
         tuple: Tuple Containing:
             | **acq_ch_position (nelec, 2):** X and Y coordinates of the electrode each acquisition channel gets data from.
                                         X position is in the first column and Y position is in the second column
             | **acq_chs (nelec):** Acquisition channels that map to electrodes (e.g. 240/256 for viventi ECoG array)
             | **connected_elecs (nelec):** Electrodes used (e.g. 240/244 for viventi ECoG array)   
     '''
+    config_files = files('aopy').joinpath('config')
     if drive_type == 'ECoG244':
-        signal_path_filepath = os.path.join(config_dir, '210910_ecog_signal_path.xlsx')
-        elec_to_pos_filepath = os.path.join(config_dir, '244ch_viventi_ecog_elec_to_pos.xlsx')
+        signal_path_filepath = as_file(config_files.joinpath('210910_ecog_signal_path.xlsx'))
+        elec_to_pos_filepath = as_file(config_files.joinpath('244ch_viventi_ecog_elec_to_pos.xlsx'))
     elif drive_type == 'Opto32':
-        signal_path_filepath = os.path.join(config_dir, '221021_opto_signal_path.xlsx')
-        elec_to_pos_filepath = os.path.join(config_dir, '32ch_fiber_optic_assy_elec_to_pos.xlsx')
+        signal_path_filepath = as_file(config_files.joinpath('221021_opto_signal_path.xlsx'))
+        elec_to_pos_filepath = as_file(config_files.joinpath('32ch_fiber_optic_assy_elec_to_pos.xlsx'))
     else:
         raise ValueError('Drive type not supported')
-    signal_path = pd.read_excel(signal_path_filepath)
-    layout = pd.read_excel(elec_to_pos_filepath)
+    
+    with signal_path_filepath as f:
+        signal_path = pd.read_excel(f)
+    with elec_to_pos_filepath as f:
+        layout = pd.read_excel(f)
     if acq_ch_subset is not None:
         acq_ch_subset = np.array(acq_ch_subset, dtype='int')
     return map_acq2pos(signal_path, layout, acq_ch_subset=acq_ch_subset)
 
 def parse_str_list(strings, str_include=None, str_avoid=None):
     '''
     This function parses a list of strings to return the strings that include/avoid specific substrings
```

### Comparing `aolab-aopy-0.6.0/aopy/data/bmi3d.py` & `aolab-aopy-0.6.1/aopy/data/bmi3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import traceback
 
 from .. import precondition
 from ..preproc.base import get_data_segments, get_trial_segments, get_trial_segments_and_times, interp_timestamps2timeseries, sample_timestamped_data, trial_align_data
 from ..whitematter import ChunkedStream, Dataset
 from ..utils import derivative, get_pulse_edge_times, compute_pulse_duty_cycles, convert_digital_to_channels, detect_edges
-from ..data import load_preproc_exp_data, load_preproc_eye_data, load_preproc_lfp_data, yaml_read, config_dir
+from ..data import load_preproc_exp_data, load_preproc_eye_data, load_preproc_lfp_data, yaml_read
 import os
 import numpy as np
 import h5py
 import tables
 import pandas as pd
 from tqdm.auto import tqdm
+from importlib.resources import files, as_file
 
 ############
 # Raw data #
 ############
 def get_ecube_data_sources(data_dir):
     '''
     Lists the available data sources in a given data directory
@@ -763,16 +764,18 @@
         include_eyedata (bool, optional): If True, includes eye trajectories in addition to cursor
             trajectories. Defaults to False.
 
     Returns:
         pd.DataFrame: pandas DataFrame containing the concatenated trial data
     '''
     # Use default "trial" definition
-    params_file = os.path.join(config_dir, 'task_codes.yaml')
-    task_codes = yaml_read(params_file)[0]        
+    config_dir = files('aopy').joinpath('config')
+    params_file = as_file(config_dir.joinpath('task_codes.yaml'))
+    with params_file as f:
+        task_codes = yaml_read(f)[0]
     trial_end_codes = [task_codes['TRIAL_END']]
     reward_codes = [task_codes['REWARD']]
     
     if include_center_target:
         trial_start_codes = [task_codes['CURSOR_ENTER_CENTER_TARGET']]
         penalty_codes = [task_codes['HOLD_PENALTY'], task_codes['TIMEOUT_PENALTY']]
         target_codes = [task_codes['CENTER_TARGET_ON']] + task_codes['PERIPHERAL_TARGET_ON']
```

### Comparing `aolab-aopy-0.6.0/aopy/data/eye.py` & `aolab-aopy-0.6.1/aopy/data/eye.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/data/neuropixel.py` & `aolab-aopy-0.6.1/aopy/data/neuropixel.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/data/optitrack.py` & `aolab-aopy-0.6.1/aopy/data/optitrack.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/data/peslab.py` & `aolab-aopy-0.6.1/aopy/data/peslab.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/postproc/base.py` & `aolab-aopy-0.6.1/aopy/postproc/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/precondition/base.py` & `aolab-aopy-0.6.1/aopy/precondition/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/precondition/eye.py` & `aolab-aopy-0.6.1/aopy/precondition/eye.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/preproc/base.py` & `aolab-aopy-0.6.1/aopy/preproc/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/preproc/bmi3d.py` & `aolab-aopy-0.6.1/aopy/preproc/bmi3d.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/preproc/neuropixel.py` & `aolab-aopy-0.6.1/aopy/preproc/neuropixel.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/preproc/oculomatic.py` & `aolab-aopy-0.6.1/aopy/preproc/oculomatic.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/preproc/optitrack.py` & `aolab-aopy-0.6.1/aopy/preproc/optitrack.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/preproc/quality.py` & `aolab-aopy-0.6.1/aopy/preproc/quality.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/preproc/wrappers.py` & `aolab-aopy-0.6.1/aopy/preproc/wrappers.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/torch.py` & `aolab-aopy-0.6.1/aopy/torch.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/tutorial_functions.py` & `aolab-aopy-0.6.1/aopy/tutorial_functions.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/utils/base.py` & `aolab-aopy-0.6.1/aopy/utils/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/utils/memory.py` & `aolab-aopy-0.6.1/aopy/utils/memory.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/visualization/animation.py` & `aolab-aopy-0.6.1/aopy/visualization/animation.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/visualization/base.py` & `aolab-aopy-0.6.1/aopy/visualization/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/whitematter/dataset.py` & `aolab-aopy-0.6.1/aopy/whitematter/dataset.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/aopy/whitematter/stream.py` & `aolab-aopy-0.6.1/aopy/whitematter/stream.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/pyproject.toml` & `aolab-aopy-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aolab-aopy"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="aolab", email="aolab.uw@gmail.com" },
 ]
 description = "Neural data analysis"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `aolab-aopy-0.6.0/setup.py` & `aolab-aopy-0.6.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     'pyyaml',
     'tqdm',
     'open-ephys-python-tools'
 ]
 
 setuptools.setup(
     name="aopy",
-    version="0.6.0",
+    version="0.6.1",
     author="aoLab",
     author_email="aorsborn@uw.edu",
     description="python code repository for aoLab @UW",
     long_description=long_description,
     url="https://github.com/aolabNeuro/analyze",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `aolab-aopy-0.6.0/tests/test_analysis.py` & `aolab-aopy-0.6.1/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/tests/test_data.py` & `aolab-aopy-0.6.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/tests/test_postproc.py` & `aolab-aopy-0.6.1/tests/test_postproc.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/tests/test_precondition.py` & `aolab-aopy-0.6.1/tests/test_precondition.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/tests/test_preproc.py` & `aolab-aopy-0.6.1/tests/test_preproc.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/tests/test_torch.py` & `aolab-aopy-0.6.1/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/tests/test_tutorial_functions.py` & `aolab-aopy-0.6.1/tests/test_tutorial_functions.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/tests/test_utils.py` & `aolab-aopy-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.0/tests/test_visualization.py` & `aolab-aopy-0.6.1/tests/test_visualization.py`

 * *Files identical despite different names*

