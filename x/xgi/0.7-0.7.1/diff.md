# Comparing `tmp/xgi-0.7.tar.gz` & `tmp/xgi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgi-0.7.tar", last modified: Thu Jun  8 12:37:05 2023, max compression
+gzip compressed data, was "xgi-0.7.1.tar", last modified: Fri Jun 16 13:32:34 2023, max compression
```

## Comparing `xgi-0.7.tar` & `xgi-0.7.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.673583 xgi-0.7/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2184 2023-05-30 02:43:06.000000 xgi-0.7/CITATION.cff
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    13449 2023-05-30 02:43:06.000000 xgi-0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3092 2023-06-08 12:32:19.000000 xgi-0.7/CONTRIBUTING.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5426 2023-04-14 16:11:20.000000 xgi-0.7/LICENSE.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      373 2023-05-05 16:04:30.000000 xgi-0.7/MANIFEST.in
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4028 2023-06-08 12:37:05.673446 xgi-0.7/PKG-INFO
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5643 2023-05-30 02:43:06.000000 xgi-0.7/README.md
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.657726 xgi-0.7/logo/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2807 2022-10-13 17:38:17.000000 xgi-0.7/logo/logo.pdf
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    56414 2022-10-13 17:38:17.000000 xgi-0.7/logo/logo.png
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9082 2022-10-13 17:38:17.000000 xgi-0.7/logo/logo.svg
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3264 2023-05-30 02:43:06.000000 xgi-0.7/long_description.rst
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      157 2022-10-13 17:38:17.000000 xgi-0.7/pytest.ini
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.658629 xgi-0.7/requirements/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      610 2022-10-13 17:38:17.000000 xgi-0.7/requirements/README.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       23 2022-11-02 17:36:41.000000 xgi-0.7/requirements/benchmarks.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       78 2023-05-30 02:43:06.000000 xgi-0.7/requirements/default.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       66 2023-05-21 19:12:05.000000 xgi-0.7/requirements/developer.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       93 2023-05-30 02:43:06.000000 xgi-0.7/requirements/documentation.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       39 2023-01-03 14:13:27.000000 xgi-0.7/requirements/release.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       27 2023-05-30 02:43:06.000000 xgi-0.7/requirements/test.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       58 2023-05-30 02:43:06.000000 xgi-0.7/requirements/tutorial.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       38 2023-06-08 12:37:05.673632 xgi-0.7/setup.cfg
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1853 2023-06-08 12:30:47.000000 xgi-0.7/setup.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.661683 xgi-0.7/tutorials/
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.663576 xgi-0.7/tutorials/.ipynb_checkpoints/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9419 2023-05-16 00:58:28.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 1 - Basic Hypergraph Functionality-checkpoint.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3684 2023-05-16 00:58:31.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 2 - Read and Write-checkpoint.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    18547 2023-05-16 00:59:22.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 3 - Basic simplicial complex usage-checkpoint.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7554 2023-05-16 01:02:54.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 4 - Generative_Models-checkpoint.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   858870 2023-05-16 01:03:14.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 5 - Plotting-checkpoint.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57344 2023-05-16 01:03:26.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 6 - Statistics-checkpoint.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   987717 2023-05-16 01:20:02.000000 xgi-0.7/tutorials/.ipynb_checkpoints/quickstart-checkpoint.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9404 2023-05-16 02:41:54.000000 xgi-0.7/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3714 2023-05-16 02:41:54.000000 xgi-0.7/tutorials/Tutorial 2 - Read and Write.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    18606 2023-05-16 02:41:54.000000 xgi-0.7/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7560 2023-05-16 02:41:54.000000 xgi-0.7/tutorials/Tutorial 4 - Generative_Models.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   858869 2023-06-08 12:07:46.000000 xgi-0.7/tutorials/Tutorial 5 - Plotting.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57352 2023-05-30 02:43:06.000000 xgi-0.7/tutorials/Tutorial 6 - Statistics.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   214664 2023-06-08 12:07:46.000000 xgi-0.7/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   119598 2023-06-08 12:07:46.000000 xgi-0.7/tutorials/Tutorial 8 - Directed Hypergraphs.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57003 2023-05-30 02:43:06.000000 xgi-0.7/tutorials/case_study_zhang2022.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   987944 2023-05-30 02:43:06.000000 xgi-0.7/tutorials/quickstart.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   150550 2023-05-05 16:04:30.000000 xgi-0.7/tutorials/simplicial_kuramoto_example.ipynb
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.664754 xgi-0.7/xgi/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      464 2022-11-02 17:36:41.000000 xgi-0.7/xgi/__init__.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.666472 xgi-0.7/xgi/algorithms/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      198 2023-05-30 02:43:06.000000 xgi-0.7/xgi/algorithms/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4776 2023-06-05 15:50:23.000000 xgi-0.7/xgi/algorithms/assortativity.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    12403 2023-06-08 12:07:46.000000 xgi-0.7/xgi/algorithms/centrality.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7654 2023-06-08 12:07:46.000000 xgi-0.7/xgi/algorithms/clustering.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5393 2023-05-30 02:43:06.000000 xgi-0.7/xgi/algorithms/connected.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3094 2023-06-05 15:50:23.000000 xgi-0.7/xgi/algorithms/shortest_path.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.668381 xgi-0.7/xgi/classes/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      190 2023-06-01 16:27:59.000000 xgi-0.7/xgi/classes/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    27188 2023-06-05 15:50:23.000000 xgi-0.7/xgi/classes/dihypergraph.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    22417 2023-06-05 15:50:23.000000 xgi-0.7/xgi/classes/direportviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    25904 2023-06-08 12:07:46.000000 xgi-0.7/xgi/classes/function.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    41479 2023-06-01 16:27:59.000000 xgi-0.7/xgi/classes/hypergraph.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2759 2023-05-30 02:43:06.000000 xgi-0.7/xgi/classes/hypergraphviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    23879 2023-06-05 15:50:23.000000 xgi-0.7/xgi/classes/reportviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    26648 2023-05-30 02:43:06.000000 xgi-0.7/xgi/classes/simplicialcomplex.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    24139 2023-06-01 16:27:59.000000 xgi-0.7/xgi/convert.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.668848 xgi-0.7/xgi/drawing/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2023-05-30 02:43:06.000000 xgi-0.7/xgi/drawing/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    60282 2023-06-08 12:13:47.000000 xgi-0.7/xgi/drawing/draw.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    15065 2023-05-30 02:43:06.000000 xgi-0.7/xgi/drawing/layout.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.669118 xgi-0.7/xgi/dynamics/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       61 2022-11-02 17:36:41.000000 xgi-0.7/xgi/dynamics/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8892 2023-05-30 02:43:06.000000 xgi-0.7/xgi/dynamics/synchronization.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      247 2022-10-13 17:38:17.000000 xgi-0.7/xgi/exception.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.670190 xgi-0.7/xgi/generators/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      227 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7405 2023-06-08 12:07:46.000000 xgi-0.7/xgi/generators/classic.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1411 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/lattice.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10637 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/random.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2749 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/simple.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8505 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/simplicial_complexes.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10058 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/uniform.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.670989 xgi-0.7/xgi/linalg/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      183 2023-05-30 02:43:06.000000 xgi-0.7/xgi/linalg/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7002 2023-05-30 02:43:06.000000 xgi-0.7/xgi/linalg/hodge_matrix.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8447 2023-05-30 02:43:06.000000 xgi-0.7/xgi/linalg/hypergraph_matrix.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6715 2023-05-30 02:43:06.000000 xgi-0.7/xgi/linalg/laplacian_matrix.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.672087 xgi-0.7/xgi/readwrite/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      215 2023-06-05 15:56:16.000000 xgi-0.7/xgi/readwrite/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3010 2023-06-08 12:13:50.000000 xgi-0.7/xgi/readwrite/bigg_data.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6048 2023-05-30 02:43:06.000000 xgi-0.7/xgi/readwrite/bipartite.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4157 2023-03-17 19:59:22.000000 xgi-0.7/xgi/readwrite/edgelist.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2181 2023-05-30 02:43:06.000000 xgi-0.7/xgi/readwrite/incidence.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1892 2023-05-30 02:43:06.000000 xgi-0.7/xgi/readwrite/json.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4405 2023-06-05 16:28:12.000000 xgi-0.7/xgi/readwrite/xgi_data.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.673003 xgi-0.7/xgi/stats/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    22043 2023-06-01 16:27:59.000000 xgi-0.7/xgi/stats/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8197 2023-06-05 15:50:23.000000 xgi-0.7/xgi/stats/diedgestats.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8355 2023-06-05 17:51:07.000000 xgi-0.7/xgi/stats/dinodestats.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6527 2023-05-30 02:43:06.000000 xgi-0.7/xgi/stats/edgestats.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    12555 2023-05-30 14:17:43.000000 xgi-0.7/xgi/stats/nodestats.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.673244 xgi-0.7/xgi/utils/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       49 2023-01-03 14:13:27.000000 xgi-0.7/xgi/utils/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7084 2023-06-05 16:01:35.000000 xgi-0.7/xgi/utils/utilities.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.665632 xgi-0.7/xgi.egg-info/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4028 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2760 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)        1 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      769 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/requires.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)        4 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/top_level.txt
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.873014 xgi-0.7.1/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2184 2023-05-30 02:43:06.000000 xgi-0.7.1/CITATION.cff
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    13449 2023-05-30 02:43:06.000000 xgi-0.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3092 2023-06-13 16:28:37.000000 xgi-0.7.1/HOW_TO_CONTRIBUTE.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5146 2023-06-13 16:28:37.000000 xgi-0.7.1/LICENSE.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      378 2023-06-13 17:16:46.000000 xgi-0.7.1/MANIFEST.in
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3670 2023-06-16 13:32:34.872868 xgi-0.7.1/PKG-INFO
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5808 2023-06-13 17:38:47.000000 xgi-0.7.1/README.md
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.850844 xgi-0.7.1/logo/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2807 2022-10-13 17:38:17.000000 xgi-0.7.1/logo/logo.pdf
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    56414 2022-10-13 17:38:17.000000 xgi-0.7.1/logo/logo.png
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9082 2022-10-13 17:38:17.000000 xgi-0.7.1/logo/logo.svg
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2995 2023-06-13 16:28:37.000000 xgi-0.7.1/long_description.rst
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      157 2022-10-13 17:38:17.000000 xgi-0.7.1/pytest.ini
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.851933 xgi-0.7.1/requirements/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      610 2022-10-13 17:38:17.000000 xgi-0.7.1/requirements/README.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       23 2022-11-02 17:36:41.000000 xgi-0.7.1/requirements/benchmarks.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       78 2023-05-30 02:43:06.000000 xgi-0.7.1/requirements/default.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       66 2023-05-21 19:12:05.000000 xgi-0.7.1/requirements/developer.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       93 2023-05-30 02:43:06.000000 xgi-0.7.1/requirements/documentation.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       39 2023-01-03 14:13:27.000000 xgi-0.7.1/requirements/release.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       27 2023-05-30 02:43:06.000000 xgi-0.7.1/requirements/test.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       58 2023-05-30 02:43:06.000000 xgi-0.7.1/requirements/tutorial.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       38 2023-06-16 13:32:34.873061 xgi-0.7.1/setup.cfg
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1642 2023-06-16 13:30:31.000000 xgi-0.7.1/setup.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.857833 xgi-0.7.1/tutorials/
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.863475 xgi-0.7.1/tutorials/.ipynb_checkpoints/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9419 2023-05-16 00:58:28.000000 xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 1 - Basic Hypergraph Functionality-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3684 2023-05-16 00:58:31.000000 xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 2 - Read and Write-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    18547 2023-05-16 00:59:22.000000 xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 3 - Basic simplicial complex usage-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7554 2023-05-16 01:02:54.000000 xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 4 - Generative_Models-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   858870 2023-05-16 01:03:14.000000 xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 5 - Plotting-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57344 2023-05-16 01:03:26.000000 xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 6 - Statistics-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   987717 2023-05-16 01:20:02.000000 xgi-0.7.1/tutorials/.ipynb_checkpoints/quickstart-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9404 2023-05-16 02:41:54.000000 xgi-0.7.1/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3714 2023-05-16 02:41:54.000000 xgi-0.7.1/tutorials/Tutorial 2 - Read and Write.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    18606 2023-05-16 02:41:54.000000 xgi-0.7.1/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7560 2023-05-16 02:41:54.000000 xgi-0.7.1/tutorials/Tutorial 4 - Generative_Models.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   858869 2023-06-08 12:07:46.000000 xgi-0.7.1/tutorials/Tutorial 5 - Plotting.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57352 2023-05-30 02:43:06.000000 xgi-0.7.1/tutorials/Tutorial 6 - Statistics.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   214664 2023-06-08 12:07:46.000000 xgi-0.7.1/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   119598 2023-06-08 12:07:46.000000 xgi-0.7.1/tutorials/Tutorial 8 - Directed Hypergraphs.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57003 2023-05-30 02:43:06.000000 xgi-0.7.1/tutorials/case_study_zhang2022.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   987944 2023-05-30 02:43:06.000000 xgi-0.7.1/tutorials/quickstart.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   150550 2023-05-05 16:04:30.000000 xgi-0.7.1/tutorials/simplicial_kuramoto_example.ipynb
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.865530 xgi-0.7.1/xgi/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      464 2022-11-02 17:36:41.000000 xgi-0.7.1/xgi/__init__.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.867346 xgi-0.7.1/xgi/algorithms/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      198 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/algorithms/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4776 2023-06-05 15:50:23.000000 xgi-0.7.1/xgi/algorithms/assortativity.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    12403 2023-06-08 12:07:46.000000 xgi-0.7.1/xgi/algorithms/centrality.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7654 2023-06-08 12:07:46.000000 xgi-0.7.1/xgi/algorithms/clustering.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5393 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/algorithms/connected.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3094 2023-06-05 15:50:23.000000 xgi-0.7.1/xgi/algorithms/shortest_path.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.868595 xgi-0.7.1/xgi/classes/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      190 2023-06-01 16:27:59.000000 xgi-0.7.1/xgi/classes/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    27188 2023-06-05 15:50:23.000000 xgi-0.7.1/xgi/classes/dihypergraph.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    22417 2023-06-05 15:50:23.000000 xgi-0.7.1/xgi/classes/direportviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    25904 2023-06-08 12:07:46.000000 xgi-0.7.1/xgi/classes/function.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    41513 2023-06-13 16:36:10.000000 xgi-0.7.1/xgi/classes/hypergraph.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2759 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/classes/hypergraphviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    23879 2023-06-15 18:57:08.000000 xgi-0.7.1/xgi/classes/reportviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    26675 2023-06-13 16:36:10.000000 xgi-0.7.1/xgi/classes/simplicialcomplex.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    25375 2023-06-15 18:47:04.000000 xgi-0.7.1/xgi/convert.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.868985 xgi-0.7.1/xgi/drawing/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/drawing/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    60660 2023-06-15 18:47:04.000000 xgi-0.7.1/xgi/drawing/draw.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    15065 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/drawing/layout.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.869216 xgi-0.7.1/xgi/dynamics/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       61 2022-11-02 17:36:41.000000 xgi-0.7.1/xgi/dynamics/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8892 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/dynamics/synchronization.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      247 2022-10-13 17:38:17.000000 xgi-0.7.1/xgi/exception.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.870238 xgi-0.7.1/xgi/generators/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      227 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/generators/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7405 2023-06-08 12:07:46.000000 xgi-0.7.1/xgi/generators/classic.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1411 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/generators/lattice.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10637 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/generators/random.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2749 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/generators/simple.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8505 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/generators/simplicial_complexes.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10058 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/generators/uniform.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.870761 xgi-0.7.1/xgi/linalg/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      183 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/linalg/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7002 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/linalg/hodge_matrix.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8447 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/linalg/hypergraph_matrix.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6715 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/linalg/laplacian_matrix.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.871605 xgi-0.7.1/xgi/readwrite/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      215 2023-06-05 15:56:16.000000 xgi-0.7.1/xgi/readwrite/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3010 2023-06-08 12:13:50.000000 xgi-0.7.1/xgi/readwrite/bigg_data.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6048 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/readwrite/bipartite.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4157 2023-03-17 19:59:22.000000 xgi-0.7.1/xgi/readwrite/edgelist.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2181 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/readwrite/incidence.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1892 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/readwrite/json.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4405 2023-06-05 16:28:12.000000 xgi-0.7.1/xgi/readwrite/xgi_data.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.872398 xgi-0.7.1/xgi/stats/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    22043 2023-06-01 16:27:59.000000 xgi-0.7.1/xgi/stats/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8197 2023-06-05 15:50:23.000000 xgi-0.7.1/xgi/stats/diedgestats.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8355 2023-06-05 17:51:07.000000 xgi-0.7.1/xgi/stats/dinodestats.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6527 2023-05-30 02:43:06.000000 xgi-0.7.1/xgi/stats/edgestats.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    12555 2023-05-30 14:17:43.000000 xgi-0.7.1/xgi/stats/nodestats.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.872665 xgi-0.7.1/xgi/utils/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       49 2023-01-03 14:13:27.000000 xgi-0.7.1/xgi/utils/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7084 2023-06-05 16:01:35.000000 xgi-0.7.1/xgi/utils/utilities.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-16 13:32:34.866357 xgi-0.7.1/xgi.egg-info/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3670 2023-06-16 13:32:34.000000 xgi-0.7.1/xgi.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2765 2023-06-16 13:32:34.000000 xgi-0.7.1/xgi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)        1 2023-06-16 13:32:34.000000 xgi-0.7.1/xgi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      769 2023-06-16 13:32:34.000000 xgi-0.7.1/xgi.egg-info/requires.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)        4 2023-06-16 13:32:34.000000 xgi-0.7.1/xgi.egg-info/top_level.txt
```

### Comparing `xgi-0.7/CITATION.cff` & `xgi-0.7.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `xgi-0.7/CODE_OF_CONDUCT.md` & `xgi-0.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `xgi-0.7/CONTRIBUTING.md` & `xgi-0.7.1/HOW_TO_CONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `xgi-0.7/LICENSE.md` & `xgi-0.7.1/LICENSE.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 XGI is distributed with the 3-clause BSD license.
 
 Copyright (C) 2023, XGI Developers
 
-Nicholas Landry <nicholas.landry.91@gmail.com>
-
-Leo Torres <leo@leotrs.com>
-
-Iacopo Iacopini <iacopiniiacopo@gmail.com>
-
-Maxime Lucas <maxime.lucas@isi.it>
-
-Giovanni Petri <giovanni.petri@isi.it>
-
-Alice Patania <apatania@uvm.edu>
-
-Alice Schwarze <alice.c.schwarze@dartmouth.edu>
-
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 * Redistributions of source code must retain the above copyright
```

