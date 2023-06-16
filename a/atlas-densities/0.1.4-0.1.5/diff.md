# Comparing `tmp/atlas-densities-0.1.4.tar.gz` & `tmp/atlas-densities-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-densities-0.1.4.tar", last modified: Tue Apr 11 08:53:26 2023, max compression
+gzip compressed data, was "atlas-densities-0.1.5.tar", last modified: Fri Jun 16 06:49:17 2023, max compression
```

## Comparing `atlas-densities-0.1.4.tar` & `atlas-densities-0.1.5.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.761378 atlas-densities-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.717378 atlas-densities-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-04-11 08:53:26.761378 atlas-densities-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    55115 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas-densities.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/atlas_densities/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/atlas_densities/app/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40078 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/cell_densities.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.725378 atlas-densities-0.1.4/atlas_densities/app/data/
--rw-r--r--   0 runner    (1001) docker     (123)   637735 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/1.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.725378 atlas-densities-0.1.4/atlas_densities/app/data/markers/
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/realigned_slices_bbp.json
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/realigned_slices_ccfv2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/measurements/
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59787 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/gaba_papers.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/homogenous_regions.csv
--rw-r--r--   0 runner    (1001) docker     (123)   839727 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/measurements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   347207 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/mmc1.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   291827 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/mmc3.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/non_density_measurements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   199258 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/std_cells.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/ca1_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/excitatory-inhibitory-splitting.json
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/isocortex_23_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/isocortex_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/thalamus_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/composition.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/meta/layers.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.737378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_DAC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_HAC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_LAC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-DA.dat
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-SA.dat
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_SAC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_SSC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_TPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TPC-C.dat
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_BPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_HPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-C.dat
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.737378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/probability_map.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/mtype_densities.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.737378 atlas-densities-0.1.4/atlas_densities/combination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/combination/annotations_combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/combination/markers_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.745378 atlas-densities-0.1.4/atlas_densities/densities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/cell_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/cell_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/excitatory_inhibitory_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/glia_densities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_densities_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    33784 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_densities_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/measurement_to_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    22055 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    21524 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/refined_inhibitory_neuron_densities.py
--rw-r--r--   0 runner    (1001) docker     (123)    26913 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/atlas_densities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.745378 atlas-densities-0.1.4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.749378 atlas-densities-0.1.4/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)   230179 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/bbpp82_628_linear_program.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/cell_densities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/combination.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/mtype_densities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:53:26.761378 atlas-densities-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.749378 atlas-densities-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   637735 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/1.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.753378 atlas-densities-0.1.4/tests/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/test_cell_densities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/test_mtype_densities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/test_refined_inhibitory_neuron_densities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.753378 atlas-densities-0.1.4/tests/combination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/combination/test_annotations_combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/combination/test_markers_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.757378 atlas-densities-0.1.4/tests/densities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/tests/densities/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.757378 atlas-densities-0.1.4/tests/densities/data/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/meta/layers.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/meta/mapping.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/meta/mapping_exc_only.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.761378 atlas-densities-0.1.4/tests/densities/data/mtypes/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/BP.dat
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/L2_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/L2_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/L3_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/L3_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/mtype-taxonomy.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_cell_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_excitatory_inhibitory_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_glia_densities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_densities_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_density_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_measurement_to_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    25302 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_optimization_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_refined_inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/markers_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/mocking_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.747795 atlas-densities-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.727795 atlas-densities-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.731795 atlas-densities-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23443 2023-06-16 06:49:17.747795 atlas-densities-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    55115 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas-densities.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.731795 atlas-densities-0.1.5/atlas_densities/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.731795 atlas-densities-0.1.5/atlas_densities/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40078 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/cell_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.731795 atlas-densities-0.1.5/atlas_densities/app/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   637735 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.731795 atlas-densities-0.1.5/atlas_densities/app/data/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/markers/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/markers/realigned_slices_bbp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/markers/realigned_slices_ccfv2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.735795 atlas-densities-0.1.5/atlas_densities/app/data/measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/measurements/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59787 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/measurements/gaba_papers.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/measurements/homogenous_regions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   839727 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/measurements/measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   347207 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/measurements/mmc1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   291827 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/measurements/mmc3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/measurements/non_density_measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   199258 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/measurements/std_cells.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.735795 atlas-densities-0.1.5/atlas_densities/app/data/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/metadata/ca1_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/metadata/excitatory-inhibitory-splitting.json
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/metadata/isocortex_23_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/metadata/isocortex_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/metadata/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/metadata/thalamus_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.735795 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.735795 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/composition/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/composition/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/composition/composition.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.735795 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.735795 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/meta/layers.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.739795 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_DAC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_HAC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_LAC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-DA.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-SA.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_SAC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_SSC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_TPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TPC-C.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_BPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_HPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-C.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.739795 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/probability_map/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/probability_map/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/data/mtypes/probability_map/probability_map.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20270 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/mtype_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.739795 atlas-densities-0.1.5/atlas_densities/combination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/combination/annotations_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/combination/markers_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.743795 atlas-densities-0.1.5/atlas_densities/densities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/cell_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25664 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/excitatory_inhibitory_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/glia_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/inhibitory_neuron_densities_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33784 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/inhibitory_neuron_densities_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/measurement_to_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/mtype_densities_from_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/mtype_densities_from_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22055 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/mtype_densities_from_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21524 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/refined_inhibitory_neuron_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26913 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/densities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/atlas_densities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.731795 atlas-densities-0.1.5/atlas_densities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23443 2023-06-16 06:49:17.000000 atlas-densities-0.1.5/atlas_densities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-16 06:49:17.000000 atlas-densities-0.1.5/atlas_densities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:49:17.000000 atlas-densities-0.1.5/atlas_densities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 06:49:17.000000 atlas-densities-0.1.5/atlas_densities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 06:49:17.000000 atlas-densities-0.1.5/atlas_densities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 06:49:17.000000 atlas-densities-0.1.5/atlas_densities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.743795 atlas-densities-0.1.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.743795 atlas-densities-0.1.5/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)   230179 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/bbpp82_628_linear_program.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/cell_densities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/combination.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/mtype_densities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/doc/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:49:17.747795 atlas-densities-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.743795 atlas-densities-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   637735 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.743795 atlas-densities-0.1.5/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/app/test_cell_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/app/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/app/test_mtype_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/app/test_refined_inhibitory_neuron_densities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.743795 atlas-densities-0.1.5/tests/combination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/combination/test_annotations_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/combination/test_markers_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.747795 atlas-densities-0.1.5/tests/densities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.727795 atlas-densities-0.1.5/tests/densities/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.747795 atlas-densities-0.1.5/tests/densities/data/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/meta/layers.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/meta/mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/meta/mapping_exc_only.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:49:17.747795 atlas-densities-0.1.5/tests/densities/data/mtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/mtypes/BP.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/mtypes/L2_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/mtypes/L2_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/mtypes/L3_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/mtypes/L3_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/data/mtypes/mtype-taxonomy.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_cell_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_excitatory_inhibitory_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_glia_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_inhibitory_neuron_densities_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_inhibitory_neuron_density_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_measurement_to_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_mtype_densities_from_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_mtype_densities_from_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_mtype_densities_from_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25302 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_optimization_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_refined_inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/densities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/markers_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/mocking_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 06:49:12.000000 atlas-densities-0.1.5/tox.ini
```

### Comparing `atlas-densities-0.1.4/.github/workflows/publish-sdist.yml` & `atlas-densities-0.1.5/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/.github/workflows/run-tox.yml` & `atlas-densities-0.1.5/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/.pylintrc` & `atlas-densities-0.1.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/CHANGELOG.rst` & `atlas-densities-0.1.5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/CONTRIBUTING.rst` & `atlas-densities-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/LICENSE.txt` & `atlas-densities-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/PKG-INFO` & `atlas-densities-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-densities
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library containing command lines and tools to compute volumetric cell densities in the rodent brain
 Home-page: https://github.com/BlueBrain/atlas-densities
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-densities
 Description: .. image:: atlas-densities.jpg
         
