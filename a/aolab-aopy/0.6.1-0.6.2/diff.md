# Comparing `tmp/aolab-aopy-0.6.1.tar.gz` & `tmp/aolab-aopy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aolab-aopy-0.6.1.tar", last modified: Fri Jun 16 17:00:19 2023, max compression
+gzip compressed data, was "aolab-aopy-0.6.2.tar", last modified: Fri Jun 16 17:33:38 2023, max compression
```

## Comparing `aolab-aopy-0.6.1.tar` & `aolab-aopy-0.6.2.tar`

### file list

```diff
@@ -1,72 +1,68 @@
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.352901 aolab-aopy-0.6.1/
--rw-r--r--   0 leoscholl   (501) staff       (20)     1106 2023-06-16 16:22:43.000000 aolab-aopy-0.6.1/LICENSE
--rw-r--r--   0 leoscholl   (501) staff       (20)      749 2023-06-16 17:00:19.352747 aolab-aopy-0.6.1/PKG-INFO
--rw-r--r--   0 leoscholl   (501) staff       (20)      203 2023-03-20 22:49:31.000000 aolab-aopy-0.6.1/README.md
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.343555 aolab-aopy-0.6.1/aolab_aopy.egg-info/
--rw-r--r--   0 leoscholl   (501) staff       (20)      749 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/PKG-INFO
--rw-r--r--   0 leoscholl   (501) staff       (20)     1397 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/SOURCES.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)        1 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/dependency_links.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)      164 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/requires.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)        5 2023-06-16 17:00:19.000000 aolab-aopy-0.6.1/aolab_aopy.egg-info/top_level.txt
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.344153 aolab-aopy-0.6.1/aopy/
--rw-r--r--   0 leoscholl   (501) staff       (20)      241 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/__init__.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.345136 aolab-aopy-0.6.1/aopy/analysis/
--rw-r--r--   0 leoscholl   (501) staff       (20)      271 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/analysis/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    28781 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/analysis/accllr.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    48803 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/analysis/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    13768 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/analysis/behavior.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     7187 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/analysis/celltype.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8263 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/analysis/kfdecoder.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4897 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/analysis/tuning.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.346273 aolab-aopy-0.6.1/aopy/data/
--rw-r--r--   0 leoscholl   (501) staff       (20)       84 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/data/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    32990 2023-06-16 16:58:07.000000 aolab-aopy-0.6.1/aopy/data/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    35802 2023-06-16 16:58:45.000000 aolab-aopy-0.6.1/aopy/data/bmi3d.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3717 2023-03-23 20:22:25.000000 aolab-aopy-0.6.1/aopy/data/eye.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     9471 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/data/neuropixel.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5284 2022-12-19 23:14:32.000000 aolab-aopy-0.6.1/aopy/data/optitrack.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    13116 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/data/peslab.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.346539 aolab-aopy-0.6.1/aopy/postproc/
--rw-r--r--   0 leoscholl   (501) staff       (20)       19 2022-12-19 23:14:32.000000 aolab-aopy-0.6.1/aopy/postproc/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    28672 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/postproc/base.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.346961 aolab-aopy-0.6.1/aopy/precondition/
--rw-r--r--   0 leoscholl   (501) staff       (20)       39 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/precondition/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    32825 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/precondition/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8200 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/precondition/eye.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.348341 aolab-aopy-0.6.1/aopy/preproc/
--rw-r--r--   0 leoscholl   (501) staff       (20)       69 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    33372 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    33999 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/bmi3d.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2577 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/neuropixel.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     7060 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/preproc/oculomatic.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3817 2022-12-19 23:14:32.000000 aolab-aopy-0.6.1/aopy/preproc/optitrack.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     9620 2022-11-29 17:21:22.000000 aolab-aopy-0.6.1/aopy/preproc/quality.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    17132 2023-03-23 20:22:25.000000 aolab-aopy-0.6.1/aopy/preproc/wrappers.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2998 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/torch.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3759 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/tutorial_functions.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.349004 aolab-aopy-0.6.1/aopy/utils/
--rw-r--r--   0 leoscholl   (501) staff       (20)       41 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/utils/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    27126 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/utils/base.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2775 2023-06-05 23:06:59.000000 aolab-aopy-0.6.1/aopy/utils/memory.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.349453 aolab-aopy-0.6.1/aopy/visualization/
--rw-r--r--   0 leoscholl   (501) staff       (20)       44 2023-06-05 22:34:46.000000 aolab-aopy-0.6.1/aopy/visualization/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8138 2023-06-05 22:34:46.000000 aolab-aopy-0.6.1/aopy/visualization/animation.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    45663 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/aopy/visualization/base.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.350530 aolab-aopy-0.6.1/aopy/whitematter/
--rw-r--r--   0 leoscholl   (501) staff       (20)       62 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/whitematter/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      365 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/whitematter/arraymethods.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    15382 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/whitematter/dataset.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5220 2022-07-26 16:06:37.000000 aolab-aopy-0.6.1/aopy/whitematter/stream.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      556 2023-06-16 17:00:09.000000 aolab-aopy-0.6.1/pyproject.toml
--rw-r--r--   0 leoscholl   (501) staff       (20)       38 2023-06-16 17:00:19.352945 aolab-aopy-0.6.1/setup.cfg
--rw-r--r--   0 leoscholl   (501) staff       (20)      897 2023-06-16 16:59:58.000000 aolab-aopy-0.6.1/setup.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:00:19.352527 aolab-aopy-0.6.1/tests/
--rw-r--r--   0 leoscholl   (501) staff       (20)    51536 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/tests/test_analysis.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    39331 2023-06-05 23:07:00.000000 aolab-aopy-0.6.1/tests/test_data.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    10364 2023-06-06 22:20:50.000000 aolab-aopy-0.6.1/tests/test_postproc.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    25303 2023-06-05 23:07:00.000000 aolab-aopy-0.6.1/tests/test_precondition.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    62987 2023-06-05 23:07:00.000000 aolab-aopy-0.6.1/tests/test_preproc.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      819 2022-07-26 16:06:39.000000 aolab-aopy-0.6.1/tests/test_torch.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2037 2022-07-26 16:06:39.000000 aolab-aopy-0.6.1/tests/test_tutorial_functions.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    17660 2023-06-05 23:07:00.000000 aolab-aopy-0.6.1/tests/test_utils.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    19118 2023-06-05 22:34:47.000000 aolab-aopy-0.6.1/tests/test_visualization.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.185778 aolab-aopy-0.6.2/
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1106 2023-06-16 16:22:43.000000 aolab-aopy-0.6.2/LICENSE
+-rw-r--r--   0 leoscholl   (501) staff       (20)      106 2023-06-16 17:33:33.000000 aolab-aopy-0.6.2/MANIFEST.in
+-rw-r--r--   0 leoscholl   (501) staff       (20)      514 2023-06-16 17:33:38.185623 aolab-aopy-0.6.2/PKG-INFO
+-rw-r--r--   0 leoscholl   (501) staff       (20)      203 2023-03-20 22:49:31.000000 aolab-aopy-0.6.2/README.md
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.179397 aolab-aopy-0.6.2/aolab_aopy.egg-info/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      514 2023-06-16 17:33:38.000000 aolab-aopy-0.6.2/aolab_aopy.egg-info/PKG-INFO
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1388 2023-06-16 17:33:38.000000 aolab-aopy-0.6.2/aolab_aopy.egg-info/SOURCES.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)        1 2023-06-16 17:33:38.000000 aolab-aopy-0.6.2/aolab_aopy.egg-info/dependency_links.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)      164 2023-06-16 17:33:38.000000 aolab-aopy-0.6.2/aolab_aopy.egg-info/requires.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)       39 2023-06-16 17:33:38.000000 aolab-aopy-0.6.2/aolab_aopy.egg-info/top_level.txt
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.179807 aolab-aopy-0.6.2/aopy/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      241 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/__init__.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.181010 aolab-aopy-0.6.2/aopy/analysis/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      271 2022-11-29 17:21:22.000000 aolab-aopy-0.6.2/aopy/analysis/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    28781 2023-06-06 22:20:50.000000 aolab-aopy-0.6.2/aopy/analysis/accllr.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    48803 2023-06-06 22:20:50.000000 aolab-aopy-0.6.2/aopy/analysis/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    13768 2023-06-06 22:20:50.000000 aolab-aopy-0.6.2/aopy/analysis/behavior.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     7187 2022-11-29 17:21:22.000000 aolab-aopy-0.6.2/aopy/analysis/celltype.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8263 2022-11-29 17:21:22.000000 aolab-aopy-0.6.2/aopy/analysis/kfdecoder.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4897 2022-11-29 17:21:22.000000 aolab-aopy-0.6.2/aopy/analysis/tuning.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.181691 aolab-aopy-0.6.2/aopy/config/
+-rw-r--r--   0 leoscholl   (501) staff       (20)    16744 2022-08-30 20:59:52.000000 aolab-aopy-0.6.2/aopy/config/210910_ecog_signal_path.xlsx
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9106 2022-11-13 21:49:53.000000 aolab-aopy-0.6.2/aopy/config/221021_opto_signal_path.xlsx
+-rw-r--r--   0 leoscholl   (501) staff       (20)    17347 2022-08-30 20:59:52.000000 aolab-aopy-0.6.2/aopy/config/244ch_viventi_ecog_elec_to_pos.xlsx
+-rw-r--r--   0 leoscholl   (501) staff       (20)    12752 2022-11-13 21:49:53.000000 aolab-aopy-0.6.2/aopy/config/32ch_fiber_optic_assy_elec_to_pos.xlsx
+-rw-r--r--   0 leoscholl   (501) staff       (20)      371 2023-03-23 20:22:25.000000 aolab-aopy-0.6.2/aopy/config/task_codes.yaml
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.182608 aolab-aopy-0.6.2/aopy/data/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       84 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/data/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    32990 2023-06-16 16:58:07.000000 aolab-aopy-0.6.2/aopy/data/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    35802 2023-06-16 16:58:45.000000 aolab-aopy-0.6.2/aopy/data/bmi3d.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3717 2023-03-23 20:22:25.000000 aolab-aopy-0.6.2/aopy/data/eye.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9471 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/data/neuropixel.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5284 2022-12-19 23:14:32.000000 aolab-aopy-0.6.2/aopy/data/optitrack.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    13116 2022-07-26 16:06:37.000000 aolab-aopy-0.6.2/aopy/data/peslab.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.182875 aolab-aopy-0.6.2/aopy/postproc/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       19 2022-12-19 23:14:32.000000 aolab-aopy-0.6.2/aopy/postproc/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    28672 2023-06-06 22:20:50.000000 aolab-aopy-0.6.2/aopy/postproc/base.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.183274 aolab-aopy-0.6.2/aopy/precondition/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       39 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/precondition/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    32825 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/precondition/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8200 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/precondition/eye.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.184198 aolab-aopy-0.6.2/aopy/preproc/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       69 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/preproc/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    33372 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/preproc/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    33999 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/preproc/bmi3d.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2577 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/preproc/neuropixel.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     7060 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/preproc/oculomatic.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3817 2022-12-19 23:14:32.000000 aolab-aopy-0.6.2/aopy/preproc/optitrack.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9620 2022-11-29 17:21:22.000000 aolab-aopy-0.6.2/aopy/preproc/quality.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    17132 2023-03-23 20:22:25.000000 aolab-aopy-0.6.2/aopy/preproc/wrappers.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2998 2022-07-26 16:06:37.000000 aolab-aopy-0.6.2/aopy/torch.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3759 2022-07-26 16:06:37.000000 aolab-aopy-0.6.2/aopy/tutorial_functions.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.184558 aolab-aopy-0.6.2/aopy/utils/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       41 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/utils/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    27126 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/utils/base.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2775 2023-06-05 23:06:59.000000 aolab-aopy-0.6.2/aopy/utils/memory.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.184901 aolab-aopy-0.6.2/aopy/visualization/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       44 2023-06-05 22:34:46.000000 aolab-aopy-0.6.2/aopy/visualization/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8138 2023-06-05 22:34:46.000000 aolab-aopy-0.6.2/aopy/visualization/animation.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    45663 2023-06-06 22:20:50.000000 aolab-aopy-0.6.2/aopy/visualization/base.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 17:33:38.185413 aolab-aopy-0.6.2/aopy/whitematter/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       62 2022-07-26 16:06:37.000000 aolab-aopy-0.6.2/aopy/whitematter/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      365 2022-07-26 16:06:37.000000 aolab-aopy-0.6.2/aopy/whitematter/arraymethods.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    15382 2022-07-26 16:06:37.000000 aolab-aopy-0.6.2/aopy/whitematter/dataset.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5220 2022-07-26 16:06:37.000000 aolab-aopy-0.6.2/aopy/whitematter/stream.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)       38 2023-06-16 17:33:38.185818 aolab-aopy-0.6.2/setup.cfg
+-rw-r--r--   0 leoscholl   (501) staff       (20)      944 2023-06-16 17:29:30.000000 aolab-aopy-0.6.2/setup.py
```

### Comparing `aolab-aopy-0.6.1/LICENSE` & `aolab-aopy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aolab_aopy.egg-info/SOURCES.txt` & `aolab-aopy-0.6.2/aolab_aopy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
+MANIFEST.in
 README.md
