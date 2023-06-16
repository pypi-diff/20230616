# Comparing `tmp/currentscape-1.0.1.tar.gz` & `tmp/currentscape-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currentscape-1.0.1.tar", last modified: Wed Jun 14 15:26:21 2023, max compression
+gzip compressed data, was "currentscape-1.0.2.tar", last modified: Fri Jun 16 08:56:14 2023, max compression
```

## Comparing `currentscape-1.0.1.tar` & `currentscape-1.0.2.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.796502 currentscape-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.780502 currentscape-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-14 15:26:14.000000 currentscape-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-14 15:26:14.000000 currentscape-1.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 15:26:14.000000 currentscape-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-14 15:26:14.000000 currentscape-1.0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-14 15:26:14.000000 currentscape-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-14 15:26:14.000000 currentscape-1.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 15:26:14.000000 currentscape-1.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-14 15:26:14.000000 currentscape-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-14 15:26:14.000000 currentscape-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-14 15:26:14.000000 currentscape-1.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-14 15:26:14.000000 currentscape-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 15:26:14.000000 currentscape-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 15:26:14.000000 currentscape-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-14 15:26:21.796502 currentscape-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-06-14 15:26:14.000000 currentscape-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-14 15:26:14.000000 currentscape-1.0.1/Tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.780502 currentscape-1.0.1/currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/currentscape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/legends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/voltages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.780502 currentscape-1.0.1/currentscape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.784502 currentscape-1.0.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.784502 currentscape-1.0.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.784502 currentscape-1.0.1/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/images/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/images/quickstart_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.784502 currentscape-1.0.1/examples/original_paper_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/LICENSE_CC0-1.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/get_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.788502 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/single_compartment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.788502 currentscape-1.0.1/examples/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/examples/use_case/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.788502 currentscape-1.0.1/examples/use_case/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/examples/use_case/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/notes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/examples/use_case/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/examples/use_case/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/python_recordings/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/extra/jjb-cells/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 15:26:14.000000 currentscape-1.0.1/extra/jjb-cells/cells.currentscape.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/spack/repos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/spack/repos/builtin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/spack/repos/builtin/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-14 15:26:14.000000 currentscape-1.0.1/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 15:26:14.000000 currentscape-1.0.1/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:26:21.796502 currentscape-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-14 15:26:14.000000 currentscape-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.796502 currentscape-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/extract_bNAC_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_dataprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_from_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_use_case_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-14 15:26:14.000000 currentscape-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 08:56:06.000000 currentscape-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 08:56:06.000000 currentscape-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 08:56:06.000000 currentscape-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 08:56:06.000000 currentscape-1.0.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 08:56:06.000000 currentscape-1.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 08:56:06.000000 currentscape-1.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-16 08:56:06.000000 currentscape-1.0.2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 08:56:06.000000 currentscape-1.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 08:56:06.000000 currentscape-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-16 08:56:06.000000 currentscape-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-16 08:56:06.000000 currentscape-1.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 08:56:06.000000 currentscape-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 08:56:06.000000 currentscape-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 08:56:06.000000 currentscape-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 08:56:14.717142 currentscape-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-16 08:56:06.000000 currentscape-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-16 08:56:06.000000 currentscape-1.0.2/Tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/currentscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/legends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-16 08:56:06.000000 currentscape-1.0.2/currentscape/voltages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/currentscape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 08:56:14.000000 currentscape-1.0.2/currentscape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.709142 currentscape-1.0.2/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/images/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/images/quickstart_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 08:56:06.000000 currentscape-1.0.2/doc/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/original_paper_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/LICENSE_CC0-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/get_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/original_paper_plot/single_compartment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/examples/use_case/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/use_case/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/use_case/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.713142 currentscape-1.0.2/examples/use_case/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/examples/use_case/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/python_recordings/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-16 08:56:06.000000 currentscape-1.0.2/examples/use_case/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/extra/jjb-cells/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 08:56:06.000000 currentscape-1.0.2/extra/jjb-cells/cells.currentscape.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/spack/repos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/spack/repos/builtin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.705142 currentscape-1.0.2/extra/spack/var/spack/repos/builtin/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 08:56:06.000000 currentscape-1.0.2/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 08:56:06.000000 currentscape-1.0.2/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:56:14.717142 currentscape-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 08:56:06.000000 currentscape-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:14.717142 currentscape-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/extract_bNAC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_dataprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_from_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_currentscape_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/test_use_case_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 08:56:06.000000 currentscape-1.0.2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-16 08:56:06.000000 currentscape-1.0.2/tox.ini
```

### Comparing `currentscape-1.0.1/.github/workflows/build.yml` & `currentscape-1.0.2/.github/workflows/build.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 name: Build
 
 on:
   push:
+    branches:
+      - main
     tags:
       - '[0-9]+.[0-9]+.[0-9]+'
 
 jobs:
   call-test-workflow:
     uses: BlueBrain/Currentscape/.github/workflows/test.yml@main
```

### Comparing `currentscape-1.0.1/.github/workflows/test.yml` & `currentscape-1.0.2/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 name: Test
 
 on:
-  push:
-    branches:
-      - main
   pull_request:
   # allows this workflow to be reusable (e.g. by the build workflow)
   workflow_call:
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `currentscape-1.0.1/.pylintrc` & `currentscape-1.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/CHANGELOG.rst` & `currentscape-1.0.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/CONTRIBUTING.md` & `currentscape-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/COPYING` & `currentscape-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/LICENSE.txt` & `currentscape-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/PKG-INFO` & `currentscape-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.1
+Version: 1.0.2
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: example
 License-File: LICENSE.txt
 License-File: COPYING
 License-File: AUTHORS.rst
 
@@ -60,42 +59,42 @@
 ========
 
 When you use this Currentscape software for your research, we ask you to cite the following publication (this includes poster presentations):
 
 .. code-block:: 
 
     @article {10.7554/eLife.42722,
-    article_type = {journal},
-    title = {Visualization of currents in neural models with similar behavior and different conductance densities},
-    author = {Alonso, Leandro M and Marder, Eve},
-    editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
-    volume = 8,
-    year = 2019,
-    month = {jan},
-    pub_date = {2019-01-31},
-    pages = {e42722},
-    citation = {eLife 2019;8:e42722},
-    doi = {10.7554/eLife.42722},
-    url = {https://doi.org/10.7554/eLife.42722},
-    abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
-    keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
-    journal = {eLife},
-    issn = {2050-084X},
-    publisher = {eLife Sciences Publications, Ltd},
+        article_type = {journal},
+        title = {Visualization of currents in neural models with similar behavior and different conductance densities},
+        author = {Alonso, Leandro M and Marder, Eve},
+        editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
+        volume = 8,
+        year = 2019,
+        month = {jan},
+        pub_date = {2019-01-31},
+        pages = {e42722},
+        citation = {eLife 2019;8:e42722},
+        doi = {10.7554/eLife.42722},
+        url = {https://doi.org/10.7554/eLife.42722},
+        abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
+        keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
+        journal = {eLife},
+        issn = {2050-084X},
+        publisher = {eLife Sciences Publications, Ltd},
     }
 
 Support
 =======
 
 We are providing support on `Gitter <https://gitter.im/BlueBrain/Currentscape>`_. We suggest you create tickets on the `Github issue tracker <https://github.com/BlueBrain/Currentscape/issues>`_ in case you encounter problems while using the software or if you have some suggestions.
 
 Main dependencies
 =================
 
-- `Python 3.7+ <https://www.python.org/downloads/release/python-370/>`_
+- `Python 3.8+ <https://www.python.org/downloads/release/python-380/>`_
 - `Numpy <https://numpy.org/>`_ (automatically installed by pip)
 - `Palettable <https://github.com/jiffyclub/palettable>`_ (automatically installed by pip)
 
 Installation
 ============
 
 Currentscape can be pip installed with the following command:
@@ -211,26 +210,26 @@
 ========
 
 A more detailed explanation on how to use Currentscape, as well as other examples can be found on the `tutorial page <Tutorial.rst>`_.
 
 API Documentation
 =================
 
