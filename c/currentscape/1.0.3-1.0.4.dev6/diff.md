# Comparing `tmp/currentscape-1.0.3.tar.gz` & `tmp/currentscape-1.0.4.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currentscape-1.0.3.tar", last modified: Fri Jun 16 08:59:52 2023, max compression
+gzip compressed data, was "currentscape-1.0.4.dev6.tar", last modified: Fri Jun 16 09:40:32 2023, max compression
```

## Comparing `currentscape-1.0.3.tar` & `currentscape-1.0.4.dev6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.870851 currentscape-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.858852 currentscape-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 08:59:46.000000 currentscape-1.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 08:59:46.000000 currentscape-1.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 08:59:46.000000 currentscape-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 08:59:46.000000 currentscape-1.0.3/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 08:59:46.000000 currentscape-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 08:59:46.000000 currentscape-1.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-16 08:59:46.000000 currentscape-1.0.3/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 08:59:46.000000 currentscape-1.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 08:59:46.000000 currentscape-1.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-16 08:59:46.000000 currentscape-1.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-16 08:59:46.000000 currentscape-1.0.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 08:59:46.000000 currentscape-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 08:59:46.000000 currentscape-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 08:59:46.000000 currentscape-1.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 08:59:52.870851 currentscape-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-16 08:59:46.000000 currentscape-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-16 08:59:46.000000 currentscape-1.0.3/Tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.858852 currentscape-1.0.3/currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/currentscape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/legends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-16 08:59:46.000000 currentscape-1.0.3/currentscape/voltages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/currentscape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 08:59:52.000000 currentscape-1.0.3/currentscape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/images/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/images/quickstart_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 08:59:46.000000 currentscape-1.0.3/doc/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/examples/original_paper_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/LICENSE_CC0-1.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/get_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.862851 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/original_paper_plot/single_compartment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/examples/use_case/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/mechanisms/notes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/examples/use_case/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/python_recordings/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-16 08:59:46.000000 currentscape-1.0.3/examples/use_case/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/extra/jjb-cells/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 08:59:46.000000 currentscape-1.0.3/extra/jjb-cells/cells.currentscape.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/spack/repos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/spack/repos/builtin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.854851 currentscape-1.0.3/extra/spack/var/spack/repos/builtin/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.866851 currentscape-1.0.3/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 08:59:46.000000 currentscape-1.0.3/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 08:59:46.000000 currentscape-1.0.3/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:59:52.870851 currentscape-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 08:59:46.000000 currentscape-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:52.870851 currentscape-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/extract_bNAC_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_dataprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_from_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_currentscape_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/test_use_case_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 08:59:46.000000 currentscape-1.0.3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-16 08:59:46.000000 currentscape-1.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.975145 currentscape-1.0.4.dev6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.963145 currentscape-1.0.4.dev6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-16 09:40:32.971145 currentscape-1.0.4.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/Tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.963145 currentscape-1.0.4.dev6/currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/currentscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/legends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/currentscape/voltages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.963145 currentscape-1.0.4.dev6/currentscape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-16 09:40:32.000000 currentscape-1.0.4.dev6/currentscape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-16 09:40:32.000000 currentscape-1.0.4.dev6/currentscape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:40:32.000000 currentscape-1.0.4.dev6/currentscape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 09:40:32.000000 currentscape-1.0.4.dev6/currentscape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 09:40:32.000000 currentscape-1.0.4.dev6/currentscape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.963145 currentscape-1.0.4.dev6/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.963145 currentscape-1.0.4.dev6/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.963145 currentscape-1.0.4.dev6/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/doc/source/images/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/doc/source/images/quickstart_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/doc/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.967145 currentscape-1.0.4.dev6/examples/original_paper_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/LICENSE_CC0-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/get_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.967145 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/original_paper_plot/single_compartment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.967145 currentscape-1.0.4.dev6/examples/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/examples/use_case/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.967145 currentscape-1.0.4.dev6/examples/use_case/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.971145 currentscape-1.0.4.dev6/examples/use_case/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.971145 currentscape-1.0.4.dev6/examples/use_case/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.971145 currentscape-1.0.4.dev6/examples/use_case/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/python_recordings/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/examples/use_case/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.971145 currentscape-1.0.4.dev6/extra/jjb-cells/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/extra/jjb-cells/cells.currentscape.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/extra/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/extra/spack/var/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/extra/spack/var/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/extra/spack/var/spack/repos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/extra/spack/var/spack/repos/builtin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.959145 currentscape-1.0.4.dev6/extra/spack/var/spack/repos/builtin/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.971145 currentscape-1.0.4.dev6/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:40:32.975145 currentscape-1.0.4.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:32.971145 currentscape-1.0.4.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/extract_bNAC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_currentscape_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_currentscape_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_currentscape_dataprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_currentscape_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_currentscape_from_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_currentscape_ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_currentscape_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_currentscape_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/test_use_case_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-16 09:40:26.000000 currentscape-1.0.4.dev6/tox.ini
```

### Comparing `currentscape-1.0.3/.github/workflows/build.yml` & `currentscape-1.0.4.dev6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/.github/workflows/test.yml` & `currentscape-1.0.4.dev6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/.pylintrc` & `currentscape-1.0.4.dev6/.pylintrc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/.zenodo.json` & `currentscape-1.0.4.dev6/.zenodo.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/CHANGELOG.rst` & `currentscape-1.0.4.dev6/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/CONTRIBUTING.md` & `currentscape-1.0.4.dev6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/COPYING` & `currentscape-1.0.4.dev6/COPYING`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/LICENSE.txt` & `currentscape-1.0.4.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/PKG-INFO` & `currentscape-1.0.4.dev6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.3
+Version: 1.0.4.dev6
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
@@ -38,14 +38,16 @@
 +----------------+------------+
 | Build Status 	 | |build|    |
 +----------------+------------+
 | Coverage       | |coverage| |
 +----------------+------------+
 | Gitter         | |gitter|   |
 +----------------+------------+
+| Citation       | |zenodo|   |
++----------------+------------+
 
 Introduction
 ============
 
 Currentscape is a Python tool enabling scientists to easily plot the currents in electrical neuron models.
 The code is based on the paper `Alonso and Marder, 2019 <https://doi.org/10.7554/eLife.42722>`__.
 