### Comparing `xgi-0.7/PKG-INFO` & `xgi-0.7.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xgi
-Version: 0.7
-Summary: XGI is a Python library for the representation
-Author: Nicholas Landry, Leo Torres, Maxime Lucas, Iacopo Iacopini, Giovanni Petri, Alice Patania, and Alice Schwarze
+Version: 0.7.1
+Summary: XGI is a Python package for higher-order networks.
+Author: XGI Developers
 Author-email: nicholas.landry@uvm.edu
 Project-URL: Documentation, https://xgi.readthedocs.io/en/latest/
 Project-URL: Bug Reports, https://github.com/xgi-org/xgi/issues
 Project-URL: Source, https://github.com/xgi-org/xgi
 Project-URL: PyPI, https://pypi.org/project/xgi/
 Project-URL: GitHub Discussions, https://github.com/xgi-org/xgi/discussions
 Provides-Extra: benchmarks
@@ -22,15 +22,15 @@
 ===
 
 .. image:: https://github.com/xgi-org/xgi/raw/main/logo/logo.svg
   :width: 200
 
 XGI is a Python package for higher-order networks.
 
-Comple**X** **G**roup **Interactions** (XGI) provides an ecosystem for the
+Comple\ **X** **G**\ roup **I**\ nteractions (XGI) provides an ecosystem for the
 representation, manipulation, and study of the
 structure, dynamics, and functions of
 complex systems with group (higher-order) interactions.
 
 Installation
 ------------
 XGI runs on Python 3.8 or higher.
