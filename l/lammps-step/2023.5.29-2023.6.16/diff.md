# Comparing `tmp/lammps_step-2023.5.29.tar.gz` & `tmp/lammps_step-2023.6.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammps_step-2023.5.29.tar", last modified: Mon May 29 19:08:16 2023, max compression
+gzip compressed data, was "lammps_step-2023.6.16.tar", last modified: Fri Jun 16 17:31:31 2023, max compression
```

## Comparing `lammps_step-2023.5.29.tar` & `lammps_step-2023.6.16.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.941673 lammps_step-2023.5.29/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.945673 lammps_step-2023.5.29/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.945673 lammps_step-2023.5.29/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9562 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.945673 lammps_step-2023.5.29/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.953673 lammps_step-2023.5.29/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)  2437613 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/density.png
--rw-r--r--   0 runner    (1001) docker     (123)   175972 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/edit_forcefield.png
--rw-r--r--   0 runner    (1001) docker     (123)   312162 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/edit_initialization.png
--rw-r--r--   0 runner    (1001) docker     (123)   877297 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/edit_npt.png
--rw-r--r--   0 runner    (1001) docker     (123)   575423 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/edit_packmol.png
--rw-r--r--   0 runner    (1001) docker     (123)   408930 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   220257 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/lammps_flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)   148973 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/nist.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.953673 lammps_step-2023.5.29/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/lammps_step/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      492 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/lammps_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/custom_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/lammps_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/data/seamm-lammps.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/heat_flux_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/heat_flux_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/initialization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/initialization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    91984 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/lammps_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/lammps_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/minimization.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/minimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    23933 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/npt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/npt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/npt_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nve_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nve_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nvt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nvt_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_minimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    30919 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_npt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_nve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/velocities_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/velocities_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.965673 lammps_step-2023.5.29/lammps_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:07:59.000000 lammps_step-2023.5.29/lammps_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/tests/data/Ar_xtal_energy.flow
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/tests/test_lammps_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/tests/test_lammps_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.890614 lammps_step-2023.6.16/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.890614 lammps_step-2023.6.16/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.890614 lammps_step-2023.6.16/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9562 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.894614 lammps_step-2023.6.16/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.902614 lammps_step-2023.6.16/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)  2437613 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/density.png
+-rw-r--r--   0 runner    (1001) docker     (123)   175972 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/edit_forcefield.png
+-rw-r--r--   0 runner    (1001) docker     (123)   312162 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/edit_initialization.png
+-rw-r--r--   0 runner    (1001) docker     (123)   877297 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/edit_npt.png
+-rw-r--r--   0 runner    (1001) docker     (123)   575423 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/edit_packmol.png
+-rw-r--r--   0 runner    (1001) docker     (123)   408930 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   220257 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/lammps_flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148973 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/nist.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.902614 lammps_step-2023.6.16/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.922614 lammps_step-2023.6.16/lammps_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      492 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 17:31:31.922614 lammps_step-2023.6.16/lammps_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/custom_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/lammps_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/data/seamm-lammps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/heat_flux_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/heat_flux_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/initialization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/initialization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91984 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/lammps_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/lammps_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/minimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/minimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23933 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/npt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/npt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/npt_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nve_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nve_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nvt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nvt_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_minimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30919 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_npt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_nve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/velocities_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/velocities_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/lammps_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:31:19.000000 lammps_step-2023.6.16/lammps_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 17:31:31.922614 lammps_step-2023.6.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/tests/data/Ar_xtal_energy.flow
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/tests/test_lammps_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/tests/test_lammps_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/versioneer.py
```

### Comparing `lammps_step-2023.5.29/CONTRIBUTING.rst` & `lammps_step-2023.6.16/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/HISTORY.rst` & `lammps_step-2023.6.16/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 =======
 History
 =======
+2023.6.16 -- Heat flux with PCFF
+   * centroid/stress/atom does not work with Class 2 forcefields, so don't use for PCFF.
 2023.5.29 -- Self diffusion and other improvements
    * Added trajectory panel to support diffusion, viscosity and simple thermal
      conductivity.
    * Added support for separate GPU versions of LAMMPS.
    * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
    * Added support for using modules.