-pyproject.toml
 setup.py
 aolab_aopy.egg-info/PKG-INFO
 aolab_aopy.egg-info/SOURCES.txt
 aolab_aopy.egg-info/dependency_links.txt
 aolab_aopy.egg-info/requires.txt
 aolab_aopy.egg-info/top_level.txt
 aopy/__init__.py
@@ -13,14 +13,19 @@
 aopy/analysis/__init__.py
 aopy/analysis/accllr.py
 aopy/analysis/base.py
 aopy/analysis/behavior.py
 aopy/analysis/celltype.py
 aopy/analysis/kfdecoder.py
 aopy/analysis/tuning.py
+aopy/config/210910_ecog_signal_path.xlsx
+aopy/config/221021_opto_signal_path.xlsx
+aopy/config/244ch_viventi_ecog_elec_to_pos.xlsx
+aopy/config/32ch_fiber_optic_assy_elec_to_pos.xlsx
+aopy/config/task_codes.yaml
 aopy/data/__init__.py
 aopy/data/base.py
 aopy/data/bmi3d.py
 aopy/data/eye.py
 aopy/data/neuropixel.py
 aopy/data/optitrack.py
 aopy/data/peslab.py
@@ -42,17 +47,8 @@
 aopy/utils/memory.py
 aopy/visualization/__init__.py
 aopy/visualization/animation.py
 aopy/visualization/base.py
 aopy/whitematter/__init__.py
 aopy/whitematter/arraymethods.py
 aopy/whitematter/dataset.py
