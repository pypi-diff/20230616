# Comparing `tmp/currentscape-1.0.4.dev8.tar.gz` & `tmp/currentscape-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currentscape-1.0.4.dev8.tar", last modified: Fri Jun 16 09:49:17 2023, max compression
+gzip compressed data, was "currentscape-1.0.5.tar", last modified: Fri Jun 16 12:44:23 2023, max compression
```

## Comparing `currentscape-1.0.4.dev8.tar` & `currentscape-1.0.5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.578519 currentscape-1.0.4.dev8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.558519 currentscape-1.0.4.dev8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.566519 currentscape-1.0.4.dev8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-16 09:49:17.578519 currentscape-1.0.4.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/Tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.566519 currentscape-1.0.4.dev8/currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/currentscape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/legends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/currentscape/voltages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.566519 currentscape-1.0.4.dev8/currentscape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-16 09:49:17.000000 currentscape-1.0.4.dev8/currentscape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-16 09:49:17.000000 currentscape-1.0.4.dev8/currentscape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:49:17.000000 currentscape-1.0.4.dev8/currentscape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 09:49:17.000000 currentscape-1.0.4.dev8/currentscape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 09:49:17.000000 currentscape-1.0.4.dev8/currentscape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.566519 currentscape-1.0.4.dev8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.566519 currentscape-1.0.4.dev8/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 09:49:07.000000 currentscape-1.0.4.dev8/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.570519 currentscape-1.0.4.dev8/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/doc/source/images/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/doc/source/images/quickstart_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/doc/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.558519 currentscape-1.0.4.dev8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.570519 currentscape-1.0.4.dev8/examples/original_paper_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/LICENSE_CC0-1.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/get_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.570519 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/original_paper_plot/single_compartment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.574519 currentscape-1.0.4.dev8/examples/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.562519 currentscape-1.0.4.dev8/examples/use_case/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.574519 currentscape-1.0.4.dev8/examples/use_case/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.574519 currentscape-1.0.4.dev8/examples/use_case/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/mechanisms/notes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.574519 currentscape-1.0.4.dev8/examples/use_case/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.574519 currentscape-1.0.4.dev8/examples/use_case/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/python_recordings/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/examples/use_case/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.562519 currentscape-1.0.4.dev8/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.574519 currentscape-1.0.4.dev8/extra/jjb-cells/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/extra/jjb-cells/cells.currentscape.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.562519 currentscape-1.0.4.dev8/extra/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.562519 currentscape-1.0.4.dev8/extra/spack/var/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.562519 currentscape-1.0.4.dev8/extra/spack/var/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.562519 currentscape-1.0.4.dev8/extra/spack/var/spack/repos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.562519 currentscape-1.0.4.dev8/extra/spack/var/spack/repos/builtin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.562519 currentscape-1.0.4.dev8/extra/spack/var/spack/repos/builtin/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.574519 currentscape-1.0.4.dev8/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:49:17.578519 currentscape-1.0.4.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:17.578519 currentscape-1.0.4.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/extract_bNAC_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_currentscape_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_currentscape_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_currentscape_dataprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_currentscape_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_currentscape_from_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_currentscape_ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_currentscape_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_currentscape_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/test_use_case_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-16 09:49:08.000000 currentscape-1.0.4.dev8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.952879 currentscape-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.944879 currentscape-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 12:44:11.000000 currentscape-1.0.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 12:44:11.000000 currentscape-1.0.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 12:44:11.000000 currentscape-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 12:44:11.000000 currentscape-1.0.5/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 12:44:11.000000 currentscape-1.0.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-16 12:44:11.000000 currentscape-1.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-16 12:44:11.000000 currentscape-1.0.5/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 12:44:11.000000 currentscape-1.0.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 12:44:11.000000 currentscape-1.0.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-16 12:44:11.000000 currentscape-1.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-16 12:44:11.000000 currentscape-1.0.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 12:44:11.000000 currentscape-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 12:44:11.000000 currentscape-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 12:44:11.000000 currentscape-1.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-16 12:44:23.952879 currentscape-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-16 12:44:11.000000 currentscape-1.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-16 12:44:11.000000 currentscape-1.0.5/Tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.944879 currentscape-1.0.5/currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/currentscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/legends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-16 12:44:11.000000 currentscape-1.0.5/currentscape/voltages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.944879 currentscape-1.0.5/currentscape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-16 12:44:23.000000 currentscape-1.0.5/currentscape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-16 12:44:23.000000 currentscape-1.0.5/currentscape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:44:23.000000 currentscape-1.0.5/currentscape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 12:44:23.000000 currentscape-1.0.5/currentscape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 12:44:23.000000 currentscape-1.0.5/currentscape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.944879 currentscape-1.0.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 12:44:11.000000 currentscape-1.0.5/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.944879 currentscape-1.0.5/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 12:44:11.000000 currentscape-1.0.5/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 12:44:11.000000 currentscape-1.0.5/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 12:44:11.000000 currentscape-1.0.5/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.944879 currentscape-1.0.5/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   183971 2023-06-16 12:44:11.000000 currentscape-1.0.5/doc/source/images/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-06-16 12:44:11.000000 currentscape-1.0.5/doc/source/images/quickstart_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 12:44:11.000000 currentscape-1.0.5/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 12:44:11.000000 currentscape-1.0.5/doc/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/examples/original_paper_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/LICENSE_CC0-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/get_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/original_paper_plot/single_compartment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/examples/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/examples/use_case/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/examples/use_case/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/examples/use_case/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/examples/use_case/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/examples/use_case/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/python_recordings/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-16 12:44:11.000000 currentscape-1.0.5/examples/use_case/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/extra/jjb-cells/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 12:44:11.000000 currentscape-1.0.5/extra/jjb-cells/cells.currentscape.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/extra/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/extra/spack/var/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/extra/spack/var/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/extra/spack/var/spack/repos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/extra/spack/var/spack/repos/builtin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.940879 currentscape-1.0.5/extra/spack/var/spack/repos/builtin/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.948879 currentscape-1.0.5/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 12:44:11.000000 currentscape-1.0.5/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 12:44:11.000000 currentscape-1.0.5/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:44:23.952879 currentscape-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-16 12:44:11.000000 currentscape-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:23.952879 currentscape-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/extract_bNAC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_currentscape_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_currentscape_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_currentscape_dataprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_currentscape_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_currentscape_from_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_currentscape_ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_currentscape_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_currentscape_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/test_use_case_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 12:44:11.000000 currentscape-1.0.5/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-16 12:44:11.000000 currentscape-1.0.5/tox.ini
```

### Comparing `currentscape-1.0.4.dev8/.github/workflows/build.yml` & `currentscape-1.0.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/.github/workflows/test.yml` & `currentscape-1.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/.pylintrc` & `currentscape-1.0.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/.zenodo.json` & `currentscape-1.0.5/.zenodo.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/CHANGELOG.rst` & `currentscape-1.0.5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/CONTRIBUTING.md` & `currentscape-1.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/COPYING` & `currentscape-1.0.5/COPYING`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/LICENSE.txt` & `currentscape-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/PKG-INFO` & `currentscape-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.4.dev8
+Version: 1.0.5
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
@@ -139,84 +139,104 @@
 .. code-block:: python
 
     import numpy as np
     from neuron import h
     from neuron.units import ms, mV
     from currentscape.currentscape import plot_currentscape
 
-    h.load_file('stdrun.hoc')
 
-    soma = h.Section(name='soma')
-    dend = h.Section(name='dend')
+    def main():
+        current_names = ["Potassium", "Sodium", "Leak"]
 
-    dend.connect(soma(1))
+        voltage, potassium, sodium, leak = run_sim()
 
-    soma.L = soma.diam = 12.6157
-    dend.L = 200
-    dend.diam = 1
-
-    for sec in h.allsec():
-        sec.Ra = 100    # Axial resistance in Ohm * cm
-        sec.cm = 1      # Membrane capacitance in micro Farads / cm^2
-
-    # Insert active Hodgkin-Huxley current in the soma
-    soma.insert('hh')
-    for seg in soma:
-        seg.hh.gnabar = 0.12  # Sodium conductance in S/cm2
-        seg.hh.gkbar = 0.036  # Potassium conductance in S/cm2
-        seg.hh.gl = 0.0003    # Leak conductance in S/cm2
-        seg.hh.el = -54.3     # Reversal potential in mV
-
-    # Insert passive current in the dendrite
-    dend.insert('pas')
-    for seg in dend:
-        seg.pas.g = 0.001  # Passive conductance in S/cm2
-        seg.pas.e = -65    # Leak reversal potential mV
-
-    stim = h.IClamp(dend(1))
-    stim.delay = 5
-    stim.dur = 10
-    stim.amp = 0.1
-
-    current_names = ["ik", "ina", "il_hh"]
-    t_vec = h.Vector()
-    v_vec = h.Vector()
-    ik_vec = h.Vector()
-    ina_vec = h.Vector()
-    il_vec = h.Vector()
-    t_vec.record(h._ref_t)
-    v_vec.record(soma(0.5)._ref_v)
-    ik_vec.record(soma(0.5)._ref_ik)
-    ina_vec.record(soma(0.5)._ref_ina)
-    il_vec.record(soma(0.5)._ref_il_hh)
-
-    h.finitialize(-65 * mV)
-    h.continuerun(25 * ms)
-
-    to_pA = 10 * soma(0.5).area() # turn mA/cm2 (*um2) into pA
-    voltage = np.asarray(v_vec)
-    potassium = np.asarray(ik_vec) * to_pA
-    sodium = np.asarray(ina_vec) * to_pA
-    leak = np.asarray(il_vec) * to_pA
-
-    config = {
-        "output": {                                                                    
-          "savefig": True,                                                           
-          "dir": ".",                                                                
-          "fname": "quickstart_plot",                                                
-          "extension": "png",                                                        
-          "dpi": 300,                                                                
-          "transparent": False                                                       
-        },   
-        "current": {"names": current_names},
-        "voltage": {"ylim": [-90, 50]},
-        "legendtextsize": 5,
-    }
-    fig = plot_currentscape(voltage, [potassium, sodium, leak], config)
-    fig.show()
+        config = {
+            "output": {
+                "savefig": True,
+                "dir": ".",
+                "fname": "quickstart_plot",
+                "extension": "png",
+                "dpi": 300,
+                "transparent": False
+            },
+            "current": {"names": current_names},
+            "voltage": {"ylim": [-90, 50]},
+            "legendtextsize": 5,
+            "adjust": {
+                "left": 0.15,
+                "right": 0.8,
+                "top": 1.0,
+                "bottom": 0.0
+            }
+        }
+
+        fig = plot_currentscape(voltage, [potassium, sodium, leak], config)
+        fig.show()
+
+
+    def run_sim():
+        h.load_file('stdrun.hoc')
+
+        soma = h.Section(name='soma')
+        dend = h.Section(name='dend')
+
+        dend.connect(soma(1))
+
+        soma.L = soma.diam = 12.6157
+        dend.L = 200
+        dend.diam = 1
+
+        for sec in h.allsec():
+            sec.Ra = 100    # Axial resistance in Ohm * cm
+            sec.cm = 1      # Membrane capacitance in micro Farads / cm^2
+
+        # Insert active Hodgkin-Huxley current in the soma
+        soma.insert('hh')
+        for seg in soma:
+            seg.hh.gnabar = 0.12  # Sodium conductance in S/cm2
+            seg.hh.gkbar = 0.036  # Potassium conductance in S/cm2
+            seg.hh.gl = 0.0003    # Leak conductance in S/cm2
+            seg.hh.el = -54.3     # Reversal potential in mV
+
+        # Insert passive current in the dendrite
+        dend.insert('pas')
+        for seg in dend:
+            seg.pas.g = 0.001  # Passive conductance in S/cm2
+            seg.pas.e = -65    # Leak reversal potential mV
+
+        stim = h.IClamp(dend(1))
+        stim.delay = 5
+        stim.dur = 10
+        stim.amp = 0.1
+
+        t_vec = h.Vector()
+        v_vec = h.Vector()
+        ik_vec = h.Vector()
+        ina_vec = h.Vector()
+        il_vec = h.Vector()
+        t_vec.record(h._ref_t)
+        v_vec.record(soma(0.5)._ref_v)
+        ik_vec.record(soma(0.5)._ref_ik)
+        ina_vec.record(soma(0.5)._ref_ina)
+        il_vec.record(soma(0.5)._ref_il_hh)
+
+        h.finitialize(-65 * mV)
+        h.continuerun(25 * ms)
+
+        to_pA = 10 * soma(0.5).area()  # turn mA/cm2 (*um2) into pA
+        voltage = np.asarray(v_vec)
+        potassium = np.asarray(ik_vec) * to_pA
+        sodium = np.asarray(ina_vec) * to_pA
+        leak = np.asarray(il_vec) * to_pA
+
+        return voltage, potassium, sodium, leak
+
+
+    if __name__ == "__main__":
+        main()
 
 When you run this code in Python, it will generate the following currentscape plot (in a window, and on disk as quickstart_plot.png):
 
 .. image:: doc/source/images/quickstart_plot.png
 
 Tutorial
 ========
```