@@ -54,15 +56,15 @@
 It allows modellers to see which currents play a role at any given time during a simulation, and check in depth the current dynamics.
 
 .. image:: doc/source/images/plot.png
 
 Citation
 ========
 
-When you use this Currentscape software for your research, we ask you to cite the following publication (this includes poster presentations):
+When you use this Currentscape software for your research, we ask you to cite the following publications (this includes poster presentations):
 
 .. code-block:: 
 
     @article {10.7554/eLife.42722,
         article_type = {journal},
         title = {Visualization of currents in neural models with similar behavior and different conductance densities},
         author = {Alonso, Leandro M and Marder, Eve},
@@ -77,14 +79,24 @@
         url = {https://doi.org/10.7554/eLife.42722},
         abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
         keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
         journal = {eLife},
         issn = {2050-084X},
         publisher = {eLife Sciences Publications, Ltd},
     }
+    
+    @article{currentscape, 
+        title={Currentscape}, 
+        DOI={10.5281/zenodo.8046484}, 
+        abstractNote={Currentscape is a Python tool enabling scientists to easily plot the currents in electrical neuron models. The code is based on the paper Alonso and Marder, 2019. Currentscape figures plot the percentage of inward and outward ionic membrane currents, the total inward and outward currents, as well as the voltage in function of time. It allows modellers to see which currents play a role at any given time during a simulation, and check in depth the current dynamics.}, 
+        publisher={Zenodo}, 
+        author={Jaquier, Aurélien and Tuncel, Anil and Van Geit, Werner and Alonso, Leandro M and Marder, Eve}, 
+        year={2023}, 
+        month={Jun} 
+    }
 
 Support
 =======
 
 We are providing support on `Gitter <https://gitter.im/BlueBrain/Currentscape>`_. We suggest you create tickets on the `Github issue tracker <https://github.com/BlueBrain/Currentscape/issues>`_ in case you encounter problems while using the software or if you have some suggestions.
 
 Main dependencies
@@ -243,7 +255,10 @@
 .. |coverage| image:: https://codecov.io/github/BlueBrain/Currentscape/coverage.svg?branch=main
                    :target: https://codecov.io/gh/BlueBrain/currentscape
                    :alt: coverage
 
 .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
                  :target: https://gitter.im/BlueBrain/Currentscape
                  :alt: Join the chat at https://gitter.im/BlueBrain/Currentscape
+
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8046484.svg
+                :target: https://doi.org/10.5281/zenodo.8046484
```

### Comparing `currentscape-1.0.3/README.rst` & `currentscape-1.0.4.dev6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 +----------------+------------+
 | Build Status 	 | |build|    |
 +----------------+------------+
 | Coverage       | |coverage| |
 +----------------+------------+
 | Gitter         | |gitter|   |
 +----------------+------------+
+| Citation       | |zenodo|   |
++----------------+------------+
 
 Introduction
 ============
 
 Currentscape is a Python tool enabling scientists to easily plot the currents in electrical neuron models.
 The code is based on the paper `Alonso and Marder, 2019 <https://doi.org/10.7554/eLife.42722>`__.
 
@@ -27,15 +29,15 @@
 It allows modellers to see which currents play a role at any given time during a simulation, and check in depth the current dynamics.
 
 .. image:: doc/source/images/plot.png
 
 Citation
 ========
 
-When you use this Currentscape software for your research, we ask you to cite the following publication (this includes poster presentations):
+When you use this Currentscape software for your research, we ask you to cite the following publications (this includes poster presentations):
 
 .. code-block:: 
 
     @article {10.7554/eLife.42722,
         article_type = {journal},
         title = {Visualization of currents in neural models with similar behavior and different conductance densities},
         author = {Alonso, Leandro M and Marder, Eve},
@@ -50,14 +52,24 @@
         url = {https://doi.org/10.7554/eLife.42722},
         abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
         keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
         journal = {eLife},
         issn = {2050-084X},
         publisher = {eLife Sciences Publications, Ltd},
     }
+    
+    @article{currentscape, 
+        title={Currentscape}, 
+        DOI={10.5281/zenodo.8046484}, 
+        abstractNote={Currentscape is a Python tool enabling scientists to easily plot the currents in electrical neuron models. The code is based on the paper Alonso and Marder, 2019. Currentscape figures plot the percentage of inward and outward ionic membrane currents, the total inward and outward currents, as well as the voltage in function of time. It allows modellers to see which currents play a role at any given time during a simulation, and check in depth the current dynamics.}, 
+        publisher={Zenodo}, 
+        author={Jaquier, Aurélien and Tuncel, Anil and Van Geit, Werner and Alonso, Leandro M and Marder, Eve}, 
+        year={2023}, 
+        month={Jun} 
+    }
 
 Support
 =======
 
 We are providing support on `Gitter <https://gitter.im/BlueBrain/Currentscape>`_. We suggest you create tickets on the `Github issue tracker <https://github.com/BlueBrain/Currentscape/issues>`_ in case you encounter problems while using the software or if you have some suggestions.
 
 Main dependencies
@@ -216,7 +228,10 @@
 .. |coverage| image:: https://codecov.io/github/BlueBrain/Currentscape/coverage.svg?branch=main
                    :target: https://codecov.io/gh/BlueBrain/currentscape
                    :alt: coverage
 
 .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
                  :target: https://gitter.im/BlueBrain/Currentscape
                  :alt: Join the chat at https://gitter.im/BlueBrain/Currentscape
+
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8046484.svg
+                :target: https://doi.org/10.5281/zenodo.8046484
```

### Comparing `currentscape-1.0.3/Tutorial.rst` & `currentscape-1.0.4.dev6/Tutorial.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/__init__.py` & `currentscape-1.0.4.dev6/currentscape/__init__.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/config_parser.py` & `currentscape-1.0.4.dev6/currentscape/config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/currents.py` & `currentscape-1.0.4.dev6/currentscape/currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/currentscape.py` & `currentscape-1.0.4.dev6/currentscape/currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/data_processing.py` & `currentscape-1.0.4.dev6/currentscape/data_processing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/datasets.py` & `currentscape-1.0.4.dev6/currentscape/datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/ions.py` & `currentscape-1.0.4.dev6/currentscape/ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/legends.py` & `currentscape-1.0.4.dev6/currentscape/legends.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/mapper.py` & `currentscape-1.0.4.dev6/currentscape/mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/plotting.py` & `currentscape-1.0.4.dev6/currentscape/plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape/voltages.py` & `currentscape-1.0.4.dev6/currentscape/voltages.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/currentscape.egg-info/PKG-INFO` & `currentscape-1.0.4.dev6/currentscape.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.3
+Version: 1.0.4.dev6
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
@@ -38,14 +38,16 @@
 +----------------+------------+
 | Build Status 	 | |build|    |
 +----------------+------------+
 | Coverage       | |coverage| |
 +----------------+------------+
 | Gitter         | |gitter|   |
 +----------------+------------+
+| Citation       | |zenodo|   |
++----------------+------------+
 
 Introduction
 ============
 
 Currentscape is a Python tool enabling scientists to easily plot the currents in electrical neuron models.
 The code is based on the paper `Alonso and Marder, 2019 <https://doi.org/10.7554/eLife.42722>`__.
 
@@ -54,15 +56,15 @@
 It allows modellers to see which currents play a role at any given time during a simulation, and check in depth the current dynamics.
 
 .. image:: doc/source/images/plot.png
 
 Citation
 ========
 
-When you use this Currentscape software for your research, we ask you to cite the following publication (this includes poster presentations):
+When you use this Currentscape software for your research, we ask you to cite the following publications (this includes poster presentations):
 
 .. code-block:: 
 
     @article {10.7554/eLife.42722,
         article_type = {journal},
         title = {Visualization of currents in neural models with similar behavior and different conductance densities},
         author = {Alonso, Leandro M and Marder, Eve},
@@ -77,14 +79,24 @@
         url = {https://doi.org/10.7554/eLife.42722},
         abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
         keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
         journal = {eLife},
         issn = {2050-084X},
         publisher = {eLife Sciences Publications, Ltd},
     }
+    
+    @article{currentscape, 
+        title={Currentscape}, 
+        DOI={10.5281/zenodo.8046484}, 
+        abstractNote={Currentscape is a Python tool enabling scientists to easily plot the currents in electrical neuron models. The code is based on the paper Alonso and Marder, 2019. Currentscape figures plot the percentage of inward and outward ionic membrane currents, the total inward and outward currents, as well as the voltage in function of time. It allows modellers to see which currents play a role at any given time during a simulation, and check in depth the current dynamics.}, 
+        publisher={Zenodo}, 
+        author={Jaquier, Aurélien and Tuncel, Anil and Van Geit, Werner and Alonso, Leandro M and Marder, Eve}, 
+        year={2023}, 
+        month={Jun} 
+    }
 
 Support
 =======
 
 We are providing support on `Gitter <https://gitter.im/BlueBrain/Currentscape>`_. We suggest you create tickets on the `Github issue tracker <https://github.com/BlueBrain/Currentscape/issues>`_ in case you encounter problems while using the software or if you have some suggestions.
 
 Main dependencies
@@ -243,7 +255,10 @@
 .. |coverage| image:: https://codecov.io/github/BlueBrain/Currentscape/coverage.svg?branch=main
                    :target: https://codecov.io/gh/BlueBrain/currentscape
                    :alt: coverage
 
 .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
                  :target: https://gitter.im/BlueBrain/Currentscape
                  :alt: Join the chat at https://gitter.im/BlueBrain/Currentscape
+
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8046484.svg
+                :target: https://doi.org/10.5281/zenodo.8046484
```

### Comparing `currentscape-1.0.3/currentscape.egg-info/SOURCES.txt` & `currentscape-1.0.4.dev6/currentscape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/doc/Makefile` & `currentscape-1.0.4.dev6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/doc/source/conf.py` & `currentscape-1.0.4.dev6/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/doc/source/images/plot.png` & `currentscape-1.0.4.dev6/doc/source/images/plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/doc/source/images/quickstart_plot.png` & `currentscape-1.0.4.dev6/doc/source/images/quickstart_plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/LICENSE_CC0-1.0` & `currentscape-1.0.4.dev6/examples/original_paper_plot/LICENSE_CC0-1.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/config.json` & `currentscape-1.0.4.dev6/examples/original_paper_plot/config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/get_currents.py` & `currentscape-1.0.4.dev6/examples/original_paper_plot/get_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py` & `currentscape-1.0.4.dev6/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt` & `currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt` & `currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt` & `currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt` & `currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt` & `currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt` & `currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt` & `currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt` & `currentscape-1.0.4.dev6/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/original_paper_plot/single_compartment.py` & `currentscape-1.0.4.dev6/examples/original_paper_plot/single_compartment.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/LICENSE.txt` & `currentscape-1.0.4.dev6/examples/use_case/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/LICENSE_CC-BY-CA-SA-4.0` & `currentscape-1.0.4.dev6/examples/use_case/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/config/params/final.json` & `currentscape-1.0.4.dev6/examples/use_case/config/params/final.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/config/params/pyr.json` & `currentscape-1.0.4.dev6/examples/use_case/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/CaDynamics_DC0.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/Ca_HVA2.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/Ca_LVAst.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/Ih.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/K_Pst.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/K_Tst.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/NaTg.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/Nap_Et2.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/SK_E2.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/SKv3_1.mod` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/mechanisms/notes.txt` & `currentscape-1.0.4.dev6/examples/use_case/mechanisms/notes.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc` & `currentscape-1.0.4.dev6/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/plot.py` & `currentscape-1.0.4.dev6/examples/use_case/plot.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/run.py` & `currentscape-1.0.4.dev6/examples/use_case/run.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/examples/use_case/run_py.sh` & `currentscape-1.0.4.dev6/examples/use_case/run_py.sh`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py` & `currentscape-1.0.4.dev6/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/requirements_docs.txt` & `currentscape-1.0.4.dev6/requirements_docs.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/setup.py` & `currentscape-1.0.4.dev6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,18 @@
     README = f.read()
 
 EXTRA_EXAMPLE = ["scipy", "bluepyopt", "emodelrunner>=1.1.5"]
 
 setup(
     name="currentscape",
     author="Blue Brain Project, EPFL",
-    use_scm_version=True,
+    use_scm_version={
+        "version_scheme": "python-simplified-semver",
+        "local_scheme": "no-local-version",
+    },
     setup_requires=["setuptools_scm"],
     description="Module to easily plot currentscape.",
     long_description=README,
     long_description_content_type="text/x-rst",
     url="https://github.com/BlueBrain/Currentscape",
     project_urls={
         "Tracker": "https://github.com/BlueBrain/Currentscape",
```

### Comparing `currentscape-1.0.3/tests/extract_bNAC_config.json` & `currentscape-1.0.4.dev6/tests/extract_bNAC_config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_currentscape_config_parser.py` & `currentscape-1.0.4.dev6/tests/test_currentscape_config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_currentscape_currents.py` & `currentscape-1.0.4.dev6/tests/test_currentscape_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_currentscape_dataprocessing.py` & `currentscape-1.0.4.dev6/tests/test_currentscape_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_currentscape_datasets.py` & `currentscape-1.0.4.dev6/tests/test_currentscape_datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_currentscape_from_paper.py` & `currentscape-1.0.4.dev6/tests/test_currentscape_from_paper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_currentscape_ions.py` & `currentscape-1.0.4.dev6/tests/test_currentscape_ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_currentscape_mapper.py` & `currentscape-1.0.4.dev6/tests/test_currentscape_mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_currentscape_plotting.py` & `currentscape-1.0.4.dev6/tests/test_currentscape_plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tests/test_use_case_example.py` & `currentscape-1.0.4.dev6/tests/test_use_case_example.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.3/tox.ini` & `currentscape-1.0.4.dev6/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -61,17 +61,17 @@
     pydocstyle
     pylint
     black
 commands =
     pycodestyle {[base]name}
     pydocstyle {[base]name}
     pylint {[base]name}
-    black --check {[base]name}
-    black --check tests
-    black --check setup.py
+    black --diff --check {[base]name}
+    black --diff --check tests
+    black --diff --check setup.py
 
 [testenv:format]
 deps = black
 commands =
     black {[base]name}
     black tests
     black setup.py
```

