# Comparing `tmp/currentscape-1.0.2.tar.gz` & `tmp/currentscape-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currentscape-1.0.2.tar", last modified: Fri Jun 16 08:56:14 2023, max compression
+gzip compressed data, was "currentscape-1.0.3.tar", last modified: Fri Jun 16 08:59:52 2023, max compression
```

## Comparing `currentscape-1.0.2.tar` & `currentscape-1.0.3.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 08:56:06.000000 currentscape-1.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 08:56:06.000000 currentscape-1.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 08:56:06.000000 currentscape-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 08:56:06.000000 currentscape-1.0.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 08:56:06.000000 currentscape-1.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 08:56:06.000000 currentscape-1.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-16 08:56:06.000000 currentscape-1.0.2/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 08:56:06.000000 currentscape-1.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 08:56:06.000000 currentscape-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-16 08:56:06.000000 currentscape-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-16 08:56:06.000000 currentscape-1.0.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 08:56:06.000000 currentscape-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 08:56:06.000000 currentscape-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 08:56:06.000000 currentscape-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 08:56:14.717142 currentscape-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-16 08:56:06.000000 currentscape-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-16 08:56:06.000000 currentscape-1.0.2/Tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/currentscape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/legends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/voltages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/currentscape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/images/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/images/quickstart_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/original_paper_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/LICENSE_CC0-1.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/get_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/single_compartment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/examples/use_case/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/use_case/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/use_case/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/notes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/use_case/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/examples/use_case/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/python_recordings/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/extra/jjb-cells/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 08:56:06.000000 currentscape-1.0.2/extra/jjb-cells/cells.currentscape.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/spack/repos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/spack/repos/builtin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/spack/repos/builtin/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 08:56:06.000000 currentscape-1.0.2/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 08:56:06.000000 currentscape-1.0.2/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:56:14.717142 currentscape-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 08:56:06.000000 currentscape-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/extract_bNAC_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_dataprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_from_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_use_case_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-16 08:56:06.000000 currentscape-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.870851 currentscape-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.858852 currentscape-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 08:59:46.000000 currentscape-1.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 08:59:46.000000 currentscape-1.0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 08:59:46.000000 currentscape-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 08:59:46.000000 currentscape-1.0.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 08:59:46.000000 currentscape-1.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 08:59:46.000000 currentscape-1.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-16 08:59:46.000000 currentscape-1.0.3/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 08:59:46.000000 currentscape-1.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 08:59:46.000000 currentscape-1.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-16 08:59:46.000000 currentscape-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-16 08:59:46.000000 currentscape-1.0.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 08:59:46.000000 currentscape-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 08:59:46.000000 currentscape-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 08:59:46.000000 currentscape-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 08:59:52.870851 currentscape-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-16 08:59:46.000000 currentscape-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-16 08:59:46.000000 currentscape-1.0.3/Tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.858852 currentscape-1.0.3/currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/currentscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/legends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/voltages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/currentscape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/images/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/images/quickstart_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/examples/original_paper_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/LICENSE_CC0-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/get_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/single_compartment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/examples/use_case/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/python_recordings/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/extra/jjb-cells/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 08:59:46.000000 currentscape-1.0.3/extra/jjb-cells/cells.currentscape.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/spack/repos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/spack/repos/builtin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/spack/repos/builtin/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 08:59:46.000000 currentscape-1.0.3/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 08:59:46.000000 currentscape-1.0.3/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:59:52.870851 currentscape-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 08:59:46.000000 currentscape-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.870851 currentscape-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/extract_bNAC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_dataprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_from_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_use_case_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-16 08:59:46.000000 currentscape-1.0.3/tox.ini
```

### Comparing `currentscape-1.0.2/.github/workflows/build.yml` & `currentscape-1.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/.github/workflows/test.yml` & `currentscape-1.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/.pylintrc` & `currentscape-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/.zenodo.json` & `currentscape-1.0.3/.zenodo.json`

 * *Files 0% similar despite different names*

```diff
@@ -75,9 +75,9 @@
 000004a0: 7220 4c61 622c 2044 6570 6172 746d 656e  r Lab, Departmen
 000004b0: 7420 6f66 2042 696f 6c6f 6779 2c20 4272  t of Biology, Br
 000004c0: 616e 6465 6973 2055 6e69 7665 7273 6974  andeis Universit
 000004d0: 7922 2c0a 2020 2020 2020 226e 616d 6522  y",.      "name"
 000004e0: 3a20 224d 6172 6465 722c 2045 7665 222c  : "Marder, Eve",
 000004f0: 0a20 2020 2020 2022 6f72 6369 6422 3a20  .      "orcid": 
 00000500: 2230 3030 302d 3030 3031 2d39 3633 322d  "0000-0001-9632-
