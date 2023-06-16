# Comparing `tmp/optimas-0.1.0.tar.gz` & `tmp/optimas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimas-0.1.0.tar", last modified: Wed May 31 07:50:46 2023, max compression
+gzip compressed data, was "optimas-0.1.1.tar", last modified: Fri Jun 16 07:35:09 2023, max compression
```

## Comparing `optimas-0.1.0.tar` & `optimas-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.790882 optimas-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-31 07:50:46.790882 optimas-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-31 07:50:33.000000 optimas-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.782882 optimas-0.1.0/optimas/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.782882 optimas-0.1.0/optimas/core/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/core/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/core/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.786882 optimas-0.1.0/optimas/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/evaluators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/evaluators/function_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/evaluators/multitask_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/evaluators/template_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.786882 optimas-0.1.0/optimas/explorations/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/explorations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/explorations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/gen_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.786882 optimas-0.1.0/optimas/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.786882 optimas-0.1.0/optimas/generators/ax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.786882 optimas-0.1.0/optimas/generators/ax/developer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/developer/ax_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/developer/multitask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.790882 optimas-0.1.0/optimas/generators/ax/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/service/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/service/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/ax/service/single_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/grid_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/line_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/generators/random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/sim_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.790882 optimas-0.1.0/optimas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-31 07:50:33.000000 optimas-0.1.0/optimas/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.782882 optimas-0.1.0/optimas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-31 07:50:46.000000 optimas-0.1.0/optimas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-31 07:50:46.000000 optimas-0.1.0/optimas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:50:46.000000 optimas-0.1.0/optimas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 07:50:46.000000 optimas-0.1.0/optimas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 07:50:46.000000 optimas-0.1.0/optimas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 07:50:33.000000 optimas-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:50:46.790882 optimas-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:50:33.000000 optimas-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:50:46.790882 optimas-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-31 07:50:33.000000 optimas-0.1.0/tests/test_analyzed_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-05-31 07:50:33.000000 optimas-0.1.0/tests/test_ax_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-31 07:50:33.000000 optimas-0.1.0/tests/test_function_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-31 07:50:33.000000 optimas-0.1.0/tests/test_grid_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-31 07:50:33.000000 optimas-0.1.0/tests/test_line_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-31 07:50:33.000000 optimas-0.1.0/tests/test_random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-31 07:50:33.000000 optimas-0.1.0/tests/test_template_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.305848 optimas-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 07:35:09.301848 optimas-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-16 07:34:57.000000 optimas-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.297848 optimas-0.1.1/optimas/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/function_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/multitask_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/template_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/explorations/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/explorations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/explorations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/gen_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/generators/ax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/generators/ax/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/developer/ax_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/developer/multitask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/generators/ax/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/service/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/service/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/service/single_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/grid_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/line_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/sim_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.297848 optimas-0.1.1/optimas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-16 07:34:57.000000 optimas-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:35:09.305848 optimas-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:34:57.000000 optimas-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_analyzed_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_ax_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_function_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_grid_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_line_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_template_evaluator.py
```

### Comparing `optimas-0.1.0/PKG-INFO` & `optimas-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimas
-Version: 0.1.0
+Version: 0.1.1
 Summary: Optimization at scale, powered by libEnsemble
 Author-email: Optimas Developers <angel.ferran.pousa@desy.de>
 License: BSD-3-Clause-LBNL
 Project-URL: Documentation, https://optimas.readthedocs.io/
 Keywords: optimization,scale,bayesian
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -20,10 +20,14 @@
 
 <p align="center">
     <img width="450" src="https://user-images.githubusercontent.com/20479420/219680583-34ac9525-7715-4e2a-b4fe-74848e9f59b2.png" alt="optimas logo"/>
 </p>
 <!-- <hr/> -->
 
 # Optimization at scale, powered by [libEnsemble](https://libensemble.readthedocs.io/)