-aopy/whitematter/stream.py
-tests/test_analysis.py
-tests/test_data.py
-tests/test_postproc.py
-tests/test_precondition.py
-tests/test_preproc.py
-tests/test_torch.py
-tests/test_tutorial_functions.py
-tests/test_utils.py
-tests/test_visualization.py
+aopy/whitematter/stream.py
```

### Comparing `aolab-aopy-0.6.1/aopy/analysis/accllr.py` & `aolab-aopy-0.6.2/aopy/analysis/accllr.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/analysis/base.py` & `aolab-aopy-0.6.2/aopy/analysis/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/analysis/behavior.py` & `aolab-aopy-0.6.2/aopy/analysis/behavior.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/analysis/celltype.py` & `aolab-aopy-0.6.2/aopy/analysis/celltype.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/analysis/kfdecoder.py` & `aolab-aopy-0.6.2/aopy/analysis/kfdecoder.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/analysis/tuning.py` & `aolab-aopy-0.6.2/aopy/analysis/tuning.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/data/base.py` & `aolab-aopy-0.6.2/aopy/data/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/data/bmi3d.py` & `aolab-aopy-0.6.2/aopy/data/bmi3d.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/data/eye.py` & `aolab-aopy-0.6.2/aopy/data/eye.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/data/neuropixel.py` & `aolab-aopy-0.6.2/aopy/data/neuropixel.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/data/optitrack.py` & `aolab-aopy-0.6.2/aopy/data/optitrack.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/data/peslab.py` & `aolab-aopy-0.6.2/aopy/data/peslab.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/postproc/base.py` & `aolab-aopy-0.6.2/aopy/postproc/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/precondition/base.py` & `aolab-aopy-0.6.2/aopy/precondition/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/precondition/eye.py` & `aolab-aopy-0.6.2/aopy/precondition/eye.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/preproc/base.py` & `aolab-aopy-0.6.2/aopy/preproc/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/preproc/bmi3d.py` & `aolab-aopy-0.6.2/aopy/preproc/bmi3d.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/preproc/neuropixel.py` & `aolab-aopy-0.6.2/aopy/preproc/neuropixel.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/preproc/oculomatic.py` & `aolab-aopy-0.6.2/aopy/preproc/oculomatic.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/preproc/optitrack.py` & `aolab-aopy-0.6.2/aopy/preproc/optitrack.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/preproc/quality.py` & `aolab-aopy-0.6.2/aopy/preproc/quality.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/preproc/wrappers.py` & `aolab-aopy-0.6.2/aopy/preproc/wrappers.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/torch.py` & `aolab-aopy-0.6.2/aopy/torch.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/tutorial_functions.py` & `aolab-aopy-0.6.2/aopy/tutorial_functions.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/utils/base.py` & `aolab-aopy-0.6.2/aopy/utils/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/utils/memory.py` & `aolab-aopy-0.6.2/aopy/utils/memory.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/visualization/animation.py` & `aolab-aopy-0.6.2/aopy/visualization/animation.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/visualization/base.py` & `aolab-aopy-0.6.2/aopy/visualization/base.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/whitematter/dataset.py` & `aolab-aopy-0.6.2/aopy/whitematter/dataset.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/aopy/whitematter/stream.py` & `aolab-aopy-0.6.2/aopy/whitematter/stream.py`

 * *Files identical despite different names*

### Comparing `aolab-aopy-0.6.1/setup.py` & `aolab-aopy-0.6.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,21 +25,22 @@
     'seaborn',
     'pyyaml',
     'tqdm',
     'open-ephys-python-tools'
 ]
 
 setuptools.setup(
-    name="aopy",
-    version="0.6.1",
+    name="aolab-aopy",
+    version="0.6.2",
     author="aoLab",
     author_email="aorsborn@uw.edu",
     description="python code repository for aoLab @UW",
     long_description=long_description,
     url="https://github.com/aolabNeuro/analyze",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_namespace_packages(),
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent"
     ],
     install_requires=install_requires,
 )
```

