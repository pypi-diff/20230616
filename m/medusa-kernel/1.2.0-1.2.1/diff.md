# Comparing `tmp/medusa-kernel-1.2.0.tar.gz` & `tmp/medusa-kernel-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-kernel-1.2.0.tar", last modified: Thu Jun  8 10:18:31 2023, max compression
+gzip compressed data, was "medusa-kernel-1.2.1.tar", last modified: Fri Jun 16 11:09:54 2023, max compression
```

## Comparing `medusa-kernel-1.2.0.tar` & `medusa-kernel-1.2.1.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.679426 medusa-kernel-1.2.0/medusa/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/artifact_removal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.679426 medusa-kernel-1.2.0/medusa/bci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/cvep_spellers.py
--rw-r--r--   0 runner    (1001) docker     (123)   106155 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/erp_spellers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    59073 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/mi_paradigms.py
--rw-r--r--   0 runner    (1001) docker     (123)    38619 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/nft_paradigms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/classification_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    67256 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.683426 medusa-kernel-1.2.0/medusa/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/connectivity/amplitude_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/connectivity/phase_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    67167 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/deep_learning_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/emg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/epoching.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/frequency_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.687425 medusa-kernel-1.2.0/medusa/graph_theory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/assortativity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/betweeenness_centrality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/clustering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/degree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/eigen_centrality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/modularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/participation_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/path_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/surrogate_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/transitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.687425 medusa-kernel-1.2.0/medusa/local_activation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   330752 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/computeLZC.dll
--rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/nonlinear_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/spectral_parameteres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.691425 medusa-kernel-1.2.0/medusa/meeg/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-05_2D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-05_3D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-10_2D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-10_3D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-20_2D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-20_3D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    33137 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/meeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/meeg_montages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/nirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/notify_me.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/performance_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.691425 medusa-kernel-1.2.0/medusa/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/brain_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/erp_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/generic_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    20860 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/head_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/mi_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/optimal_subplots.py
--rw-r--r--   0 runner    (1001) docker     (123)    21087 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/timeplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    20211 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/topographic_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/signal_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/signal_orthogonalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    34207 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/spatial_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/tensorflow_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/medusa_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/tests/local_activation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/local_activation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/plots/test_topographics_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/test_signal_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.931995 medusa-kernel-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-16 11:09:54.931995 medusa-kernel-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.923995 medusa-kernel-1.2.1/medusa/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18934 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/artifact_removal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.923995 medusa-kernel-1.2.1/medusa/bci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/bci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/bci/cvep_spellers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106155 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/bci/erp_spellers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/bci/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59073 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/bci/mi_paradigms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38619 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/bci/nft_paradigms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/classification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67256 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.923995 medusa-kernel-1.2.1/medusa/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/connectivity/amplitude_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/connectivity/phase_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67167 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/deep_learning_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/emg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/epoching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/frequency_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.927996 medusa-kernel-1.2.1/medusa/graph_theory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/betweeenness_centrality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/clustering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/degree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/eigen_centrality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/modularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/participation_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/path_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/surrogate_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/graph_theory/transitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.927996 medusa-kernel-1.2.1/medusa/local_activation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/local_activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   330752 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/local_activation/computeLZC.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/local_activation/nonlinear_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/local_activation/spectral_parameteres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/local_activation/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.927996 medusa-kernel-1.2.1/medusa/meeg/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-05_2D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-05_3D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-10_2D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-10_3D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-20_2D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-20_3D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    32952 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/meeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/meeg/meeg_montages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/nirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/notify_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/performance_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.931995 medusa-kernel-1.2.1/medusa/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/plots/brain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/plots/erp_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/plots/generic_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20859 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/plots/head_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/plots/mi_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/plots/optimal_subplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22746 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/plots/timeplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/signal_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/signal_orthogonalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34207 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/spatial_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/tensorflow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/medusa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.931995 medusa-kernel-1.2.1/medusa_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-16 11:09:54.000000 medusa-kernel-1.2.1/medusa_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-16 11:09:54.000000 medusa-kernel-1.2.1/medusa_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:09:54.000000 medusa-kernel-1.2.1/medusa_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-16 11:09:54.000000 medusa-kernel-1.2.1/medusa_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 11:09:54.000000 medusa-kernel-1.2.1/medusa_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:09:54.931995 medusa-kernel-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.931995 medusa-kernel-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.931995 medusa-kernel-1.2.1/tests/local_activation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/tests/local_activation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:54.931995 medusa-kernel-1.2.1/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/tests/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/tests/plots/test_topographics_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/tests/test_signal_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-16 11:09:42.000000 medusa-kernel-1.2.1/tests/test_transforms.py
```

### Comparing `medusa-kernel-1.2.0/LICENSE` & `medusa-kernel-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/PKG-INFO` & `medusa-kernel-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-kernel
-Version: 1.2.0
+Version: 1.2.1
 Summary: Advanced biosignal processing toolbox
 Home-page: https://medusabci.com/
 Author: Eduardo Santamaría-Vázquez, Víctor Martínez-Cagigal, Diego Marcos-Martínez, Víctor Rodríguez-González, Sergio Pérez-Velasco
 Author-email: support@medusabci.com
 License: CC Attribution-NonCommercial-NoDerivs 2.0
 Keywords: Signal,Biosignal,EEG,BCI
 Classifier: Development Status :: 4 - Beta