@@ -344,34 +344,24 @@
                 --metadata-path=$DATA/metadata/isocortex_23_metadata.json            \
                 --mtypes-config-path=$DATA/mtypes/mtypes_probability_map_config.yaml \
                 --output-dir=data/ccfv2/me-types/
         
         Subdivide excitatory files into pyramidal subtypes
         --------------------------------------------------
         
-        This should run after the ME mapping from Roussel. To run:
+        This should run after the inhibitory/excitatory computation above. To run:
         
-        make_new_inhib_exc_outside_SSCX.py
-        
-        Input support files needed:
-        
-        annotation atlas (with L23 split): brain_regions.nrrd
-        
-        annotation hierarchy (with L23 split): hierarchy.json
-        
-        inhibitory: gad67+_density_v3_MMB.nrrd
-        
-        total neuron: neuron_density_v3_MMB.nrrd
-        
-        Output:
-        
-        excitatory nrrd files in output directory
-        
-        inhibitory minus cortex in output directory
+        .. code-block:: bash
         
+            atlas-densities cell-densities excitatory-split                         \
+                --annotation-path=data/ccfv2/annotation_25.nrrd                     \
+                --hierarchy-path=data/1.json                                        \
+                --neuron-density=data/ccfv2/density_volumes/neuron_density.nrrd     \
+                --inhibitory-density=data/ccfv2/density_volumes/gad67+_density.nrrd \
+                --output-dir=data/ccfv2/excitatory_split
         
         Instructions for developers
         ===========================
         
         Run the following commands before submitting your code for review:
         
         .. code-block:: bash
