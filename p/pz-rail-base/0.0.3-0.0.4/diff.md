# Comparing `tmp/pz-rail-base-0.0.3.tar.gz` & `tmp/pz-rail-base-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-base-0.0.3.tar", last modified: Tue Jun 13 20:16:02 2023, max compression
+gzip compressed data, was "pz-rail-base-0.0.4.tar", last modified: Fri Jun 16 04:47:15 2023, max compression
```

## Comparing `pz-rail-base-0.0.3.tar` & `pz-rail-base-0.0.4.tar`

### file list

```diff
@@ -1,128 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.794632 pz-rail-base-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.758633 pz-rail-base-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.758633 pz-rail-base-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-13 20:16:02.794632 pz-rail-base-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:16:02.794632 pz-rail-base-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.750633 pz-rail-base-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.758633 pz-rail-base-0.0.3/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-13 20:16:02.000000 pz-rail-base-0.0.3/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-13 20:16:02.000000 pz-rail-base-0.0.3/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:16:02.000000 pz-rail-base-0.0.3/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-13 20:16:02.000000 pz-rail-base-0.0.3/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 20:16:02.000000 pz-rail-base-0.0.3/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.754633 pz-rail-base-0.0.3/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.762632 pz-rail-base-0.0.3/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 20:16:02.000000 pz-rail-base-0.0.3/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/core/utilStages.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.762632 pz-rail-base-0.0.3/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.762632 pz-rail-base-0.0.3/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (123)    30116 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/creation/degradation/lsst_error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (123)    22286 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/creation/degradation/spectroscopic_selections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/creation/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.766632 pz-rail-base-0.0.3/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.766632 pz-rail-base-0.0.3/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/estimation/algos/naiveStack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/estimation/algos/pointEstimateHist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/estimation/algos/randomPZ.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/estimation/algos/trainZ.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/estimation/algos/varInference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.766632 pz-rail-base-0.0.3/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.766632 pz-rail-base-0.0.3/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/evaluation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.766632 pz-rail-base-0.0.3/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.750633 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.770633 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.770633 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.770633 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1000000 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)   431705 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.750633 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.774633 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.774633 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.774633 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (123)    98003 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (123)    95326 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (123)    96635 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (123)    90216 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (123)   100126 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (123)    93013 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.778632 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (123)    43750 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    42830 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    72228 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    68560 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    43351 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    42789 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)   179585 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)   179584 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.778632 pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.782632 pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.782632 pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1158108 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   873947 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.790632 pz-rail-base-0.0.3/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    91936 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (123)    24574 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (123)   662976 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)   873930 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (123)  1192254 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (123)  1316984 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.790632 pz-rail-base-0.0.3/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.754633 pz-rail-base-0.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:16:02.794632 pz-rail-base-0.0.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/tests/core/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/tests/core/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/tests/core/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/tests/core/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-13 20:15:45.000000 pz-rail-base-0.0.3/tests/core/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.822332 pz-rail-base-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.818332 pz-rail-base-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.822332 pz-rail-base-0.0.4/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/algo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/utilStages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)    30116 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/degradation/lsst_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/degradation/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22286 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/degradation/spectroscopic_selections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/degrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/naiveStack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/pointEstimateHist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/randomPZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/trainZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/varInference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.818332 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1000000 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   431705 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.822332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (123)    98003 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (123)    95326 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (123)    96635 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (123)    90216 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (123)   100126 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (123)    93013 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43750 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42830 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    72228 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68560 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43351 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42789 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)   179585 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)   179584 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.842332 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.842332 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.842332 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1158108 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   873947 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    91936 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    24574 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (123)   662976 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)   873930 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (123)  1192254 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (123)  1316984 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.822332 pz-rail-base-0.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/core/test_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/core/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.0.3/.github/pull_request_template.md` & `pz-rail-base-0.0.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/.github/workflows/linting.yml` & `pz-rail-base-0.0.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/.github/workflows/publish-to-pypi.yml` & `pz-rail-base-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/.github/workflows/smoke-test.yml` & `pz-rail-base-0.0.4/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/.github/workflows/testing-and-coverage.yml` & `pz-rail-base-0.0.4/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/.gitignore` & `pz-rail-base-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/.pre-commit-config.yaml` & `pz-rail-base-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/LICENSE` & `pz-rail-base-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/PKG-INFO` & `pz-rail-base-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.0.3
+Version: 0.0.4
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.0.3/README.md` & `pz-rail-base-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/pyproject.toml` & `pz-rail-base-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 dynamic = ["version"]
 dependencies = [
     "deprecated",
+    "pyyaml",
     "numpy",
+    "click",
     "ceci>=1.10.1",
     "qp-prob>=0.8.3",
     "scipy>=1.9.0",
 ]
 
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
@@ -29,14 +31,17 @@
     "qp-prob[full]", 
     "pytest",
     "pytest-cov", # Used to report total code coverage
     "pre-commit", # Used to run checks before finalizing a git commit
     "pylint", # Used for static linting of files
 ]
 