```

### Comparing `lammps_step-2023.5.29/LICENSE` & `lammps_step-2023.6.16/LICENSE`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/PKG-INFO` & `lammps_step-2023.6.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps_step
-Version: 2023.5.29
+Version: 2023.6.16
 Summary: A SEAMM plug-in for LAMMPS, a forcefield-based molecular dynamics code.
 Home-page: https://github.com/molssi-seamm/lammps_step
 Author: MolSSI @ Virginia Tech
 Author-email: seamm@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM,molecular dynamics,atomistic,MD
 Platform: Linux
@@ -109,14 +109,16 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.6.16 -- Heat flux with PCFF
+   * centroid/stress/atom does not work with Class 2 forcefields, so don't use for PCFF.
 2023.5.29 -- Self diffusion and other improvements
    * Added trajectory panel to support diffusion, viscosity and simple thermal
      conductivity.
    * Added support for separate GPU versions of LAMMPS.
    * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
    * Added support for using modules.
```

### Comparing `lammps_step-2023.5.29/README.rst` & `lammps_step-2023.6.16/README.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/Makefile` & `lammps_step-2023.6.16/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/_static/SEAMM inverted.png` & `lammps_step-2023.6.16/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/_static/SEAMM logo.png` & `lammps_step-2023.6.16/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/_static/molssi_main_logo.png` & `lammps_step-2023.6.16/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/_static/molssi_main_logo_inverted_white.png` & `lammps_step-2023.6.16/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/_static/molssi_square.png` & `lammps_step-2023.6.16/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/_static/nsf.png` & `lammps_step-2023.6.16/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/conf.py` & `lammps_step-2023.6.16/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/developer_guide/installation.rst` & `lammps_step-2023.6.16/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/density.png` & `lammps_step-2023.6.16/docs/getting_started/density.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/edit_forcefield.png` & `lammps_step-2023.6.16/docs/getting_started/edit_forcefield.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/edit_initialization.png` & `lammps_step-2023.6.16/docs/getting_started/edit_initialization.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/edit_npt.png` & `lammps_step-2023.6.16/docs/getting_started/edit_npt.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/edit_packmol.png` & `lammps_step-2023.6.16/docs/getting_started/edit_packmol.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/flowchart.png` & `lammps_step-2023.6.16/docs/getting_started/flowchart.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/index.rst` & `lammps_step-2023.6.16/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/lammps_flowchart.png` & `lammps_step-2023.6.16/docs/getting_started/lammps_flowchart.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/getting_started/nist.png` & `lammps_step-2023.6.16/docs/getting_started/nist.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/index.rst` & `lammps_step-2023.6.16/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/docs/make.bat` & `lammps_step-2023.6.16/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/__init__.py` & `lammps_step-2023.6.16/lammps_step/__init__.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/custom.py` & `lammps_step-2023.6.16/lammps_step/custom.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/custom_parameters.py` & `lammps_step-2023.6.16/lammps_step/custom_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/custom_step.py` & `lammps_step-2023.6.16/lammps_step/custom_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/data/configuration.txt` & `lammps_step-2023.6.16/lammps_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/data/properties.csv` & `lammps_step-2023.6.16/lammps_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/data/references.bib` & `lammps_step-2023.6.16/lammps_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/energy.py` & `lammps_step-2023.6.16/lammps_step/energy.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/energy_parameters.py` & `lammps_step-2023.6.16/lammps_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/energy_step.py` & `lammps_step-2023.6.16/lammps_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/heat_flux.py` & `lammps_step-2023.6.16/lammps_step/heat_flux.py`

 * *Files 13% similar despite different names*