```

### Comparing `atlas-densities-0.1.4/README.rst` & `atlas-densities-0.1.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -336,34 +336,24 @@
         --metadata-path=$DATA/metadata/isocortex_23_metadata.json            \
         --mtypes-config-path=$DATA/mtypes/mtypes_probability_map_config.yaml \
         --output-dir=data/ccfv2/me-types/
 
 Subdivide excitatory files into pyramidal subtypes
 --------------------------------------------------
 
-This should run after the ME mapping from Roussel. To run:
+This should run after the inhibitory/excitatory computation above. To run:
 
-make_new_inhib_exc_outside_SSCX.py
-
-Input support files needed:
-
-annotation atlas (with L23 split): brain_regions.nrrd
-
-annotation hierarchy (with L23 split): hierarchy.json
-
-inhibitory: gad67+_density_v3_MMB.nrrd
-
-total neuron: neuron_density_v3_MMB.nrrd
-
-Output:
-
-excitatory nrrd files in output directory
-
-inhibitory minus cortex in output directory
+.. code-block:: bash
 
+    atlas-densities cell-densities excitatory-split                         \
+        --annotation-path=data/ccfv2/annotation_25.nrrd                     \
+        --hierarchy-path=data/1.json                                        \
+        --neuron-density=data/ccfv2/density_volumes/neuron_density.nrrd     \
+        --inhibitory-density=data/ccfv2/density_volumes/gad67+_density.nrrd \
+        --output-dir=data/ccfv2/excitatory_split
 
 Instructions for developers
 ===========================
 
 Run the following commands before submitting your code for review:
 
 .. code-block:: bash
```

### Comparing `atlas-densities-0.1.4/atlas-densities.jpg` & `atlas-densities-0.1.5/atlas-densities.jpg`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/cell_densities.py` & `atlas-densities-0.1.5/atlas_densities/app/cell_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/cli.py` & `atlas-densities-0.1.5/atlas_densities/app/cli.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/combination.py` & `atlas-densities-0.1.5/atlas_densities/app/combination.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/1.json` & `atlas-densities-0.1.5/atlas_densities/app/data/1.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/markers/README.rst` & `atlas-densities-0.1.5/atlas_densities/app/data/markers/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml` & `atlas-densities-0.1.5/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/markers/realigned_slices_bbp.json` & `atlas-densities-0.1.5/atlas_densities/app/data/markers/realigned_slices_bbp.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/markers/realigned_slices_ccfv2.json` & `atlas-densities-0.1.5/atlas_densities/app/data/markers/realigned_slices_ccfv2.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/measurements/README.rst` & `atlas-densities-0.1.5/atlas_densities/app/data/measurements/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/measurements/gaba_papers.xlsx` & `atlas-densities-0.1.5/atlas_densities/app/data/measurements/gaba_papers.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/measurements/homogenous_regions.csv` & `atlas-densities-0.1.5/atlas_densities/app/data/measurements/homogenous_regions.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/measurements/measurements.csv` & `atlas-densities-0.1.5/atlas_densities/app/data/measurements/measurements.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/measurements/mmc1.xlsx` & `atlas-densities-0.1.5/atlas_densities/app/data/measurements/mmc1.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/measurements/mmc3.xlsx` & `atlas-densities-0.1.5/atlas_densities/app/data/measurements/mmc3.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/measurements/non_density_measurements.csv` & `atlas-densities-0.1.5/atlas_densities/app/data/measurements/non_density_measurements.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/measurements/std_cells.json` & `atlas-densities-0.1.5/atlas_densities/app/data/measurements/std_cells.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/metadata/thalamus_metadata.json` & `atlas-densities-0.1.5/atlas_densities/app/data/metadata/thalamus_metadata.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/README.rst` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/composition/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/composition.yaml` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/composition/composition.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/README.rst` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/README.rst` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/probability_map/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/probability_map.csv` & `atlas-densities-0.1.5/atlas_densities/app/data/mtypes/probability_map/probability_map.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/app/mtype_densities.py` & `atlas-densities-0.1.5/atlas_densities/app/mtype_densities.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
 
 
 def standardize_probability_map(probability_map: "pd.DataFrame") -> "pd.DataFrame":
     """
     Standardize the labels of the rows and the columns of `probability_map` and
     remove unused rows.
 
-    Output labels are all lower case.
+    Output row labels are all lower case.
     The underscore is the only delimiter used in an output label.
     The layer names refered to by output labels are:
         "layer_1," "layer_23", "layer_4", "layer_5" and "layer_6".
     Rows whose labels contain "VIP" or "6b" are removed.
 
     Row example: "L2/3 Pvalb-IRES-Cre" -> "layer_23_pv"
     Column example: "NGC-SA" -> "ngc_sa"
@@ -238,17 +238,15 @@
     def standardize_column_label(col_label: str):
         """
         Lowercase labels and use underscore as delimiter for composed
         molecular types such as NGC-DA or NGC-SA.
 
         Example: "NGC-SA" -> "ngc_sa"
         """
-        col_label = col_label.replace("-", "_")
-
-        return col_label.lower()
+        return col_label.replace("-", "_")
 
     bbp_mtypes_map = {"DLAC": "LAC", "SLAC": "SAC"}
     probability_map.rename(bbp_mtypes_map, axis="columns", inplace=True)
     probability_map.rename(standardize_column_label, axis="columns", inplace=True)
     probability_map.rename(standardize_row_label, axis="rows", inplace=True)
 
     return probability_map
@@ -308,15 +306,15 @@
     L.info("Loading probability mapping ...")
     probability_map = pd.DataFrame(pd.read_csv(config["probabilityMapPath"]))
     if "molecular_type" in probability_map.columns:
         probability_map.set_index("molecular_type", inplace=True)
     else:
         probability_map.set_index(probability_map.columns[0], inplace=True)
 
-    # Remove useless lines, use lower case and "standardized" explicit label names
+    # Remove useless lines, use lower case row labels and "standardized" explicit label names
     probability_map = standardize_probability_map(probability_map)
     check_probability_map_sanity(probability_map)
 
     L.info("Loading brain region metadata ...")
     with open(metadata_path, "r", encoding="utf-8") as file_:
         metadata = json.load(file_)
         assert_metadata_content(metadata)
```