```

### Comparing `medusa-kernel-1.2.0/README.md` & `medusa-kernel-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/artifact_removal.py` & `medusa-kernel-1.2.1/medusa/artifact_removal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # External imports
-import numpy as npMinor
+import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 from scipy.signal import welch
 
 # Medusa imports
 from medusa.plots.head_plots import plot_head,plot_topography
 from medusa.meeg.meeg import EEGChannelSet
@@ -352,15 +352,15 @@
 
         if ch_offset is None:
             ch_offset = np.max(np.abs(sources[:, 0]))
         fig, ax = plt.subplots(1,1)
         time_plot(sources, self.fs, self.ica_labels,
                             ch_to_show=sources_to_show,
                             time_to_show=time_to_show,
-                            channel_offset=ch_offset,show=False,fig=fig,
+                            ch_offset=ch_offset,show=False,fig=fig,
                   axes=ax)
 
     def plot_summary(self, signal, component, psd_freq_range=[1,70],
                      psd_window='hamming', time_to_show=2,cmap='bwr'):
         # Check error
         if isinstance(component,int):
             component = np.array([component])
```

### Comparing `medusa-kernel-1.2.0/medusa/bci/cvep_spellers.py` & `medusa-kernel-1.2.1/medusa/bci/cvep_spellers.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/bci/erp_spellers.py` & `medusa-kernel-1.2.1/medusa/bci/erp_spellers.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/bci/metrics.py` & `medusa-kernel-1.2.1/medusa/bci/metrics.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/bci/mi_paradigms.py` & `medusa-kernel-1.2.1/medusa/bci/mi_paradigms.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/bci/nft_paradigms.py` & `medusa-kernel-1.2.1/medusa/bci/nft_paradigms.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/classification_utils.py` & `medusa-kernel-1.2.1/medusa/classification_utils.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/components.py` & `medusa-kernel-1.2.1/medusa/components.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/connectivity/amplitude_connectivity.py` & `medusa-kernel-1.2.1/medusa/connectivity/amplitude_connectivity.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/connectivity/phase_connectivity.py` & `medusa-kernel-1.2.1/medusa/connectivity/phase_connectivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     angles_2 = np.tile(phase_data, (1, 1, n_chan))
 
     if measure == 'pli':
         return __pli(angles_1, angles_2, n_epochs, n_chan, 'CPU')
     elif measure == 'wpli':
         return __wpli(angles_1, angles_2, n_epochs, n_chan, 'CPU')
     elif measure == 'plv':
