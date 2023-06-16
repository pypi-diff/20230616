# Comparing `tmp/ismn-1.3.3.tar.gz` & `tmp/ismn-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ismn-1.3.3.tar", last modified: Mon Mar  6 09:02:16 2023, max compression
+gzip compressed data, was "ismn-1.3.4.tar", last modified: Fri Jun 16 19:52:10 2023, max compression
```

## Comparing `ismn-1.3.3.tar` & `ismn-1.3.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.315698 ismn-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-06 08:48:34.000000 ismn-1.3.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.291699 ismn-1.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-03-06 08:48:34.000000 ismn-1.3.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-06 08:48:34.000000 ismn-1.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-06 08:48:34.000000 ismn-1.3.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-06 08:48:34.000000 ismn-1.3.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-06 08:48:34.000000 ismn-1.3.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-06 08:48:34.000000 ismn-1.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-03-06 09:02:16.315698 ismn-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-03-06 08:48:34.000000 ismn-1.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/docs_env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.299698 ismn-1.3.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/examples/custom_meta.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   603022 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/examples/interface.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   510142 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/examples/ismn.png
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/examples/vod.csv
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-06 08:48:34.000000 ismn-1.3.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-06 08:48:34.000000 ismn-1.3.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-06 08:48:34.000000 ismn-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-06 09:02:16.315698 ismn-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-06 08:48:34.000000 ismn-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.291699 ismn-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.299698 ismn-1.3.3/src/ismn/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28723 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/citations.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26220 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16181 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/filecollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/filehandlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-03-06 08:48:34.000000 ismn-1.3.3/src/ismn/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.299698 ismn-1.3.3/src/ismn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-03-06 09:02:16.000000 ismn-1.3.3/src/ismn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-06 09:02:16.000000 ismn-1.3.3/src/ismn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 09:02:16.000000 ismn-1.3.3/src/ismn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 09:01:55.000000 ismn-1.3.3/src/ismn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-06 09:02:16.000000 ismn-1.3.3/src/ismn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-06 09:02:16.000000 ismn-1.3.3/src/ismn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.303699 ismn-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.303699 ismn-1.3.3/tests/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    98165 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/baseline/test_interface_plotting.png
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_custom_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.303699 ismn-1.3.3/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.303699 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.303699 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/
--rw-r--r--   0 runner    (1001) docker     (123)   948144 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.303699 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/
--rw-r--r--   0 runner    (1001) docker     (123)   979186 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.311699 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7186150 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_sm_0.050000_0.050000_ThetaProbe-ML2X_19500101_20210131.stm
--rwxr-xr-x   0 runner    (1001) docker     (123)     2885 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_static_variables.csv
--rw-r--r--   0 runner    (1001) docker     (123)    41902 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/Metadata.xml
--rw-r--r--   0 runner    (1001) docker     (123)   481431 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.311699 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.311699 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/
--rw-r--r--   0 runner    (1001) docker     (123)   213697 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.311699 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/
--rw-r--r--   0 runner    (1001) docker     (123)   223981 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv
--rw-r--r--   0 runner    (1001) docker     (123)    41902 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/Metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.311699 ismn-1.3.3/tests/test_data/custom_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/custom_metadata/custom_sensormeta.csv
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/custom_metadata/custom_stationmeta.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/tests/test_data/format_ceop_sep/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.311699 ismn-1.3.3/tests/test_data/format_ceop_sep/SMOSMANIA/
--rwxr-xr-x   0 runner    (1001) docker     (123)   102268 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/format_ceop_sep/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/tests/test_data/format_header_values/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.315698 ismn-1.3.3/tests/test_data/format_header_values/SMOSMANIA/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23088 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/format_header_values/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.315698 ismn-1.3.3/tests/test_data/malformed/
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/malformed/mal_formed_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/tests/test_data/zip_archives/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.315698 ismn-1.3.3/tests/test_data/zip_archives/ceop/
--rw-r--r--   0 runner    (1001) docker     (123)   105176 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/zip_archives/ceop/Data_seperate_files_20170810_20180809.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.315698 ismn-1.3.3/tests/test_data/zip_archives/format_header_values/
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/zip_archives/format_header_values/Data_SMOSMANIA.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.315698 ismn-1.3.3/tests/test_data/zip_archives/header/
--rw-r--r--   0 runner    (1001) docker     (123)    52474 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/zip_archives/header/Data_seperate_files_header_20170810_20180809.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.295699 ismn-1.3.3/tests/test_data/zip_archives/multinetwork/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:02:16.315698 ismn-1.3.3/tests/test_data/zip_archives/multinetwork/header_values/
--rw-r--r--   0 runner    (1001) docker     (123)   609917 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_data/zip_archives/multinetwork/header_values/Data_header_values.zip
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_filecollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_filehandler_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_filehandler_static.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-03-06 08:48:34.000000 ismn-1.3.3/tests/test_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.237495 ismn-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-16 19:49:03.000000 ismn-1.3.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.197495 ismn-1.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.205495 ismn-1.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-16 19:49:03.000000 ismn-1.3.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 19:49:03.000000 ismn-1.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 19:49:03.000000 ismn-1.3.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 19:49:03.000000 ismn-1.3.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-16 19:49:03.000000 ismn-1.3.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 19:49:03.000000 ismn-1.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-06-16 19:52:10.237495 ismn-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-06-16 19:49:03.000000 ismn-1.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.205495 ismn-1.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.205495 ismn-1.3.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/docs_env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.209495 ismn-1.3.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/examples/custom_meta.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  1084721 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/examples/interface.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   510142 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/examples/ismn.png
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/examples/vod.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 19:49:03.000000 ismn-1.3.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-16 19:49:03.000000 ismn-1.3.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-16 19:49:03.000000 ismn-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-16 19:52:10.237495 ismn-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-16 19:49:03.000000 ismn-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.197495 ismn-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.213495 ismn-1.3.4/src/ismn/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28723 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/citations.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/filecollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/filehandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36313 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-06-16 19:49:03.000000 ismn-1.3.4/src/ismn/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.213495 ismn-1.3.4/src/ismn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-06-16 19:52:10.000000 ismn-1.3.4/src/ismn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-16 19:52:10.000000 ismn-1.3.4/src/ismn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:52:10.000000 ismn-1.3.4/src/ismn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:51:47.000000 ismn-1.3.4/src/ismn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 19:52:10.000000 ismn-1.3.4/src/ismn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 19:52:10.000000 ismn-1.3.4/src/ismn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.217495 ismn-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.217495 ismn-1.3.4/tests/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    98165 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/baseline/test_interface_plotting.png
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_custom_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.217495 ismn-1.3.4/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.217495 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.201495 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.217495 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/
+-rw-r--r--   0 runner    (1001) docker     (123)   948144 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.221495 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/
+-rw-r--r--   0 runner    (1001) docker     (123)   979186 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.201495 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.229495 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7186150 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_sm_0.050000_0.050000_ThetaProbe-ML2X_19500101_20210131.stm
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2885 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_static_variables.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41902 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/Metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   481431 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.229495 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.201495 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/
+-rw-r--r--   0 runner    (1001) docker     (123)   213697 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/
+-rw-r--r--   0 runner    (1001) docker     (123)   223981 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41902 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/Metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/custom_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/custom_metadata/custom_sensormeta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/custom_metadata/custom_stationmeta.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.201495 ismn-1.3.4/tests/test_data/format_ceop_sep/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/format_ceop_sep/SMOSMANIA/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   102268 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/format_ceop_sep/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.201495 ismn-1.3.4/tests/test_data/format_header_values/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/format_header_values/SMOSMANIA/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23088 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/format_header_values/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/malformed/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/malformed/mal_formed_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.201495 ismn-1.3.4/tests/test_data/zip_archives/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/zip_archives/ceop/
+-rw-r--r--   0 runner    (1001) docker     (123)   105176 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/zip_archives/ceop/Data_seperate_files_20170810_20180809.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/zip_archives/format_header_values/
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/zip_archives/format_header_values/Data_SMOSMANIA.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/zip_archives/header/
+-rw-r--r--   0 runner    (1001) docker     (123)    52474 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/zip_archives/header/Data_seperate_files_header_20170810_20180809.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.201495 ismn-1.3.4/tests/test_data/zip_archives/multinetwork/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:52:10.233495 ismn-1.3.4/tests/test_data/zip_archives/multinetwork/header_values/
+-rw-r--r--   0 runner    (1001) docker     (123)   609917 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_data/zip_archives/multinetwork/header_values/Data_header_values.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_filecollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_filehandler_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_filehandler_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-16 19:49:03.000000 ismn-1.3.4/tests/test_readers.py
```

### Comparing `ismn-1.3.3/.coveragerc` & `ismn-1.3.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/.github/workflows/build.yml` & `ismn-1.3.4/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,22 @@
           - os: "windows-latest"
             python-version: '3.10'
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: true
           fetch-depth: 0