### Comparing `atlas-densities-0.1.4/atlas_densities/combination/annotations_combinator.py` & `atlas-densities-0.1.5/atlas_densities/combination/annotations_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/combination/markers_combinator.py` & `atlas-densities-0.1.5/atlas_densities/combination/markers_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/cell_counts.py` & `atlas-densities-0.1.5/atlas_densities/densities/cell_counts.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/cell_density.py` & `atlas-densities-0.1.5/atlas_densities/densities/cell_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/excel_reader.py` & `atlas-densities-0.1.5/atlas_densities/densities/excel_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         are filled with nan. This function replaces those nans by the 'source title' value of the
         first line in the block.
 
         The same applies to the 'comment' column. Source title blocks and comment blocks do not
         always coincide.
         """
         columns: Dict[str, List[str]] = defaultdict(list)
-        for (start, end) in zip(collapsed_blocks.index, collapsed_blocks.index[1:]):
+        for start, end in zip(collapsed_blocks.index, collapsed_blocks.index[1:]):
             columns[header].extend([dataframe[header][start]] * (end - start))
         # Handle the tail of the column
         delta = len(dataframe.index) - len(columns[header])
         dataframe[header] = (
             columns[header] + [dataframe[header][collapsed_blocks.index[-1]]] * delta
         )
```

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/excitatory_inhibitory_splitting.py` & `atlas-densities-0.1.5/atlas_densities/densities/excitatory_inhibitory_splitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/fitting.py` & `atlas-densities-0.1.5/atlas_densities/densities/fitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/glia_densities.py` & `atlas-densities-0.1.5/atlas_densities/densities/glia_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_densities_helper.py` & `atlas-densities-0.1.5/atlas_densities/densities/inhibitory_neuron_densities_helper.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_densities_optimization.py` & `atlas-densities-0.1.5/atlas_densities/densities/inhibitory_neuron_densities_optimization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_density.py` & `atlas-densities-0.1.5/atlas_densities/densities/inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/measurement_to_density.py` & `atlas-densities-0.1.5/atlas_densities/densities/measurement_to_density.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Densities are expressed in number of cells per mm^3.
 """
 from typing import Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from atlas_commons.typing import AnnotationT, FloatArray