-        return __plv(angles_1, angles_2, n_epochs, n_chan, 'CPU')
+        return __plv(angles_1, angles_2, n_epochs, n_samples, n_chan, 'CPU')
     else:
-        plv = __plv(angles_1, angles_2, n_epochs, n_chan, 'CPU')
+        plv = __plv(angles_1, angles_2, n_epochs, n_samples, n_chan, 'CPU')
         pli = __pli(angles_1, angles_2, n_epochs, n_chan, 'CPU')
         wpli = __wpli(angles_1, angles_2, n_epochs, n_chan, 'CPU')
         return plv, pli, wpli
 
 
 def __phase_connectivity_gpu(data, measure=None):
     """ This method implements three phase-based connectivity parameters using
```

### Comparing `medusa-kernel-1.2.0/medusa/deep_learning_models.py` & `medusa-kernel-1.2.1/medusa/deep_learning_models.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/emg.py` & `medusa-kernel-1.2.1/medusa/emg.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/epoching.py` & `medusa-kernel-1.2.1/medusa/epoching.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/frequency_filtering.py` & `medusa-kernel-1.2.1/medusa/frequency_filtering.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/assortativity.py` & `medusa-kernel-1.2.1/medusa/graph_theory/assortativity.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/betweeenness_centrality.py` & `medusa-kernel-1.2.1/medusa/graph_theory/betweeenness_centrality.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/clustering_coefficient.py` & `medusa-kernel-1.2.1/medusa/graph_theory/clustering_coefficient.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/complexity.py` & `medusa-kernel-1.2.1/medusa/graph_theory/complexity.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/degree.py` & `medusa-kernel-1.2.1/medusa/graph_theory/degree.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/density.py` & `medusa-kernel-1.2.1/medusa/graph_theory/density.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/efficiency.py` & `medusa-kernel-1.2.1/medusa/graph_theory/efficiency.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/eigen_centrality.py` & `medusa-kernel-1.2.1/medusa/graph_theory/eigen_centrality.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/modularity.py` & `medusa-kernel-1.2.1/medusa/graph_theory/modularity.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/participation_coefficient.py` & `medusa-kernel-1.2.1/medusa/graph_theory/participation_coefficient.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/path_length.py` & `medusa-kernel-1.2.1/medusa/graph_theory/path_length.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/surrogate_graph.py` & `medusa-kernel-1.2.1/medusa/graph_theory/surrogate_graph.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/graph_theory/transitivity.py` & `medusa-kernel-1.2.1/medusa/graph_theory/transitivity.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/local_activation/computeLZC.dll` & `medusa-kernel-1.2.1/medusa/local_activation/computeLZC.dll`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/local_activation/nonlinear_parameters.py` & `medusa-kernel-1.2.1/medusa/local_activation/nonlinear_parameters.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/local_activation/spectral_parameteres.py` & `medusa-kernel-1.2.1/medusa/local_activation/spectral_parameteres.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/local_activation/statistics.py` & `medusa-kernel-1.2.1/medusa/local_activation/statistics.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-05_2D.tsv` & `medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-05_2D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-05_3D.tsv` & `medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-05_3D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-10_2D.tsv` & `medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-10_2D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-10_3D.tsv` & `medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-10_3D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-20_3D.tsv` & `medusa-kernel-1.2.1/medusa/meeg/eeg_standard_10-20_3D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/meeg/meeg.py` & `medusa-kernel-1.2.1/medusa/meeg/meeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from medusa import meeg
 
 
 class MEEGChannel(components.SerializableComponent):
     """This class implements a M/EEG channel.
     """
 
-    # TODO: This class is till not being used for compatibility reasons, but it
+    # TODO: This class is still not being used for compatibility reasons, but it
     #  should be introduced in the next major update of medusa kernel to remove
     #  channel dictionaries and simplify the management of MEEG signals
 
     def __init__(self, label, coordinates=None, reference=None):
         """Constructor for class MEEGChannel.
 
         Parameters