+[project.scripts]
+rail = "rail.cli.commands:cli"
+
 [build-system]
 requires = [
     "setuptools>=62", # Used to build and package the Python project
     "setuptools_scm>=6.2", # Gets release version from git. Makes it available programmatically
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `pz-rail-base-0.0.3/src/pz_rail_base.egg-info/PKG-INFO` & `pz-rail-base-0.0.4/src/pz_rail_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.0.3
+Version: 0.0.4
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.0.3/src/pz_rail_base.egg-info/SOURCES.txt` & `pz-rail-base-0.0.4/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 .copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
+environment.yml
 pyproject.toml
+rail_packages.yml
 setup.py
 .github/pull_request_template.md
 .github/workflows/add-issue-to-project-tracker.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 src/pz_rail_base.egg-info/PKG-INFO
 src/pz_rail_base.egg-info/SOURCES.txt
 src/pz_rail_base.egg-info/dependency_links.txt
+src/pz_rail_base.egg-info/entry_points.txt
 src/pz_rail_base.egg-info/requires.txt
 src/pz_rail_base.egg-info/top_level.txt
+src/rail/cli/commands.py
+src/rail/cli/options.py
+src/rail/cli/scripts.py
 src/rail/core/__init__.py
 src/rail/core/_version.py
 src/rail/core/algo_utils.py
 src/rail/core/common_params.py
 src/rail/core/data.py
 src/rail/core/introspection.py
 src/rail/core/stage.py
@@ -83,14 +89,15 @@
 src/rail/examples_data/testdata/test_dc2_training_9816.pq
 src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
 src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
 src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
 src/rail/examples_data/testdata/training_100gal.hdf5
 src/rail/examples_data/testdata/validation_10gal.hdf5
 src/rail/stages/__init__.py
-tests/core/test_algos.py
+tests/cli/test_scripts.py
 tests/core/test_core.py
 tests/core/test_degraders.py
-tests/core/test_evaluation.py
 tests/core/test_introspection.py
 tests/core/test_pipeline.py
-tests/core/test_summarizers.py
+tests/estimation/test_algos.py
+tests/estimation/test_summarizers.py
+tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.0.3/src/rail/core/__init__.py` & `pz-rail-base-0.0.4/src/rail/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/core/algo_utils.py` & `pz-rail-base-0.0.4/src/rail/core/algo_utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/core/common_params.py` & `pz-rail-base-0.0.4/src/rail/core/common_params.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/core/data.py` & `pz-rail-base-0.0.4/src/rail/core/data.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/core/introspection.py` & `pz-rail-base-0.0.4/src/rail/core/introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/core/stage.py` & `pz-rail-base-0.0.4/src/rail/core/stage.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/core/utilStages.py` & `pz-rail-base-0.0.4/src/rail/core/utilStages.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/core/utils.py` & `pz-rail-base-0.0.4/src/rail/core/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/creation/degradation/lsst_error_model.py` & `pz-rail-base-0.0.4/src/rail/creation/degradation/lsst_error_model.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/creation/degradation/quantityCut.py` & `pz-rail-base-0.0.4/src/rail/creation/degradation/quantityCut.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/creation/degradation/spectroscopic_selections.py` & `pz-rail-base-0.0.4/src/rail/creation/degradation/spectroscopic_selections.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/creation/degrader.py` & `pz-rail-base-0.0.4/src/rail/creation/degrader.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/creation/engine.py` & `pz-rail-base-0.0.4/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/estimation/algos/naiveStack.py` & `pz-rail-base-0.0.4/src/rail/estimation/algos/naiveStack.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/estimation/algos/pointEstimateHist.py` & `pz-rail-base-0.0.4/src/rail/estimation/algos/pointEstimateHist.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/estimation/algos/randomPZ.py` & `pz-rail-base-0.0.4/src/rail/estimation/algos/randomPZ.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/estimation/algos/trainZ.py` & `pz-rail-base-0.0.4/src/rail/estimation/algos/trainZ.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/estimation/algos/varInference.py` & `pz-rail-base-0.0.4/src/rail/estimation/algos/varInference.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/estimation/estimator.py` & `pz-rail-base-0.0.4/src/rail/estimation/estimator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/estimation/summarizer.py` & `pz-rail-base-0.0.4/src/rail/estimation/summarizer.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/evaluation/evaluator.py` & `pz-rail-base-0.0.4/src/rail/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/evaluation/metrics/base.py` & `pz-rail-base-0.0.4/src/rail/evaluation/metrics/base.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/evaluation/metrics/cdeloss.py` & `pz-rail-base-0.0.4/src/rail/evaluation/metrics/cdeloss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/evaluation/metrics/pointestimates.py` & `pz-rail-base-0.0.4/src/rail/evaluation/metrics/pointestimates.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/README.md` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/lsst_filters.npy` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz-rail-base-0.0.4/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/src/rail/stages/__init__.py` & `pz-rail-base-0.0.4/src/rail/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/tests/core/test_algos.py` & `pz-rail-base-0.0.4/tests/estimation/test_algos.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/tests/core/test_core.py` & `pz-rail-base-0.0.4/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/tests/core/test_degraders.py` & `pz-rail-base-0.0.4/tests/core/test_degraders.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/tests/core/test_evaluation.py` & `pz-rail-base-0.0.4/tests/evaluation/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/tests/core/test_introspection.py` & `pz-rail-base-0.0.4/tests/core/test_introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/tests/core/test_pipeline.py` & `pz-rail-base-0.0.4/tests/core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.3/tests/core/test_summarizers.py` & `pz-rail-base-0.0.4/tests/estimation/test_summarizers.py`

 * *Files identical despite different names*