### Comparing `currentscape-1.0.4.dev8/README.rst` & `currentscape-1.0.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -112,84 +112,104 @@
 .. code-block:: python
 
     import numpy as np
     from neuron import h
     from neuron.units import ms, mV
     from currentscape.currentscape import plot_currentscape
 
-    h.load_file('stdrun.hoc')
 
-    soma = h.Section(name='soma')
-    dend = h.Section(name='dend')
+    def main():
+        current_names = ["Potassium", "Sodium", "Leak"]
 
-    dend.connect(soma(1))
+        voltage, potassium, sodium, leak = run_sim()
 
-    soma.L = soma.diam = 12.6157
-    dend.L = 200
-    dend.diam = 1
-
-    for sec in h.allsec():
-        sec.Ra = 100    # Axial resistance in Ohm * cm
-        sec.cm = 1      # Membrane capacitance in micro Farads / cm^2
-
-    # Insert active Hodgkin-Huxley current in the soma
-    soma.insert('hh')
-    for seg in soma:
-        seg.hh.gnabar = 0.12  # Sodium conductance in S/cm2
-        seg.hh.gkbar = 0.036  # Potassium conductance in S/cm2
-        seg.hh.gl = 0.0003    # Leak conductance in S/cm2
-        seg.hh.el = -54.3     # Reversal potential in mV
-
-    # Insert passive current in the dendrite
-    dend.insert('pas')
-    for seg in dend:
-        seg.pas.g = 0.001  # Passive conductance in S/cm2
-        seg.pas.e = -65    # Leak reversal potential mV
-
-    stim = h.IClamp(dend(1))
-    stim.delay = 5
-    stim.dur = 10
-    stim.amp = 0.1
-
-    current_names = ["ik", "ina", "il_hh"]
-    t_vec = h.Vector()
-    v_vec = h.Vector()
-    ik_vec = h.Vector()
-    ina_vec = h.Vector()
-    il_vec = h.Vector()
-    t_vec.record(h._ref_t)
-    v_vec.record(soma(0.5)._ref_v)
-    ik_vec.record(soma(0.5)._ref_ik)
-    ina_vec.record(soma(0.5)._ref_ina)
-    il_vec.record(soma(0.5)._ref_il_hh)
-
-    h.finitialize(-65 * mV)
-    h.continuerun(25 * ms)
-
-    to_pA = 10 * soma(0.5).area() # turn mA/cm2 (*um2) into pA
-    voltage = np.asarray(v_vec)
-    potassium = np.asarray(ik_vec) * to_pA
-    sodium = np.asarray(ina_vec) * to_pA
-    leak = np.asarray(il_vec) * to_pA
-
-    config = {
-        "output": {                                                                    
-          "savefig": True,                                                           
-          "dir": ".",                                                                
-          "fname": "quickstart_plot",                                                
-          "extension": "png",                                                        
-          "dpi": 300,                                                                
-          "transparent": False                                                       
-        },   
-        "current": {"names": current_names},
-        "voltage": {"ylim": [-90, 50]},
-        "legendtextsize": 5,
-    }
-    fig = plot_currentscape(voltage, [potassium, sodium, leak], config)
-    fig.show()
+        config = {
+            "output": {
+                "savefig": True,
+                "dir": ".",
+                "fname": "quickstart_plot",
+                "extension": "png",
+                "dpi": 300,
+                "transparent": False
+            },
+            "current": {"names": current_names},
+            "voltage": {"ylim": [-90, 50]},
+            "legendtextsize": 5,
+            "adjust": {
+                "left": 0.15,
+                "right": 0.8,
+                "top": 1.0,
+                "bottom": 0.0
+            }
+        }
+
+        fig = plot_currentscape(voltage, [potassium, sodium, leak], config)
+        fig.show()
+
+
+    def run_sim():
+        h.load_file('stdrun.hoc')
+
+        soma = h.Section(name='soma')
+        dend = h.Section(name='dend')
+
+        dend.connect(soma(1))
+
+        soma.L = soma.diam = 12.6157
+        dend.L = 200
+        dend.diam = 1
+
+        for sec in h.allsec():
+            sec.Ra = 100    # Axial resistance in Ohm * cm
+            sec.cm = 1      # Membrane capacitance in micro Farads / cm^2
+
+        # Insert active Hodgkin-Huxley current in the soma
+        soma.insert('hh')
+        for seg in soma:
+            seg.hh.gnabar = 0.12  # Sodium conductance in S/cm2
+            seg.hh.gkbar = 0.036  # Potassium conductance in S/cm2
+            seg.hh.gl = 0.0003    # Leak conductance in S/cm2
+            seg.hh.el = -54.3     # Reversal potential in mV
+
+        # Insert passive current in the dendrite
+        dend.insert('pas')
+        for seg in dend:
+            seg.pas.g = 0.001  # Passive conductance in S/cm2
+            seg.pas.e = -65    # Leak reversal potential mV
+
+        stim = h.IClamp(dend(1))
+        stim.delay = 5
+        stim.dur = 10
+        stim.amp = 0.1
+
+        t_vec = h.Vector()
+        v_vec = h.Vector()
+        ik_vec = h.Vector()
+        ina_vec = h.Vector()
+        il_vec = h.Vector()
+        t_vec.record(h._ref_t)
+        v_vec.record(soma(0.5)._ref_v)
+        ik_vec.record(soma(0.5)._ref_ik)
+        ina_vec.record(soma(0.5)._ref_ina)
+        il_vec.record(soma(0.5)._ref_il_hh)
+
+        h.finitialize(-65 * mV)
+        h.continuerun(25 * ms)
+
+        to_pA = 10 * soma(0.5).area()  # turn mA/cm2 (*um2) into pA
+        voltage = np.asarray(v_vec)
+        potassium = np.asarray(ik_vec) * to_pA
+        sodium = np.asarray(ina_vec) * to_pA
+        leak = np.asarray(il_vec) * to_pA
+
+        return voltage, potassium, sodium, leak
+
+
+    if __name__ == "__main__":
+        main()
 
 When you run this code in Python, it will generate the following currentscape plot (in a window, and on disk as quickstart_plot.png):
 
 .. image:: doc/source/images/quickstart_plot.png
 
 Tutorial
 ========