-The API documentation can be found on `ReadTheDocs <"https://currentscape.readthedocs.io">`_.
+The API documentation can be found on `ReadTheDocs <https://currentscape.readthedocs.io>`_.
 
 Funding & Acknowledgements
 ==========================
 
 We wish to thank the authors of `Alonso and Marder, 2019 <https://doi.org/10.7554/eLife.42722>`__ to let us integrate a part of their `code <https://datadryad.org/stash/dataset/doi:10.5061/dryad.d0779mb>`_ into this repository.
 
 The part of the code in this repository developed by the EPFL Blue Brain Project was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government's ETH Board of the Swiss Federal Institutes of Technology.
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/currentscape.svg
-               :target: https://test.pypi.org/project/currentscape/
+               :target: https://pypi.org/project/currentscape/
                :alt: latest release
 
 .. |docs| image:: https://readthedocs.org/projects/currentscape/badge/?version=latest
                :target: https://currentscape.readthedocs.io/
                :alt: latest documentation
 
 .. |license| image:: https://img.shields.io/pypi/l/currentscape.svg
@@ -242,9 +241,9 @@
                 :alt: actions build status
 
 .. |coverage| image:: https://codecov.io/github/BlueBrain/Currentscape/coverage.svg?branch=main
                    :target: https://codecov.io/gh/BlueBrain/currentscape
                    :alt: coverage
 
 .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