+from tqdm import tqdm
 from voxcell import RegionMap  # type: ignore
 
 from atlas_densities.densities.utils import compute_region_volumes, get_hierarchy_info
 
 
 def get_parent_region(region_name: str, region_map: RegionMap) -> Union[str, None]:
     """
@@ -65,16 +66,17 @@
              brain region                    cell density
         5    Basic cell groups and regions   0.005
         123  Cerebrum                        0.001
         ...  ...                             ...
         The index is the sorted list of all region identifiers.
     """
     densities = []
-    for set_ in hierarchy_info["descendant_id_set"]:
-        mask = np.isin(annotation, list(set_))
+    descendants = hierarchy_info["descendant_id_set"]
+    for iset_ in tqdm(range(len(descendants))):
+        mask = np.isin(annotation, list(descendants.iloc[iset_]))
         densities.append(np.sum(cell_density[mask]) / np.count_nonzero(mask))
 
     return pd.DataFrame(
         {"brain_region": hierarchy_info["brain_region"], "cell density": densities},
         index=hierarchy_info.index,
     )
```

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_composition.py` & `atlas-densities-0.1.5/atlas_densities/densities/mtype_densities_from_composition.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_map.py` & `atlas-densities-0.1.5/atlas_densities/densities/mtype_densities_from_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     Args:
         dataframe: the data frame to be checked.
 
     Raises:
         AtlasBuildingTools error on failure.
     """
     d_f = dataframe.copy()
-    d_f = d_f.rename(str.lower, axis="columns")
     d_f = d_f.rename(str.lower, axis="rows")
     d_f.columns = d_f.columns.str.replace(" ", "")
     d_f.index = d_f.index.str.replace(" ", "")
 
     if np.any(dataframe.columns != d_f.columns) or np.any(dataframe.index != d_f.index):
         raise AtlasDensitiesError(
             "Rows and columns aren't all labeled with lowercase strings or contain white spaces."
@@ -157,22 +156,22 @@
     output_dirpath: str,
 ) -> None:
     """
     Create a density field for each mtype listed in `probability_map.csv`.
 
     The ouput volumetric density for the mtype named ``mtype`` is saved into
     `<output_dirpath>/no_layers` under the name ``<mtype>_densities.nrrd`` if its sum is not too
-    close to zero where <mtype> is uppercase and dash separated.
+    close to zero, where <mtype> is dash separated.
     Example: if mtype = "ngc_sa", then output_file_name = "NGC-SA_densities.nrrd".
 
     The restriction of the volumetric density for the mtype named ``mtype`` to layer
     ``layer_name`` is saved into `<output_dirpath>/with_layers` under the name
     ``<layer_name>_<mtype>_densities.nrrd`` if its sum is not too close to zero.
     The string <layer_name> is of the form "L<layer_index>", e,g, "L1" for "layer_1" and
-    the string <mtype> is upper case and dash-separted.
+    the string <mtype> is dash-separted.
     Example: if mtype = "ngc_sa", layer_name = "layer_23",  then
     output_file_name = "L23_NGC-SA_densities.nrrd".
 
     Args:
         annotation: VoxelData holding an int array of shape (W, H, D) where W, H and D are integer
             dimensions; this array is the annotated volume of the brain region of interest.
         region_map: RegionMap object to navigate the brain regions hierarchy.
@@ -239,28 +238,26 @@
 
         density = molecular_type_densities["gad67"]
         mtype_density[layer_masks["layer_1"]] = (
             density[layer_masks["layer_1"]] * probability_map.at["layer_1_gad67", mtype]
         )
 
         # Saving to file
+        mtype_filename = f"{mtype.replace('_', '-')}_densities.nrrd"
         (Path(output_dirpath) / "no_layers").mkdir(exist_ok=True, parents=True)
         if not np.isclose(np.sum(mtype_density), 0.0):
-            filename = f"{mtype.upper().replace('_', '-')}_densities.nrrd"
-            filepath = str(Path(output_dirpath) / "no_layers" / filename)
+            filepath = str(Path(output_dirpath) / "no_layers" / mtype_filename)
             L.info("Saving %s ...", filepath)
             annotation.with_data(mtype_density).save_nrrd(filepath)
 
         (Path(output_dirpath) / "with_layers").mkdir(exist_ok=True, parents=True)
         for layer_name, layer_mask in layer_masks.items():
             layer_density = np.zeros(layer_mask.shape, dtype=float)
             layer_density[layer_mask] = mtype_density[layer_mask]
-            filename = (
-                f"L{layer_name.split('_')[-1]}_{mtype.upper().replace('_', '-')}_densities.nrrd"
-            )
+            filename = f"L{layer_name.split('_')[-1]}_{mtype_filename}"
             if not np.isclose(np.sum(layer_density), 0.0):
                 filepath = str(Path(output_dirpath) / "with_layers" / filename)
                 L.info("Saving %s ...", filepath)
                 annotation.with_data(layer_density).save_nrrd(filepath)
             else:
                 zero_density_mtypes.append(filename.replace("_densities.nrrd", ""))
```

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_profiles.py` & `atlas-densities-0.1.5/atlas_densities/densities/mtype_densities_from_profiles.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/refined_inhibitory_neuron_densities.py` & `atlas-densities-0.1.5/atlas_densities/densities/refined_inhibitory_neuron_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/densities/utils.py` & `atlas-densities-0.1.5/atlas_densities/densities/utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/atlas_densities/utils.py` & `atlas-densities-0.1.5/atlas_densities/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     metadata_layers = metadata["layers"]
     layers = np.zeros_like(annotated_volume, dtype=np.uint8)
     region_ids = region_map.find(
         metadata["region"]["query"],
         attr=metadata["region"]["attribute"],
         with_descendants=metadata["region"].get("with_descendants", False),
     )