```

### Comparing `currentscape-1.0.4.dev8/Tutorial.rst` & `currentscape-1.0.5/Tutorial.rst`

 * *Files 0% similar despite different names*

```diff
@@ -155,16 +155,16 @@
         "titlesize": 12,
         "labelpad": 1,
         "textsize": 6,
         "lw": 0.5,
         "adjust": {
             "left": 0.15,
             "right": 0.85,
-            "top": null,
-            "bottom": null
+            "top": 0.95,
+            "bottom": 0.0
         }
     }
 
 If you do not want to modify the default values, you should at least specify the current names if you want to plot with the legend.
 Your configuration file could be as small as:
 
 .. code-block:: json
```

### Comparing `currentscape-1.0.4.dev8/currentscape/__init__.py` & `currentscape-1.0.5/currentscape/__init__.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/config_parser.py` & `currentscape-1.0.5/currentscape/config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,16 +187,16 @@
     # forced to 0 if pattern:use is False and current:stackplot is False
     legend["handlelength"] = 1.4
     config["legend"] = legend
 
     adjust_ = {}
     adjust_["left"] = 0.15
     adjust_["right"] = 0.85
-    adjust_["top"] = None
-    adjust_["bottom"] = None
+    adjust_["top"] = 0.95
+    adjust_["bottom"] = 0.0
     config["adjust"] = adjust_
 
     config["title"] = None
     config["figsize"] = (3, 4)
     config["labelpad"] = 1
     config["textsize"] = 6
     config["titlesize"] = 12