-00000510: 3534 3438 220a 2020 2020 7d2c 0a20 2020  5448".    },.   
-00000520: 205d 0a7d 0a                              ].}.
+00000510: 3534 3438 220a 2020 2020 7d0a 2020 5d0a  5448".    }.  ].
+00000520: 7d0a                                     }.
```

### Comparing `currentscape-1.0.2/CHANGELOG.rst` & `currentscape-1.0.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/CONTRIBUTING.md` & `currentscape-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/COPYING` & `currentscape-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/LICENSE.txt` & `currentscape-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/PKG-INFO` & `currentscape-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.2
+Version: 1.0.3
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
```

### Comparing `currentscape-1.0.2/README.rst` & `currentscape-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/Tutorial.rst` & `currentscape-1.0.3/Tutorial.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/__init__.py` & `currentscape-1.0.3/currentscape/__init__.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/config_parser.py` & `currentscape-1.0.3/currentscape/config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/currents.py` & `currentscape-1.0.3/currentscape/currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/currentscape.py` & `currentscape-1.0.3/currentscape/currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/data_processing.py` & `currentscape-1.0.3/currentscape/data_processing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/datasets.py` & `currentscape-1.0.3/currentscape/datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/ions.py` & `currentscape-1.0.3/currentscape/ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/legends.py` & `currentscape-1.0.3/currentscape/legends.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/mapper.py` & `currentscape-1.0.3/currentscape/mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/plotting.py` & `currentscape-1.0.3/currentscape/plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape/voltages.py` & `currentscape-1.0.3/currentscape/voltages.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/currentscape.egg-info/PKG-INFO` & `currentscape-1.0.3/currentscape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.2
+Version: 1.0.3
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
```

### Comparing `currentscape-1.0.2/currentscape.egg-info/SOURCES.txt` & `currentscape-1.0.3/currentscape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/doc/Makefile` & `currentscape-1.0.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/doc/source/conf.py` & `currentscape-1.0.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/doc/source/images/plot.png` & `currentscape-1.0.3/doc/source/images/plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/doc/source/images/quickstart_plot.png` & `currentscape-1.0.3/doc/source/images/quickstart_plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/LICENSE_CC0-1.0` & `currentscape-1.0.3/examples/original_paper_plot/LICENSE_CC0-1.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/config.json` & `currentscape-1.0.3/examples/original_paper_plot/config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/get_currents.py` & `currentscape-1.0.3/examples/original_paper_plot/get_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py` & `currentscape-1.0.3/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt` & `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt` & `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt` & `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt` & `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt` & `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt` & `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt` & `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt` & `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/original_paper_plot/single_compartment.py` & `currentscape-1.0.3/examples/original_paper_plot/single_compartment.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/LICENSE.txt` & `currentscape-1.0.3/examples/use_case/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/LICENSE_CC-BY-CA-SA-4.0` & `currentscape-1.0.3/examples/use_case/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/config/params/final.json` & `currentscape-1.0.3/examples/use_case/config/params/final.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/config/params/pyr.json` & `currentscape-1.0.3/examples/use_case/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/CaDynamics_DC0.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/Ca_HVA2.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/Ca_LVAst.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/Ih.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/K_Pst.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/K_Tst.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/NaTg.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/Nap_Et2.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/SK_E2.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/SKv3_1.mod` & `currentscape-1.0.3/examples/use_case/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/mechanisms/notes.txt` & `currentscape-1.0.3/examples/use_case/mechanisms/notes.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc` & `currentscape-1.0.3/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/plot.py` & `currentscape-1.0.3/examples/use_case/plot.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/run.py` & `currentscape-1.0.3/examples/use_case/run.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/examples/use_case/run_py.sh` & `currentscape-1.0.3/examples/use_case/run_py.sh`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py` & `currentscape-1.0.3/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/requirements_docs.txt` & `currentscape-1.0.3/requirements_docs.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/setup.py` & `currentscape-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/extract_bNAC_config.json` & `currentscape-1.0.3/tests/extract_bNAC_config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_currentscape_config_parser.py` & `currentscape-1.0.3/tests/test_currentscape_config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_currentscape_currents.py` & `currentscape-1.0.3/tests/test_currentscape_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_currentscape_dataprocessing.py` & `currentscape-1.0.3/tests/test_currentscape_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_currentscape_datasets.py` & `currentscape-1.0.3/tests/test_currentscape_datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_currentscape_from_paper.py` & `currentscape-1.0.3/tests/test_currentscape_from_paper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_currentscape_ions.py` & `currentscape-1.0.3/tests/test_currentscape_ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_currentscape_mapper.py` & `currentscape-1.0.3/tests/test_currentscape_mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_currentscape_plotting.py` & `currentscape-1.0.3/tests/test_currentscape_plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tests/test_use_case_example.py` & `currentscape-1.0.3/tests/test_use_case_example.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.2/tox.ini` & `currentscape-1.0.3/tox.ini`

 * *Files identical despite different names*

