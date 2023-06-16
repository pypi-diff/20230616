# Comparing `tmp/pz-rail-0.99.0.tar.gz` & `tmp/pz-rail-0.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-0.99.0.tar", last modified: Thu Jun 15 22:27:45 2023, max compression
+gzip compressed data, was "pz-rail-0.99.1.tar", last modified: Fri Jun 16 04:45:31 2023, max compression
```

## Comparing `pz-rail-0.99.0.tar` & `pz-rail-0.99.1.tar`

### file list

```diff
@@ -1,102 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.369068 pz-rail-0.99.0/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.361067 pz-rail-0.99.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.361067 pz-rail-0.99.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-15 22:27:32.000000 pz-rail-0.99.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-15 22:27:32.000000 pz-rail-0.99.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-15 22:27:45.369068 pz-rail-0.99.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-15 22:27:32.000000 pz-rail-0.99.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-15 22:27:32.000000 pz-rail-0.99.0/conda-reqs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.365068 pz-rail-0.99.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.361067 pz-rail-0.99.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.365068 pz-rail-0.99.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/_static/css/notebooks.css
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/demos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/nbconvert-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.365068 pz-rail-0.99.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/source/citing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/source/futureplans.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/source/immediateplans.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-06-15 22:27:32.000000 pz-rail-0.99.0/docs/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 22:27:32.000000 pz-rail-0.99.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.365068 pz-rail-0.99.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.365068 pz-rail-0.99.0/examples/core_examples/
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/core_examples/FileIO_DataStore.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/core_examples/Pipe_Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/core_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/core_examples/Run_Pipe.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/core_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/core_examples/hyperbolic_magnitude_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/core_examples/iterator_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.365068 pz-rail-0.99.0/examples/creation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/degradation-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/dsps_sed_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/example_GridSelection_for_HSC.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/example_ObsConditions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/photometric_realization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24628 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/creation_examples/posterior-demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.369068 pz-rail-0.99.0/examples/estimation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/NZDir.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/RAIL_estimation_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    28480 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/nzdir_as_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/somocluSOM_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/somocluSOMcluster_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/estimation_examples/test_sampled_summarizers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.369068 pz-rail-0.99.0/examples/evaluation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/evaluation_examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/evaluation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/evaluation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/evaluation_examples/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/evaluation_examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.369068 pz-rail-0.99.0/examples/goldenspike_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/goldenspike_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/goldenspike_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/goldenspike_examples/cleanup_pipeline.sh
--rw-r--r--   0 runner    (1001) docker     (123)    25570 2023-06-15 22:27:32.000000 pz-rail-0.99.0/examples/goldenspike_examples/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-15 22:27:32.000000 pz-rail-0.99.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 22:27:32.000000 pz-rail-0.99.0/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 22:27:32.000000 pz-rail-0.99.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:27:45.369068 pz-rail-0.99.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:27:32.000000 pz-rail-0.99.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.361067 pz-rail-0.99.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.369068 pz-rail-0.99.0/src/pz_rail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-15 22:27:45.000000 pz-rail-0.99.0/src/pz_rail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-15 22:27:45.000000 pz-rail-0.99.0/src/pz_rail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:27:45.000000 pz-rail-0.99.0/src/pz_rail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:27:45.000000 pz-rail-0.99.0/src/pz_rail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 22:27:45.000000 pz-rail-0.99.0/src/pz_rail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:27:45.000000 pz-rail-0.99.0/src/pz_rail.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.361067 pz-rail-0.99.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.369068 pz-rail-0.99.0/src/rail/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:27:32.000000 pz-rail-0.99.0/src/rail/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 22:27:45.000000 pz-rail-0.99.0/src/rail/hub/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-15 22:27:32.000000 pz-rail-0.99.0/src/rail/hub/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-15 22:27:32.000000 pz-rail-0.99.0/src/rail/hub/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-15 22:27:32.000000 pz-rail-0.99.0/src/rail/hub/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:45.369068 pz-rail-0.99.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:27:32.000000 pz-rail-0.99.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 22:27:32.000000 pz-rail-0.99.0/tests/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.732254 pz-rail-0.99.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-16 04:45:19.000000 pz-rail-0.99.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-16 04:45:31.748254 pz-rail-0.99.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-16 04:45:19.000000 pz-rail-0.99.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 04:45:19.000000 pz-rail-0.99.1/conda-reqs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.728254 pz-rail-0.99.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/_static/css/notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/nbconvert-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/futureplans.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/immediateplans.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-16 04:45:19.000000 pz-rail-0.99.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.740254 pz-rail-0.99.1/examples/core_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/FileIO_DataStore.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/Pipe_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/Run_Pipe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/hyperbolic_magnitude_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/iterator_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/pipe_example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/pipe_example_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.740254 pz-rail-0.99.1/examples/creation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/degradation-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/dsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/example_ObsConditions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/photometric_realization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24628 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/posterior-demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.744254 pz-rail-0.99.1/examples/estimation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/NZDir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/RAIL_estimation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    28480 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/nzdir_as_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/somocluSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/test_sampled_summarizers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.744254 pz-rail-0.99.1/examples/evaluation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/examples/goldenspike_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/goldenspike_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/goldenspike_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/goldenspike_examples/cleanup_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    25570 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/goldenspike_examples/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-16 04:45:19.000000 pz-rail-0.99.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-16 04:45:19.000000 pz-rail-0.99.1/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 04:45:19.000000 pz-rail-0.99.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:45:31.748254 pz-rail-0.99.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 04:45:19.000000 pz-rail-0.99.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.728254 pz-rail-0.99.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/src/pz_rail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.728254 pz-rail-0.99.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/src/rail/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 04:45:19.000000 pz-rail-0.99.1/src/rail/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/rail/hub/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.728254 pz-rail-0.99.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 04:45:19.000000 pz-rail-0.99.1/tests/hub/test_import.py
```

### Comparing `pz-rail-0.99.0/.github/pull_request_template.md` & `pz-rail-0.99.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/.github/workflows/build_documentation.yml` & `pz-rail-0.99.1/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/.github/workflows/linting.yml` & `pz-rail-0.99.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/.github/workflows/publish-to-pypi.yml` & `pz-rail-0.99.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/.github/workflows/smoke-test.yml` & `pz-rail-0.99.1/.github/workflows/smoke-test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -35,9 +35,8 @@
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Run unit tests with pytest
       run: |
         python -m pytest tests
     - name: Run notebooks
       run: |
         rail render-nb examples/${{ matrix.notebook-dir }}_examples/*.ipynb
-      continue-on-error: true
```

### Comparing `pz-rail-0.99.0/.github/workflows/testing-and-coverage.yml` & `pz-rail-0.99.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/.gitignore` & `pz-rail-0.99.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/.pre-commit-config.yaml` & `pz-rail-0.99.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/.readthedocs.yaml` & `pz-rail-0.99.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/LICENSE` & `pz-rail-0.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/PKG-INFO` & `pz-rail-0.99.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail
-Version: 0.99.0
+Version: 0.99.1
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-0.99.0/README.md` & `pz-rail-0.99.1/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/Makefile` & `pz-rail-0.99.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/_static/css/notebooks.css` & `pz-rail-0.99.1/docs/_static/css/notebooks.css`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/conf.py` & `pz-rail-0.99.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/demos.rst` & `pz-rail-0.99.1/docs/demos.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/index.rst` & `pz-rail-0.99.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/source/citing.rst` & `pz-rail-0.99.1/docs/source/citing.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/source/contributing.rst` & `pz-rail-0.99.1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/source/futureplans.rst` & `pz-rail-0.99.1/docs/source/futureplans.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/source/immediateplans.rst` & `pz-rail-0.99.1/docs/source/immediateplans.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/docs/source/installation.rst` & `pz-rail-0.99.1/docs/source/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 .. code-block:: bash
 
     git clone https://github.com/LSSTDESC/rail.git
     cd rail
     conda env create -f environment.yml -n [env]  # or mamba env create, which is much faster
     conda activate [env]
     pip install .
-    rail clone --package-file rail_packages.yml
+    rail clone-source --package-file rail_packages.yml
     rail install --package-file rail_packages.yml --from-source 
 
     
 
 RAIL packages
 =============
```

### Comparing `pz-rail-0.99.0/docs/source/overview.rst` & `pz-rail-0.99.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/core_examples/FileIO_DataStore.ipynb` & `pz-rail-0.99.1/examples/core_examples/FileIO_DataStore.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb` & `pz-rail-0.99.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/core_examples/Pipe_Example.ipynb` & `pz-rail-0.99.1/examples/core_examples/Pipe_Example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/core_examples/README.md` & `pz-rail-0.99.1/examples/core_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/core_examples/Run_Pipe.ipynb` & `pz-rail-0.99.1/examples/core_examples/Run_Pipe.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964657738095238%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'from rail.core.utils import find_rail_file\\n'), (3, "*

 * *            '"flow_file = '*

 * *            'find_rail_file(\'examples_data/goldenspike_data/data/pretrained_flow.pkl\')\\n"), (4, '*

 * *            '"os.environ[\'FLOWDIR\'] = os.path.dirname(flow_file)")], delete: [4, 3, 2]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.11.4'}}"}*

```diff
@@ -20,17 +20,17 @@
             "execution_count": null,
             "id": "a29a1b21",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "import ceci\n",
-                "from rail.core.utils import RAILDIR\n",
-                "os.environ['RAILDIR'] = RAILDIR\n",
-                "model_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')"
+                "from rail.core.utils import find_rail_file\n",
+                "flow_file = find_rail_file('examples_data/goldenspike_data/data/pretrained_flow.pkl')\n",
+                "os.environ['FLOWDIR'] = os.path.dirname(flow_file)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2657aca0",
             "metadata": {},
@@ -78,13 +78,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.11.4"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz-rail-0.99.0/examples/core_examples/hyperbolic_magnitude_test.ipynb` & `pz-rail-0.99.1/examples/core_examples/hyperbolic_magnitude_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/core_examples/iterator_test.ipynb` & `pz-rail-0.99.1/examples/core_examples/iterator_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/creation_examples/README.md` & `pz-rail-0.99.1/examples/creation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/creation_examples/degradation-demo.ipynb` & `pz-rail-0.99.1/examples/creation_examples/degradation-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/creation_examples/dsps_sed_demo.ipynb` & `pz-rail-0.99.1/examples/creation_examples/dsps_sed_demo.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9936011904761906%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(5, '\\n')], delete: [6, 5]}}, insert: [(1, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict()), ('outputs', []), ('source', ['import os\\n', 'import numpy as np\\n', "*

 * *            '"os.environ[\'SPS_HOME\'] = '*

 * *            'os.path.join(os.path.dirname(np.__file__).replace(\'/numpy\',\'\'), \'fsps\')"])]))]}',*

 * * "'metadata'": "{'language_info': {'version': '3.11.4'}}"}*

```diff
@@ -19,21 +19,31 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import os\n",
+                "import numpy as np\n",
+                "os.environ['SPS_HOME'] = os.path.join(os.path.dirname(np.__file__).replace('/numpy',''), 'fsps')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "import rail\n",
                 "from rail.core.stage import RailStage\n",
                 "from rail.creation.engines.dsps_sed_modeler import DSPSSingleSedModeler, DSPSPopulationSedModeler\n",
                 "from rail.creation.engines.dsps_photometry_creator import DSPSPhotometryCreator\n",
                 "from dsps.load_fsps_data import load_fsps_testing_data\n",
-                "import numpy as np\n",
-                "import os\n",
+                "\n",
                 "from dsps.utils import _jax_get_dt_array"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -373,13 +383,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.11.4"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `pz-rail-0.99.0/examples/creation_examples/example_GridSelection_for_HSC.ipynb` & `pz-rail-0.99.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/creation_examples/example_ObsConditions.ipynb` & `pz-rail-0.99.1/examples/creation_examples/example_ObsConditions.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb` & `pz-rail-0.99.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/creation_examples/photometric_realization_demo.ipynb` & `pz-rail-0.99.1/examples/creation_examples/photometric_realization_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/creation_examples/posterior-demo.ipynb` & `pz-rail-0.99.1/examples/creation_examples/posterior-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/estimation_examples/NZDir.ipynb` & `pz-rail-0.99.1/examples/estimation_examples/NZDir.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/estimation_examples/RAIL_estimation_demo.ipynb` & `pz-rail-0.99.1/examples/estimation_examples/RAIL_estimation_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/estimation_examples/README.md` & `pz-rail-0.99.1/examples/estimation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme` & `pz-rail-0.99.1/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/estimation_examples/nzdir_as_pipeline.ipynb` & `pz-rail-0.99.1/examples/estimation_examples/nzdir_as_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/estimation_examples/somocluSOM_demo.ipynb` & `pz-rail-0.99.1/examples/estimation_examples/somocluSOM_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/estimation_examples/somocluSOMcluster_demo.ipynb` & `pz-rail-0.99.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/estimation_examples/test_sampled_summarizers.ipynb` & `pz-rail-0.99.1/examples/estimation_examples/test_sampled_summarizers.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/evaluation_examples/demo.ipynb` & `pz-rail-0.99.1/examples/evaluation_examples/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/evaluation_examples/utils.py` & `pz-rail-0.99.1/examples/evaluation_examples/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/goldenspike_examples/cleanup.sh` & `pz-rail-0.99.1/examples/goldenspike_examples/cleanup.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/examples/goldenspike_examples/goldenspike.ipynb` & `pz-rail-0.99.1/examples/goldenspike_examples/goldenspike.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.0/pyproject.toml` & `pz-rail-0.99.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 dynamic = ["version"]
 
 dependencies = [
     "pz-rail-base",
-    "click",
-    "pyaml",
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 algos = [
     "pz-rail-pipelines[full]",
 ]
@@ -47,17 +45,14 @@
 docs = [
     "nbsphinx",
     "sphinx==6.1.3", # Used to automatically generate documentation
     "sphinx_rtd_theme==1.2.0", # Used to render documentation
     "sphinx-autoapi==2.0.1", # Used to automatically generate api documentation    
 ]
 
-[project.scripts]
-rail = "rail.hub.commands:cli"
-
 [build-system]
 requires = [
     "setuptools>=62", # Used to build and package the Python project
     "setuptools_scm>=6.2", # Gets release version from git. Makes it available programmatically
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `pz-rail-0.99.0/src/pz_rail.egg-info/PKG-INFO` & `pz-rail-0.99.1/src/pz_rail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail
-Version: 0.99.0
+Version: 0.99.1
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-0.99.0/src/pz_rail.egg-info/SOURCES.txt` & `pz-rail-0.99.1/src/pz_rail.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
 examples/core_examples/Pipe_Example.ipynb
 examples/core_examples/README.md
 examples/core_examples/Run_Pipe.ipynb
 examples/core_examples/cleanup.sh
 examples/core_examples/hyperbolic_magnitude_test.ipynb
 examples/core_examples/iterator_test.ipynb
+examples/core_examples/pipe_example.yml
+examples/core_examples/pipe_example_config.yml
 examples/creation_examples/README.md
 examples/creation_examples/cleanup.sh
 examples/creation_examples/degradation-demo.ipynb
 examples/creation_examples/dsps_sed_demo.ipynb
 examples/creation_examples/example_GridSelection_for_HSC.ipynb
 examples/creation_examples/example_ObsConditions.ipynb
 examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
@@ -66,17 +68,12 @@
 examples/goldenspike_examples/README.md
 examples/goldenspike_examples/cleanup.sh
 examples/goldenspike_examples/cleanup_pipeline.sh
 examples/goldenspike_examples/goldenspike.ipynb
 src/pz_rail.egg-info/PKG-INFO
 src/pz_rail.egg-info/SOURCES.txt
 src/pz_rail.egg-info/dependency_links.txt
-src/pz_rail.egg-info/entry_points.txt
 src/pz_rail.egg-info/requires.txt
 src/pz_rail.egg-info/top_level.txt
 src/rail/hub/__init__.py
 src/rail/hub/_version.py
-src/rail/hub/commands.py
-src/rail/hub/options.py
-src/rail/hub/scripts.py
-tests/test_import.py
-tests/test_scripts.py
+tests/hub/test_import.py
```