```

### Comparing `currentscape-1.0.4.dev8/currentscape/currents.py` & `currentscape-1.0.5/currentscape/currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/currentscape.py` & `currentscape-1.0.5/currentscape/currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/data_processing.py` & `currentscape-1.0.5/currentscape/data_processing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/datasets.py` & `currentscape-1.0.5/currentscape/datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/ions.py` & `currentscape-1.0.5/currentscape/ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/legends.py` & `currentscape-1.0.5/currentscape/legends.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/mapper.py` & `currentscape-1.0.5/currentscape/mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/plotting.py` & `currentscape-1.0.5/currentscape/plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape/voltages.py` & `currentscape-1.0.5/currentscape/voltages.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/currentscape.egg-info/PKG-INFO` & `currentscape-1.0.5/currentscape.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.4.dev8
+Version: 1.0.5
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
@@ -139,84 +139,104 @@
 .. code-block:: python
 
     import numpy as np
     from neuron import h
     from neuron.units import ms, mV
     from currentscape.currentscape import plot_currentscape
 
-    h.load_file('stdrun.hoc')
 
-    soma = h.Section(name='soma')
-    dend = h.Section(name='dend')
+    def main():
+        current_names = ["Potassium", "Sodium", "Leak"]
 
-    dend.connect(soma(1))
+        voltage, potassium, sodium, leak = run_sim()
 