+[![PyPI](https://img.shields.io/pypi/v/optimas)](https://pypi.org/project/optimas/)
+[![tests badge](https://github.com/optimas-org/optimas/actions/workflows/unix.yml/badge.svg)](https://github.com/optimas-org/optimas/actions)
 [![Documentation Status](https://readthedocs.org/projects/optimas/badge/?version=latest)](https://optimas.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/287560975.svg)](https://zenodo.org/badge/latestdoi/287560975)
+[![License](https://img.shields.io/pypi/l/optimas.svg)](license.txt)
 
 Optimas is a Python library for scalable optimization on massively-parallel supercomputers. See the [documentation](https://optimas.readthedocs.io/) for installation instructions, tutorials, and more information.
```

### Comparing `optimas-0.1.0/optimas/core/evaluation.py` & `optimas-0.1.1/optimas/core/evaluation.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/core/parameter.py` & `optimas-0.1.1/optimas/core/parameter.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/core/task.py` & `optimas-0.1.1/optimas/core/task.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/core/trial.py` & `optimas-0.1.1/optimas/core/trial.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/evaluators/base.py` & `optimas-0.1.1/optimas/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/evaluators/function_evaluator.py` & `optimas-0.1.1/optimas/evaluators/function_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/evaluators/multitask_evaluator.py` & `optimas-0.1.1/optimas/evaluators/multitask_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/evaluators/template_evaluator.py` & `optimas-0.1.1/optimas/evaluators/template_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/explorations/base.py` & `optimas-0.1.1/optimas/explorations/base.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/gen_functions.py` & `optimas-0.1.1/optimas/gen_functions.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/generators/__init__.py` & `optimas-0.1.1/optimas/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/generators/ax/base.py` & `optimas-0.1.1/optimas/generators/ax/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Whether to allow the generator to run on a CUDA GPU. By default
         ``False``.
     gpu_id : int, optional
         The ID of the GPU in which to run the generator. By default, ``0``.
     dedicated_resources : bool, optional
         Whether to allocated dedicated resources (e.g., the GPU) for the
         generator. These resources will not be available to the
-        simulation workers. By default, ``True``.
+        simulation workers. By default, ``False``.
     save_model : bool, optional
         Whether to save the optimization model (e.g., the surrogate model) to
         disk. By default ``False``.
     model_save_period : int, optional
         Periodicity, in number of evaluated Trials, with which to save the
         model to disk. By default, ``5``.
     model_history_dir : str, optional
@@ -45,15 +45,15 @@
     def __init__(
         self,
         varying_parameters: List[VaryingParameter],
         objectives: List[Objective],
         analyzed_parameters: Optional[List[Parameter]] = None,
         use_cuda: Optional[bool] = False,
         gpu_id: Optional[int] = 0,
-        dedicated_resources: Optional[bool] = True,
+        dedicated_resources: Optional[bool] = False,
         save_model: Optional[bool] = False,
         model_save_period: Optional[int] = 5,
         model_history_dir: Optional[str] = 'model_history',
         custom_trial_parameters: Optional[TrialParameter] = None
     ) -> None:
         super().__init__(
             varying_parameters=varying_parameters,
```

### Comparing `optimas-0.1.0/optimas/generators/ax/developer/ax_metric.py` & `optimas-0.1.1/optimas/generators/ax/developer/ax_metric.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/generators/ax/developer/multitask.py` & `optimas-0.1.1/optimas/generators/ax/developer/multitask.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         Whether to allow the generator to run on a CUDA GPU. By default
         ``False``.
     gpu_id : int, optional
         The ID of the GPU in which to run the generator. By default, ``0``.
     dedicated_resources : bool, optional
         Whether to allocated dedicated resources (e.g., the GPU) for the
         generator. These resources will not be available to the
-        simulation workers. By default, ``True``.
+        simulation workers. By default, ``False``.
     save_model : bool, optional
         Whether to save the optimization model (in this case, the Ax
         experiment) to disk. By default ``True``.
     model_save_period : int, optional
         Periodicity, in number of evaluated Trials, with which to save the
         model to disk. By default, ``5``.
     model_history_dir : str, optional
@@ -78,15 +78,15 @@
         varying_parameters: List[VaryingParameter],
         objectives: List[Objective],
         lofi_task: Task,
         hifi_task: Task,
         analyzed_parameters: Optional[List[Parameter]] = None,
         use_cuda: Optional[bool] = False,
         gpu_id: Optional[int] = 0,
-        dedicated_resources: Optional[bool] = True,
+        dedicated_resources: Optional[bool] = False,
         save_model: Optional[bool] = True,
         model_save_period: Optional[int] = 5,
         model_history_dir: Optional[str] = 'model_history'
     ) -> None:
         custom_trial_parameters = [
             TrialParameter('arm_name', 'ax_arm_name', dtype='U32'),
             TrialParameter('trial_type', 'ax_trial_type', dtype='U32'),
```

### Comparing `optimas-0.1.0/optimas/generators/ax/service/base.py` & `optimas-0.1.1/optimas/generators/ax/service/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Whether to allow the generator to run on a CUDA GPU. By default
         ``False``.
     gpu_id : int, optional
         The ID of the GPU in which to run the generator. By default, ``0``.
     dedicated_resources : bool, optional
         Whether to allocated dedicated resources (e.g., the GPU) for the
         generator. These resources will not be available to the
-        simulation workers. By default, ``True``.
+        simulation workers. By default, ``False``.
     save_model : bool, optional
         Whether to save the optimization model (in this case, the Ax client) to
         disk. By default ``True``.
     model_save_period : int, optional
         Periodicity, in number of evaluated Trials, with which to save the
         model to disk. By default, ``5``.
     model_history_dir : str, optional
@@ -48,15 +48,15 @@
         self,
         varying_parameters: List[VaryingParameter],
         objectives: List[Objective],
         analyzed_parameters: Optional[List[Parameter]] = None,
         n_init: Optional[int] = 4,
         use_cuda: Optional[bool] = False,
         gpu_id: Optional[int] = 0,
-        dedicated_resources: Optional[bool] = True,
+        dedicated_resources: Optional[bool] = False,
         save_model: Optional[bool] = True,
         model_save_period: Optional[int] = 5,
         model_history_dir: Optional[str] = 'model_history',
     ) -> None:
         super().__init__(
             varying_parameters=varying_parameters,
             objectives=objectives,
```

### Comparing `optimas-0.1.0/optimas/generators/ax/service/multi_fidelity.py` & `optimas-0.1.1/optimas/generators/ax/service/multi_fidelity.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Whether to allow the generator to run on a CUDA GPU. By default
         ``False``.
     gpu_id : int, optional
         The ID of the GPU in which to run the generator. By default, ``0``.
     dedicated_resources : bool, optional
         Whether to allocated dedicated resources (e.g., the GPU) for the
         generator. These resources will not be available to the
-        simulation workers. By default, ``True``.
+        simulation workers. By default, ``False``.
     save_model : bool, optional
         Whether to save the optimization model (in this case, the Ax client) to
         disk. By default ``True``.
     model_save_period : int, optional
         Periodicity, in number of evaluated Trials, with which to save the
         model to disk. By default, ``5``.
     model_history_dir : str, optional
@@ -57,15 +57,15 @@
         varying_parameters: List[VaryingParameter],
         objectives: List[Objective],
         analyzed_parameters: Optional[List[Parameter]] = None,
         n_init: Optional[int] = 4,
         fidel_cost_intercept: Optional[float] = 1.,
         use_cuda: Optional[bool] = False,
         gpu_id: Optional[int] = 0,
-        dedicated_resources: Optional[bool] = True,
+        dedicated_resources: Optional[bool] = False,
         save_model: Optional[bool] = True,
         model_save_period: Optional[int] = 5,
         model_history_dir: Optional[str] = 'model_history',
     ) -> None:
         self.fidel_cost_intercept = fidel_cost_intercept
         super().__init__(
             varying_parameters=varying_parameters,
```

### Comparing `optimas-0.1.0/optimas/generators/ax/service/single_fidelity.py` & `optimas-0.1.1/optimas/generators/ax/service/single_fidelity.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         Whether to allow the generator to run on a CUDA GPU. By default
         ``False``.
     gpu_id : int, optional
         The ID of the GPU in which to run the generator. By default, ``0``.
     dedicated_resources : bool, optional
         Whether to allocated dedicated resources (e.g., the GPU) for the
         generator. These resources will not be available to the
-        simulation workers. By default, ``True``.
+        simulation workers. By default, ``False``.
     save_model : bool, optional
         Whether to save the optimization model (in this case, the Ax client) to
         disk. By default ``True``.
     model_save_period : int, optional
         Periodicity, in number of evaluated Trials, with which to save the
         model to disk. By default, ``5``.
     model_history_dir : str, optional
@@ -52,15 +52,15 @@
         self,
         varying_parameters: List[VaryingParameter],
         objectives: List[Objective],
         analyzed_parameters: Optional[List[Parameter]] = None,
         n_init: Optional[int] = 4,
         use_cuda: Optional[bool] = False,
         gpu_id: Optional[int] = 0,
-        dedicated_resources: Optional[bool] = True,
+        dedicated_resources: Optional[bool] = False,
         save_model: Optional[bool] = True,
         model_save_period: Optional[int] = 5,
         model_history_dir: Optional[str] = 'model_history',
     ) -> None:
         super().__init__(
             varying_parameters=varying_parameters,
             objectives=objectives,
```

### Comparing `optimas-0.1.0/optimas/generators/base.py` & `optimas-0.1.1/optimas/generators/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Whether to allow the generator to run on a CUDA GPU. By default
         ``False``.
     gpu_id : int, optional
         The ID of the GPU in which to run the generator. By default, ``0``.
     dedicated_resources : bool, optional
         Whether to allocated dedicated resources (e.g., the GPU) for the
         generator. These resources will not be available to the
-        simulation workers. By default, ``True``.
+        simulation workers. By default, ``False``.
     save_model : bool, optional
         Whether to save the optimization model (e.g., the surrogate model) to
         disk. By default ``False``.
     model_save_period : int, optional
         Periodicity, in number of evaluated Trials, with which to save the
         model to disk. By default, ``5``.
     model_history_dir : str, optional
@@ -55,15 +55,15 @@
         self,
         varying_parameters: List[VaryingParameter],
         objectives: List[Objective],
         constraints: Optional[List[Parameter]] = None,
         analyzed_parameters: Optional[List[Parameter]] = None,
         use_cuda: Optional[bool] = False,
         gpu_id: Optional[int] = 0,
-        dedicated_resources: Optional[bool] = True,
+        dedicated_resources: Optional[bool] = False,
         save_model: Optional[bool] = False,
         model_save_period: Optional[int] = 5,
         model_history_dir: Optional[str] = 'model_history',
         custom_trial_parameters: Optional[TrialParameter] = None
     ) -> None:
         if objectives is None:
             objectives = [Objective()]
```

### Comparing `optimas-0.1.0/optimas/generators/grid_sampling.py` & `optimas-0.1.1/optimas/generators/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/generators/line_sampling.py` & `optimas-0.1.1/optimas/generators/line_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/generators/random_sampling.py` & `optimas-0.1.1/optimas/generators/random_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/post_processing.py` & `optimas-0.1.1/optimas/post_processing.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas/sim_functions.py` & `optimas-0.1.1/optimas/sim_functions.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/optimas.egg-info/PKG-INFO` & `optimas-0.1.1/optimas.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimas
-Version: 0.1.0
+Version: 0.1.1
 Summary: Optimization at scale, powered by libEnsemble
 Author-email: Optimas Developers <angel.ferran.pousa@desy.de>
 License: BSD-3-Clause-LBNL
 Project-URL: Documentation, https://optimas.readthedocs.io/
 Keywords: optimization,scale,bayesian
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -20,10 +20,14 @@
 
 <p align="center">
     <img width="450" src="https://user-images.githubusercontent.com/20479420/219680583-34ac9525-7715-4e2a-b4fe-74848e9f59b2.png" alt="optimas logo"/>
 </p>
 <!-- <hr/> -->
 
 # Optimization at scale, powered by [libEnsemble](https://libensemble.readthedocs.io/)
+[![PyPI](https://img.shields.io/pypi/v/optimas)](https://pypi.org/project/optimas/)
+[![tests badge](https://github.com/optimas-org/optimas/actions/workflows/unix.yml/badge.svg)](https://github.com/optimas-org/optimas/actions)
 [![Documentation Status](https://readthedocs.org/projects/optimas/badge/?version=latest)](https://optimas.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/287560975.svg)](https://zenodo.org/badge/latestdoi/287560975)
+[![License](https://img.shields.io/pypi/l/optimas.svg)](license.txt)
 
 Optimas is a Python library for scalable optimization on massively-parallel supercomputers. See the [documentation](https://optimas.readthedocs.io/) for installation instructions, tutorials, and more information.
```

### Comparing `optimas-0.1.0/optimas.egg-info/SOURCES.txt` & `optimas-0.1.1/optimas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/pyproject.toml` & `optimas-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/tests/test_analyzed_parameters.py` & `optimas-0.1.1/tests/test_analyzed_parameters.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/tests/test_ax_generators.py` & `optimas-0.1.1/tests/test_ax_generators.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/tests/test_function_evaluator.py` & `optimas-0.1.1/tests/test_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/tests/test_grid_sampling.py` & `optimas-0.1.1/tests/test_grid_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/tests/test_line_sampling.py` & `optimas-0.1.1/tests/test_line_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/tests/test_random_sampling.py` & `optimas-0.1.1/tests/test_random_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.0/tests/test_template_evaluator.py` & `optimas-0.1.1/tests/test_template_evaluator.py`

 * *Files identical despite different names*