@@ -211,15 +211,15 @@
         self.channels = channels
         self.ground = ground
         self.n_cha = len(self.channels)
         self.l_cha = [cha['label'] for cha in self.channels]
 
     def set_standard_montage(self, l_cha=None, l_reference=None, l_ground=None,
                              montage='10-05', drop_landmarks=True,
-                             allow_unlocated_channels=False, standard=None):
+                             allow_unlocated_channels=False):
         """Set standard EEG channels with common reference. In 3 dimensions,
         the equator is taken a Nz-T10-Iz-T9.
 
         Parameters
         ----------
         l_cha : list, optional
             List of channels labels. The data will be returned keeping the
@@ -246,29 +246,25 @@
         allow_unlocated_channels: bool
             If False, all the labels in parameter l_cha must be contained in the
             montage, which contains the corresponding coordinates. If True, the
             channels may not be in the standard, and they will be saved with no
             coordinates. This allows to save labels that are not defined in the
             montage, but the behaviour in functions that need locations
             (e.g., topographic_plots) is unpredictable.
-        standard: str
-            DEPRECATED. Only left for compatibility reasons.
         """
         # Check errors
         if self.reference_method != 'common':
             raise ValueError('Function set_standard_channels is available '
                              'only for recordings with common reference. For '
                              'custom montages use set_custom_channels')
         assert self.dim == '2D' or self.dim == '3D', \
             'Incorrect input on dim parameter'
         assert self.coord_system == 'cartesian' or \
                self.coord_system == 'spherical', \
             'Incorrect input on coord_system parameter'
-        # Compatibility
-        montage = standard if standard is not None else montage
         # Get montage
         if isinstance(montage, str):
             # Load standard montage
             self.montage = montage
             montage = meeg.get_standard_montage(standard=montage,
                                                 dim=self.dim,
                                                 coord_system=self.coord_system)
```

### Comparing `medusa-kernel-1.2.0/medusa/meeg/meeg_montages.py` & `medusa-kernel-1.2.1/medusa/meeg/meeg_montages.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/nirs.py` & `medusa-kernel-1.2.1/medusa/nirs.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/notify_me.py` & `medusa-kernel-1.2.1/medusa/notify_me.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/optimization.py` & `medusa-kernel-1.2.1/medusa/optimization.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/plots/brain_plots.py` & `medusa-kernel-1.2.1/medusa/plots/brain_plots.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/plots/erp_plots.py` & `medusa-kernel-1.2.1/medusa/plots/erp_plots.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/plots/generic_plots.py` & `medusa-kernel-1.2.1/medusa/plots/generic_plots.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/plots/head_plots.py` & `medusa-kernel-1.2.1/medusa/plots/head_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
     from matplotlib import pyplot as plt
     from medusa.meeg.meeg import EEGChannelSet
     from medusa.plots.head_plots import *
     import numpy as np
 
     # Set channel set
     channel_set = EEGChannelSet()
-    channel_set.set_standard_montage(standard='10-20')
+    channel_set.set_standard_montage(montage='10-20')
 
     # Initialize figure
     fig = plt.figure()
     fig.add_subplot(1, 1, 1)
 
     # # Plot topography
     # values = np.random.random(channel_set.n_cha)