-    soma.L = soma.diam = 12.6157
-    dend.L = 200
-    dend.diam = 1
-
-    for sec in h.allsec():
-        sec.Ra = 100    # Axial resistance in Ohm * cm
-        sec.cm = 1      # Membrane capacitance in micro Farads / cm^2
-
-    # Insert active Hodgkin-Huxley current in the soma
-    soma.insert('hh')
-    for seg in soma:
-        seg.hh.gnabar = 0.12  # Sodium conductance in S/cm2
-        seg.hh.gkbar = 0.036  # Potassium conductance in S/cm2
-        seg.hh.gl = 0.0003    # Leak conductance in S/cm2
-        seg.hh.el = -54.3     # Reversal potential in mV
-
-    # Insert passive current in the dendrite
-    dend.insert('pas')
-    for seg in dend:
-        seg.pas.g = 0.001  # Passive conductance in S/cm2
-        seg.pas.e = -65    # Leak reversal potential mV
-
-    stim = h.IClamp(dend(1))
-    stim.delay = 5
-    stim.dur = 10
-    stim.amp = 0.1
-
-    current_names = ["ik", "ina", "il_hh"]
-    t_vec = h.Vector()
-    v_vec = h.Vector()
-    ik_vec = h.Vector()
-    ina_vec = h.Vector()
-    il_vec = h.Vector()
-    t_vec.record(h._ref_t)
-    v_vec.record(soma(0.5)._ref_v)
-    ik_vec.record(soma(0.5)._ref_ik)
-    ina_vec.record(soma(0.5)._ref_ina)
-    il_vec.record(soma(0.5)._ref_il_hh)
-
-    h.finitialize(-65 * mV)
-    h.continuerun(25 * ms)
-
-    to_pA = 10 * soma(0.5).area() # turn mA/cm2 (*um2) into pA
-    voltage = np.asarray(v_vec)
-    potassium = np.asarray(ik_vec) * to_pA
-    sodium = np.asarray(ina_vec) * to_pA
-    leak = np.asarray(il_vec) * to_pA
-
-    config = {
-        "output": {                                                                    
-          "savefig": True,                                                           
-          "dir": ".",                                                                
-          "fname": "quickstart_plot",                                                
-          "extension": "png",                                                        
-          "dpi": 300,                                                                
-          "transparent": False                                                       
-        },   
-        "current": {"names": current_names},
-        "voltage": {"ylim": [-90, 50]},
-        "legendtextsize": 5,
-    }
-    fig = plot_currentscape(voltage, [potassium, sodium, leak], config)
-    fig.show()
+        config = {
+            "output": {
+                "savefig": True,
+                "dir": ".",
+                "fname": "quickstart_plot",
+                "extension": "png",
+                "dpi": 300,
+                "transparent": False
+            },
+            "current": {"names": current_names},
+            "voltage": {"ylim": [-90, 50]},
+            "legendtextsize": 5,
+            "adjust": {
+                "left": 0.15,
+                "right": 0.8,
+                "top": 1.0,
+                "bottom": 0.0
+            }
+        }
+
+        fig = plot_currentscape(voltage, [potassium, sodium, leak], config)
+        fig.show()
+
+
+    def run_sim():
+        h.load_file('stdrun.hoc')
+
+        soma = h.Section(name='soma')
+        dend = h.Section(name='dend')
+
+        dend.connect(soma(1))
+
+        soma.L = soma.diam = 12.6157
+        dend.L = 200
+        dend.diam = 1
+
+        for sec in h.allsec():
+            sec.Ra = 100    # Axial resistance in Ohm * cm
+            sec.cm = 1      # Membrane capacitance in micro Farads / cm^2
+
+        # Insert active Hodgkin-Huxley current in the soma
+        soma.insert('hh')
+        for seg in soma:
+            seg.hh.gnabar = 0.12  # Sodium conductance in S/cm2
+            seg.hh.gkbar = 0.036  # Potassium conductance in S/cm2
+            seg.hh.gl = 0.0003    # Leak conductance in S/cm2
+            seg.hh.el = -54.3     # Reversal potential in mV
+
+        # Insert passive current in the dendrite
+        dend.insert('pas')
+        for seg in dend:
+            seg.pas.g = 0.001  # Passive conductance in S/cm2
+            seg.pas.e = -65    # Leak reversal potential mV
+
+        stim = h.IClamp(dend(1))
+        stim.delay = 5
+        stim.dur = 10
+        stim.amp = 0.1
+
+        t_vec = h.Vector()
+        v_vec = h.Vector()
+        ik_vec = h.Vector()
+        ina_vec = h.Vector()
+        il_vec = h.Vector()
+        t_vec.record(h._ref_t)
+        v_vec.record(soma(0.5)._ref_v)
+        ik_vec.record(soma(0.5)._ref_ik)
+        ina_vec.record(soma(0.5)._ref_ina)
+        il_vec.record(soma(0.5)._ref_il_hh)
+
+        h.finitialize(-65 * mV)
+        h.continuerun(25 * ms)
+
+        to_pA = 10 * soma(0.5).area()  # turn mA/cm2 (*um2) into pA
+        voltage = np.asarray(v_vec)
+        potassium = np.asarray(ik_vec) * to_pA
+        sodium = np.asarray(ina_vec) * to_pA
+        leak = np.asarray(il_vec) * to_pA
+
+        return voltage, potassium, sodium, leak
+
+
+    if __name__ == "__main__":
+        main()
 
 When you run this code in Python, it will generate the following currentscape plot (in a window, and on disk as quickstart_plot.png):
 
 .. image:: doc/source/images/quickstart_plot.png
 
 Tutorial
 ========