```diff
@@ -90,14 +90,61 @@
 parser = argparse.ArgumentParser()
 parser.add_argument("--cmd-args", help="Command line arguments for LAMMPS")
 kwords = vars(parser.parse_args())
 
 run_thermal_conductivity(**kwords)
 """
 
+script2 = """\
+#!/usr/bin/env python
+
+import argparse
+import sys
+
+from lammps import lammps, LMP_STYLE_ATOM, LMP_TYPE_VECTOR, LMP_TYPE_ARRAY
+from mpi4py import MPI
+import numpy as np
+
+def J_filter_cb(lmp, ntimestep, nlocal, ids, xyz, fext, args = []):
+    # Set forces to 0.0
+    fext.fill(0.0)
+
+    # update energy
+    PE0 = lmp.numpy.extract_fix("PE_ave", LMP_STYLE_ATOM, LMP_TYPE_VECTOR)
+    lmp.numpy.fix_external_set_energy_peratom("J_filter", -PE0);
+
+    # and stress
+    S_p0 = lmp.numpy.extract_fix("S_p_ave", LMP_STYLE_ATOM, LMP_TYPE_ARRAY)
+
+    S = np.reshape(S_p0, (nlocal, 6))
+
+    lmp.numpy.fix_external_set_virial_peratom("J_filter", -S)
+
+def run_thermal_conductivity(cmd_args=None):
+    if cmd_args is None:
+        lmp = lammps()
+    else:
+        lmp = lammps(cmdargs=cmd_args.split())
+    lmp.file("lammps.dat")
+
+    lmp.set_fix_external_callback("J_filter", J_filter_cb, lmp)
+
+    lmp.file("lammps_post.dat")
+
+    lmp.close()
+    lmp.finalize()
+
+# Get any arguments
+parser = argparse.ArgumentParser()
+parser.add_argument("--cmd-args", help="Command line arguments for LAMMPS")
+kwords = vars(parser.parse_args())
+
+run_thermal_conductivity(**kwords)
+"""
+
 
 class HeatFlux(NVE):
     """
     The non-graphical part of a Heat Flux step in a flowchart.
 
     Attributes
     ----------
@@ -197,14 +244,20 @@
             "heat flux will be sampled every {sampling}."
         )
 
         return self.header + "\n" + __(text, **P, indent=4 * " ").__str__()
 
     def get_input(self, extras=None):
         """Get the input for a heat flux run in LAMMPS"""
+        # See what type of forcefield we have and handle it
+        ff = self.get_variable("_forcefield")
+        if ff == "OpenKIM":
+            ffname = ""
+        else:
+            ffname = ff.current_forcefield
 
         self.description = []
 
         P = self.parameters.current_values_to_dict(
             context=seamm.flowchart_variables._data
         )
 
@@ -252,16 +305,83 @@
         # Unit conversion factor
         if lammps_step.get_lammps_unit_system() == "metal":
             factor = Q_("eV/Å^2/ps")
         else:
             factor = Q_("kcal/Å^2/fs/mol") / Q_("kcal/mol") * Q_("kcal/mol").to("kJ")
         factor = factor.m_as("W/m^2")
 
-        lines.append(
-            f"""
+        if "cff" in ffname:
+            # Centroid/stress/atom does not handle class2 ff ... cross-terms?
+            lines.append(
+                f"""
+#          Green-Kubo method
+
+fix                 dynamics all nve
+
+compute             KE all ke/atom
+compute             PE all pe/atom
+
+#          centroid doesn't work with kspace, so split into pair and non-pair parts
+
+compute             S_p all stress/atom NULL virial
+compute             flux_p all heat/flux KE PE S_p
+
+#          An initial run to settle things down.
+
+run                 1000 post no
+
+#          A run to get the averages for PE and S for scheme 2
+
+fix                 ave all ave/atom 1 1000 1000 c_PE
+fix                 p_ave all ave/atom 1 1000 1000 c_S_p[1] c_S_p[2] c_S_p[3] &
+                                                   c_S_p[4] c_S_p[5] c_S_p[6]
+
+run                 1000 post no
+
+fix                 PE_ave all store/state 0 f_ave
+fix                 S_p_ave all store/state 0 f_p_ave[1] f_p_ave[2] f_p_ave[3] &
+                                              f_p_ave[4] f_p_ave[5] f_p_ave[6]
+
+#          Store the initial values for scheme 1
+
+fix                 PE0 all store/state 0 c_PE
+fix                 S_p0 all store/state 0 c_S_p[1] c_S_p[2] c_S_p[3] &
+                                           c_S_p[4] c_S_p[5] c_S_p[6]
+
+#          The run is need to capture the store/state fixes
+
+run                 0
+
+unfix               p_ave
+unfix               ave
+
+reset_timestep      0
+
+#          Conversion from kcal/Å^2/fs/mol to W/m^2")
+
+variable            factor equal {factor}
+variable            Jx equal v_factor*c_flux_p[1]/vol
+variable            Jy equal v_factor*c_flux_p[2]/vol
+variable            Jz equal v_factor*c_flux_p[3]/vol
+
+#          The thermo output
+
+thermo              {nsteps // 100}
+thermo_style        custom {thermo_properties}
+
+#          The external fix to adjust the peratom PE and S
+
+fix                 J_filter all external pf/callback 1 1
+fix_modify          J_filter energy yes
+fix_modify          J_filter virial yes
+"""
+            )
+        else:
+            lines.append(
+                f"""
 #          Green-Kubo method
 
 fix                 dynamics all nve
 
 compute             KE all ke/atom
 compute             PE all pe/atom
 
@@ -327,15 +447,15 @@
 
 #          The external fix to adjust the peratom PE and S
 
 fix                 J_filter all external pf/callback 1 1
 fix_modify          J_filter energy yes
 fix_modify          J_filter virial yes
 """
-        )
+            )
 
         # instantaneous output written for averaging
         if P["sampling"] == "none":
             self.description.append(
                 __(
                     "The run will be {nsteps:n} steps of dynamics.",
                     nsteps=nsteps,
@@ -377,52 +497,14 @@
                         "sampled every {nevery:n} steps."
                     ),
                     nsteps=nsteps,
                     nevery=nevery,
                     indent=7 * " ",
                 )
             )
-        # # handling of trajectory
-        # nevery = max(1, round(sampling / timestep))
-        # nrepeat = 1
-        # nfreq = nevery * nrepeat
-        # properties = "v_time v_temp v_etotal v_ke v_pe v_Jx v_Jy v_Jz "
-        # filename = f"@{self._id[-1]}+heat_flux_state.trj"
-
-        # dt = (nevery * P["timestep"]).to_compact()
-        # text = json.dumps(
-        #     {
-        #         "code": "LAMMPS",
-        #         "type": "NVE",
-        #         "dt": dt.magnitude,
-        #         "tunits": str(dt.u),
-        #         "nsteps": nsteps // nevery,
-        #     },
-        #     separators=(",", ":"),
-        # )
-        # title1 = "!MolSSI trajectory 2.0 " + text
-        # title2 = "tstep t T Etot Eke Epe Jx Jy Jz "
-        # lines.append(
-        #     f"fix                 trajectory all ave/time {nevery} 1 {nfreq} &\n"
-        #     f"                       {properties} &\n"
-        #     "                       off 2 &\n"
-        #     f"                       title1 '{title1}' &\n"
-        #     f"                       title2 '{title2}' &\n"
-        #     f"                       file {filename}"
-        # )
-
-        # self.description.append(
-        #     __(
-        #         "The run will be {nsteps:,d} steps of dynamics "
-        #         "sampled every {nevery:n} steps.",
-        #         nsteps=nsteps,
-        #         nevery=nevery,
-        #         indent=7 * " ",
-        #     )
-        # )
 
         nevery = 10
         nfreq = int(nsteps / 10)
         nrepeat = int(nfreq / nevery)
         nfreq = nevery * nrepeat
 
         filename = f"@{self._id[-1]}+heat_flux_summary.trj"
@@ -482,13 +564,21 @@
         for n in range(1, nfixes + 1):
             post_lines.append(f"unfix               {n}")
         for n in range(1, ncomputes + 1):
             post_lines.append(f"uncompute           {n}")
         for n in range(1, ndumps + 1):
             post_lines.append(f"undump              {n}")
 
-        return {
-            "script": lines,
-            "postscript": post_lines,
-            "use python": True,
-            "python script": script,
-        }
+        if "cff" in ffname:
+            return {
+                "script": lines,
+                "postscript": post_lines,
+                "use python": True,
+                "python script": script2,
+            }
+        else:
+            return {
+                "script": lines,
+                "postscript": post_lines,
+                "use python": True,
+                "python script": script,
+            }
```