@@ -56,15 +56,15 @@
 Corresponding Data
 ------------------
 A number of higher-order datasets are available in the `XGI-DATA repository <https://gitlab.com/complexgroupinteractions/xgi-data>`_ and can be easily accessed with the ``load_xgi_data()`` function.
 
 Contributing
 ------------
 If you want to contribute to this project, please make sure to read the
-`contributing guidelines <CONTRIBUTING.md>`_.
+`contributing guidelines <HOW_TO_CONTRIBUTE.md>`_.
 We expect respectful and kind interactions by all contributors and users
 as laid out in our `code of conduct <CODE_OF_CONDUCT.md>`_.
 
 The XGI community always welcomes contributions, no matter how small.
 We're happy to help troubleshoot XGI issues you run into,
 assist you if you would like to add functionality or fixes to the codebase,
 or answer any questions you may have.
@@ -88,21 +88,7 @@
 a citation in your preferred format, and will also integrate well with citation managers.
 
 License
 -------
 Released under the 3-Clause BSD license (see the `license file <https://github.com/xgi-org/xgi/tree/main/license.md>`_)
 
 Copyright (C) 2021-2023 XGI Developers
-
-Nicholas Landry <nicholas.landry@colorado.edu>
-
-Leo Torres <leo@leotrs.com>
-
-Iacopo Iacopini <iacopiniiacopo@gmail.com>
-
-Maxime Lucas <maxime.lucas@isi.it>
-
-Giovanni Petri <giovanni.petri@isi.it>
-
-Alice Patania <apatania@uvm.edu>
-
-Alice Schwarze <alice.c.schwarze@dartmouth.edu>
```

### Comparing `xgi-0.7/README.md` & `xgi-0.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 [![Test Status](https://github.com/xgi-org/xgi/workflows/test/badge.svg?branch=main)](https://github.com/xgi-org/xgi/actions?query=workflow%3A%22test%22)
 [![codecov](https://codecov.io/gh/xgi-org/xgi/branch/main/graph/badge.svg?token=BI6TX2WDSG)](https://codecov.io/gh/xgi-org/xgi)
 [![Good First Issue](https://img.shields.io/badge/contribute-Good%20First%20Issue-%232EBC4F)](https://github.com/xgi-org/xgi/issues?q=is%3Aopen+is%3Aissue+label%3A%22Good+First+Issue%22)
 
 * [**Source**](../../)
 * [**Bug reports**](../../issues)
 * [**GitHub Discussions**](../../discussions)
-* [**Documentation**](https://xgi.readthedocs.io/en/latest/)
+* [**Documentation**](https://xgi.readthedocs.io)
+* [**Contributors**](https://xgi.readthedocs.io/en/stable/contributors.html)
 
 Sign up for our [mailing list](http://eepurl.com/igE6ez) and follow XGI on [Twitter](https://twitter.com/xginets) or [Mastodon](https://mathstodon.xyz/@xginets)!
 
 ## Table of Contents:
+- [XGI](#xgi)
+  - [Table of Contents:](#table-of-contents)
   - [Installation](#installation)
   - [Getting Started](#getting-started)
-  - [How to Contribute](#contributing)
   - [Corresponding Data](#corresponding-data)
+  - [How to Contribute](#how-to-contribute)
   - [How to Cite](#how-to-cite)
   - [License](#license)
   - [Funding](#funding)
   - [Other Resources](#other-resources)
 
 
 ## Installation
@@ -51,15 +54,15 @@
 
 ## Corresponding Data
 A number of higher-order datasets are available in the [XGI-DATA repository](https://gitlab.com/complexgroupinteractions/xgi-data) and can be easily accessed with the `load_xgi_data()` function.
 
 
 ## How to Contribute
 If you want to contribute to this project, please make sure to read the
-[contributing guidelines](CONTRIBUTING.md). We expect respectful and kind interactions by all contributors and users as laid out in our [code of conduct](CODE_OF_CONDUCT.md).
+[contributing guidelines](HOW_TO_CONTRIBUTE.md). We expect respectful and kind interactions by all contributors and users as laid out in our [code of conduct](CODE_OF_CONDUCT.md).
 
 The XGI community always welcomes contributions, no matter how small. We're happy to help troubleshoot XGI issues you run into, assist you if you would like to add functionality or fixes to the codebase, or answer any questions you may have.
 
 Some concrete ways that you can get involved:
 
 * **Get XGI updates** by following the XGI [Twitter](https://twitter.com/xginets) account, signing up for our [mailing list](http://eepurl.com/igE6ez), or starring this repository.
 * **Spread the word** when you use XGI by sharing with your colleagues and friends.
@@ -79,28 +82,22 @@
 
 
 ## License
 Released under the 3-Clause BSD license (see [`LICENSE.md`](LICENSE.md))
 
 Copyright (C) 2021-2023 XGI Developers
 
-* Nicholas Landry <nicholas.landry@uvm.edu>
-* Leo Torres <leo@leotrs.com>
-* Iacopo Iacopini <iacopiniiacopo@gmail.com>
-* Maxime Lucas <maxime.lucas@centai.eu>
-* Giovanni Petri <giovanni.petri@centai.eu>
-* Alice Patania <apatania@uvm.edu>
-* Alice Schwarze <alice.c.schwarze@dartmouth.edu>
-
 The XGI library has copied or modified code from the HyperNetX and NetworkX libraries, the licenses of which can be found in our [license file](LICENSE.md)
 
 ## Funding
 The XGI package has been supported by NSF Grant 2121905, ["HNDS-I: Using Hypergraphs to Study Spreading Processes in Complex Social Networks"](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2121905).
 
 ## Other Resources
 This library may not meet your needs and if this is this case, consider checking out these other resources:
-* [HyperNetX](https://pnnl.github.io/HyperNetX): A package in Python for representing, analyzing, and visualizing hypergraphs.
-* [Reticula](https://docs.reticula.network/): A package with a Python wrapper of C++ functions for representing, analyzing, and visualizing temporal and static graphs and hypergraphs.
-* [SimpleHypergraphs.jl](https://pszufe.github.io/SimpleHypergraphs.jl/v0.1/): A package in Julia for representing, analyzing, and generating hypergraphs.
-* [HyperGraphs.jl](https://github.com/lpmdiaz/HyperGraphs.jl): A package in Julia for representing, analyzing, and generating hypergraphs which may be oriented and weighted.
-* [hyperG](https://cran.r-project.org/package=HyperG): A package in R for storing and analyzing hypergraphs
-* [NetworkX](https://networkx.org/): A package in Python for representing, analyzing, and visualizing networks.
+* [HyperNetX](https://pnnl.github.io/HyperNetX): A Python package for representing, analyzing, and visualizing hypergraphs.
+* [Hypergraph Analysis Toolbox (HAT)](https://hypergraph-analysis-toolbox.readthedocs.io): A Python/Matlab package for hypergraph construction, visualization, and analysis (Especially for Pore-C data).
+* [halp](http://murali-group.github.io/halp): A Python package with directed and undirected hypergraph implementations and several algorithms.
+* [Reticula](https://docs.reticula.network): A Python package wrapping C++ functions for representing, analyzing, and visualizing temporal and static graphs and hypergraphs.
+* [SimpleHypergraphs.jl](https://pszufe.github.io/SimpleHypergraphs.jl/v0.1): A Julia package for representing, analyzing, and generating hypergraphs.
+* [HyperGraphs.jl](https://github.com/lpmdiaz/HyperGraphs.jl): A Julia package for representing, analyzing, and generating hypergraphs which may be oriented and weighted.
+* [hyperG](https://cran.r-project.org/package=HyperG): An R package for storing and analyzing hypergraphs
+* [NetworkX](https://networkx.org): A Python package for representing, analyzing, and visualizing networks.
```

### Comparing `xgi-0.7/logo/logo.pdf` & `xgi-0.7.1/logo/logo.pdf`

 * *Files identical despite different names*

### Comparing `xgi-0.7/logo/logo.png` & `xgi-0.7.1/logo/logo.png`

 * *Files identical despite different names*

### Comparing `xgi-0.7/logo/logo.svg` & `xgi-0.7.1/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `xgi-0.7/long_description.rst` & `xgi-0.7.1/long_description.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ===
 
 .. image:: https://github.com/xgi-org/xgi/raw/main/logo/logo.svg
   :width: 200
 
 XGI is a Python package for higher-order networks.
 
-Comple**X** **G**roup **Interactions** (XGI) provides an ecosystem for the
+Comple\ **X** **G**\ roup **I**\ nteractions (XGI) provides an ecosystem for the
 representation, manipulation, and study of the
 structure, dynamics, and functions of
 complex systems with group (higher-order) interactions.
 
 Installation
 ------------
 XGI runs on Python 3.8 or higher.
@@ -36,15 +36,15 @@
 Corresponding Data
 ------------------
 A number of higher-order datasets are available in the `XGI-DATA repository <https://gitlab.com/complexgroupinteractions/xgi-data>`_ and can be easily accessed with the ``load_xgi_data()`` function.
 
 Contributing
 ------------
 If you want to contribute to this project, please make sure to read the
-`contributing guidelines <CONTRIBUTING.md>`_.
+`contributing guidelines <HOW_TO_CONTRIBUTE.md>`_.
 We expect respectful and kind interactions by all contributors and users
 as laid out in our `code of conduct <CODE_OF_CONDUCT.md>`_.
 
 The XGI community always welcomes contributions, no matter how small.
 We're happy to help troubleshoot XGI issues you run into,
 assist you if you would like to add functionality or fixes to the codebase,
 or answer any questions you may have.
@@ -67,22 +67,8 @@
 click the "cite this repository" button on the right sidebar. This will generate
 a citation in your preferred format, and will also integrate well with citation managers.
 
 License
 -------
 Released under the 3-Clause BSD license (see the `license file <https://github.com/xgi-org/xgi/tree/main/license.md>`_)
 
-Copyright (C) 2021-2023 XGI Developers
-
-Nicholas Landry <nicholas.landry@colorado.edu>
-
-Leo Torres <leo@leotrs.com>
-
-Iacopo Iacopini <iacopiniiacopo@gmail.com>
-
-Maxime Lucas <maxime.lucas@isi.it>
-
-Giovanni Petri <giovanni.petri@isi.it>
-
-Alice Patania <apatania@uvm.edu>
-
-Alice Schwarze <alice.c.schwarze@dartmouth.edu>
+Copyright (C) 2021-2023 XGI Developers
```

### Comparing `xgi-0.7/requirements/README.md` & `xgi-0.7.1/requirements/README.md`

 * *Files identical despite different names*

### Comparing `xgi-0.7/setup.py` & `xgi-0.7.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 import sys
 
 import setuptools
 from setuptools import setup
 
-__version__ = "0.7"
+__version__ = "0.7.1"
 
 if sys.version_info < (3, 8):
     sys.exit("XGI requires Python 3.8 or later.")
 
 name = "xgi"
 
 version = __version__
 
-authors = (
-    "Nicholas Landry, "
-    "Leo Torres, "
-    "Maxime Lucas, "
-    "Iacopo Iacopini, "
-    "Giovanni Petri, "
-    "Alice Patania, "
-    "and Alice Schwarze"
-)
+authors = "XGI Developers"
 
 author_email = "nicholas.landry@uvm.edu"
 
 project_urls = {
     "Documentation": "https://xgi.readthedocs.io/en/latest/",
     "Bug Reports": "https://github.com/xgi-org/xgi/issues",
     "Source": "https://github.com/xgi-org/xgi",
     "PyPI": "https://pypi.org/project/xgi/",
     "GitHub Discussions": "https://github.com/xgi-org/xgi/discussions",
 }
 
-description = """XGI is a Python library for the representation
-and analysis of complex systems with group (higher-order) interactions."""
+description = """XGI is a Python package for higher-order networks."""
 
 with open("long_description.rst") as file:
     long_description = file.read()
 
 
 def parse_requirements_file(filename):
     with open(filename) as fid:
```

### Comparing `xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 1 - Basic Hypergraph Functionality-checkpoint.ipynb` & `xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 1 - Basic Hypergraph Functionality-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 2 - Read and Write-checkpoint.ipynb` & `xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 2 - Read and Write-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 3 - Basic simplicial complex usage-checkpoint.ipynb` & `xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 3 - Basic simplicial complex usage-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 4 - Generative_Models-checkpoint.ipynb` & `xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 4 - Generative_Models-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 5 - Plotting-checkpoint.ipynb` & `xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 5 - Plotting-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 6 - Statistics-checkpoint.ipynb` & `xgi-0.7.1/tutorials/.ipynb_checkpoints/Tutorial 6 - Statistics-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/.ipynb_checkpoints/quickstart-checkpoint.ipynb` & `xgi-0.7.1/tutorials/.ipynb_checkpoints/quickstart-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb` & `xgi-0.7.1/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/Tutorial 2 - Read and Write.ipynb` & `xgi-0.7.1/tutorials/Tutorial 2 - Read and Write.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb` & `xgi-0.7.1/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/Tutorial 4 - Generative_Models.ipynb` & `xgi-0.7.1/tutorials/Tutorial 4 - Generative_Models.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/Tutorial 5 - Plotting.ipynb` & `xgi-0.7.1/tutorials/Tutorial 5 - Plotting.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/Tutorial 6 - Statistics.ipynb` & `xgi-0.7.1/tutorials/Tutorial 6 - Statistics.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb` & `xgi-0.7.1/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/Tutorial 8 - Directed Hypergraphs.ipynb` & `xgi-0.7.1/tutorials/Tutorial 8 - Directed Hypergraphs.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/case_study_zhang2022.ipynb` & `xgi-0.7.1/tutorials/case_study_zhang2022.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/quickstart.ipynb` & `xgi-0.7.1/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/tutorials/simplicial_kuramoto_example.ipynb` & `xgi-0.7.1/tutorials/simplicial_kuramoto_example.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/algorithms/assortativity.py` & `xgi-0.7.1/xgi/algorithms/assortativity.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/algorithms/centrality.py` & `xgi-0.7.1/xgi/algorithms/centrality.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/algorithms/clustering.py` & `xgi-0.7.1/xgi/algorithms/clustering.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/algorithms/connected.py` & `xgi-0.7.1/xgi/algorithms/connected.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/algorithms/shortest_path.py` & `xgi-0.7.1/xgi/algorithms/shortest_path.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/classes/dihypergraph.py` & `xgi-0.7.1/xgi/classes/dihypergraph.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/classes/direportviews.py` & `xgi-0.7.1/xgi/classes/direportviews.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/classes/function.py` & `xgi-0.7.1/xgi/classes/function.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/classes/hypergraph.py` & `xgi-0.7.1/xgi/classes/hypergraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         hypergraph is created, i.e. one with no nodes or edges.
         The data can be in the following formats:
 
         * hyperedge list
         * hyperedge dictionary
         * 2-column Pandas dataframe (bipartite edges)
         * Scipy/Numpy incidence matrix
-        * Hypergraph object.
+        * Hypergraph object
+        * SimplicialComplex object
 
     **attr : dict, optional
         Attributes to add to the hypergraph as key, value pairs.
         By default, None.
 
     Notes
     -----
```

### Comparing `xgi-0.7/xgi/classes/hypergraphviews.py` & `xgi-0.7.1/xgi/classes/hypergraphviews.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/classes/reportviews.py` & `xgi-0.7.1/xgi/classes/reportviews.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/classes/simplicialcomplex.py` & `xgi-0.7.1/xgi/classes/simplicialcomplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         simplicial complex is created, i.e. one with no nodes or simplices.  The data
         can be in the following formats:
 
         * simplex list
         * simplex dictionary
         * 2-column Pandas dataframe (bipartite edges)
         * Scipy/Numpy incidence matrix
-        * SimplicialComplex object.
+        * SimplicialComplex object
+        * Hypergraph object
 
     **attr : dict, optional
         Attributes to add to the simplicial complex as key, value pairs.
         By default, None.
 
     See Also
     --------
```

### Comparing `xgi-0.7/xgi/convert.py` & `xgi-0.7.1/xgi/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "from_incidence_matrix",
     "from_max_simplices",
     "to_incidence_matrix",
     "from_bipartite_graph",
     "to_bipartite_graph",
     "dict_to_hypergraph",
     "to_line_graph",
+    "from_simplex_dict",
 ]
 
 
 def convert_to_hypergraph(data, create_using=None):
     """Make a hypergraph from a known data structure.
 
     The preferred way to call this is automatically from the class constructor.
@@ -65,14 +66,18 @@
         populated.
 
     Returns
     -------
     Hypergraph object
         A hypergraph constructed from the data
 
+    See Also
+    --------
+    from_max_simplices : Constructs a hypergraph from the maximal simplices of a simplicial complex.
+
     """
     if data is None:
         return empty_hypergraph(create_using)
 
     elif isinstance(data, Hypergraph) and not isinstance(data, SimplicialComplex):
         H = empty_hypergraph(create_using)
         H.add_nodes_from((n, attr) for n, attr in data.nodes.items())
@@ -87,15 +92,20 @@
         ee = data.edges
         H.add_edges_from((ee.members(e), e, deepcopy(attr)) for e, attr in ee.items())
         H._hypergraph = deepcopy(data._hypergraph)
         if not isinstance(create_using, DiHypergraph):
             return H
 
     elif isinstance(data, SimplicialComplex):
-        return from_max_simplices(data)
+        H = empty_hypergraph(create_using)
+        H.add_nodes_from((n, attr) for n, attr in data.nodes.items())
+        ee = data.edges
+        H.add_edges_from((ee.members(e), e, deepcopy(attr)) for e, attr in ee.items())
+        H._hypergraph = deepcopy(data._hypergraph)
+        return H
 
     elif isinstance(data, list):
         # edge list
         result = from_hyperedge_list(data, create_using)
         if not isinstance(create_using, Hypergraph):
             return result
 
@@ -304,16 +314,17 @@
 
     elif isinstance(data, pd.DataFrame):
         result = from_bipartite_pandas_dataframe(data, create_using)
         if not isinstance(create_using, SimplicialComplex):
             return convert_to_simplicial_complex(result)
 
     elif isinstance(data, dict):
-        # edge dict in the form we need
-        raise XGIError("Cannot generate SimplicialComplex from simplex dictionary")
+        result = from_simplex_dict(data, create_using)
+        if not isinstance(create_using, SimplicialComplex):
+            return convert_to_simplicial_complex(result)
     elif isinstance(
         data,
         (
             ndarray,
             matrix,
             csr_array,
             csc_array,
@@ -840,7 +851,32 @@
             H,
             edge_data,
         )
     except KeyError as e:
         raise XGIError("Failed to import edge attributes.") from e
 
     return H
+
+
+def from_simplex_dict(d, create_using=None):
+    """Creates a Simplicial Complex from a dictionary of simplices,
+    if the subfaces of existing simplices are not given in the dict
+    then the function adds them with integer IDs.
+
+
+    Parameters
+    ----------
+    d : dict
+        A dictionary where the keys are simplex IDs and the values
+        are containers of nodes specifying the simplices.
+    create_using : SimplicialComplex constructor, optional
+        The simplicial complex object to add the data to, by default None
+
+    Returns
+    -------
+    SimplicialComplex object
+        The constructed simplicial complex object
+
+    """
+    SC = empty_simplicial_complex(create_using)
+    SC.add_simplices_from((members, uid) for uid, members in d.items())
+    return SC
```

### Comparing `xgi-0.7/xgi/drawing/draw.py` & `xgi-0.7.1/xgi/drawing/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1629,69 +1629,74 @@
 
     node_size = _scalar_arg_to_dict(
         node_size, H_conv.nodes, settings["min_node_size"], settings["max_node_size"]
     )
 
     G_aug = _augmented_projection(H_conv)
     for dyad in H_conv.edges.filterby("size", 2).members():
-        index = max(G_aug.nodes) + 1
+        try:
+            index = max(n for n in G_aug.nodes if isinstance(n, int)) + 1
+        except ValueError:
+            # The list of node-labels has no integers, so I start from 0
+            index = 0
         G_aug.add_edges_from([[list(dyad)[0], index], [list(dyad)[1], index]])
 
     phantom_nodes = [n for n in list(G_aug.nodes) if n not in list(H_conv.nodes)]
     pos = spring_layout(G_aug)
 
     for id, he in DH.edges.members(dtype=dict).items():
         d = len(he) - 1
-        # identify the center of the edge in the augemented projection
-        center = [n for n in phantom_nodes if set(G_aug.neighbors(n)) == he][0]
-        x_center, y_center = pos[center]
-        for node in DH.edges.dimembers(id)[0]:
-            x_coords = [pos[node][0], x_center]
-            y_coords = [pos[node][1], y_center]
-            line = plt.Line2D(
-                x_coords,
-                y_coords,
-                color=lines_fc[id],
-                lw=lines_lw[id],
-                zorder=max_order - d,
-            )
-            ax.add_line(line)
-        for node in DH.edges.dimembers(id)[1]:
-            dx, dy = pos[node][0] - x_center, pos[node][1] - y_center
-            # the following to avoid the point of the arrow overlapping the node
-            distance = np.hypot(dx, dy)
-            direction_vector = np.array([dx, dy]) / distance
-            shortened_distance = (
-                distance - node_size[node] * 0.003
-            )  # Calculate the shortened length
-            dx = direction_vector[0] * shortened_distance
-            dy = direction_vector[1] * shortened_distance
-            arrow = FancyArrow(
-                x_center,
-                y_center,
-                dx,
-                dy,
-                color=lines_fc[id],
-                width=lines_lw[id] * 0.001,
-                length_includes_head=True,
-                head_width=line_head_width,
-                zorder=max_order - d,
-            )
-            ax.add_patch(arrow)
-        if edge_marker_toggle:
-            ax.scatter(
-                x=x_center,
-                y=y_center,
-                marker=edge_marker,
-                s=edge_marker_size**2,
-                c=edge_marker_fc[id],
-                edgecolors=edge_marker_ec[id],
-                linewidths=edge_marker_lw,
-                zorder=max_order,
-            )
+        if d > 0:
+            # identify the center of the edge in the augemented projection
+            center = [n for n in phantom_nodes if set(G_aug.neighbors(n)) == he][0]
+            x_center, y_center = pos[center]
+            for node in DH.edges.dimembers(id)[0]:
+                x_coords = [pos[node][0], x_center]
+                y_coords = [pos[node][1], y_center]
+                line = plt.Line2D(
+                    x_coords,
+                    y_coords,
+                    color=lines_fc[id],
+                    lw=lines_lw[id],
+                    zorder=max_order - d,
+                )
+                ax.add_line(line)
+            for node in DH.edges.dimembers(id)[1]:
+                dx, dy = pos[node][0] - x_center, pos[node][1] - y_center
+                # the following to avoid the point of the arrow overlapping the node
+                distance = np.hypot(dx, dy)
+                direction_vector = np.array([dx, dy]) / distance
+                shortened_distance = (
+                    distance - node_size[node] * 0.003
+                )  # Calculate the shortened length
+                dx = direction_vector[0] * shortened_distance
+                dy = direction_vector[1] * shortened_distance
+                arrow = FancyArrow(
+                    x_center,
+                    y_center,
+                    dx,
+                    dy,
+                    color=lines_fc[id],
+                    width=lines_lw[id] * 0.001,
+                    length_includes_head=True,
+                    head_width=line_head_width,
+                    zorder=max_order - d,
+                )
+                ax.add_patch(arrow)
+            if edge_marker_toggle:
+                ax.scatter(
+                    x=x_center,
+                    y=y_center,
+                    marker=edge_marker,
+                    s=edge_marker_size**2,
+                    c=edge_marker_fc[id],
+                    edgecolors=edge_marker_ec[id],
+                    linewidths=edge_marker_lw,
+                    zorder=max_order,
+                )
 
     if hyperedge_labels:
         # Get all valid keywords by inspecting the signatures of draw_node_labels
         valid_label_kwds = signature(draw_hyperedge_labels).parameters.keys()
         # Remove the arguments of this function (draw_networkx)
         valid_label_kwds = valid_label_kwds - {"H", "pos", "ax", "hyperedge_labels"}
         if any([k not in valid_label_kwds for k in kwargs]):
```

### Comparing `xgi-0.7/xgi/drawing/layout.py` & `xgi-0.7.1/xgi/drawing/layout.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/dynamics/synchronization.py` & `xgi-0.7.1/xgi/dynamics/synchronization.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/generators/classic.py` & `xgi-0.7.1/xgi/generators/classic.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/generators/lattice.py` & `xgi-0.7.1/xgi/generators/lattice.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/generators/random.py` & `xgi-0.7.1/xgi/generators/random.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/generators/simple.py` & `xgi-0.7.1/xgi/generators/simple.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/generators/simplicial_complexes.py` & `xgi-0.7.1/xgi/generators/simplicial_complexes.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/generators/uniform.py` & `xgi-0.7.1/xgi/generators/uniform.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/linalg/hodge_matrix.py` & `xgi-0.7.1/xgi/linalg/hodge_matrix.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/linalg/hypergraph_matrix.py` & `xgi-0.7.1/xgi/linalg/hypergraph_matrix.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/linalg/laplacian_matrix.py` & `xgi-0.7.1/xgi/linalg/laplacian_matrix.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/readwrite/bigg_data.py` & `xgi-0.7.1/xgi/readwrite/bigg_data.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/readwrite/bipartite.py` & `xgi-0.7.1/xgi/readwrite/bipartite.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/readwrite/edgelist.py` & `xgi-0.7.1/xgi/readwrite/edgelist.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/readwrite/incidence.py` & `xgi-0.7.1/xgi/readwrite/incidence.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/readwrite/json.py` & `xgi-0.7.1/xgi/readwrite/json.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/readwrite/xgi_data.py` & `xgi-0.7.1/xgi/readwrite/xgi_data.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/stats/__init__.py` & `xgi-0.7.1/xgi/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/stats/diedgestats.py` & `xgi-0.7.1/xgi/stats/diedgestats.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/stats/dinodestats.py` & `xgi-0.7.1/xgi/stats/dinodestats.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/stats/edgestats.py` & `xgi-0.7.1/xgi/stats/edgestats.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/stats/nodestats.py` & `xgi-0.7.1/xgi/stats/nodestats.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi/utils/utilities.py` & `xgi-0.7.1/xgi/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `xgi-0.7/xgi.egg-info/PKG-INFO` & `xgi-0.7.1/xgi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xgi
-Version: 0.7
-Summary: XGI is a Python library for the representation
-Author: Nicholas Landry, Leo Torres, Maxime Lucas, Iacopo Iacopini, Giovanni Petri, Alice Patania, and Alice Schwarze
+Version: 0.7.1
+Summary: XGI is a Python package for higher-order networks.
+Author: XGI Developers
 Author-email: nicholas.landry@uvm.edu
 Project-URL: Documentation, https://xgi.readthedocs.io/en/latest/
 Project-URL: Bug Reports, https://github.com/xgi-org/xgi/issues
 Project-URL: Source, https://github.com/xgi-org/xgi
 Project-URL: PyPI, https://pypi.org/project/xgi/
 Project-URL: GitHub Discussions, https://github.com/xgi-org/xgi/discussions
 Provides-Extra: benchmarks
@@ -22,15 +22,15 @@
 ===
 
 .. image:: https://github.com/xgi-org/xgi/raw/main/logo/logo.svg
   :width: 200
 
 XGI is a Python package for higher-order networks.
 
-Comple**X** **G**roup **Interactions** (XGI) provides an ecosystem for the
+Comple\ **X** **G**\ roup **I**\ nteractions (XGI) provides an ecosystem for the
 representation, manipulation, and study of the
 structure, dynamics, and functions of
 complex systems with group (higher-order) interactions.
 
 Installation
 ------------
 XGI runs on Python 3.8 or higher.
@@ -56,15 +56,15 @@
 Corresponding Data
 ------------------
 A number of higher-order datasets are available in the `XGI-DATA repository <https://gitlab.com/complexgroupinteractions/xgi-data>`_ and can be easily accessed with the ``load_xgi_data()`` function.
 
 Contributing
 ------------
 If you want to contribute to this project, please make sure to read the
-`contributing guidelines <CONTRIBUTING.md>`_.
+`contributing guidelines <HOW_TO_CONTRIBUTE.md>`_.
 We expect respectful and kind interactions by all contributors and users
 as laid out in our `code of conduct <CODE_OF_CONDUCT.md>`_.
 
 The XGI community always welcomes contributions, no matter how small.
 We're happy to help troubleshoot XGI issues you run into,
 assist you if you would like to add functionality or fixes to the codebase,
 or answer any questions you may have.
@@ -88,21 +88,7 @@
 a citation in your preferred format, and will also integrate well with citation managers.
 
 License
 -------
 Released under the 3-Clause BSD license (see the `license file <https://github.com/xgi-org/xgi/tree/main/license.md>`_)
 
 Copyright (C) 2021-2023 XGI Developers
-
-Nicholas Landry <nicholas.landry@colorado.edu>
-
-Leo Torres <leo@leotrs.com>
-
-Iacopo Iacopini <iacopiniiacopo@gmail.com>
-
-Maxime Lucas <maxime.lucas@isi.it>
-
-Giovanni Petri <giovanni.petri@isi.it>
-
-Alice Patania <apatania@uvm.edu>
-
-Alice Schwarze <alice.c.schwarze@dartmouth.edu>
```

### Comparing `xgi-0.7/xgi.egg-info/SOURCES.txt` & `xgi-0.7.1/xgi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 CITATION.cff
 CODE_OF_CONDUCT.md
-CONTRIBUTING.md
+HOW_TO_CONTRIBUTE.md
 LICENSE.md
 MANIFEST.in
 README.md
 long_description.rst
 pytest.ini
 setup.py
 logo/logo.pdf
```

### Comparing `xgi-0.7/xgi.egg-info/requires.txt` & `xgi-0.7.1/xgi.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 scipy>=1.8
 pandas>=1.3
 networkx>=2.7
 requests>=2.0
 matplotlib>=3.4
 
 [all]
+black[jupyter]==22.3.0
 pytest-cov>=4.0
-github-changelog
-pytest>=7.2
 pillow>=8.2
-black[jupyter]==22.3.0
+twine>=3.4
+sphinx~=6.0
+seaborn>=0.10
+wheel>=0.36
+matplotlib>=3.3
+isort==5.10.1
+jupyter>=1.0
 sphinx-rtd-theme>=1.2
-asv>=0.5
+github-changelog
 hypernetx>=1.0
-ipython<=8.12.0
+pytest>=7.2
 numpydoc>=1.1
+sphinx_copybutton
 pylint>=2.10
-seaborn>=0.10
-matplotlib>=3.3
-sphinx~=6.0
-twine>=3.4
+asv>=0.5
+ipython<=8.12.0
 pre-commit>=2.12
-sphinx_copybutton
-isort==5.10.1
-jupyter>=1.0
-wheel>=0.36
 
 [benchmarks]
 hypernetx>=1.0
 asv>=0.5
 
 [developer]
 black[jupyter]==22.3.0
```