```

### Comparing `currentscape-1.0.4.dev8/currentscape.egg-info/SOURCES.txt` & `currentscape-1.0.5/currentscape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/doc/Makefile` & `currentscape-1.0.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/doc/source/conf.py` & `currentscape-1.0.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/LICENSE_CC0-1.0` & `currentscape-1.0.5/examples/original_paper_plot/LICENSE_CC0-1.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/config.json` & `currentscape-1.0.5/examples/original_paper_plot/config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/get_currents.py` & `currentscape-1.0.5/examples/original_paper_plot/get_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py` & `currentscape-1.0.5/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt` & `currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt` & `currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt` & `currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt` & `currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt` & `currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt` & `currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt` & `currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt` & `currentscape-1.0.5/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/original_paper_plot/single_compartment.py` & `currentscape-1.0.5/examples/original_paper_plot/single_compartment.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/LICENSE.txt` & `currentscape-1.0.5/examples/use_case/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/LICENSE_CC-BY-CA-SA-4.0` & `currentscape-1.0.5/examples/use_case/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/config/params/final.json` & `currentscape-1.0.5/examples/use_case/config/params/final.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/config/params/pyr.json` & `currentscape-1.0.5/examples/use_case/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/CaDynamics_DC0.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/Ca_HVA2.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/Ca_LVAst.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/Ih.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/K_Pst.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/K_Tst.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/NaTg.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/Nap_Et2.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/SK_E2.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/SKv3_1.mod` & `currentscape-1.0.5/examples/use_case/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/mechanisms/notes.txt` & `currentscape-1.0.5/examples/use_case/mechanisms/notes.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc` & `currentscape-1.0.5/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/plot.py` & `currentscape-1.0.5/examples/use_case/plot.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/run.py` & `currentscape-1.0.5/examples/use_case/run.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/examples/use_case/run_py.sh` & `currentscape-1.0.5/examples/use_case/run_py.sh`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py` & `currentscape-1.0.5/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/requirements_docs.txt` & `currentscape-1.0.5/requirements_docs.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/setup.py` & `currentscape-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/extract_bNAC_config.json` & `currentscape-1.0.5/tests/extract_bNAC_config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_currentscape_config_parser.py` & `currentscape-1.0.5/tests/test_currentscape_config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_currentscape_currents.py` & `currentscape-1.0.5/tests/test_currentscape_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_currentscape_dataprocessing.py` & `currentscape-1.0.5/tests/test_currentscape_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_currentscape_datasets.py` & `currentscape-1.0.5/tests/test_currentscape_datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_currentscape_from_paper.py` & `currentscape-1.0.5/tests/test_currentscape_from_paper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_currentscape_ions.py` & `currentscape-1.0.5/tests/test_currentscape_ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_currentscape_mapper.py` & `currentscape-1.0.5/tests/test_currentscape_mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_currentscape_plotting.py` & `currentscape-1.0.5/tests/test_currentscape_plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tests/test_use_case_example.py` & `currentscape-1.0.5/tests/test_use_case_example.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.4.dev8/tox.ini` & `currentscape-1.0.5/tox.ini`

 * *Files identical despite different names*