-      - uses: conda-incubator/setup-miniconda@v2.0.1
+      - uses: conda-incubator/setup-miniconda@v2
         with:
           miniconda-version: "latest"
           auto-update-conda: true
+          channel-priority: flexible
           python-version: ${{ matrix.python-version }}
           environment-file: environment.yml
+          mamba-version: "*"
           activate-environment: ismn
           auto-activate-base: false
       - name: Print environment infos
         shell: bash -l {0}
         run: |
           conda info -a
           conda list
```

### Comparing `ismn-1.3.3/.gitignore` & `ismn-1.3.4/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -49,8 +49,11 @@
 # Per-project virtualenvs
 .venv*/
 
 # ismn metadata files
 **/python_metadata/*
 networks/*
 .artifacts/*
-.coverage*
+.coverage*
+
+# VSC config file
+.vscode/*
```

### Comparing `ismn-1.3.3/CHANGELOG.rst` & `ismn-1.3.4/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 =========
 
 Unreleased changes in master branch
 ===================================
 
 -
 
+Version 1.3.4
+=============
+
+- Fixed bug with parsing sensor files for RISMA network in "header & files" format
+
 Version 1.3.3
 =============
 
 - Continue metadata collection for station on any type of error (PR #64)
 
 Version 1.3.2
 =============
```

### Comparing `ismn-1.3.3/LICENSE.txt` & `ismn-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/PKG-INFO` & `ismn-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ismn
-Version: 1.3.3
+Version: 1.3.4
 Summary: Readers for the data from the International Soil Moisture Database
 Home-page: http://ismn.geo.tuwien.ac.at
 Author: TU Wien
 Author-email: ismn@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, https://ismn.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `ismn-1.3.3/README.rst` & `ismn-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/docs/Makefile` & `ismn-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/docs/conf.py` & `ismn-1.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/docs/examples/custom_meta.ipynb` & `ismn-1.3.4/docs/examples/custom_meta.ipynb`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/docs/examples/ismn.png` & `ismn-1.3.4/docs/examples/ismn.png`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/setup.cfg` & `ismn-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/setup.py` & `ismn-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/src/ismn/__init__.py` & `ismn-1.3.4/src/ismn/__init__.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/src/ismn/base.py` & `ismn-1.3.4/src/ismn/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,18 +123,16 @@
             warnings.warn("Remove leading (back)slash in passed subpath.")
             subpath = Path(*subpath.parts[1:])
 
         if self.zip:
             subpath = PurePosixPath(subpath)
         else:
             if not (self.path / Path(subpath)).exists():
-                raise ValueError(
-                    f"Subpath {subpath} does not exist"
-                    f" in archive {self.path}"
-                )
+                raise ValueError(f"Subpath {subpath} does not exist"
+                                 f" in archive {self.path}")
 
         return subpath
 
     @property
     def cont(self):
         """Get cont of object, or scan to create cont."""
         if self.__cont is None:
```

### Comparing `ismn-1.3.3/src/ismn/citations.txt` & `ismn-1.3.4/src/ismn/citations.txt`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/src/ismn/components.py` & `ismn-1.3.4/src/ismn/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,16 +682,17 @@
 
     def __repr__(self, indent: str = ""):
         return ",\n".join([
             f"{indent}{net.name}: {list(net.stations.keys())}"
             for net in self.networks.values()
         ])
 
-    def __getitem__(self, item: Union[int, str, list]) -> \
-            Union["NetworkCollection", Network]:
+    def __getitem__(
+            self, item: Union[int, str,
+                              list]) -> Union["NetworkCollection", Network]:
         # shortcut to access networks directly
         if isinstance(item, (int, str)):
             if isinstance(item, int):
                 item = list(self.networks.keys())[item]
             net: Network = self.networks[item]
             return net
         else:
```

### Comparing `ismn-1.3.3/src/ismn/const.py` & `ismn-1.3.4/src/ismn/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,24 +104,23 @@
     "depth_from[m]",
     "depth_to[m]",
     "value",
     "description",
     "quantity_source_name",
 ]
 
-lc_num_vars = ['lc_2000', 'lc_2005', 'lc_2010']
-lc_str_vars = ['lc_insitu']
+lc_num_vars = ["lc_2000", "lc_2005", "lc_2010"]
+lc_str_vars = ["lc_insitu"]
 LC_VARS = [*lc_num_vars, *lc_str_vars]
-CLIM_VARS = ['climate_KG', 'climate_insitu']
+CLIM_VARS = ["climate_KG", "climate_insitu"]
 
-CSV_META_TEMPLATE_SURF_VAR = OrderedDict(
-    [(c, np.nan) for c in lc_num_vars] +
-    [(c, 'unknown') for c in lc_str_vars] +
-    [(c, 'unknown') for c in CLIM_VARS]
-)
+CSV_META_TEMPLATE_SURF_VAR = OrderedDict([(c, np.nan) for c in lc_num_vars] +
+                                         [(c, "unknown")
+                                          for c in lc_str_vars] +
+                                         [(c, "unknown") for c in CLIM_VARS])
 CSV_META_TEMPLATE_GROUND_VAR = OrderedDict([
     ("saturation", np.nan),
     ("clay_fraction", np.nan),
     ("sand_fraction", np.nan),
     ("silt_fraction", np.nan),
     ("organic_carbon", np.nan),
 ])
```

### Comparing `ismn-1.3.3/src/ismn/custom.py` & `ismn-1.3.4/src/ismn/custom.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,63 +78,62 @@
     transferred into the python metadata
     - where <var1>_depth_from and <var1>_depth_to etc are the depths that
     are assigned to the metadata (if columns exist)
     """
 
     def __init__(self, station_meta_csv, fill_values=None, **kwargs):
         """
-        Parameters
-        ----------
-        station_meta_csv: str
-            Path to the csv file with the above described content
-       fill_values: dict, optional (default: None)
-            Values to use for a certain custom metadata variable, if no
-            match is found.
-        kwargs:
-            Additional kwargs as passed to :func:`pandas.read_csv`
-            To use a different separator than the default semicolon, use `sep`
+         Parameters
+         ----------
+         station_meta_csv: str
+             Path to the csv file with the above described content
+        fill_values: dict, optional (default: None)
+             Values to use for a certain custom metadata variable, if no
+             match is found.
+         kwargs:
+             Additional kwargs as passed to :func:`pandas.read_csv`
+             To use a different separator than the default semicolon, use `sep`
         """
-        if 'sep' in kwargs:
-            sep = kwargs.pop('sep')
+        if "sep" in kwargs:
+            sep = kwargs.pop("sep")
         else:
-            sep = ';'
+            sep = ";"
 
         self.fill_values = dict() if fill_values is None else fill_values
         self.df = pd.read_csv(station_meta_csv, sep=sep, **kwargs)
 
     def _empty_var(self, varnames) -> list:
         """
         For all passed variable names, create an empty MetaVar if a fill value
         for the name is set in `self.fill_value`.
         """
         vars = []
         for var in varnames:
-            if var in self.fill_values.keys() and \
-                not (var.endswith('_depth_from') or
-                     var.endswith('_depth_to')):
+            if var in self.fill_values.keys() and not (
+                    var.endswith("_depth_from") or var.endswith("_depth_to")):
                 vars.append(MetaVar(var, self.fill_values[var]))
         return vars
 
     @staticmethod
     def _row2var(row: dict) -> list:
         """
         Extract name, value, depth from row.
         """
         vars = []
 
         for k, v in row.items():
-            if k.endswith('_depth_from') or k.endswith('_depth_to'):
+            if k.endswith("_depth_from") or k.endswith("_depth_to"):
                 continue
 
-            if f'{k}_depth_from' in row:
-                depth_from = row[f'{k}_depth_from']
+            if f"{k}_depth_from" in row:
+                depth_from = row[f"{k}_depth_from"]
             else:
                 depth_from = None
-            if f'{k}_depth_to' in row:
-                depth_to = row[f'{k}_depth_to']
+            if f"{k}_depth_to" in row:
+                depth_to = row[f"{k}_depth_to"]
             else:
                 depth_to = None
 
             if (depth_from is None) and (depth_to is None):
                 depth = None
             else:
                 if depth_from is None:
@@ -162,28 +161,28 @@
         Returns
         -------
         meta: dict
             Additional depth-independent metadata at the location
 
         """
 
-        cond = (self.df['network'] == meta['network'].val) & \
-               (self.df['station'] == meta['station'].val)
+        cond = (self.df["network"] == meta["network"].val) & (
+            self.df["station"] == meta["station"].val)
 
-        df = self.df[cond].set_index(['network', 'station'])
+        df = self.df[cond].set_index(["network", "station"])
 
         # drop potential duplicates, keep first
-        df = df[~df.index.duplicated(keep='first')]
+        df = df[~df.index.duplicated(keep="first")]
 
         vars = []
 
         if df.empty and (self.fill_values is not None):
             vars += self._empty_var(df.columns.values)
         else:
-            for row in df.to_dict('records'):
+            for row in df.to_dict("records"):
                 vars += self._row2var(row)
 
         return MetaData(vars)
 
 
 class CustomSensorMetadataCsv(CustomStationMetadataCsv):
     """
@@ -211,29 +210,31 @@
             the network, station, instrument, and instrument depths match.
 
         Returns
         -------
         meta: Metadata
             Additional depth-dependent metadata at the location
         """
-        cond = (self.df['network'] == meta['network'].val) & \
-               (self.df['station'] == meta['station'].val) & \
-               (self.df['instrument'] == meta['instrument'].val) & \
-               (self.df['variable'] == meta['variable'].val) & \
-               (self.df['depth_from'] == meta['instrument'].depth[0]) & \
-               (self.df['depth_to'] == meta['instrument'].depth[1])
-
-        df = self.df[cond].set_index(
-            ['network', 'station', 'instrument', 'variable', 'depth_from', 'depth_to'])
+        cond = ((self.df["network"] == meta["network"].val)
+                & (self.df["station"] == meta["station"].val)
+                & (self.df["instrument"] == meta["instrument"].val)
+                & (self.df["variable"] == meta["variable"].val)
+                & (self.df["depth_from"] == meta["instrument"].depth[0])
+                & (self.df["depth_to"] == meta["instrument"].depth[1]))
+
+        df = self.df[cond].set_index([
+            "network", "station", "instrument", "variable", "depth_from",
+            "depth_to"
+        ])
 
         # drop potential duplicates, keep first
-        df = df[~df.index.duplicated(keep='first')]
+        df = df[~df.index.duplicated(keep="first")]
 
         vars = []
 
         if df.empty and (self.fill_values is not None):
             vars += self._empty_var(df.columns.values)
         else:
-            for row in df.to_dict('records'):
+            for row in df.to_dict("records"):
                 vars += self._row2var(row)
 
         return MetaData(vars)
```

### Comparing `ismn-1.3.3/src/ismn/filecollection.py` & `ismn-1.3.4/src/ismn/filecollection.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,28 @@
 
 import numpy as np
 from tqdm import tqdm
 from typing import Union
 from multiprocessing import Pool, cpu_count
 from operator import itemgetter
 import time
+from typing import Tuple
 
 from ismn.base import IsmnRoot
 from ismn.const import *
 from ismn.filehandlers import DataFile, StaticMetaFile
 from ismn.meta import MetaData, MetaVar, Depth
 
 
 def _read_station_dir(
     root: Union[IsmnRoot, Path, str],
     stat_dir: Union[Path, str],
     temp_root: Path,
     custom_meta_reader: list,
-) -> (dict, list):
+) -> Tuple[dict, list]:
     """
     Parallelizable function to read metadata for files in station dir
     """
     infos = []
 
     if not isinstance(root, IsmnRoot):
         proc_root = True
@@ -121,16 +122,15 @@
     """
 
     metadata_df = pd.read_csv(
         meta_csv_file,
         index_col=0,
         header=[0, 1],
         low_memory=False,
-        engine="c",
-    )
+        engine="c")
 
     # parse date cols as datetime
     for col in ["timerange_from", "timerange_to"]:
         metadata_df[col, "val"] = pd.to_datetime(metadata_df[col, "val"])
 
     lvars = []
     for c in metadata_df.columns:
@@ -329,15 +329,15 @@
             root = IsmnRoot(data_root)
 
         filelist = OrderedDict([])
 
         columns = np.array(list(metadata_df.columns))
 
         for i, row in enumerate(metadata_df.values):
-            #this_nw = row.loc['network', 'val']
+            # this_nw = row.loc['network', 'val']
             vars = np.unique(columns[:-2][:, 0])
             vals = row[:-2].reshape(-1, 3)
 
             metadata = MetaData([
                 MetaVar.from_tuple(
                     (vars[i], vals[i][2], vals[i][0], vals[i][1]))
                 for i in range(len(vars))
@@ -390,15 +390,15 @@
             network = np.atleast_1d(network)
 
         print(f"Found existing ismn metadata in {meta_csv_file}.")
 
         metadata_df = _load_metadata_df(meta_csv_file)
 
         if network is not None:
-            metadata_df = metadata_df[np.isin(metadata_df['network'].values,
+            metadata_df = metadata_df[np.isin(metadata_df["network"].values,
                                               network)]
 
         metadata_df.index = range(len(metadata_df.index))
 
         return cls.from_metadata_df(
             data_root, metadata_df, temp_root=temp_root)
```

### Comparing `ismn-1.3.3/src/ismn/filehandlers.py` & `ismn-1.3.4/src/ismn/filehandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,26 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import pandas as pd
+import warnings
+
+warnings.simplefilter(action="ignore", category=UserWarning)
 from ismn.base import IsmnRoot
 from ismn.components import *
 from ismn import const
 from ismn.const import IsmnFileError
 from ismn.meta import MetaVar, MetaData
 
 from tempfile import gettempdir, TemporaryDirectory
 from pathlib import Path
-
+from typing import Tuple
 
 class IsmnFile(object):
     """
     General base class for data and static metadata files (station csv file)
     in ismn archive.
 
     Attributes
@@ -199,15 +202,14 @@
                      new_name=None) -> np.array:
         """
         Extract a field from the loaded csv metadata
         """
         field_vars = []
 
         if fieldname in data.index:
-
             froms = np.atleast_1d(data.loc[fieldname]["depth_from[m]"])
             tos = np.atleast_1d(data.loc[fieldname]["depth_to[m]"])
             vals = np.atleast_1d(data.loc[fieldname]["value"])
 
             for d_from, d_to, val in zip(froms, tos, vals):
                 d = Depth(d_from, d_to)
                 name = new_name if new_name is not None else fieldname
@@ -270,16 +272,16 @@
             "koeppen_geiger_2007": const.CSV_META_TEMPLATE["climate_KG"],
             "insitu": const.CSV_META_TEMPLATE["climate_insitu"],
         }
 
         for key in lc_dict.keys():
             if key in lc["quantity_source_name"].values:
                 if key != "insitu":
-                    lc_dict[key] = np.int32(lc.loc[lc["quantity_source_name"] ==
-                                                 key]["value"].values[0])
+                    lc_dict[key] = np.int32(lc.loc[lc["quantity_source_name"]
+                                                   == key]["value"].values[0])
                 else:
                     lc_dict[key] = lc.loc[lc["quantity_source_name"] ==
                                           key]["value"].values[0]
                     logging.info(
                         f"insitu land cover classification available: {self.file_path}"
                     )
 
@@ -373,15 +375,15 @@
 
         self.metadata = None
 
         if load_metadata:
             self.metadata = self.read_metadata(best_meta_for_sensor=True)
 
     @staticmethod
-    def __read_lines(filename: Path) -> (list, list, list):
+    def __read_lines(filename: Path) -> Tuple[list, list, list]:
         """
         Read fist and last line from file as list, skips empty lines.
         """
         with filename.open(mode="rb", newline=None) as f:
             lines = f.read().splitlines()
             headr = lines[0].split()
 
@@ -591,17 +593,24 @@
             "date",
             "time",
             varname,
             varname + "_flag",
             varname + "_orig_flag",
         ]
 
-        return self.__read_csv(names, skiprows=1)
+        return self.__read_csv(
+            names=names,
+            usecols=[0, 1, 2, 3, 4],
+            skiprows=1,
+            #sep=" ",
+            low_memory=False,
+            delim_whitespace=True,
+        )
 
-    def __read_csv(self, names=None, usecols=None, skiprows=0):
+    def __read_csv(self, names=None, usecols=None, skiprows=0, **kwargs):
         """
         Read data from csv.
 
         Parameters
         ----------
         names : list, optional (default: None)
             List of column names to use.
@@ -611,32 +620,54 @@
             See pd.read_csv()
 
         Returns
         -------
         data : pd.DataFrame
             Time series.
         """
-        readf = lambda f: pd.read_csv(
+
+        def readf(
             f,
-            skiprows=skiprows,
-            usecols=usecols,
             names=names,
-            delim_whitespace=True,
+            usecols=usecols,
+            skiprows=skiprows,
             parse_dates=[[0, 1]],
             engine="c",
-        )
-        if self.root.zip:
+            **kwargs
+        ):
+            try:
+                return pd.read_csv(
+                    filepath_or_buffer=f,
+                    skiprows=skiprows,
+                    usecols=usecols,
+                    names=names,
+                    parse_dates=parse_dates,
+                    engine=engine,
+                    **kwargs
+                )
+            except pd.errors.ParserError:
+                return pd.read_csv(
+                    filepath_or_buffer=f,
+                    skiprows=skiprows,
+                    usecols=usecols,
+                    names=names,
+                    delim_whitespace=True,
+                    parse_dates=parse_dates,
+                    engine="c",
+                    **kwargs
+                )
 
+        if self.root.zip:
             with TemporaryDirectory(
                     prefix="ismn", dir=self.temp_root) as tempdir:
                 filename = self.root.extract_file(self.file_path, tempdir)
-                data = readf(filename)
+                data = readf(filename, **kwargs)
 
         else:
-            data = readf(self.root.path / self.file_path)
+            data = readf(self.root.path / self.file_path, **kwargs)
 
         data.set_index("date_time", inplace=True)
 
         return data
 
     def read_data(self) -> pd.DataFrame:
         """
```

### Comparing `ismn-1.3.3/src/ismn/interface.py` & `ismn-1.3.4/src/ismn/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,14 @@
             meta_path=None,
             network=None,
             parallel=False,
             keep_loaded_data=False,
             temp_root=gettempdir(),
             custom_meta_reader=None,
     ):
-
         self.climate, self.landcover = KOEPPENGEIGER, LANDCOVER
         self.parallel = parallel
 
         self.root = IsmnRoot(data_path)
 
         self.keep_loaded_data = keep_loaded_data
 
@@ -170,15 +169,16 @@
 
         if not os.path.isfile(meta_csv_file):
             self.__file_collection = IsmnFileCollection.build_from_scratch(
                 self.root,
                 parallel=self.parallel,
                 log_path=meta_path,
                 temp_root=temp_root,
-                custom_meta_readers=self.custom_meta_reader)
+                custom_meta_readers=self.custom_meta_reader,
+            )
             self.__file_collection.to_metadata_csv(meta_csv_file)
 
         self.__file_collection = IsmnFileCollection.from_metadata_csv(
             self.root, meta_csv_file, network=network)
 
         networks = self._collect()
         self.collection = NetworkCollection(networks)
@@ -189,15 +189,14 @@
         """
         Build Networks and fill them with Stations and Sensors and apply
         according filehandlers from filelist for data reading.
         """
         networks = OrderedDict([])
 
         for f in self.__file_collection.iter_filehandlers():  # network_names):
-
             nw_name, st_name, instrument = (
                 f.metadata["network"].val,
                 f.metadata["station"].val,
                 f.metadata["instrument"].val,
             )
 
             if nw_name not in networks:
@@ -268,15 +267,16 @@
             keep_loaded_data=self.keep_loaded_data,
             temp_root=self.temp_root,
             custom_meta_reader=self.custom_meta_reader,
         )
         subset.__file_collection = IsmnFileCollection.from_metadata_df(
             self.root,
             metadata_df=self.metadata.loc[ids, :].copy(),
-            temp_root=self.temp_root)
+            temp_root=self.temp_root,
+        )
         subset.metadata = subset.__file_collection.metadata_df.copy()
         subset.metadata.index = range(len(subset.metadata.index))
         subset.collection = NetworkCollection(subset._collect())
 
         return subset
 
     @deprecated
@@ -548,15 +548,15 @@
         else:
             data = []
             metadata = []
             for i in idx:
                 filehandler = self.__file_collection.get_filehandler(i)
                 d = filehandler.read_data()
                 d.columns = pd.MultiIndex.from_product(
-                    [[i], list(d.columns)], names=['idx', 'variable'])
+                    [[i], list(d.columns)], names=["idx", "variable"])
                 data.append(d)
                 if return_meta:
                     m = filehandler.metadata.to_pd()
                     m = pd.DataFrame(data={i: m})
                     metadata.append(m)
 
             data = pd.concat(data, axis=1)
@@ -765,28 +765,28 @@
 
         if stats_text:
             text = ax.text(
                 0.5,
                 1.05,
                 feedback,
                 transform=ax.transAxes,
-                fontsize=5 * text_scalefactor,  #"xx-small",
+                fontsize=5 * text_scalefactor,  # "xx-small",
                 horizontalalignment="center",
             )
         else:
             text = None
 
         if fig:
             fig.set_size_inches([6, 3.5 + (0.25 * text_scalefactor) * nrows])
 
         if filename is not None:
             fig.savefig(
                 filename,
                 bbox_extra_artists=(lgd, text) if stats_text else (lgd),
-                bbox_inches='tight',
+                bbox_inches="tight",
                 dpi=dpi,
             )
         else:
             counts = (len(act_networks), len(act_stations), n_sens)
             return fig, ax, counts
 
     def get_min_max_obs_timestamps(
@@ -837,15 +837,14 @@
         t_max = None
 
         for net, stat, sens in self.collection.iter_sensors(
                 variable=variable,
                 depth=Depth(min_depth, max_depth),
                 filter_meta_dict=filter_meta_dict,
         ):
-
             time_from = pd.Timestamp(sens.metadata["timerange_from"].val)
             time_to = pd.Timestamp(sens.metadata["timerange_to"].val)
 
             if t_min is None:
                 t_min = time_from
             if t_max is None:
                 t_max = time_to
```

### Comparing `ismn-1.3.3/src/ismn/meta.py` & `ismn-1.3.4/src/ismn/meta.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/src/ismn.egg-info/PKG-INFO` & `ismn-1.3.4/src/ismn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ismn
-Version: 1.3.3
+Version: 1.3.4
 Summary: Readers for the data from the International Soil Moisture Database
 Home-page: http://ismn.geo.tuwien.ac.at
 Author: TU Wien
 Author-email: ismn@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, https://ismn.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `ismn-1.3.3/src/ismn.egg-info/SOURCES.txt` & `ismn-1.3.4/src/ismn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/baseline/test_interface_plotting.png` & `ismn-1.3.4/tests/baseline/test_interface_plotting.png`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_base.py` & `ismn-1.3.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_components.py` & `ismn-1.3.4/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_custom_meta.py` & `ismn-1.3.4/tests/test_custom_meta.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm` & `ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv` & `ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm` & `ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv` & `ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_sm_0.050000_0.050000_ThetaProbe-ML2X_19500101_20210131.stm` & `ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_sm_0.050000_0.050000_ThetaProbe-ML2X_19500101_20210131.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_static_variables.csv` & `ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809/Metadata.xml` & `ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809/Metadata.xml`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_20170810_20180809.zip` & `ismn-1.3.4/tests/test_data/Data_seperate_files_20170810_20180809.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm` & `ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv` & `ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm` & `ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv` & `ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/Data_seperate_files_header_20170810_20180809/Metadata.xml` & `ismn-1.3.4/tests/test_data/Data_seperate_files_header_20170810_20180809/Metadata.xml`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/format_ceop_sep/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm` & `ismn-1.3.4/tests/test_data/format_ceop_sep/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/format_header_values/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm` & `ismn-1.3.4/tests/test_data/format_header_values/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/zip_archives/ceop/Data_seperate_files_20170810_20180809.zip` & `ismn-1.3.4/tests/test_data/zip_archives/ceop/Data_seperate_files_20170810_20180809.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/zip_archives/format_header_values/Data_SMOSMANIA.zip` & `ismn-1.3.4/tests/test_data/zip_archives/format_header_values/Data_SMOSMANIA.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/zip_archives/header/Data_seperate_files_header_20170810_20180809.zip` & `ismn-1.3.4/tests/test_data/zip_archives/header/Data_seperate_files_header_20170810_20180809.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_data/zip_archives/multinetwork/header_values/Data_header_values.zip` & `ismn-1.3.4/tests/test_data/zip_archives/multinetwork/header_values/Data_header_values.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_depth.py` & `ismn-1.3.4/tests/test_depth.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_filecollection.py` & `ismn-1.3.4/tests/test_filecollection.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_filehandler_data.py` & `ismn-1.3.4/tests/test_filehandler_data.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_filehandler_static.py` & `ismn-1.3.4/tests/test_filehandler_static.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_interface.py` & `ismn-1.3.4/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_meta.py` & `ismn-1.3.4/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ismn-1.3.3/tests/test_readers.py` & `ismn-1.3.4/tests/test_readers.py`

 * *Files identical despite different names*