```

### Comparing `medusa-kernel-1.2.0/medusa/plots/mi_plots.py` & `medusa-kernel-1.2.1/medusa/plots/mi_plots.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/plots/optimal_subplots.py` & `medusa-kernel-1.2.1/medusa/plots/optimal_subplots.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/plots/timeplot.py` & `medusa-kernel-1.2.1/medusa/plots/timeplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Created on Thu Aug 25 17:09:18 2022
 Edited on Mon Jan 09 14:00:00 2023
 @author: Diego Marcos-Martínez
 """
+import warnings
+
 # External imports
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib
 
 matplotlib.use('Qt5Agg')
 from matplotlib.widgets import Slider
@@ -18,15 +20,15 @@
 
 def __plot_epochs_lines(ax, blocks, samples_per_block, fs, min_val, max_val):
     """Aux function to plot vertical lines in case of signal is divided in two
         or more epochs"""
     t_ = np.arange(1,blocks) * int(samples_per_block / fs)
     ax.vlines(t_, min_val, max_val, colors='k',
                   linewidth=2, linestyles='solid')
-def __plot_events_lines(ax, events_dict, min_val, max_val):
+def __plot_events_lines(ax, events_dict, min_val, max_val, display_times):
     """Aux function to plot vertical lines corresponding  to marked events"""
     # Check errors
     if not isinstance(events_dict, dict):
         raise ValueError("'events_dict' must be a dict."
                          "Please, read carefully the time_plot documentation"
                          "to know how to define 'events_dict' properly. ")
     if not 'events' in events_dict.keys():
@@ -53,14 +55,20 @@
 
     if ax.legend_ is not None:
         handles, labels = ax.get_legend_handles_labels()
         previous_conditions = list(np.unique(labels))
 
 
     events_timestamps = np.array(events_dict['events_times'])
+
+    # Check if events_timestamps are referenced to recording start
+    if np.any(events_timestamps > display_times[-1]):
+        raise ValueError("Incorrect format of events_timestamps. "
+                         "The values must be referenced to the beginning "
+                         "of the record, so that the first timestamp has value 0.")
     for event_idx, event_type in enumerate(set(events_order)):
         t_ = events_timestamps[events_order == event_type]
         l = ax.vlines(t_, min_val, max_val, colors=cmap[event_idx],
                       linewidth=2, linestyles='dashed',
                       label=events_names[event_idx])
         if event_type not in legend_lines.keys():
             legend_lines[event_type] = l
@@ -112,29 +120,54 @@
     if not isinstance(condition_timestamps,np.ndarray) and \
         not isinstance(condition_timestamps,list):
         condition_timestamps = np.asarray([condition_timestamps])
         labels_order = np.array([conditions_dict['conditions_labels']])
     else:
         labels_order = np.array(conditions_dict['conditions_labels'])
 
+    # Check if timestamps are referenced to recording start
+    if np.any(condition_timestamps > display_times[-1]):
+        raise ValueError("Incorrect format of condition_timestamps. "
+                         "The values must be referenced to the beginning "
+                         "of the record, so that the first timestamp has value 0.")
+
     # Check if all conditions have a start and an end and fix it if not
     c_idx = 0
+    corrected = False
     while c_idx < len(labels_order)-1:
-    # for c_idx in range(len(labels_order)):
-        if (labels_order[c_idx] != labels_order[c_idx+1]) and \
-            (condition_timestamps[c_idx] != condition_timestamps[c_idx+1]):
-            labels_order = np.insert(labels_order,c_idx+1,labels_order[c_idx])
-            condition_timestamps = np.insert(condition_timestamps,
-                                             c_idx+1,
-                                             condition_timestamps[c_idx+1])
+        if (labels_order[c_idx] != labels_order[c_idx+1]):
+            if c_idx != 0:
+                if labels_order[c_idx] != labels_order[c_idx-1]:
+                    labels_order = np.insert(labels_order, c_idx + 1,
+                                             labels_order[c_idx])
+                    condition_timestamps = np.insert(condition_timestamps,
+                                                     c_idx + 1,
+                                                     condition_timestamps[
+                                                         c_idx + 1])
+                    corrected = True
+            else:
+                labels_order = np.insert(labels_order,c_idx+1,labels_order[c_idx])
+                condition_timestamps = np.insert(condition_timestamps,
+                                                 c_idx+1,
+                                                 condition_timestamps[c_idx+1])
+                corrected = True
         c_idx += 1
     if labels_order[-1] != labels_order[-2]:
         labels_order = np.append(labels_order,labels_order[-1])
         condition_timestamps = np.append(condition_timestamps,
                                                  display_times[-1])
+        corrected = True
+
+    if corrected:
+        warnings.warn("The dictionary of conditions does not follow the "
+                "correct format ([Start condition X, End condition X,"
+                " Start condition Y, End condition Y ...]). "
+                "The labels and timestamps vector has been "
+                "automatically corrected. Check that the OK "
+                "is correct. ")
 
     cmap = plt.get_cmap('jet')(np.linspace(0,1,len(conditions_names)))
 
     for condition_margin_idx in np.arange(0,len(condition_timestamps),2):
         l = ax.fill_betweenx([min_val,max_val],
                              condition_timestamps[condition_margin_idx],
                              condition_timestamps[condition_margin_idx+1],
@@ -401,15 +434,15 @@
     #  Call the aux function to plot conditions
     if conditions_dict is not None:
         __plot_condition_shades(axes, conditions_dict, display_times,
                                 min_val, max_val)
 
     #  Call the aux function to plot vertical lines to mark the events
     if events_dict is not None:
-        __plot_events_lines(axes, events_dict, min_val, max_val)
+        __plot_events_lines(axes, events_dict, min_val, max_val, display_times)
 
     # Plot the signal
     axes.plot(display_times, epoch_c, color, linewidth=0.5)
     axes.set_yticks(-ch_off, labels=ch_labels)
     if len(ch_off) > 1:
         axes.set_ylim(-ch_off[max_y - 1] - 0.5 * ch_off[1],
                       -ch_off[0] + 0.5 * ch_off[1])
```

### Comparing `medusa-kernel-1.2.0/medusa/signal_generators.py` & `medusa-kernel-1.2.1/medusa/signal_generators.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/signal_orthogonalization.py` & `medusa-kernel-1.2.1/medusa/signal_orthogonalization.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/spatial_filtering.py` & `medusa-kernel-1.2.1/medusa/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/tensorflow_integration.py` & `medusa-kernel-1.2.1/medusa/tensorflow_integration.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa/transforms.py` & `medusa-kernel-1.2.1/medusa/transforms.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.2.0/medusa_kernel.egg-info/PKG-INFO` & `medusa-kernel-1.2.1/medusa_kernel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-kernel
-Version: 1.2.0
+Version: 1.2.1
 Summary: Advanced biosignal processing toolbox
 Home-page: https://medusabci.com/
 Author: Eduardo Santamaría-Vázquez, Víctor Martínez-Cagigal, Diego Marcos-Martínez, Víctor Rodríguez-González, Sergio Pérez-Velasco
 Author-email: support@medusabci.com
 License: CC Attribution-NonCommercial-NoDerivs 2.0
 Keywords: Signal,Biosignal,EEG,BCI
 Classifier: Development Status :: 4 - Beta
```

### Comparing `medusa-kernel-1.2.0/medusa_kernel.egg-info/SOURCES.txt` & `medusa-kernel-1.2.1/medusa_kernel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 medusa/plots/brain_plots.py
 medusa/plots/erp_plots.py
 medusa/plots/generic_plots.py
 medusa/plots/head_plots.py
 medusa/plots/mi_plots.py
 medusa/plots/optimal_subplots.py
 medusa/plots/timeplot.py
-medusa/plots/topographic_plots.py
 medusa_kernel.egg-info/PKG-INFO
 medusa_kernel.egg-info/SOURCES.txt
 medusa_kernel.egg-info/dependency_links.txt
 medusa_kernel.egg-info/requires.txt
 medusa_kernel.egg-info/top_level.txt
 tests/__init__.py
 tests/test_components.py
```

### Comparing `medusa-kernel-1.2.0/setup.py` & `medusa-kernel-1.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='medusa-kernel',
     packages=find_packages(),
-    version='1.2.0',
+    version='1.2.1',
     keywords=['Signal', 'Biosignal', 'EEG', 'BCI'],
     url='https://medusabci.com/',
     author='Eduardo Santamaría-Vázquez, '
            'Víctor Martínez-Cagigal, '
            'Diego Marcos-Martínez, '
            'Víctor Rodríguez-González, '
            'Sergio Pérez-Velasco',
```