-                 :target: https://gitter.im/bluebrain/currentscape
-                 :alt: Join the chat at https://gitter.im/bluebrain/currentscape
+                 :target: https://gitter.im/BlueBrain/Currentscape
+                 :alt: Join the chat at https://gitter.im/BlueBrain/Currentscape
```

### Comparing `currentscape-1.0.1/README.rst` & `currentscape-1.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,42 +32,42 @@
 ========
 
 When you use this Currentscape software for your research, we ask you to cite the following publication (this includes poster presentations):
 
 .. code-block:: 
 
     @article {10.7554/eLife.42722,
-    article_type = {journal},
-    title = {Visualization of currents in neural models with similar behavior and different conductance densities},
-    author = {Alonso, Leandro M and Marder, Eve},
-    editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
-    volume = 8,
-    year = 2019,
-    month = {jan},
-    pub_date = {2019-01-31},
-    pages = {e42722},
-    citation = {eLife 2019;8:e42722},
-    doi = {10.7554/eLife.42722},
-    url = {https://doi.org/10.7554/eLife.42722},
-    abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
-    keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
-    journal = {eLife},
-    issn = {2050-084X},
-    publisher = {eLife Sciences Publications, Ltd},
+        article_type = {journal},
+        title = {Visualization of currents in neural models with similar behavior and different conductance densities},
+        author = {Alonso, Leandro M and Marder, Eve},
+        editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
+        volume = 8,
+        year = 2019,
+        month = {jan},
+        pub_date = {2019-01-31},
+        pages = {e42722},
+        citation = {eLife 2019;8:e42722},
+        doi = {10.7554/eLife.42722},
+        url = {https://doi.org/10.7554/eLife.42722},
+        abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
+        keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
+        journal = {eLife},
+        issn = {2050-084X},
+        publisher = {eLife Sciences Publications, Ltd},
     }
 
 Support
 =======
 
 We are providing support on `Gitter <https://gitter.im/BlueBrain/Currentscape>`_. We suggest you create tickets on the `Github issue tracker <https://github.com/BlueBrain/Currentscape/issues>`_ in case you encounter problems while using the software or if you have some suggestions.
 
 Main dependencies
 =================
 
-- `Python 3.7+ <https://www.python.org/downloads/release/python-370/>`_
+- `Python 3.8+ <https://www.python.org/downloads/release/python-380/>`_
 - `Numpy <https://numpy.org/>`_ (automatically installed by pip)
 - `Palettable <https://github.com/jiffyclub/palettable>`_ (automatically installed by pip)
 
 Installation
 ============
 
 Currentscape can be pip installed with the following command:
@@ -183,26 +183,26 @@
 ========
 
 A more detailed explanation on how to use Currentscape, as well as other examples can be found on the `tutorial page <Tutorial.rst>`_.
 
 API Documentation
 =================
 
-The API documentation can be found on `ReadTheDocs <"https://currentscape.readthedocs.io">`_.
+The API documentation can be found on `ReadTheDocs <https://currentscape.readthedocs.io>`_.
 
 Funding & Acknowledgements
 ==========================
 
 We wish to thank the authors of `Alonso and Marder, 2019 <https://doi.org/10.7554/eLife.42722>`__ to let us integrate a part of their `code <https://datadryad.org/stash/dataset/doi:10.5061/dryad.d0779mb>`_ into this repository.
 
 The part of the code in this repository developed by the EPFL Blue Brain Project was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government's ETH Board of the Swiss Federal Institutes of Technology.
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/currentscape.svg
-               :target: https://test.pypi.org/project/currentscape/
+               :target: https://pypi.org/project/currentscape/
                :alt: latest release
 
 .. |docs| image:: https://readthedocs.org/projects/currentscape/badge/?version=latest
                :target: https://currentscape.readthedocs.io/
                :alt: latest documentation
 
 .. |license| image:: https://img.shields.io/pypi/l/currentscape.svg
@@ -214,9 +214,9 @@
                 :alt: actions build status
 
 .. |coverage| image:: https://codecov.io/github/BlueBrain/Currentscape/coverage.svg?branch=main
                    :target: https://codecov.io/gh/BlueBrain/currentscape
                    :alt: coverage
 
 .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
-                 :target: https://gitter.im/bluebrain/currentscape
-                 :alt: Join the chat at https://gitter.im/bluebrain/currentscape
+                 :target: https://gitter.im/BlueBrain/Currentscape
+                 :alt: Join the chat at https://gitter.im/BlueBrain/Currentscape
```

### Comparing `currentscape-1.0.1/Tutorial.rst` & `currentscape-1.0.2/Tutorial.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/__init__.py` & `currentscape-1.0.2/currentscape/__init__.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/config_parser.py` & `currentscape-1.0.2/currentscape/config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/currents.py` & `currentscape-1.0.2/currentscape/currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/currentscape.py` & `currentscape-1.0.2/currentscape/currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/data_processing.py` & `currentscape-1.0.2/currentscape/data_processing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/datasets.py` & `currentscape-1.0.2/currentscape/datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/ions.py` & `currentscape-1.0.2/currentscape/ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/legends.py` & `currentscape-1.0.2/currentscape/legends.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/mapper.py` & `currentscape-1.0.2/currentscape/mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/plotting.py` & `currentscape-1.0.2/currentscape/plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape/voltages.py` & `currentscape-1.0.2/currentscape/voltages.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/currentscape.egg-info/PKG-INFO` & `currentscape-1.0.2/currentscape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.1
+Version: 1.0.2
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: example
 License-File: LICENSE.txt
 License-File: COPYING
 License-File: AUTHORS.rst
 
@@ -60,42 +59,42 @@
 ========
 
 When you use this Currentscape software for your research, we ask you to cite the following publication (this includes poster presentations):
 
 .. code-block:: 
 
     @article {10.7554/eLife.42722,
-    article_type = {journal},
-    title = {Visualization of currents in neural models with similar behavior and different conductance densities},
-    author = {Alonso, Leandro M and Marder, Eve},
-    editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
-    volume = 8,
-    year = 2019,
-    month = {jan},
-    pub_date = {2019-01-31},
-    pages = {e42722},
-    citation = {eLife 2019;8:e42722},
-    doi = {10.7554/eLife.42722},
-    url = {https://doi.org/10.7554/eLife.42722},
-    abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
-    keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
-    journal = {eLife},
-    issn = {2050-084X},
-    publisher = {eLife Sciences Publications, Ltd},
+        article_type = {journal},
+        title = {Visualization of currents in neural models with similar behavior and different conductance densities},
+        author = {Alonso, Leandro M and Marder, Eve},
+        editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
+        volume = 8,
+        year = 2019,
+        month = {jan},
+        pub_date = {2019-01-31},
+        pages = {e42722},
+        citation = {eLife 2019;8:e42722},
+        doi = {10.7554/eLife.42722},
+        url = {https://doi.org/10.7554/eLife.42722},
+        abstract = {Conductance-based models of neural activity produce large amounts of data that can be hard to visualize and interpret. We introduce visualization methods to display the dynamics of the ionic currents and to display the models’ response to perturbations. To visualize the currents’ dynamics, we compute the percent contribution of each current and display them over time using stacked-area plots. The waveform of the membrane potential and the contribution of each current change as the models are perturbed. To represent these changes over a range of the perturbation control parameter, we compute and display the distributions of these waveforms. We illustrate these procedures in six examples of bursting model neurons with similar activity but that differ as much as threefold in their conductance densities. These visualization methods provide heuristic insight into why individual neurons or networks with similar behavior can respond widely differently to perturbations.},
+        keywords = {neuronal oscillators, Na+ channels, Ca++ channels, K+ channels, conductance-based, ionic channels},
+        journal = {eLife},
+        issn = {2050-084X},
+        publisher = {eLife Sciences Publications, Ltd},
     }
 
 Support
 =======
 
 We are providing support on `Gitter <https://gitter.im/BlueBrain/Currentscape>`_. We suggest you create tickets on the `Github issue tracker <https://github.com/BlueBrain/Currentscape/issues>`_ in case you encounter problems while using the software or if you have some suggestions.
 
 Main dependencies
 =================
 
-- `Python 3.7+ <https://www.python.org/downloads/release/python-370/>`_
+- `Python 3.8+ <https://www.python.org/downloads/release/python-380/>`_
 - `Numpy <https://numpy.org/>`_ (automatically installed by pip)
 - `Palettable <https://github.com/jiffyclub/palettable>`_ (automatically installed by pip)
 
 Installation
 ============
 
 Currentscape can be pip installed with the following command:
@@ -211,26 +210,26 @@
 ========
 
 A more detailed explanation on how to use Currentscape, as well as other examples can be found on the `tutorial page <Tutorial.rst>`_.
 
 API Documentation
 =================
 
-The API documentation can be found on `ReadTheDocs <"https://currentscape.readthedocs.io">`_.
+The API documentation can be found on `ReadTheDocs <https://currentscape.readthedocs.io>`_.
 
 Funding & Acknowledgements
 ==========================
 
 We wish to thank the authors of `Alonso and Marder, 2019 <https://doi.org/10.7554/eLife.42722>`__ to let us integrate a part of their `code <https://datadryad.org/stash/dataset/doi:10.5061/dryad.d0779mb>`_ into this repository.
 
 The part of the code in this repository developed by the EPFL Blue Brain Project was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government's ETH Board of the Swiss Federal Institutes of Technology.
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/currentscape.svg
-               :target: https://test.pypi.org/project/currentscape/
+               :target: https://pypi.org/project/currentscape/
                :alt: latest release
 
 .. |docs| image:: https://readthedocs.org/projects/currentscape/badge/?version=latest
                :target: https://currentscape.readthedocs.io/
                :alt: latest documentation
 
 .. |license| image:: https://img.shields.io/pypi/l/currentscape.svg
@@ -242,9 +241,9 @@
                 :alt: actions build status
 
 .. |coverage| image:: https://codecov.io/github/BlueBrain/Currentscape/coverage.svg?branch=main
                    :target: https://codecov.io/gh/BlueBrain/currentscape
                    :alt: coverage
 
 .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
-                 :target: https://gitter.im/bluebrain/currentscape
-                 :alt: Join the chat at https://gitter.im/bluebrain/currentscape
+                 :target: https://gitter.im/BlueBrain/Currentscape
+                 :alt: Join the chat at https://gitter.im/BlueBrain/Currentscape
```

### Comparing `currentscape-1.0.1/currentscape.egg-info/SOURCES.txt` & `currentscape-1.0.2/currentscape.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .gitlab-ci.yml
 .pylintrc
 .readthedocs.yml
+.zenodo.json
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.md
 COPYING
 LICENSE.txt
 MANIFEST.in
 Makefile
```

### Comparing `currentscape-1.0.1/doc/Makefile` & `currentscape-1.0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/doc/source/conf.py` & `currentscape-1.0.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/doc/source/images/plot.png` & `currentscape-1.0.2/doc/source/images/plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/doc/source/images/quickstart_plot.png` & `currentscape-1.0.2/doc/source/images/quickstart_plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/LICENSE_CC0-1.0` & `currentscape-1.0.2/examples/original_paper_plot/LICENSE_CC0-1.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/config.json` & `currentscape-1.0.2/examples/original_paper_plot/config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/get_currents.py` & `currentscape-1.0.2/examples/original_paper_plot/get_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py` & `currentscape-1.0.2/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt` & `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt` & `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt` & `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt` & `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt` & `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt` & `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt` & `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt` & `currentscape-1.0.2/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/original_paper_plot/single_compartment.py` & `currentscape-1.0.2/examples/original_paper_plot/single_compartment.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/LICENSE.txt` & `currentscape-1.0.2/examples/use_case/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/LICENSE_CC-BY-CA-SA-4.0` & `currentscape-1.0.2/examples/use_case/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/config/params/final.json` & `currentscape-1.0.2/examples/use_case/config/params/final.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/config/params/pyr.json` & `currentscape-1.0.2/examples/use_case/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/CaDynamics_DC0.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/Ca_HVA2.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/Ca_LVAst.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/Ih.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/K_Pst.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/K_Tst.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/NaTg.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/Nap_Et2.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/SK_E2.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/SKv3_1.mod` & `currentscape-1.0.2/examples/use_case/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/mechanisms/notes.txt` & `currentscape-1.0.2/examples/use_case/mechanisms/notes.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc` & `currentscape-1.0.2/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/plot.py` & `currentscape-1.0.2/examples/use_case/plot.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/run.py` & `currentscape-1.0.2/examples/use_case/run.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/examples/use_case/run_py.sh` & `currentscape-1.0.2/examples/use_case/run_py.sh`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py` & `currentscape-1.0.2/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/requirements_docs.txt` & `currentscape-1.0.2/requirements_docs.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/setup.py` & `currentscape-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 from setuptools import setup, find_packages
 
-if sys.version_info < (3, 7):
-    sys.exit("Sorry, Python < 3.7 is not supported")
+if sys.version_info < (3, 8):
+    sys.exit("Sorry, Python < 3.8 is not supported")
 
 # read the contents of the README file
 with open("README.rst", encoding="utf-8") as f:
     README = f.read()
 
 EXTRA_EXAMPLE = ["scipy", "bluepyopt", "emodelrunner>=1.1.5"]
 
@@ -43,26 +43,25 @@
     license="Apache 2.0",
     install_requires=[
         "numpy",
         "matplotlib",
         "palettable",
     ],
     packages=find_packages(exclude=["tests"]),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     extras_require={
         "docs": ["sphinx", "sphinx-bluebrain-theme"],
         "example": EXTRA_EXAMPLE,
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
 )
```

### Comparing `currentscape-1.0.1/tests/extract_bNAC_config.json` & `currentscape-1.0.2/tests/extract_bNAC_config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_currentscape_config_parser.py` & `currentscape-1.0.2/tests/test_currentscape_config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_currentscape_currents.py` & `currentscape-1.0.2/tests/test_currentscape_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_currentscape_dataprocessing.py` & `currentscape-1.0.2/tests/test_currentscape_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_currentscape_datasets.py` & `currentscape-1.0.2/tests/test_currentscape_datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_currentscape_from_paper.py` & `currentscape-1.0.2/tests/test_currentscape_from_paper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_currentscape_ions.py` & `currentscape-1.0.2/tests/test_currentscape_ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_currentscape_mapper.py` & `currentscape-1.0.2/tests/test_currentscape_mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_currentscape_plotting.py` & `currentscape-1.0.2/tests/test_currentscape_plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tests/test_use_case_example.py` & `currentscape-1.0.2/tests/test_use_case_example.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.1/tox.ini` & `currentscape-1.0.2/tox.ini`

 * *Files identical despite different names*