### Comparing `lammps_step-2023.5.29/lammps_step/heat_flux_parameters.py` & `lammps_step-2023.6.16/lammps_step/heat_flux_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/heat_flux_step.py` & `lammps_step-2023.6.16/lammps_step/heat_flux_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/initialization.py` & `lammps_step-2023.6.16/lammps_step/initialization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/initialization_parameters.py` & `lammps_step-2023.6.16/lammps_step/initialization_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/initialization_step.py` & `lammps_step-2023.6.16/lammps_step/initialization_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/installer.py` & `lammps_step-2023.6.16/lammps_step/installer.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/lammps.py` & `lammps_step-2023.6.16/lammps_step/lammps.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/lammps_step.py` & `lammps_step-2023.6.16/lammps_step/lammps_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/lammps_units.py` & `lammps_step-2023.6.16/lammps_step/lammps_units.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/metadata.py` & `lammps_step-2023.6.16/lammps_step/metadata.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/minimization.py` & `lammps_step-2023.6.16/lammps_step/minimization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/minimization_step.py` & `lammps_step-2023.6.16/lammps_step/minimization_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/npt.py` & `lammps_step-2023.6.16/lammps_step/npt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/npt_parameters.py` & `lammps_step-2023.6.16/lammps_step/npt_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/npt_step.py` & `lammps_step-2023.6.16/lammps_step/npt_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/nve.py` & `lammps_step-2023.6.16/lammps_step/nve.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/nve_parameters.py` & `lammps_step-2023.6.16/lammps_step/nve_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/nve_step.py` & `lammps_step-2023.6.16/lammps_step/nve_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/nvt.py` & `lammps_step-2023.6.16/lammps_step/nvt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/nvt_parameters.py` & `lammps_step-2023.6.16/lammps_step/nvt_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/nvt_step.py` & `lammps_step-2023.6.16/lammps_step/nvt_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_custom.py` & `lammps_step-2023.6.16/lammps_step/tk_custom.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_energy.py` & `lammps_step-2023.6.16/lammps_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_heat_flux.py` & `lammps_step-2023.6.16/lammps_step/tk_heat_flux.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_initialization.py` & `lammps_step-2023.6.16/lammps_step/tk_initialization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_lammps.py` & `lammps_step-2023.6.16/lammps_step/tk_lammps.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_minimization.py` & `lammps_step-2023.6.16/lammps_step/tk_minimization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_npt.py` & `lammps_step-2023.6.16/lammps_step/tk_npt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_nve.py` & `lammps_step-2023.6.16/lammps_step/tk_nve.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_nvt.py` & `lammps_step-2023.6.16/lammps_step/tk_nvt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/tk_velocities.py` & `lammps_step-2023.6.16/lammps_step/tk_velocities.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/velocities.py` & `lammps_step-2023.6.16/lammps_step/velocities.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/velocities_parameters.py` & `lammps_step-2023.6.16/lammps_step/velocities_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step/velocities_step.py` & `lammps_step-2023.6.16/lammps_step/velocities_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step.egg-info/PKG-INFO` & `lammps_step-2023.6.16/lammps_step.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps-step
-Version: 2023.5.29
+Version: 2023.6.16
 Summary: A SEAMM plug-in for LAMMPS, a forcefield-based molecular dynamics code.
 Home-page: https://github.com/molssi-seamm/lammps_step
 Author: MolSSI @ Virginia Tech
 Author-email: seamm@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM,molecular dynamics,atomistic,MD
 Platform: Linux
@@ -109,14 +109,16 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.6.16 -- Heat flux with PCFF
+   * centroid/stress/atom does not work with Class 2 forcefields, so don't use for PCFF.
 2023.5.29 -- Self diffusion and other improvements
    * Added trajectory panel to support diffusion, viscosity and simple thermal
      conductivity.
    * Added support for separate GPU versions of LAMMPS.
    * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
    * Added support for using modules.
```

### Comparing `lammps_step-2023.5.29/lammps_step.egg-info/SOURCES.txt` & `lammps_step-2023.6.16/lammps_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/lammps_step.egg-info/entry_points.txt` & `lammps_step-2023.6.16/lammps_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/setup.py` & `lammps_step-2023.6.16/setup.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/tests/data/Ar_xtal_energy.flow` & `lammps_step-2023.6.16/tests/data/Ar_xtal_energy.flow`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/tests/test_lammps_step.py` & `lammps_step-2023.6.16/tests/test_lammps_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/tests/test_lammps_units.py` & `lammps_step-2023.6.16/tests/test_lammps_units.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.5.29/versioneer.py` & `lammps_step-2023.6.16/versioneer.py`

 * *Files identical despite different names*