-    for (index, query) in enumerate(metadata_layers["queries"], 1):
+    for index, query in enumerate(metadata_layers["queries"], 1):
         layer_ids = region_map.find(
             query,
             attr=metadata_layers["attribute"],
             with_descendants=metadata_layers.get("with_descendants", False),
         )
         layers[np.isin(annotated_volume, list(layer_ids & region_ids))] = index
```

### Comparing `atlas-densities-0.1.4/atlas_densities.egg-info/PKG-INFO` & `atlas-densities-0.1.5/atlas_densities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-densities
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library containing command lines and tools to compute volumetric cell densities in the rodent brain
 Home-page: https://github.com/BlueBrain/atlas-densities
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-densities
 Description: .. image:: atlas-densities.jpg
         
@@ -344,34 +344,24 @@
                 --metadata-path=$DATA/metadata/isocortex_23_metadata.json            \
                 --mtypes-config-path=$DATA/mtypes/mtypes_probability_map_config.yaml \
                 --output-dir=data/ccfv2/me-types/
         
         Subdivide excitatory files into pyramidal subtypes
         --------------------------------------------------
         
-        This should run after the ME mapping from Roussel. To run:
+        This should run after the inhibitory/excitatory computation above. To run:
         
-        make_new_inhib_exc_outside_SSCX.py
-        
-        Input support files needed:
-        
-        annotation atlas (with L23 split): brain_regions.nrrd
-        
-        annotation hierarchy (with L23 split): hierarchy.json
-        
-        inhibitory: gad67+_density_v3_MMB.nrrd
-        
-        total neuron: neuron_density_v3_MMB.nrrd
-        
-        Output:
-        
-        excitatory nrrd files in output directory
-        
-        inhibitory minus cortex in output directory
+        .. code-block:: bash
         
+            atlas-densities cell-densities excitatory-split                         \
+                --annotation-path=data/ccfv2/annotation_25.nrrd                     \
+                --hierarchy-path=data/1.json                                        \
+                --neuron-density=data/ccfv2/density_volumes/neuron_density.nrrd     \
+                --inhibitory-density=data/ccfv2/density_volumes/gad67+_density.nrrd \
+                --output-dir=data/ccfv2/excitatory_split
         
         Instructions for developers
         ===========================
         
         Run the following commands before submitting your code for review:
         
         .. code-block:: bash
```

### Comparing `atlas-densities-0.1.4/atlas_densities.egg-info/SOURCES.txt` & `atlas-densities-0.1.5/atlas_densities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/doc/Makefile` & `atlas-densities-0.1.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/doc/source/bbpp82_628_linear_program.pdf` & `atlas-densities-0.1.5/doc/source/bbpp82_628_linear_program.pdf`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/doc/source/conf.py` & `atlas-densities-0.1.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/doc/source/index.rst` & `atlas-densities-0.1.5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/setup.py` & `atlas-densities-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/1.json` & `atlas-densities-0.1.5/tests/1.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/app/test_cell_densities.py` & `atlas-densities-0.1.5/tests/app/test_cell_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/app/test_combination.py` & `atlas-densities-0.1.5/tests/app/test_combination.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/app/test_mtype_densities.py` & `atlas-densities-0.1.5/tests/app/test_mtype_densities.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,31 +156,31 @@
                 "L23_Pvalb",
                 "L4_Vip",
             ],
         )
         actual = tested.standardize_probability_map(probability_map)
         expected = pd.DataFrame(
             {
-                "chc": [0.5, 0.0, 0.0, 0.0],
-                "ngc_sa": [0.5, 0.0, 0.0, 0.0],
-                "lac": [0.0] * 4,
-                "sac": [0.0] * 4,
+                "ChC": [0.5, 0.0, 0.0, 0.0],
+                "NGC_SA": [0.5, 0.0, 0.0, 0.0],
+                "LAC": [0.0] * 4,
+                "SAC": [0.0] * 4,
             },
             index=["layer_1_gad67", "layer_6_vip", "layer_23_pv", "layer_4_vip"],
         )
         pdt.assert_frame_equal(actual, expected)
 
     def test_output(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
             self.save_input_data_to_file()
             result = get_result_from_probablity_map_(runner)
             assert result.exit_code == 0
 
-            chc = VoxelData.load_nrrd(str(Path("output_dir") / "no_layers" / "CHC_densities.nrrd"))
+            chc = VoxelData.load_nrrd(str(Path("output_dir") / "no_layers" / "ChC_densities.nrrd"))
             assert chc.raw.dtype == float
             npt.assert_array_equal(chc.voxel_dimensions, self.data["annotation"].voxel_dimensions)
 
     def test_wrong_config(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
             self.save_input_data_to_file()
```

