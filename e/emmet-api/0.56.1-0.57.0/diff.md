# Comparing `tmp/emmet-api-0.56.1.tar.gz` & `tmp/emmet-api-0.57.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.56.1.tar", last modified: Tue Jun 13 23:45:55 2023, max compression
+gzip compressed data, was "emmet-api-0.57.0.tar", last modified: Fri Jun 16 17:20:17 2023, max compression
```

## Comparing `emmet-api-0.56.1.tar` & `emmet-api-0.57.0.tar`

### file list

```diff
@@ -1,350 +1,359 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-13 23:45:47.000000 emmet-api-0.56.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 23:45:55.873441 emmet-api-0.56.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-13 23:45:47.000000 emmet-api-0.56.1/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.845440 emmet-api-0.56.1/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/_messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_messages/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/_messages/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.853441 emmet-api-0.56.1/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.857441 emmet-api-0.56.1/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.861441 emmet-api-0.56.1/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-13 23:45:47.000000 emmet-api-0.56.1/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 23:45:55.000000 emmet-api-0.56.1/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-06-13 23:45:55.000000 emmet-api-0.56.1/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:45:55.000000 emmet-api-0.56.1/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:45:55.000000 emmet-api-0.56.1/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-13 23:45:55.000000 emmet-api-0.56.1/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 23:45:55.000000 emmet-api-0.56.1/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-13 23:45:47.000000 emmet-api-0.56.1/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-06-13 23:45:47.000000 emmet-api-0.56.1/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-13 23:45:47.000000 emmet-api-0.56.1/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-06-13 23:45:47.000000 emmet-api-0.56.1/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:45:55.873441 emmet-api-0.56.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 23:45:47.000000 emmet-api-0.56.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-13 23:45:47.000000 emmet-api-0.56.1/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.865441 emmet-api-0.56.1/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.849440 emmet-api-0.56.1/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.849440 emmet-api-0.56.1/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.869441 emmet-api-0.56.1/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:55.873441 emmet-api-0.56.1/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-13 23:45:47.000000 emmet-api-0.56.1/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.216471 emmet-api-0.57.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-16 17:20:10.000000 emmet-api-0.57.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 17:20:17.212471 emmet-api-0.57.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-16 17:20:10.000000 emmet-api-0.57.0/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.176471 emmet-api-0.57.0/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/_messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_messages/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/_messages/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.196471 emmet-api-0.57.0/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.200471 emmet-api-0.57.0/emmet/api/routes/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/metal_binding/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/metal_binding/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-16 17:20:10.000000 emmet-api-0.57.0/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.204471 emmet-api-0.57.0/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 17:20:16.000000 emmet-api-0.57.0/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-16 17:20:17.000000 emmet-api-0.57.0/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:20:16.000000 emmet-api-0.57.0/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:20:16.000000 emmet-api-0.57.0/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 17:20:16.000000 emmet-api-0.57.0/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 17:20:16.000000 emmet-api-0.57.0/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-16 17:20:10.000000 emmet-api-0.57.0/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-06-16 17:20:10.000000 emmet-api-0.57.0/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-16 17:20:10.000000 emmet-api-0.57.0/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-06-16 17:20:10.000000 emmet-api-0.57.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:20:17.216471 emmet-api-0.57.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-16 17:20:10.000000 emmet-api-0.57.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-16 17:20:10.000000 emmet-api-0.57.0/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.188471 emmet-api-0.57.0/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.192471 emmet-api-0.57.0/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.208471 emmet-api-0.57.0/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/metal_binding/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:17.212471 emmet-api-0.57.0/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-16 17:20:10.000000 emmet-api-0.57.0/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.56.1/Dockerfile` & `emmet-api-0.57.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/app.py` & `emmet-api-0.57.0/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/core/api.py` & `emmet-api-0.57.0/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.57.0/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.57.0/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/core/documentation.py` & `emmet-api-0.57.0/emmet/api/core/documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,14 +290,19 @@
     },
     {
         "name": "Molecules Bonds",
         "description": "Route for molecular bonding data. See the `MoleculeBondingDoc` schema for a full list \
             of fields returned by this route.",
     },
     {
+        "name": "Molecules Metal Binding",
+        "description": "Route for data regarding metal binding to molecules. See the `MetalBindingDoc` schema \
+            for a full list of fields returned by this route.",
+    },
+    {
         "name": "Molecules Orbitals",
         "description": "Route for molecular orbital information obtained via Natural Bonding Orbital analysis. \
             See the `OrbitalDoc` schema for a full list of fields returned by this route.",
     },
     {
         "name": "Molecules Redox",
         "description": "Route for molecular redox information (e.g. ionization energy, reduction free energy, \
```

### Comparing `emmet-api-0.56.1/emmet/api/core/global_header.py` & `emmet-api-0.57.0/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/core/settings.py` & `emmet-api-0.57.0/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.57.0/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.57.0/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.57.0/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.57.0/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/_messages/query_operator.py` & `emmet-api-0.57.0/emmet/api/routes/_messages/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/_messages/resources.py` & `emmet-api-0.57.0/emmet/api/routes/_messages/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/dois/resources.py` & `emmet-api-0.57.0/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.57.0/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.57.0/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.57.0/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.57.0/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.57.0/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.57.0/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.57.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.57.0/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.57.0/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.57.0/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.57.0/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/summary/hint_scheme.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from maggma.api.query_operator import QueryOperator
 from maggma.api.utils import STORE_PARAMS
 from fastapi import Query
 from typing import Optional
 
+from monty.json import jsanitize
 
-# TODO: might need these utils once pmg changes are in place (see below)
-# from emmet.api.routes.tasks.utils import calcs_reversed_to_trajectory, task_to_entry
+from emmet.api.routes.molecules.tasks.utils import calcs_reversed_to_trajectory
 
 
 class MultipleTaskIDsQuery(QueryOperator):
     """
     Method to generate a query on search docs using multiple task_id values
     """
 
@@ -89,12 +89,47 @@
                     break
 
             d.append(deprecation)
 
         return d
 
 
-# TODO: class TrajectoryQuery(QueryOperator):
-# Need to write Trajectory class in pmg for Molecules
+class TrajectoryQuery(QueryOperator):
+    """
+    Method to generate a query on calculation trajectory data from task documents
+    """
+
+    def query(
+        self,
+        task_ids: Optional[str] = Query(
+            None, description="Comma-separated list of task_ids to query on"
+        ),
+    ) -> STORE_PARAMS:
+        crit = {}
+
+        if task_ids:
+            crit.update(
+                {
+                    "task_id": {
+                        "$in": [task_id.strip() for task_id in task_ids.split(",")]
+                    }
+                }
+            )
+
+        return {"criteria": crit}
 
-# TODO: class EntryQuery(QueryOperator):
-# Need to write MoleculeEntry class in pmg
+    def post_process(self, docs, query):
+        """
+        Post processing to generatore trajectory data
+        """
+
+        d = [
+            {
+                "task_id": doc["task_id"],
+                "trajectories": jsanitize(
+                    calcs_reversed_to_trajectory(doc["calcs_reversed"])
+                ),
+            }
+            for doc in docs
+        ]
+
+        return d
```

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/thermo/resources.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 from maggma.api.resource import ReadOnlyResource
+from emmet.core.molecules.thermo import MoleculeThermoDoc
 
+from maggma.api.query_operator import (
+    NumericQuery,
+    PaginationQuery,
+    SortQuery,
+    SparseFieldsQuery,
+)
+
+from emmet.api.routes.molecules.thermo.query_operators import (
+    ThermoCorrectionQuery,
+)
 from emmet.api.routes.molecules.molecules.query_operators import (
+    MultiMPculeIDQuery,
+    ExactCalcMethodQuery,
+    FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
-    FormulaQuery,
+    ChargeSpinQuery,
 )
-from emmet.api.routes.molecules.tasks.hint_scheme import TasksHintScheme
-from emmet.api.routes.molecules.tasks.query_operators import (
-    DeprecationQuery,
-    MultipleTaskIDsQuery,
-    # TODO:
-    # TrajectoryQuery,
-    # EntryQuery,
-)
-from emmet.api.core.global_header import GlobalHeaderProcessor
+from emmet.api.routes.molecules.utils import MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
-from emmet.core.tasks import DeprecationDoc
-from emmet.core.qchem.task import TaskDocument
-
-timeout = MAPISettings().TIMEOUT
+from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
-def task_resource(task_store):
+def thermo_resource(thermo_store):
     resource = ReadOnlyResource(
-        task_store,
-        TaskDocument,
+        thermo_store,
+        MoleculeThermoDoc,
         query_operators=[
+            MultiMPculeIDQuery(),
+            ExactCalcMethodQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
-            MultipleTaskIDsQuery(),
+            ChargeSpinQuery(),
+            MultiPropertyIDQuery(),
+            ThermoCorrectionQuery(),
+            NumericQuery(
+                model=MoleculeThermoDoc,
+                excluded_fields=[
+                    "charge",
+                    "spin_multiplicity",
+                    "natoms",
+                    "nelements",
+                    "nelectrons",
+                    "rt",
+                ],
+            ),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
-                TaskDocument,
-                default_fields=["task_id", "formula_alphabetical", "last_updated"],
+                MoleculeThermoDoc,
+                default_fields=[
+                    "molecule_id",
+                    "property_id",
+                    "solvent",
+                    "method",
+                    "last_updated",
+                ],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        hint_scheme=TasksHintScheme(),
-        tags=["Molecules Tasks"],
-        sub_path="/tasks/",
-        timeout=timeout,
+        tags=["Molecules Thermo"],
+        sub_path="/thermo/",
         disable_validation=True,
+        timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
-
-
-def task_deprecation_resource(task_store):
-    resource = ReadOnlyResource(
-        task_store,
-        DeprecationDoc,
-        query_operators=[DeprecationQuery(), PaginationQuery()],
-        tags=["Molecules Tasks"],
-        enable_get_by_key=False,
-        enable_default_search=True,
-        sub_path="/tasks/deprecation/",
-        header_processor=GlobalHeaderProcessor(),
-        timeout=timeout,
-    )
-
-    return resource
-
-
-# TODO: def trajectory_resource(task_store):
-# TODO: def entries_resource(task_store):
```

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,50 @@
 from maggma.api.resource import ReadOnlyResource
-from emmet.core.molecules.thermo import MoleculeThermoDoc
+from emmet.core.molecules.vibration import VibrationDoc
 
-from maggma.api.query_operator import (
-    NumericQuery,
-    PaginationQuery,
-    SortQuery,
-    SparseFieldsQuery,
-)
+from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
-from emmet.api.routes.molecules.thermo.query_operators import (
-    ThermoCorrectionQuery,
-)
 from emmet.api.routes.molecules.molecules.query_operators import (
     MultiMPculeIDQuery,
     ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery,
 )
 from emmet.api.routes.molecules.utils import MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
-def thermo_resource(thermo_store):
+def vibration_resource(vibes_store):
     resource = ReadOnlyResource(
-        thermo_store,
-        MoleculeThermoDoc,
+        vibes_store,
+        VibrationDoc,
         query_operators=[
             MultiMPculeIDQuery(),
             ExactCalcMethodQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
             ChargeSpinQuery(),
             MultiPropertyIDQuery(),
-            ThermoCorrectionQuery(),
-            NumericQuery(
-                model=MoleculeThermoDoc,
-                excluded_fields=[
-                    "charge",
-                    "spin_multiplicity",
-                    "natoms",
-                    "nelements",
-                    "nelectrons",
-                    "rt",
-                ],
-            ),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
-                MoleculeThermoDoc,
+                VibrationDoc,
                 default_fields=[
                     "molecule_id",
                     "property_id",
                     "solvent",
-                    "method",
                     "last_updated",
                 ],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Molecules Thermo"],
-        sub_path="/thermo/",
+        tags=["Molecules Vibrations"],
+        sub_path="/vibrations/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/utils.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.57.0/emmet/api/routes/molecules/metal_binding/resources.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from maggma.api.resource import ReadOnlyResource
-from emmet.core.molecules.vibration import VibrationDoc
+from emmet.core.molecules.metal_binding import MetalBindingDoc
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
 from emmet.api.routes.molecules.molecules.query_operators import (
     MultiMPculeIDQuery,
     ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery,
 )
-from emmet.api.routes.molecules.utils import MultiPropertyIDQuery
+from emmet.api.routes.molecules.metal_binding.query_operators import BindingDataQuery
+from emmet.api.routes.molecules.utils import MethodQuery, MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
-def vibration_resource(vibes_store):
+def metal_binding_resource(metal_binding_store):
     resource = ReadOnlyResource(
-        vibes_store,
-        VibrationDoc,
+        metal_binding_store,
+        MetalBindingDoc,
         query_operators=[
             MultiMPculeIDQuery(),
             ExactCalcMethodQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
             ChargeSpinQuery(),
+            MethodQuery(),
+            BindingDataQuery(),
             MultiPropertyIDQuery(),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
-                VibrationDoc,
+                MetalBindingDoc,
                 default_fields=[
                     "molecule_id",
                     "property_id",
                     "solvent",
+                    "method",
                     "last_updated",
                 ],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Molecules Vibrations"],
-        sub_path="/vibrations/",
+        tags=["Molecules Metal Binding"],
+        sub_path="/metal_binding/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.56.1/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.57.0/emmet_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,17 @@
 emmet/api/routes/molecules/__init__.py
 emmet/api/routes/molecules/utils.py
 emmet/api/routes/molecules/association/__init__.py
 emmet/api/routes/molecules/association/resources.py
 emmet/api/routes/molecules/bonds/__init__.py
 emmet/api/routes/molecules/bonds/query_operators.py
 emmet/api/routes/molecules/bonds/resources.py
+emmet/api/routes/molecules/metal_binding/__init__.py
+emmet/api/routes/molecules/metal_binding/query_operators.py
+emmet/api/routes/molecules/metal_binding/resources.py
 emmet/api/routes/molecules/molecules/__init__.py
 emmet/api/routes/molecules/molecules/hint_scheme.py
 emmet/api/routes/molecules/molecules/query_operators.py
 emmet/api/routes/molecules/molecules/resources.py
 emmet/api/routes/molecules/orbitals/__init__.py
 emmet/api/routes/molecules/orbitals/query_operators.py
 emmet/api/routes/molecules/orbitals/resources.py
@@ -143,14 +146,15 @@
 emmet/api/routes/molecules/summary/hint_scheme.py
 emmet/api/routes/molecules/summary/query_operators.py
 emmet/api/routes/molecules/summary/resources.py
 emmet/api/routes/molecules/tasks/__init__.py
 emmet/api/routes/molecules/tasks/hint_scheme.py
 emmet/api/routes/molecules/tasks/query_operators.py
 emmet/api/routes/molecules/tasks/resources.py
+emmet/api/routes/molecules/tasks/utils.py
 emmet/api/routes/molecules/thermo/__init__.py
 emmet/api/routes/molecules/thermo/query_operators.py
 emmet/api/routes/molecules/thermo/resources.py
 emmet/api/routes/molecules/vibrations/__init__.py
 emmet/api/routes/molecules/vibrations/resources.py
 emmet_api.egg-info/PKG-INFO
 emmet_api.egg-info/SOURCES.txt
@@ -235,22 +239,25 @@
 tests/materials/thermo/__init__.py
 tests/materials/thermo/test_query_operators.py
 tests/materials/xas/__init__.py
 tests/materials/xas/test_query_operators.py
 tests/molecules/__init__.py
 tests/molecules/bonds/__init__.py
 tests/molecules/bonds/test_query_operators.py
+tests/molecules/metal_binding/__init__.py
+tests/molecules/metal_binding/test_query_operators.py
 tests/molecules/molecules/__init__.py
 tests/molecules/molecules/test_hint_scheme.py
 tests/molecules/molecules/test_query_operators.py
 tests/molecules/orbitals/__init__.py
 tests/molecules/orbitals/test_query_operators.py
 tests/molecules/redox/__init__.py
 tests/molecules/redox/test_query_operators.py
 tests/molecules/summary/__init__.py
 tests/molecules/summary/test_hint_scheme.py
 tests/molecules/summary/test_query_operators.py
 tests/molecules/tasks/__init__.py
 tests/molecules/tasks/test_hint_scheme.py
 tests/molecules/tasks/test_query_operators.py
+tests/molecules/tasks/test_utils.py
 tests/molecules/thermo/__init__.py
 tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.56.1/legacy_resources.py` & `emmet-api-0.57.0/legacy_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/material_resources.py` & `emmet-api-0.57.0/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/molecule_resources.py` & `emmet-api-0.57.0/molecule_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
 from emmet.api.core.settings import MAPISettings
 from maggma.stores import MongoURIStore
 
 from emmet.api.routes.molecules.tasks.resources import (
     task_resource,
     task_deprecation_resource,
+    trajectory_resource,
 )
 from emmet.api.routes.molecules.association.resources import (
     find_molecule_assoc_resource,
     mol_assoc_resource,
 )
 from emmet.api.routes.molecules.molecules.resources import (
     find_molecule_resource,
     molecules_resource,
 )
 from emmet.api.routes.molecules.partial_charges.resources import charges_resource
 from emmet.api.routes.molecules.partial_spins.resources import spins_resource
 from emmet.api.routes.molecules.bonds.resources import bonding_resource
+from emmet.api.routes.molecules.metal_binding.resources import metal_binding_resource
 from emmet.api.routes.molecules.orbitals.resources import orbitals_resource
 from emmet.api.routes.molecules.redox.resources import redox_resource
 from emmet.api.routes.molecules.thermo.resources import thermo_resource
 from emmet.api.routes.molecules.vibrations.resources import vibration_resource
 from emmet.api.routes.molecules.summary.resources import summary_resource
 
 
@@ -76,14 +78,21 @@
     bonds_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
         collection_name="molecules_bonds",
     )
 
+    metal_binding_store = MongoURIStore(
+        uri=db_uri,
+        database="mp_molecules",
+        key="property_id",
+        collection_name="molecules_metal_binding",
+    )
+
     orbitals_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
         collection_name="molecules_orbitals",
     )
 
@@ -119,15 +128,19 @@
     raise RuntimeError("Must specify MongoDB URI containing inputs.")
 
 
 mp_molecules_resources = list()
 
 # Tasks
 mp_molecules_resources.extend(
-    [task_resource(task_store), task_deprecation_resource(task_store)]
+    [
+        task_resource(task_store),
+        task_deprecation_resource(task_store),
+        trajectory_resource(task_store),
+    ]
 )
 
 # Assoc
 mp_molecules_resources.extend(
     [mol_assoc_resource(assoc_store), find_molecule_assoc_resource(assoc_store)]
 )
 
@@ -144,14 +157,17 @@
 
 # Partial spins
 mp_molecules_resources.extend([spins_resource(spins_store)])
 
 # Bonds
 mp_molecules_resources.extend([bonding_resource(bonds_store)])
 
+# Metal binding
+mp_molecules_resources.extend([metal_binding_resource(metal_binding_store)])
+
 # Orbitals
 mp_molecules_resources.extend([orbitals_resource(orbitals_store)])
 
 # Redox
 mp_molecules_resources.extend([redox_resource(redox_store)])
 
 # Thermo
```

### Comparing `emmet-api-0.56.1/requirements/deployment.txt` & `emmet-api-0.57.0/requirements/deployment.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,31 +38,31 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (emmet/emmet-api/setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -108,15 +108,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (emmet/emmet-api/setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -181,15 +181,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -297,17 +297,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
```

### Comparing `emmet-api-0.56.1/requirements/macos-latest_py3.10.txt` & `emmet-api-0.57.0/requirements/macos-latest_py3.10.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,31 +38,31 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -108,15 +108,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -177,15 +177,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -292,17 +292,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
```

### Comparing `emmet-api-0.56.1/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.57.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -45,37 +45,37 @@
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -145,15 +145,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -271,17 +271,17 @@
     # via matplotlib
 platformdirs==3.5.3
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -420,17 +420,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   mypy
     #   pytest
```

### Comparing `emmet-api-0.56.1/requirements/macos-latest_py3.11.txt` & `emmet-api-0.57.0/requirements/macos-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,31 +38,31 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 fastapi==0.97.0
     # via
@@ -104,15 +104,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -173,15 +173,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -288,17 +288,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
```

### Comparing `emmet-api-0.56.1/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.57.0/requirements/macos-latest_py3.11_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -45,37 +45,37 @@
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 fastapi==0.97.0
     # via
@@ -140,15 +140,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -266,17 +266,17 @@
     # via matplotlib
 platformdirs==3.5.3
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -415,17 +415,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
```

### Comparing `emmet-api-0.56.1/requirements/macos-latest_py3.8.txt` & `emmet-api-0.57.0/requirements/macos-latest_py3.8.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,31 +38,31 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -114,15 +114,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -185,15 +185,15 @@
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -300,17 +300,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
```

### Comparing `emmet-api-0.56.1/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.57.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -45,37 +45,37 @@
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -154,15 +154,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -282,17 +282,17 @@
     # via jsonschema
 platformdirs==3.5.3
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -431,17 +431,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   mypy
     #   pytest
```

### Comparing `emmet-api-0.56.1/requirements/macos-latest_py3.9.txt` & `emmet-api-0.57.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,31 +38,31 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -85,19 +85,15 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -112,15 +108,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -181,15 +177,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -296,35 +292,30 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.6.3
     # via
-    #   aioitertools
-    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
-    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
@@ -334,13 +325,11 @@
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.56.1/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.57.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -45,37 +45,37 @@
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -152,15 +152,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -278,17 +278,17 @@
     # via matplotlib
 platformdirs==3.5.3
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -427,17 +427,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   mypy
     #   pytest
```

### Comparing `emmet-api-0.56.1/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.57.0/requirements/ubuntu-latest_py3.11.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,40 +38,36 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.1
-    # via
-    #   anyio
-    #   cattrs
 fastapi==0.97.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
@@ -108,15 +104,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -177,15 +173,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -292,27 +288,24 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.6.3
     # via
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
```

### Comparing `emmet-api-0.56.1/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.57.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -45,37 +45,37 @@
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -145,15 +145,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -271,17 +271,17 @@
     # via matplotlib
 platformdirs==3.5.3
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -420,17 +420,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   mypy
     #   pytest
```

### Comparing `emmet-api-0.56.1/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.57.0/requirements/macos-latest_py3.9.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,36 +38,40 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
+exceptiongroup==1.1.1
+    # via
+    #   anyio
+    #   cattrs
 fastapi==0.97.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
@@ -81,15 +85,19 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via matplotlib
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -104,15 +112,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -173,15 +181,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -288,31 +296,33 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.6.3
     # via
+    #   aioitertools
+    #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
@@ -322,11 +332,13 @@
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.56.1/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.57.0/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -45,37 +45,37 @@
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 fastapi==0.97.0
     # via
@@ -140,15 +140,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -266,17 +266,17 @@
     # via matplotlib
 platformdirs==3.5.3
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -415,17 +415,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
```

### Comparing `emmet-api-0.56.1/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.57.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,31 +38,31 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -114,15 +114,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -185,15 +185,15 @@
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -300,17 +300,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
```

### Comparing `emmet-api-0.56.1/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.57.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -45,37 +45,37 @@
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -154,15 +154,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -282,17 +282,17 @@
     # via jsonschema
 platformdirs==3.5.3
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -431,17 +431,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   mypy
     #   pytest
```

### Comparing `emmet-api-0.56.1/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.57.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,31 +38,31 @@
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -112,15 +112,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -181,15 +181,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -296,17 +296,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
```

### Comparing `emmet-api-0.56.1/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.57.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.152
+boto3==1.26.153
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.152
+botocore==1.29.153
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -45,37 +45,37 @@
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.14.0
+ddtrace==1.15.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.5
+emmet-core[all]==0.56.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
@@ -152,15 +152,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.7
+maggma==0.51.8
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -278,17 +278,17 @@
     # via matplotlib
 platformdirs==3.5.3
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.2
+protobuf==4.23.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -427,17 +427,15 @@
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
-    # via
-    #   ddtrace
-    #   plotly
+    # via plotly
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   mypy
     #   pytest
```

### Comparing `emmet-api-0.56.1/setup.py` & `emmet-api-0.57.0/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/_consumer/test_query_operators.py` & `emmet-api-0.57.0/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/_general_store/test_query_operators.py` & `emmet-api-0.57.0/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/core/test_mapi.py` & `emmet-api-0.57.0/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.57.0/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/electrodes/test_utils.py` & `emmet-api-0.57.0/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/materials/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/materials/test_utils.py` & `emmet-api-0.57.0/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/summary/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.57.0/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.57.0/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/synthesis/test_utils.py` & `emmet-api-0.57.0/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/tasks/test_utils.py` & `emmet-api-0.57.0/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/materials/xas/test_query_operators.py` & `emmet-api-0.57.0/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.57.0/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.57.0/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.57.0/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.57.0/tests/molecules/redox/test_query_operators.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,34 +2,32 @@
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_redox_potential_query():
     op = RedoxPotentialQuery()
     assert op.query(
-        electrode="Li",
         min_reduction_potential=0.0,
         max_reduction_potential=0.8,
         min_oxidation_potential=4.0,
         max_oxidation_potential=6.0,
     ) == {
         "criteria": {
-            "oxidation_potentials.Li": {"$gte": 4.0, "$lte": 6.0},
-            "reduction_potentials.Li": {"$gte": 0.0, "$lte": 0.8},
+            "oxidation_potential": {"$gte": 4.0, "$lte": 6.0},
+            "reduction_potential": {"$gte": 0.0, "$lte": 0.8},
         }
     }
 
     with ScratchDir("."):
         dumpfn(op, "temp.json")
         new_op = loadfn("temp.json")
         assert new_op.query(
-            electrode="Li",
             min_reduction_potential=0.0,
             max_reduction_potential=0.8,
             min_oxidation_potential=4.0,
             max_oxidation_potential=6.0,
         ) == {
             "criteria": {
-                "oxidation_potentials.Li": {"$gte": 4.0, "$lte": 6.0},
-                "reduction_potentials.Li": {"$gte": 0.0, "$lte": 0.8},
+                "oxidation_potential": {"$gte": 4.0, "$lte": 6.0},
+                "reduction_potential": {"$gte": 0.0, "$lte": 0.8},
             }
         }
```

### Comparing `emmet-api-0.56.1/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.57.0/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.57.0/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.56.1/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.57.0/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