### Comparing `atlas-densities-0.1.4/tests/app/test_refined_inhibitory_neuron_densities.py` & `atlas-densities-0.1.5/tests/app/test_refined_inhibitory_neuron_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/combination/test_annotations_combinator.py` & `atlas-densities-0.1.5/tests/combination/test_annotations_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/combination/test_markers_combinator.py` & `atlas-densities-0.1.5/tests/combination/test_markers_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/data/mtypes/mtype-taxonomy.tsv` & `atlas-densities-0.1.5/tests/densities/data/mtypes/mtype-taxonomy.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_cell_counts.py` & `atlas-densities-0.1.5/tests/densities/test_cell_counts.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_cell_density.py` & `atlas-densities-0.1.5/tests/densities/test_cell_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_excel_reader.py` & `atlas-densities-0.1.5/tests/densities/test_excel_reader.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_excitatory_inhibitory_splitting.py` & `atlas-densities-0.1.5/tests/densities/test_excitatory_inhibitory_splitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_fitting.py` & `atlas-densities-0.1.5/tests/densities/test_fitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_glia_densities.py` & `atlas-densities-0.1.5/tests/densities/test_glia_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_densities_helper.py` & `atlas-densities-0.1.5/tests/densities/test_inhibitory_neuron_densities_helper.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_density.py` & `atlas-densities-0.1.5/tests/densities/test_inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_density_optimization.py` & `atlas-densities-0.1.5/tests/densities/test_inhibitory_neuron_density_optimization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_measurement_to_density.py` & `atlas-densities-0.1.5/tests/densities/test_measurement_to_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_composition.py` & `atlas-densities-0.1.5/tests/densities/test_mtype_densities_from_composition.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_map.py` & `atlas-densities-0.1.5/tests/densities/test_mtype_densities_from_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             "L6_Vip",
             "L6_Lamp5",
         ],
     )
 
     probability_map = DataFrame(
         {
-            "chc": [
+            "ChC": [
                 0.0,
                 0.0,
                 0.0,
                 0.0,
                 0.0,
                 0.0,
                 0.0,
@@ -151,15 +151,15 @@
                 1.0,
                 1.0,
                 0.4,
                 1.0,
                 1.0,
                 1.0,
             ],
-            "lac": [
+            "LAC": [
                 1.0,
                 1.0,
                 1.0,
                 1.0,
                 1.0,
                 1.0,
                 1.0,
@@ -231,62 +231,62 @@
         self.tmpdir.cleanup()
 
     def test_filenames(self):
         tmpdir = self.tmpdir.name
         no_layers_filepaths = {
             Path.resolve(f).name for f in Path(tmpdir, "no_layers").glob("*.nrrd")
         }
-        assert no_layers_filepaths == {"CHC_densities.nrrd", "LAC_densities.nrrd"}
+        assert no_layers_filepaths == {"ChC_densities.nrrd", "LAC_densities.nrrd"}
         with_layers_filepaths = {
             Path.resolve(f).name for f in Path(tmpdir, "with_layers").glob("*.nrrd")
         }
         assert with_layers_filepaths == {
             "L1_LAC_densities.nrrd",
             "L4_LAC_densities.nrrd",
             "L23_LAC_densities.nrrd",
             "L6_LAC_densities.nrrd",
-            "L6_CHC_densities.nrrd",
-            "L5_CHC_densities.nrrd",
+            "L6_ChC_densities.nrrd",
+            "L5_ChC_densities.nrrd",
         }
 
     def test_output_consistency(self):
         sum_ = {
-            "CHC": np.zeros(self.data["annotation"].shape, dtype=float),
+            "ChC": np.zeros(self.data["annotation"].shape, dtype=float),
             "LAC": np.zeros(self.data["annotation"].shape, dtype=float),
         }
         tmpdir = self.tmpdir.name
-        for filename in ["L5_CHC_densities.nrrd", "L6_CHC_densities.nrrd"]:
+        for filename in ["L5_ChC_densities.nrrd", "L6_ChC_densities.nrrd"]:
             filepath = str(Path(tmpdir) / "with_layers" / filename)
-            sum_["CHC"] += VoxelData.load_nrrd(filepath).raw
+            sum_["ChC"] += VoxelData.load_nrrd(filepath).raw
 
         for filename in [
             "L1_LAC_densities.nrrd",
             "L23_LAC_densities.nrrd",
             "L4_LAC_densities.nrrd",
             "L6_LAC_densities.nrrd",
         ]:
             filepath = str(Path(tmpdir) / "with_layers" / filename)
             sum_["LAC"] += VoxelData.load_nrrd(filepath).raw
 
-        for mtype in ["CHC", "LAC"]:
+        for mtype in ["ChC", "LAC"]:
             filepath = str(Path(tmpdir) / "no_layers" / f"{mtype}_densities.nrrd")
             density = VoxelData.load_nrrd(filepath)
             npt.assert_array_equal(
                 density.voxel_dimensions, self.data["annotation"].voxel_dimensions
             )
             assert density.raw.dtype == float
             npt.assert_array_almost_equal(sum_[mtype], density.raw)
 
     def test_output_values(self):
         tmpdir = self.tmpdir.name
         expected_densities = {
-            "CHC": np.array([[[0.0, 0.0, 0.0, 2.0, 0.4]]], dtype=float),
+            "ChC": np.array([[[0.0, 0.0, 0.0, 2.0, 0.4]]], dtype=float),
             "LAC": np.array([[[1.5, 2.0, 1.0, 0.0, 0.6]]], dtype=float),
         }
-        for mtype in ["CHC", "LAC"]:
+        for mtype in ["ChC", "LAC"]:
             filepath = str(Path(tmpdir) / "no_layers" / f"{mtype}_densities.nrrd")
             npt.assert_array_almost_equal(
                 VoxelData.load_nrrd(filepath).raw, expected_densities[mtype]
             )
 
 
 class Test_create_from_probability_map_exceptions:
@@ -304,25 +304,25 @@
             self.data["metadata"],
             self.data["molecular_type_densities"],
             self.data["probability_map"],
             self.tmpdir.name,
         )
 
     def test_probability_map_sanity_negative_probability(self):
-        self.data["probability_map"].loc["layer_1_gad67", "chc"] = -0.0025
+        self.data["probability_map"].loc["layer_1_gad67", "ChC"] = -0.0025
         with pytest.raises(AtlasDensitiesError):
             self.create_densities()
 
     def test_probability_map_sanity_row_sum_is_1(self):
-        self.data["probability_map"].loc["layer_1_gad67", "chc"] = 2.0
+        self.data["probability_map"].loc["layer_1_gad67", "ChC"] = 2.0
         with pytest.raises(AtlasDensitiesError):
             self.create_densities()
 
     def test_labels_sanity(self):
-        self.data["probability_map"].rename(str.upper, axis="columns", inplace=True)
+        self.data["probability_map"].rename(str.upper, axis="rows", inplace=True)
         with pytest.raises(AtlasDensitiesError):
             self.create_densities()
 
     def test_probability_map_layer_1_gad67_exists(self):
         self.data["probability_map"].drop("layer_1_gad67", axis="rows", inplace=True)
         with pytest.raises(AtlasDensitiesError):
             self.create_densities()
```

### Comparing `atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_profiles.py` & `atlas-densities-0.1.5/tests/densities/test_mtype_densities_from_profiles.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_optimization_initialization.py` & `atlas-densities-0.1.5/tests/densities/test_optimization_initialization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_refined_inhibitory_neuron_density.py` & `atlas-densities-0.1.5/tests/densities/test_refined_inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/densities/test_utils.py` & `atlas-densities-0.1.5/tests/densities/test_utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/markers_config.yaml` & `atlas-densities-0.1.5/tests/markers_config.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/mocking_tools.py` & `atlas-densities-0.1.5/tests/mocking_tools.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tests/test_utils.py` & `atlas-densities-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.4/tox.ini` & `atlas-densities-0.1.5/tox.ini`

 * *Files identical despite different names*

