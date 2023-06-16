# Comparing `tmp/nevergrad-0.6.0.tar.gz` & `tmp/nevergrad-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nevergrad-0.6.0.tar", last modified: Wed Feb 22 16:06:29 2023, max compression
+gzip compressed data, was "dist/nevergrad-0.7.0.tar", last modified: Fri Jun 16 09:57:59 2023, max compression
```

## Comparing `nevergrad-0.6.0.tar` & `nevergrad-0.7.0.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.972730 nevergrad-0.6.0/
--rw-r--r--   0 jrapin     (501) staff       (20)     1086 2023-02-20 09:45:06.000000 nevergrad-0.6.0/LICENSE
--rw-r--r--   0 jrapin     (501) staff       (20)       53 2023-02-20 09:45:06.000000 nevergrad-0.6.0/MANIFEST.in
--rw-r--r--   0 jrapin     (501) staff       (20)     4797 2023-02-22 16:06:29.972456 nevergrad-0.6.0/PKG-INFO
--rw-r--r--   0 jrapin     (501) staff       (20)     3325 2023-02-20 09:45:06.000000 nevergrad-0.6.0/README.md
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.859775 nevergrad-0.6.0/nevergrad/
--rw-r--r--   0 jrapin     (501) staff       (20)      623 2023-02-22 15:53:36.000000 nevergrad-0.6.0/nevergrad/__init__.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.881820 nevergrad-0.6.0/nevergrad/benchmark/
--rw-r--r--   0 jrapin     (501) staff       (20)      271 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4910 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/__main__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    11376 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4979 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/execution.py
--rw-r--r--   0 jrapin     (501) staff       (20)    95004 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/experiments.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2922 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/exporttable.py
--rw-r--r--   0 jrapin     (501) staff       (20)    11579 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/frozenexperiments.py
--rw-r--r--   0 jrapin     (501) staff       (20)    13529 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/gymexperiments.py
--rw-r--r--   0 jrapin     (501) staff       (20)     8693 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/optgroups.py
--rw-r--r--   0 jrapin     (501) staff       (20)    41063 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/plotting.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6365 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3826 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/test_execution.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6535 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/test_experiments.py
--rw-r--r--   0 jrapin     (501) staff       (20)     8519 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/test_plotting.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2231 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/test_utils.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5902 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/test_xpbase.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4175 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/utils.py
--rw-r--r--   0 jrapin     (501) staff       (20)    13468 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/benchmark/xpbase.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.887235 nevergrad-0.6.0/nevergrad/common/
--rw-r--r--   0 jrapin     (501) staff       (20)      179 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2450 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/decorators.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2584 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/errors.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1653 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/test_decorators.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3458 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/test_testing.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2468 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/test_tools.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5710 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/testing.py
--rw-r--r--   0 jrapin     (501) staff       (20)     7429 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/tools.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2135 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/common/typing.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.897822 nevergrad-0.6.0/nevergrad/functions/
--rw-r--r--   0 jrapin     (501) staff       (20)      615 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/__init__.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.901632 nevergrad-0.6.0/nevergrad/functions/ac/
--rw-r--r--   0 jrapin     (501) staff       (20)      221 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/ac/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2923 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/ac/ac.py
--rw-r--r--   0 jrapin     (501) staff       (20)      506 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/ac/test_ac.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.904441 nevergrad-0.6.0/nevergrad/functions/arcoating/
--rw-r--r--   0 jrapin     (501) staff       (20)      221 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/arcoating/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3700 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/arcoating/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1957 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/arcoating/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)    18068 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/base.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.907788 nevergrad-0.6.0/nevergrad/functions/causaldiscovery/
--rw-r--r--   0 jrapin     (501) staff       (20)      233 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/causaldiscovery/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4136 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/causaldiscovery/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1711 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/causaldiscovery/test_core.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.916809 nevergrad-0.6.0/nevergrad/functions/control/
--rw-r--r--   0 jrapin     (501) staff       (20)      404 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/control/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    31738 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/control/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2677 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/control/mujoco.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2270 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/control/test_mujoco.py
--rw-r--r--   0 jrapin     (501) staff       (20)    13026 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/corefuncs.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.922859 nevergrad-0.6.0/nevergrad/functions/cycling/
--rw-r--r--   0 jrapin     (501) staff       (20)      247 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/cycling/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4456 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/cycling/cycling.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5024 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/cycling/cyclist.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4296 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/cycling/mensteampursuit.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1436 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/cycling/simulationresult.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4942 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/cycling/teampursuit.py
--rw-r--r--   0 jrapin     (501) staff       (20)      564 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/cycling/test_cycling.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3691 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/cycling/womensteampursuit.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.923820 nevergrad-0.6.0/nevergrad/functions/fishing/
--rw-r--r--   0 jrapin     (501) staff       (20)      227 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/fishing/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2059 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/fishing/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)      482 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/fishing/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)    15194 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/functionlib.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.925003 nevergrad-0.6.0/nevergrad/functions/games/
--rw-r--r--   0 jrapin     (501) staff       (20)      199 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/games/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    17992 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/games/game.py
--rw-r--r--   0 jrapin     (501) staff       (20)      936 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/games/test_game.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.926818 nevergrad-0.6.0/nevergrad/functions/gym/
--rw-r--r--   0 jrapin     (501) staff       (20)      267 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/gym/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    30916 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/gym/multigym.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4015 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/gym/test_multigym.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1569 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/gym/tuple_gym_env.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5735 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/helpers.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.929554 nevergrad-0.6.0/nevergrad/functions/images/
--rw-r--r--   0 jrapin     (501) staff       (20)      268 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/images/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    14277 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/images/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5594 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/images/imagelosses.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1311 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/images/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2138 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/images/test_imagelosses.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.930773 nevergrad-0.6.0/nevergrad/functions/iohprofiler/
--rw-r--r--   0 jrapin     (501) staff       (20)      276 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/iohprofiler/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6141 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/iohprofiler/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2396 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/iohprofiler/test_core.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.931798 nevergrad-0.6.0/nevergrad/functions/mixsimulator/
--rw-r--r--   0 jrapin     (501) staff       (20)      225 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/mixsimulator/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1643 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/mixsimulator/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)      468 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/mixsimulator/test_core.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.932825 nevergrad-0.6.0/nevergrad/functions/ml/
--rw-r--r--   0 jrapin     (501) staff       (20)      228 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/ml/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    15750 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/ml/mlfunctionlib.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3145 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/ml/test_mlfunctionlib.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.934986 nevergrad-0.6.0/nevergrad/functions/mlda/
--rw-r--r--   0 jrapin     (501) staff       (20)      372 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/mlda/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3757 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/mlda/datasets.py
--rw-r--r--   0 jrapin     (501) staff       (20)    10034 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/mlda/problems.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3322 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/mlda/test_datasets.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4334 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/mlda/test_problems.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.935380 nevergrad-0.6.0/nevergrad/functions/multiobjective/
--rw-r--r--   0 jrapin     (501) staff       (20)     1147 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/multiobjective/__init__.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.936401 nevergrad-0.6.0/nevergrad/functions/olympussurfaces/
--rw-r--r--   0 jrapin     (501) staff       (20)      284 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/olympussurfaces/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4355 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/olympussurfaces/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1670 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/olympussurfaces/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5637 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/pbt.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.937822 nevergrad-0.6.0/nevergrad/functions/photonics/
--rw-r--r--   0 jrapin     (501) staff       (20)      221 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/photonics/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     8008 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/photonics/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)    15293 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/photonics/photonics.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6864 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/photonics/test_core.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.938947 nevergrad-0.6.0/nevergrad/functions/powersystems/
--rw-r--r--   0 jrapin     (501) staff       (20)      225 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/powersystems/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    13522 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/powersystems/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)      859 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/powersystems/test_core.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.940431 nevergrad-0.6.0/nevergrad/functions/pyomo/
--rw-r--r--   0 jrapin     (501) staff       (20)      213 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/pyomo/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     8344 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/pyomo/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3463 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/pyomo/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2859 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/pyomo/test_pyomo_doc.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.942354 nevergrad-0.6.0/nevergrad/functions/rl/
--rw-r--r--   0 jrapin     (501) staff       (20)      295 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rl/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     7070 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rl/agents.py
--rw-r--r--   0 jrapin     (501) staff       (20)     9742 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rl/base.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5317 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rl/envs.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3016 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rl/test_agents.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3538 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rl/test_envs.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.944094 nevergrad-0.6.0/nevergrad/functions/rocket/
--rw-r--r--   0 jrapin     (501) staff       (20)      217 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rocket/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    12181 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rocket/rocket.py
--rw-r--r--   0 jrapin     (501) staff       (20)      446 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/rocket/test_rocket.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.945675 nevergrad-0.6.0/nevergrad/functions/stsp/
--rw-r--r--   0 jrapin     (501) staff       (20)      211 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/stsp/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1757 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/stsp/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)      562 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/stsp/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     8614 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/test_base.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3746 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/test_corefuncs.py
--rw-r--r--   0 jrapin     (501) staff       (20)     9269 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/test_functionlib.py
--rw-r--r--   0 jrapin     (501) staff       (20)      655 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/test_utils.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.946698 nevergrad-0.6.0/nevergrad/functions/unitcommitment/
--rw-r--r--   0 jrapin     (501) staff       (20)      245 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/unitcommitment/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3453 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/unitcommitment/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)      665 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/unitcommitment/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1371 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/functions/utils.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.947792 nevergrad-0.6.0/nevergrad/ops/
--rw-r--r--   0 jrapin     (501) staff       (20)      374 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/ops/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3824 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/ops/constraints.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1025 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/ops/test_constraints.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.959777 nevergrad-0.6.0/nevergrad/optimization/
--rw-r--r--   0 jrapin     (501) staff       (20)      319 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    41000 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/base.py
--rw-r--r--   0 jrapin     (501) staff       (20)    14126 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/callbacks.py
--rw-r--r--   0 jrapin     (501) staff       (20)    17534 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/differentialevolution.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6295 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/es.py
--rw-r--r--   0 jrapin     (501) staff       (20)    19628 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/experimentalvariants.py
--rw-r--r--   0 jrapin     (501) staff       (20)     9958 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/externalbo.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1537 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/families.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2769 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/helpers.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3131 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/metamodel.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.962394 nevergrad-0.6.0/nevergrad/optimization/multiobjective/
--rw-r--r--   0 jrapin     (501) staff       (20)      350 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/multiobjective/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    12534 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/multiobjective/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)    13167 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/multiobjective/hypervolume.py
--rw-r--r--   0 jrapin     (501) staff       (20)     9935 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/multiobjective/nsga2.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5561 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/multiobjective/test_core.py
--rw-r--r--   0 jrapin     (501) staff       (20)     9883 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/multiobjective/test_hypervolume.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5819 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/multiobjective/test_nsga2.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6561 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/mutations.py
--rw-r--r--   0 jrapin     (501) staff       (20)    20194 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/oneshot.py
--rw-r--r--   0 jrapin     (501) staff       (20)   137696 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/optimizerlib.py
--rw-r--r--   0 jrapin     (501) staff       (20)    18010 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/recaster.py
--rw-r--r--   0 jrapin     (501) staff       (20)    20594 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/recastlib.py
--rw-r--r--   0 jrapin     (501) staff       (20)      761 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/requirements_check.py
--rw-r--r--   0 jrapin     (501) staff       (20)     8616 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/sequences.py
--rw-r--r--   0 jrapin     (501) staff       (20)     8138 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_base.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6692 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_callbacks.py
--rw-r--r--   0 jrapin     (501) staff       (20)     7557 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_doc.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5143 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_externalbo.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3191 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_mutations.py
--rw-r--r--   0 jrapin     (501) staff       (20)    37750 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_optimizerlib.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6927 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_recaster.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1389 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_sa.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3756 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_sequences.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3296 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_special.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4419 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_suggest.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2463 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_tabu.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5267 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/test_utils.py
--rw-r--r--   0 jrapin     (501) staff       (20)    14309 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/optimization/utils.py
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.970938 nevergrad-0.6.0/nevergrad/parametrization/
--rw-r--r--   0 jrapin     (501) staff       (20)      472 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/__init__.py
--rw-r--r--   0 jrapin     (501) staff       (20)    14333 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/_datalayers.py
--rw-r--r--   0 jrapin     (501) staff       (20)    10997 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/_layering.py
--rw-r--r--   0 jrapin     (501) staff       (20)    10415 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/choice.py
--rw-r--r--   0 jrapin     (501) staff       (20)     9435 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/container.py
--rw-r--r--   0 jrapin     (501) staff       (20)    21684 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/core.py
--rw-r--r--   0 jrapin     (501) staff       (20)    21250 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/data.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5375 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/discretization.py
--rw-r--r--   0 jrapin     (501) staff       (20)     9664 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/helpers.py
--rw-r--r--   0 jrapin     (501) staff       (20)    12840 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/instantiate.py
--rw-r--r--   0 jrapin     (501) staff       (20)    13948 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/mutation.py
--rw-r--r--   0 jrapin     (501) staff       (20)     1101 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/parameter.py
--rw-r--r--   0 jrapin     (501) staff       (20)     2166 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_discretization.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6133 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_instantiate.py
--rw-r--r--   0 jrapin     (501) staff       (20)     5599 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_layers.py
--rw-r--r--   0 jrapin     (501) staff       (20)     4599 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_mutation.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3098 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_param_doc.py
--rw-r--r--   0 jrapin     (501) staff       (20)    16652 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_parameter.py
--rw-r--r--   0 jrapin     (501) staff       (20)     6548 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_parameters_legacy.py
--rw-r--r--   0 jrapin     (501) staff       (20)     3994 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_transforms.py
--rw-r--r--   0 jrapin     (501) staff       (20)    11025 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/test_utils.py
--rw-r--r--   0 jrapin     (501) staff       (20)    10944 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/transforms.py
--rw-r--r--   0 jrapin     (501) staff       (20)     9987 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/parametrization/utils.py
--rw-r--r--   0 jrapin     (501) staff       (20)        0 2023-02-20 09:45:06.000000 nevergrad-0.6.0/nevergrad/py.typed
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.862492 nevergrad-0.6.0/nevergrad.egg-info/
--rw-r--r--   0 jrapin     (501) staff       (20)     4797 2023-02-22 16:06:29.000000 nevergrad-0.6.0/nevergrad.egg-info/PKG-INFO
--rw-r--r--   0 jrapin     (501) staff       (20)     7356 2023-02-22 16:06:29.000000 nevergrad-0.6.0/nevergrad.egg-info/SOURCES.txt
--rw-r--r--   0 jrapin     (501) staff       (20)        1 2023-02-22 16:06:29.000000 nevergrad-0.6.0/nevergrad.egg-info/dependency_links.txt
--rw-r--r--   0 jrapin     (501) staff       (20)     1891 2023-02-22 16:06:29.000000 nevergrad-0.6.0/nevergrad.egg-info/requires.txt
--rw-r--r--   0 jrapin     (501) staff       (20)       10 2023-02-22 16:06:29.000000 nevergrad-0.6.0/nevergrad.egg-info/top_level.txt
--rw-r--r--   0 jrapin     (501) staff       (20)      206 2023-02-20 09:45:06.000000 nevergrad-0.6.0/pyproject.toml
-drwxr-xr-x   0 jrapin     (501) staff       (20)        0 2023-02-22 16:06:29.972001 nevergrad-0.6.0/requirements/
--rw-r--r--   0 jrapin     (501) staff       (20)      827 2023-02-20 09:45:06.000000 nevergrad-0.6.0/requirements/bench.txt
--rw-r--r--   0 jrapin     (501) staff       (20)      348 2023-02-20 09:45:06.000000 nevergrad-0.6.0/requirements/dev.txt
--rw-r--r--   0 jrapin     (501) staff       (20)       86 2023-02-20 09:45:06.000000 nevergrad-0.6.0/requirements/main.txt
--rw-r--r--   0 jrapin     (501) staff       (20)       38 2023-02-22 16:06:29.972819 nevergrad-0.6.0/setup.cfg
--rw-r--r--   0 jrapin     (501) staff       (20)     3131 2023-02-20 09:45:06.000000 nevergrad-0.6.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1086 2023-06-16 09:52:50.000000 nevergrad-0.7.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-16 09:52:50.000000 nevergrad-0.7.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4076 2023-06-16 09:57:59.000000 nevergrad-0.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2023-06-16 09:52:50.000000 nevergrad-0.7.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/benchmark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4910 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11376 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4979 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/execution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    95004 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/experiments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2922 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/exporttable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11579 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/frozenexperiments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13529 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/gymexperiments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8693 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/optgroups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41063 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/plotting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3826 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_execution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6658 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_experiments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8519 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_plotting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2231 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5902 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_xpbase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4175 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13468 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/xpbase.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2450 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/decorators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2584 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/test_decorators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3458 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/test_testing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2468 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/test_tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5710 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/testing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2135 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/ac/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/ac/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2923 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/ac/ac.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      506 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/ac/test_ac.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/arcoating/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/arcoating/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3700 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/arcoating/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1957 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/arcoating/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18068 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/causaldiscovery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/causaldiscovery/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4136 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/causaldiscovery/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/causaldiscovery/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/control/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/control/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/control/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2677 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/control/mujoco.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/control/test_mujoco.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13026 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/corefuncs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/cycling/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/cycling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5024 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/cyclist.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4296 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/mensteampursuit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1436 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/simulationresult.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4942 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/teampursuit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      564 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/test_cycling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3691 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/womensteampursuit.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/fishing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/fishing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2059 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/fishing/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/fishing/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15194 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/functionlib.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/games/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/games/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17992 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/games/game.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      936 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/games/test_game.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/gym/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/gym/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30916 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/gym/multigym.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/gym/test_multigym.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/gym/tuple_gym_env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5735 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/helpers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14277 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5594 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/imagelosses.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1311 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/test_imagelosses.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/iohprofiler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      276 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/iohprofiler/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6141 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/iohprofiler/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2396 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/iohprofiler/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/mixsimulator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mixsimulator/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mixsimulator/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      468 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mixsimulator/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/ml/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/ml/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15750 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/ml/mlfunctionlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3145 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/ml/test_mlfunctionlib.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/mlda/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      372 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3757 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/datasets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10034 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/problems.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3322 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/test_datasets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4334 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/test_problems.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/multiobjective/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/multiobjective/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/olympussurfaces/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/olympussurfaces/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4355 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/olympussurfaces/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1670 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/olympussurfaces/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5637 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pbt.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/photonics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/photonics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8008 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/photonics/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15293 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/photonics/photonics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6864 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/photonics/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/powersystems/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/powersystems/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13522 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/powersystems/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/powersystems/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8360 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3463 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2859 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/test_pyomo_doc.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/rl/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7070 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9742 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5317 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/envs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3016 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/test_agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3538 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/test_envs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/rocket/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rocket/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12181 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rocket/rocket.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rocket/test_rocket.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/stsp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/stsp/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/stsp/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/stsp/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8614 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3746 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/test_corefuncs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/test_functionlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/unitcommitment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/unitcommitment/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3453 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/unitcommitment/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/unitcommitment/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1371 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/ops/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/ops/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3824 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/ops/constraints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/ops/test_constraints.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/optimization/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41000 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14126 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/callbacks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17988 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/differentialevolution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6295 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20000 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/experimentalvariants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9958 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/externalbo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1537 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/families.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3664 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/metamodel.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12534 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13167 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/hypervolume.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9935 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/nsga2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5561 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9883 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_hypervolume.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5819 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_nsga2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/mutations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20194 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/oneshot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   138230 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/optimizerlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18010 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/recaster.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20594 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/recastlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/requirements_check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8616 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/sequences.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8138 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6692 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_callbacks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7557 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_doc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5143 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_externalbo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_mutations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38904 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_optimizerlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6927 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_recaster.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_sa.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3756 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_sequences.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_special.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4609 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_suggest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2405 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_tabu.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5267 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14309 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/parametrization/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      472 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14333 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/_datalayers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10997 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/_layering.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10415 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/choice.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9435 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/container.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21684 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21250 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5375 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/discretization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9664 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12840 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/instantiate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/mutation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1101 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/parameter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2166 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_discretization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_instantiate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5599 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_layers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4599 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_mutation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3098 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_param_doc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16652 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_parameter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6548 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_parameters_legacy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3994 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_transforms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11025 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10944 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/transforms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9987 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4076 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1876 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-06-16 09:52:51.000000 nevergrad-0.7.0/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/requirements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2023-06-16 09:52:51.000000 nevergrad-0.7.0/requirements/bench.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2023-06-16 09:52:51.000000 nevergrad-0.7.0/requirements/dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-06-16 09:52:51.000000 nevergrad-0.7.0/requirements/main.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-16 09:57:59.000000 nevergrad-0.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3131 2023-06-16 09:52:51.000000 nevergrad-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nevergrad-0.6.0/LICENSE` & `nevergrad-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/PKG-INFO` & `nevergrad-0.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 Metadata-Version: 2.1
 Name: nevergrad
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python toolbox for performing gradient-free optimization
 Home-page: https://github.com/facebookresearch/nevergrad
 Author: Facebook AI Research
 License: MIT
-Description: [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-ukraine) [![CircleCI](https://circleci.com/gh/facebookresearch/nevergrad/tree/main.svg?style=svg)](https://circleci.com/gh/facebookresearch/nevergrad/tree/main)
-        
-        # Nevergrad - A gradient-free optimization platform
-        
-        ![Nevergrad](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.6.0/docs/resources/Nevergrad-LogoMark.png)
-        
-        
-        `nevergrad` is a Python 3.6+ library. It can be installed with:
-        
-        ```
-        pip install nevergrad
-        ```
-        
-        More installation options, including windows installation, and complete instructions are available in the "Getting started" section of the [**documentation**](https://facebookresearch.github.io/nevergrad/).
-        
-        You can join Nevergrad users Facebook group [here](https://www.facebook.com/groups/nevergradusers/).
-        
-        Minimizing a function using an optimizer (here `NGOpt`) is straightforward:
-        
-        ```python
-        import nevergrad as ng
-        
-        def square(x):
-            return sum((x - .5)**2)
-        
-        optimizer = ng.optimizers.NGOpt(parametrization=2, budget=100)
-        recommendation = optimizer.minimize(square)
-        print(recommendation.value)  # recommended value
-        >>> [0.49971112 0.5002944]
-        ```
-        
-        `nevergrad` can also support bounded continuous variables as well as discrete variables, and mixture of those.
-        To do this, one can specify the input space:
-        
-        ```python
-        import nevergrad as ng
-        
-        def fake_training(learning_rate: float, batch_size: int, architecture: str) -> float:
-            # optimal for learning_rate=0.2, batch_size=4, architecture="conv"
-            return (learning_rate - 0.2)**2 + (batch_size - 4)**2 + (0 if architecture == "conv" else 10)
-        
-        # Instrumentation class is used for functions with multiple inputs
-        # (positional and/or keywords)
-        parametrization = ng.p.Instrumentation(
-            # a log-distributed scalar between 0.001 and 1.0
-            learning_rate=ng.p.Log(lower=0.001, upper=1.0),
-            # an integer from 1 to 12
-            batch_size=ng.p.Scalar(lower=1, upper=12).set_integer_casting(),
-            # either "conv" or "fc"
-            architecture=ng.p.Choice(["conv", "fc"])
-        )
-        
-        optimizer = ng.optimizers.NGOpt(parametrization=parametrization, budget=100)
-        recommendation = optimizer.minimize(fake_training)
-        
-        # show the recommended keyword arguments of the function
-        print(recommendation.kwargs)
-        >>> {'learning_rate': 0.1998, 'batch_size': 4, 'architecture': 'conv'}
-        ```
-        
-        Learn more on parametrization in the [**documentation**](https://facebookresearch.github.io/nevergrad/)!
-        
-        ![Example of optimization](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.6.0/docs/resources/TwoPointsDE.gif)
-        
-        *Convergence of a population of points to the minima with two-points DE.*
-        
-        
-        ## Documentation
-        
-        Check out our [**documentation**](https://facebookresearch.github.io/nevergrad/)! It's still a work in progress, don't hesitate to submit issues and/or PR to update it and make it clearer!
-        
-        
-        ## Citing
-        
-        ```bibtex
-        @misc{nevergrad,
-            author = {J. Rapin and O. Teytaud},
-            title = {{Nevergrad - A gradient-free optimization platform}},
-            year = {2018},
-            publisher = {GitHub},
-            journal = {GitHub repository},
-            howpublished = {\url{https://GitHub.com/FacebookResearch/Nevergrad}},
-        }
-        ```
-        
-        ## License
-        
-        `nevergrad` is released under the MIT license. See [LICENSE](https://github.com/facebookresearch/nevergrad/blob/0.6.0/LICENSE) for additional details about it.
-        See also our [Terms of Use](https://opensource.facebook.com/legal/terms) and [Privacy Policy](https://opensource.facebook.com/legal/privacy).
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: benchmark
+License-File: LICENSE
+
+[![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-ukraine) [![CircleCI](https://circleci.com/gh/facebookresearch/nevergrad/tree/main.svg?style=svg)](https://circleci.com/gh/facebookresearch/nevergrad/tree/main)
+
+# Nevergrad - A gradient-free optimization platform
+
+![Nevergrad](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.7.0/docs/resources/Nevergrad-LogoMark.png)
+
+
+`nevergrad` is a Python 3.6+ library. It can be installed with:
+
+```
+pip install nevergrad
+```
+
+More installation options, including windows installation, and complete instructions are available in the "Getting started" section of the [**documentation**](https://facebookresearch.github.io/nevergrad/).
+
+You can join Nevergrad users Facebook group [here](https://www.facebook.com/groups/nevergradusers/).
+
+Minimizing a function using an optimizer (here `NGOpt`) is straightforward:
+
+```python
+import nevergrad as ng
+
+def square(x):
+    return sum((x - .5)**2)
+
+optimizer = ng.optimizers.NGOpt(parametrization=2, budget=100)
+recommendation = optimizer.minimize(square)
+print(recommendation.value)  # recommended value
+>>> [0.49971112 0.5002944]
+```
+
+`nevergrad` can also support bounded continuous variables as well as discrete variables, and mixture of those.
+To do this, one can specify the input space:
+
+```python
+import nevergrad as ng
+
+def fake_training(learning_rate: float, batch_size: int, architecture: str) -> float:
+    # optimal for learning_rate=0.2, batch_size=4, architecture="conv"
+    return (learning_rate - 0.2)**2 + (batch_size - 4)**2 + (0 if architecture == "conv" else 10)
+
+# Instrumentation class is used for functions with multiple inputs
+# (positional and/or keywords)
+parametrization = ng.p.Instrumentation(
+    # a log-distributed scalar between 0.001 and 1.0
+    learning_rate=ng.p.Log(lower=0.001, upper=1.0),
+    # an integer from 1 to 12
+    batch_size=ng.p.Scalar(lower=1, upper=12).set_integer_casting(),
+    # either "conv" or "fc"
+    architecture=ng.p.Choice(["conv", "fc"])
+)
+
+optimizer = ng.optimizers.NGOpt(parametrization=parametrization, budget=100)
+recommendation = optimizer.minimize(fake_training)
+
+# show the recommended keyword arguments of the function
+print(recommendation.kwargs)
+>>> {'learning_rate': 0.1998, 'batch_size': 4, 'architecture': 'conv'}
+```
+
+Learn more on parametrization in the [**documentation**](https://facebookresearch.github.io/nevergrad/)!
+
+![Example of optimization](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.7.0/docs/resources/TwoPointsDE.gif)
+
+*Convergence of a population of points to the minima with two-points DE.*
+
+
+## Documentation
+
+Check out our [**documentation**](https://facebookresearch.github.io/nevergrad/)! It's still a work in progress, don't hesitate to submit issues and/or PR to update it and make it clearer!
+
+
+## Citing
+
+```bibtex
+@misc{nevergrad,
+    author = {J. Rapin and O. Teytaud},
+    title = {{Nevergrad - A gradient-free optimization platform}},
+    year = {2018},
+    publisher = {GitHub},
+    journal = {GitHub repository},
+    howpublished = {\url{https://GitHub.com/FacebookResearch/Nevergrad}},
+}
+```
+
+## License
+
+`nevergrad` is released under the MIT license. See [LICENSE](https://github.com/facebookresearch/nevergrad/blob/0.7.0/LICENSE) for additional details about it.
+See also our [Terms of Use](https://opensource.facebook.com/legal/terms) and [Privacy Policy](https://opensource.facebook.com/legal/privacy).
```

### Comparing `nevergrad-0.6.0/README.md` & `nevergrad-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/__init__.py` & `nevergrad-0.7.0/nevergrad/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 from .common import errors as errors
 from . import ops as ops
 
 
 __all__ = ["optimizers", "families", "callbacks", "p", "typing", "errors", "ops"]
 
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
```

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/__main__.py` & `nevergrad-0.7.0/nevergrad/benchmark/__main__.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/core.py` & `nevergrad-0.7.0/nevergrad/benchmark/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/execution.py` & `nevergrad-0.7.0/nevergrad/benchmark/execution.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/experiments.py` & `nevergrad-0.7.0/nevergrad/benchmark/experiments.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/exporttable.py` & `nevergrad-0.7.0/nevergrad/benchmark/exporttable.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/frozenexperiments.py` & `nevergrad-0.7.0/nevergrad/benchmark/frozenexperiments.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/gymexperiments.py` & `nevergrad-0.7.0/nevergrad/benchmark/gymexperiments.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/optgroups.py` & `nevergrad-0.7.0/nevergrad/benchmark/optgroups.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/plotting.py` & `nevergrad-0.7.0/nevergrad/benchmark/plotting.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/test_core.py` & `nevergrad-0.7.0/nevergrad/benchmark/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/test_execution.py` & `nevergrad-0.7.0/nevergrad/benchmark/test_execution.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/test_experiments.py` & `nevergrad-0.7.0/nevergrad/benchmark/test_experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 from .utils import Selector
 from . import experiments
 from . import optgroups
 
 
 @testing.parametrized(**{name: (name, maker) for name, maker in experiments.registry.items()})
 def test_experiments_registry(name: str, maker: tp.Callable[[], tp.Iterator[experiments.Experiment]]) -> None:
+    if sum([ord(c) for c in name]) % 4 > 0:
+        raise SkipTest("Too expensive: we randomly skip 3/4 of these tests.")
+
     # "mav" is not availablefor now.
     if "conformant" in name or name == "neuro_planning":
         raise SkipTest("This is user parametric and can not be tested.")
 
     if "compiler" in name or "emulators" in name:
         raise SkipTest("Compiler/emulator stuff too heavy for CircleCI.")
```

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/test_plotting.py` & `nevergrad-0.7.0/nevergrad/benchmark/test_plotting.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/test_utils.py` & `nevergrad-0.7.0/nevergrad/benchmark/test_utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/test_xpbase.py` & `nevergrad-0.7.0/nevergrad/benchmark/test_xpbase.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/utils.py` & `nevergrad-0.7.0/nevergrad/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/benchmark/xpbase.py` & `nevergrad-0.7.0/nevergrad/benchmark/xpbase.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/common/decorators.py` & `nevergrad-0.7.0/nevergrad/common/decorators.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/common/errors.py` & `nevergrad-0.7.0/nevergrad/common/errors.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/common/test_decorators.py` & `nevergrad-0.7.0/nevergrad/common/test_decorators.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/common/test_testing.py` & `nevergrad-0.7.0/nevergrad/common/test_testing.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/common/test_tools.py` & `nevergrad-0.7.0/nevergrad/common/test_tools.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/common/testing.py` & `nevergrad-0.7.0/nevergrad/common/testing.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/common/tools.py` & `nevergrad-0.7.0/nevergrad/common/tools.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/common/typing.py` & `nevergrad-0.7.0/nevergrad/common/typing.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/__init__.py` & `nevergrad-0.7.0/nevergrad/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/ac/ac.py` & `nevergrad-0.7.0/nevergrad/functions/ac/ac.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/arcoating/core.py` & `nevergrad-0.7.0/nevergrad/functions/arcoating/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/arcoating/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/arcoating/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/base.py` & `nevergrad-0.7.0/nevergrad/functions/base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/causaldiscovery/core.py` & `nevergrad-0.7.0/nevergrad/functions/causaldiscovery/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/causaldiscovery/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/causaldiscovery/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/control/core.py` & `nevergrad-0.7.0/nevergrad/functions/control/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/control/mujoco.py` & `nevergrad-0.7.0/nevergrad/functions/control/mujoco.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/control/test_mujoco.py` & `nevergrad-0.7.0/nevergrad/functions/control/test_mujoco.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/corefuncs.py` & `nevergrad-0.7.0/nevergrad/functions/corefuncs.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/cycling/cycling.py` & `nevergrad-0.7.0/nevergrad/functions/cycling/cycling.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/cycling/cyclist.py` & `nevergrad-0.7.0/nevergrad/functions/cycling/cyclist.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/cycling/mensteampursuit.py` & `nevergrad-0.7.0/nevergrad/functions/cycling/mensteampursuit.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/cycling/simulationresult.py` & `nevergrad-0.7.0/nevergrad/functions/cycling/simulationresult.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/cycling/teampursuit.py` & `nevergrad-0.7.0/nevergrad/functions/cycling/teampursuit.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/cycling/test_cycling.py` & `nevergrad-0.7.0/nevergrad/functions/cycling/test_cycling.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/cycling/womensteampursuit.py` & `nevergrad-0.7.0/nevergrad/functions/cycling/womensteampursuit.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/fishing/core.py` & `nevergrad-0.7.0/nevergrad/functions/fishing/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/functionlib.py` & `nevergrad-0.7.0/nevergrad/functions/functionlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/games/game.py` & `nevergrad-0.7.0/nevergrad/functions/games/game.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/games/test_game.py` & `nevergrad-0.7.0/nevergrad/functions/games/test_game.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/gym/multigym.py` & `nevergrad-0.7.0/nevergrad/functions/gym/multigym.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/gym/test_multigym.py` & `nevergrad-0.7.0/nevergrad/functions/gym/test_multigym.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,37 +19,32 @@
         assert env_name in GYM_ENV_NAMES, f"{env_name} unknown!"
         assert env_name not in multigym.NO_LENGTH, f"{env_name} in no length and in ng_gym!"
     for env_name in multigym.GUARANTEED_GYM_ENV_NAMES:
         assert env_name in GYM_ENV_NAMES, f"{env_name} should be guaranteed!"
     assert len(GYM_ENV_NAMES) >= 10 or os.name == "nt"
 
 
-def test_cartpole() -> None:
-    func = multigym.GymMulti(name="CartPole-v0", control="neural", neural_factor=1, randomized=True)
-    results = [func(np.zeros(func.dimension)) for _ in range(40)]
-    assert min(results) != max(results), "CartPole should not be deterministic."
-    candidate = func.parametrization.sample()
-    results = [func.evaluation_function(candidate) for _ in range(40)]
-    assert min(results) != max(results), "CartPole should not be deterministic."
-
-
-def test_sparse_cartpole() -> None:
-    func = multigym.GymMulti(
-        name="CartPole-v0", control="neural", neural_factor=1, randomized=True, sparse_limit=2
-    )
-    results = []
-    for _ in range(40):
-        param = func.parametrization.sample()
-        results.append(func(*param.args, **param.kwargs))
-    assert min(results) != max(results), "CartPole should not be deterministic."
-    candidate = func.parametrization.sample()
-    results = [func.evaluation_function(candidate) for _ in range(40)]
-    assert min(results) != max(results), "CartPole should not be deterministic."
-
-
+# def test_cartpole() -> None:
+#    func = multigym.GymMulti(name="CartPole-v0", control="neural", neural_factor=1, randomized=True)
+#    candidate = func.parametrization.sample()
+#    results = [func.evaluation_function(candidate) for _ in range(40)]
+#    assert min(results) != max(results), "CartPole should not be deterministic."
+#
+#
+# def test_sparse_cartpole() -> None:
+#    func = multigym.GymMulti(
+#        name="CartPole-v0", control="neural", neural_factor=1, randomized=True, sparse_limit=2
+#    )
+#    param = func.parametrization.sample()
+#    func(*param.args, **param.kwargs)
+#    candidate = func.parametrization.sample()
+#    results = [func.evaluation_function(candidate) for _ in range(40)]
+#    assert min(results) != max(results), "CartPole should not be deterministic."
+#
+#
 @pytest.mark.parametrize("name", ["LunarLander-v2"])  # type: ignore
 def test_run_multigym(name: str) -> None:
     if os.name == "nt" or np.random.randint(8) or "CubeCrash" in name:
         raise SkipTest("Skipping Windows and running only 1 out of 8")
     if "ANM" in name:
         raise SkipTest("We skip ANM6Easy and related problems.")
```

### Comparing `nevergrad-0.6.0/nevergrad/functions/gym/tuple_gym_env.py` & `nevergrad-0.7.0/nevergrad/functions/gym/tuple_gym_env.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/helpers.py` & `nevergrad-0.7.0/nevergrad/functions/helpers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/images/core.py` & `nevergrad-0.7.0/nevergrad/functions/images/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/images/imagelosses.py` & `nevergrad-0.7.0/nevergrad/functions/images/imagelosses.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/images/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/images/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/images/test_imagelosses.py` & `nevergrad-0.7.0/nevergrad/functions/images/test_imagelosses.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/iohprofiler/core.py` & `nevergrad-0.7.0/nevergrad/functions/iohprofiler/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/iohprofiler/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/iohprofiler/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/mixsimulator/core.py` & `nevergrad-0.7.0/nevergrad/functions/mixsimulator/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/ml/mlfunctionlib.py` & `nevergrad-0.7.0/nevergrad/functions/ml/mlfunctionlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/ml/test_mlfunctionlib.py` & `nevergrad-0.7.0/nevergrad/functions/ml/test_mlfunctionlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/mlda/datasets.py` & `nevergrad-0.7.0/nevergrad/functions/mlda/datasets.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/mlda/problems.py` & `nevergrad-0.7.0/nevergrad/functions/mlda/problems.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/mlda/test_datasets.py` & `nevergrad-0.7.0/nevergrad/functions/mlda/test_datasets.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/mlda/test_problems.py` & `nevergrad-0.7.0/nevergrad/functions/mlda/test_problems.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/multiobjective/__init__.py` & `nevergrad-0.7.0/nevergrad/functions/multiobjective/__init__.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/olympussurfaces/core.py` & `nevergrad-0.7.0/nevergrad/functions/olympussurfaces/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/olympussurfaces/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/olympussurfaces/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/pbt.py` & `nevergrad-0.7.0/nevergrad/functions/pbt.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/photonics/core.py` & `nevergrad-0.7.0/nevergrad/functions/photonics/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/photonics/photonics.py` & `nevergrad-0.7.0/nevergrad/functions/photonics/photonics.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/photonics/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/photonics/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/powersystems/core.py` & `nevergrad-0.7.0/nevergrad/functions/powersystems/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/powersystems/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/powersystems/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/pyomo/core.py` & `nevergrad-0.7.0/nevergrad/functions/pyomo/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         self.add_descriptors(name=exp_tag)
 
     def _pyomo_value_assignment(self, k_model_variables: tp.Dict[str, tp.Any]) -> None:
         if self._value_assignment_code_obj == "":
             code_str = ""
             for k in k_model_variables:
                 code_str += f"self._model_instance.{k} = k_model_variables['{k}']\n"
-            self._value_assignment_code_obj = compile(code_str, "<string>", "exec")
+            self._value_assignment_code_obj = compile(code_str, "<string>", "exec")  # type: ignore
         # TODO find a way to avoid exec
         exec(self._value_assignment_code_obj)  # pylint: disable=exec-used
 
     def _pyomo_obj_function_wrapper(self, i: int, **k_model_variables: tp.Dict[str, tp.Any]) -> float:
         self._pyomo_value_assignment(k_model_variables)
         return float(
             pyomo.value(self.all_objectives[i] * self.all_objectives[i].sense)
```

### Comparing `nevergrad-0.6.0/nevergrad/functions/pyomo/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/pyomo/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/pyomo/test_pyomo_doc.py` & `nevergrad-0.7.0/nevergrad/functions/pyomo/test_pyomo_doc.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/rl/agents.py` & `nevergrad-0.7.0/nevergrad/functions/rl/agents.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/rl/base.py` & `nevergrad-0.7.0/nevergrad/functions/rl/base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/rl/envs.py` & `nevergrad-0.7.0/nevergrad/functions/rl/envs.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/rl/test_agents.py` & `nevergrad-0.7.0/nevergrad/functions/rl/test_agents.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/rl/test_envs.py` & `nevergrad-0.7.0/nevergrad/functions/rl/test_envs.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/rocket/rocket.py` & `nevergrad-0.7.0/nevergrad/functions/rocket/rocket.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/stsp/core.py` & `nevergrad-0.7.0/nevergrad/functions/stsp/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/stsp/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/stsp/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/test_base.py` & `nevergrad-0.7.0/nevergrad/functions/test_base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/test_corefuncs.py` & `nevergrad-0.7.0/nevergrad/functions/test_corefuncs.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/test_functionlib.py` & `nevergrad-0.7.0/nevergrad/functions/test_functionlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/test_utils.py` & `nevergrad-0.7.0/nevergrad/functions/test_utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/unitcommitment/core.py` & `nevergrad-0.7.0/nevergrad/functions/unitcommitment/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/unitcommitment/test_core.py` & `nevergrad-0.7.0/nevergrad/functions/unitcommitment/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/functions/utils.py` & `nevergrad-0.7.0/nevergrad/functions/utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/ops/constraints.py` & `nevergrad-0.7.0/nevergrad/ops/constraints.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/ops/test_constraints.py` & `nevergrad-0.7.0/nevergrad/ops/test_constraints.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/base.py` & `nevergrad-0.7.0/nevergrad/optimization/base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/callbacks.py` & `nevergrad-0.7.0/nevergrad/optimization/callbacks.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/differentialevolution.py` & `nevergrad-0.7.0/nevergrad/optimization/differentialevolution.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,17 +84,19 @@
 
     def __init__(
         self,
         parametrization: base.IntOrParameter,
         budget: tp.Optional[int] = None,
         num_workers: int = 1,
         config: tp.Optional["DifferentialEvolution"] = None,
+        weights: tp.Any = None,
     ) -> None:
         super().__init__(parametrization, budget=budget, num_workers=num_workers)
         # config
+        self.objective_weights = weights
         self._config = DifferentialEvolution() if config is None else config
         self.scale = (
             float(1.0 / np.sqrt(self.dimension))
             if isinstance(self._config.scale, str)
             else self._config.scale
         )
         pop_choice = {"standard": 0, "dimension": self.dimension + 1, "large": 7 * self.dimension}
@@ -110,14 +112,17 @@
         self._MULTIOBJECTIVE_AUTO_BOUND = max(self._MULTIOBJECTIVE_AUTO_BOUND, self.llambda)
         self._penalize_cheap_violations = True
         self._uid_queue = base.utils.UidQueue()
         self.population: tp.Dict[str, p.Parameter] = {}
         self.sampler: tp.Optional[base.Optimizer] = None
         self._no_hypervolume = self._config.multiobjective_adaptation
 
+    def set_objective_weights(self, weights: tp.Any) -> None:
+        self.objective_weights = weights
+
     def recommend(self) -> p.Parameter:  # This is NOT the naive version. We deal with noise.
         sample_size = int((self.dimension * (self.dimension - 1)) / 2 + 2 * self.dimension + 1)
         if self._config.high_speed and len(self.archive) >= sample_size:
             try:
                 meta_data = metamodel.learn_on_k_best(self.archive, sample_size)
                 return self.parametrization.spawn_child().set_standardized_data(meta_data)
             except metamodel.MetaModelFailure:  # The optimum is at infinity. Shit happens.
@@ -196,19 +201,25 @@
         uid = candidate.heritage["lineage"]
         if uid not in self.population:  # parent was removed, revert to tell_not_asked
             self._internal_tell_not_asked(candidate, loss)
             return
         self._uid_queue.tell(uid)  # only add to queue if not a "tell_not_asked" (from a removed parent)
         parent = self.population[uid]
         mo_adapt = self._config.multiobjective_adaptation and self.num_objectives > 1
+        if mo_adapt:
+            if self.objective_weights is None:
+                self.objective_weights = np.ones(self.num_objectives)
+            else:
+                assert len(self.objective_weights) == self.num_objectives
         mo_adapt &= candidate._losses is not None  # can happen with bad constraints
         if not mo_adapt and loss <= base._loss(parent):
             self.population[uid] = candidate
         elif mo_adapt and (
-            parent._losses is None or np.mean(candidate.losses < parent.losses) > self._rng.rand()
+            parent._losses is None
+            or np.average(candidate.losses < parent.losses, weights=self.objective_weights) > self._rng.rand()
         ):
             # multiobjective case, with adaptation,
             # randomly replaces the parent depending on the number of better losses
             self.population[uid] = candidate
         elif self._config.propagate_heritage and loss <= float("inf"):
             self.population[uid].heritage.update(candidate.heritage)
```

### Comparing `nevergrad-0.6.0/nevergrad/optimization/es.py` & `nevergrad-0.7.0/nevergrad/optimization/es.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/experimentalvariants.py` & `nevergrad-0.7.0/nevergrad/optimization/experimentalvariants.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,19 @@
 MetaModelDiagonalCMA = ParametrizedMetaModel(multivariate_optimizer=ParametrizedCMA(diagonal=True)).set_name(
     "MetaModelDiagonalCMA", register=True
 )
 MetaModelFmin2 = ParametrizedMetaModel(multivariate_optimizer=CmaFmin2).set_name(
     "MetaModelFmin2", register=True
 )
 MetaModelFmin2.no_parallelization = True
+LSCMA = ParametrizedCMA(high_speed=False).set_name("LSCMA", register=True)
 HSCMA = ParametrizedCMA(high_speed=True).set_name("HSCMA", register=True)
+HSNeuralCMA = ParametrizedCMA(high_speed=True, algorithm="neural").set_name("HSNeuralCMA", register=True)
+HSSVMCMA = ParametrizedCMA(high_speed=True, algorithm="svm").set_name("HSSVMCMA", register=True)
+HSRFCMA = ParametrizedCMA(high_speed=True, algorithm="rf").set_name("HSRFCMA", register=True)
 HSMetaModel = ParametrizedMetaModel(multivariate_optimizer=HSCMA).set_name("HSMetaModel", register=True)
 
 # OnePlusOne
 FastGADiscreteOnePlusOne = ParametrizedOnePlusOne(mutation="fastga").set_name(
     "FastGADiscreteOnePlusOne", register=True
 )
 DoubleFastGAOptimisticNoisyDiscreteOnePlusOne = ParametrizedOnePlusOne(
```

### Comparing `nevergrad-0.6.0/nevergrad/optimization/externalbo.py` & `nevergrad-0.7.0/nevergrad/optimization/externalbo.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/families.py` & `nevergrad-0.7.0/nevergrad/optimization/families.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/helpers.py` & `nevergrad-0.7.0/nevergrad/optimization/helpers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/metamodel.py` & `nevergrad-0.7.0/nevergrad/optimization/metamodel.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from . import callbacks
 
 
 class MetaModelFailure(ValueError):
     """Sometimes the optimum of the metamodel is at infinity."""
 
 
-def learn_on_k_best(archive: utils.Archive[utils.MultiValue], k: int) -> tp.ArrayLike:
+def learn_on_k_best(
+    archive: utils.Archive[utils.MultiValue], k: int, algorithm: str = "quad"
+) -> tp.ArrayLike:
     """Approximate optimum learnt from the k best.
 
     Parameters
     ----------
     archive: utils.Archive[utils.Value]
     """
     items = list(archive.items_as_arrays())
@@ -30,29 +32,42 @@
 
     # Recenter the best.
     middle = np.array(sum(p[0] for p in first_k_individuals) / k)
     normalization = 1e-15 + np.sqrt(np.sum((first_k_individuals[-1][0] - first_k_individuals[0][0]) ** 2))
     y = np.asarray([archive[c[0]].get_estimation("pessimistic") for c in first_k_individuals])
     X = np.asarray([(c[0] - middle) / normalization for c in first_k_individuals])
 
-    # We need SKLearn.
-    from sklearn.linear_model import LinearRegression
     from sklearn.preprocessing import PolynomialFeatures
 
     polynomial_features = PolynomialFeatures(degree=2)
     X2 = polynomial_features.fit_transform(X)
-
-    # Fit a linear model.
     if not max(y) - min(y) > 1e-20:  # better use "not" for dealing with nans
         raise MetaModelFailure
-
     y = (y - min(y)) / (max(y) - min(y))
-    model = LinearRegression()
-    model.fit(X2, y)
+    if algorithm == "neural":
+        from sklearn.neural_network import MLPRegressor
 
+        model = MLPRegressor(hidden_layer_sizes=(16, 16), solver="lbfgs")
+    elif algorithm in ["svm", "svr"]:
+        from sklearn.svm import SVR
+
+        model = SVR()
+    elif algorithm == "rf":
+        from sklearn.ensemble import RandomForestRegressor
+
+        model = RandomForestRegressor()
+    else:
+        assert algorithm == "quad", f"Metamodelling algorithm {algorithm} not recognized."
+        # We need SKLearn.
+        from sklearn.linear_model import LinearRegression
+
+        # Fit a linear model.
+        model = LinearRegression()
+
+    model.fit(X2, y)
     # Check model quality.
     model_outputs = model.predict(X2)
     indices = np.argsort(y)
     ordered_model_outputs = [model_outputs[i] for i in indices]
     if not np.all(np.diff(ordered_model_outputs) > 0):
         raise MetaModelFailure("Unlearnable objective function.")
```

### Comparing `nevergrad-0.6.0/nevergrad/optimization/multiobjective/core.py` & `nevergrad-0.7.0/nevergrad/optimization/multiobjective/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/multiobjective/hypervolume.py` & `nevergrad-0.7.0/nevergrad/optimization/multiobjective/hypervolume.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/multiobjective/nsga2.py` & `nevergrad-0.7.0/nevergrad/optimization/multiobjective/nsga2.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/multiobjective/test_core.py` & `nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/multiobjective/test_hypervolume.py` & `nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_hypervolume.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/multiobjective/test_nsga2.py` & `nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_nsga2.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/mutations.py` & `nevergrad-0.7.0/nevergrad/optimization/mutations.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/oneshot.py` & `nevergrad-0.7.0/nevergrad/optimization/oneshot.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/optimizerlib.py` & `nevergrad-0.7.0/nevergrad/optimization/optimizerlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,16 +513,18 @@
 
     def __init__(
         self,
         parametrization: IntOrParameter,
         budget: tp.Optional[int] = None,
         num_workers: int = 1,
         config: tp.Optional["ParametrizedCMA"] = None,
+        algorithm: str = "quad",
     ) -> None:
         super().__init__(parametrization, budget=budget, num_workers=num_workers)
+        self.algorithm = algorithm
         self._config = ParametrizedCMA() if config is None else config
         pop = self._config.popsize
         self._popsize = (
             max(num_workers, 4 + int(self._config.popsize_factor * np.log(self.dimension)))
             if pop is None
             else pop
         )
@@ -606,15 +608,15 @@
             reference=self.parametrization
         )
         d = self.dimension
         n = self.num_ask
         sample_size = int(d * d / 2 + d / 2 + 3)
         if self._config.high_speed and n >= sample_size:
             try:
-                data = learn_on_k_best(self.archive, sample_size)
+                data = learn_on_k_best(self.archive, sample_size, self.algorithm)
                 return data  # type: ignore
             except MetaModelFailure:  # Failures in the metamodeling can happen.
                 pass
         if self._es is None:
             return pessimistic
         cma_best: tp.Optional[np.ndarray] = self.es.best_x if self._config.fcmaes else self.es.result.xbest
         if cma_best is None:
@@ -664,14 +666,15 @@
         popsize: tp.Optional[int] = None,
         popsize_factor: float = 3.0,
         diagonal: bool = False,
         high_speed: bool = False,
         fcmaes: bool = False,
         random_init: bool = False,
         inopts: tp.Optional[tp.Dict[str, tp.Any]] = None,
+        algorithm: str = "quad",
     ) -> None:
         super().__init__(_CMA, locals(), as_config=True)
         if fcmaes:
             if diagonal:
                 raise RuntimeError("fcmaes doesn't support diagonal=True, use fcmaes=False")
         self.scale = scale
         self.elitist = elitist
@@ -1705,32 +1708,34 @@
         self,
         parametrization: IntOrParameter,
         budget: tp.Optional[int] = None,
         num_workers: int = 1,
         *,
         multivariate_optimizer: tp.Optional[base.OptCls] = None,
         frequency_ratio: float = 0.9,
+        algorithm: str,  # Quad or NN or SVR
     ) -> None:
         super().__init__(parametrization, budget=budget, num_workers=num_workers)
         self.frequency_ratio = frequency_ratio
+        self.algorithm = algorithm
         if multivariate_optimizer is None:
             multivariate_optimizer = (
                 ParametrizedCMA(elitist=(self.dimension < 3)) if self.dimension > 1 else OnePlusOne
             )
         self._optim = multivariate_optimizer(
             self.parametrization, budget, num_workers
         )  # share parametrization and its rng
 
     def _internal_ask_candidate(self) -> p.Parameter:
         # We request a bit more points than what is really necessary for our dimensionality (+dimension).
         sample_size = int((self.dimension * (self.dimension - 1)) / 2 + 2 * self.dimension + 1)
         freq = max(13, self.num_workers, self.dimension, int(self.frequency_ratio * sample_size))
         if len(self.archive) >= sample_size and not self._num_ask % freq:
             try:
-                data = learn_on_k_best(self.archive, sample_size)
+                data = learn_on_k_best(self.archive, sample_size, self.algorithm)
                 candidate = self.parametrization.spawn_child().set_standardized_data(data)
             except MetaModelFailure:  # The optimum is at infinity. Shit happens.
                 candidate = self._optim.ask()
         else:
             candidate = self._optim.ask()
         return candidate
 
@@ -1760,20 +1765,24 @@
 
     # pylint: disable=unused-argument
     def __init__(
         self,
         *,
         multivariate_optimizer: tp.Optional[base.OptCls] = None,
         frequency_ratio: float = 0.9,
+        algorithm: str = "quad",
     ) -> None:
         super().__init__(_MetaModel, locals())
         assert 0 <= frequency_ratio <= 1.0
 
 
 MetaModel = ParametrizedMetaModel().set_name("MetaModel", register=True)
+NeuralMetaModel = ParametrizedMetaModel(algorithm="neural").set_name("NeuralMetaModel", register=True)
+SVMMetaModel = ParametrizedMetaModel(algorithm="svr").set_name("SVMMetaModel", register=True)
+RFMetaModel = ParametrizedMetaModel(algorithm="rf").set_name("RFMetaModel", register=True)
 MetaModelOnePlusOne = ParametrizedMetaModel(multivariate_optimizer=OnePlusOne).set_name(
     "MetaModelOnePlusOne", register=True
 )
 
 
 @registry.register
 class SQPCMA(Portfolio):
```

### Comparing `nevergrad-0.6.0/nevergrad/optimization/recaster.py` & `nevergrad-0.7.0/nevergrad/optimization/recaster.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/recastlib.py` & `nevergrad-0.7.0/nevergrad/optimization/recastlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/requirements_check.py` & `nevergrad-0.7.0/nevergrad/optimization/requirements_check.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/sequences.py` & `nevergrad-0.7.0/nevergrad/optimization/sequences.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_base.py` & `nevergrad-0.7.0/nevergrad/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_callbacks.py` & `nevergrad-0.7.0/nevergrad/optimization/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_doc.py` & `nevergrad-0.7.0/nevergrad/optimization/test_doc.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_externalbo.py` & `nevergrad-0.7.0/nevergrad/optimization/test_externalbo.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_mutations.py` & `nevergrad-0.7.0/nevergrad/optimization/test_mutations.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_optimizerlib.py` & `nevergrad-0.7.0/nevergrad/optimization/test_optimizerlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,23 @@
         )
 
 
 @skip_win_perf  # type: ignore
 @pytest.mark.parametrize("name", registry)  # type: ignore
 def test_optimizers(name: str) -> None:
     """Checks that each optimizer is able to converge on a simple test case"""
+    if sum([ord(c) for c in name]) % 4 > 0 and name not in [
+        "DE",
+        "CMA",
+        "OnePlusOne",
+        "Cobyla",
+        "DiscreteLenglerOnePlusOne",
+        "PSO",
+    ]:
+        raise SkipTest("Too expensive: we randomly skip 3/4 of these tests.")
     if name in ["CMAbounded", "NEWUOA"]:  # Not a general purpose optimization method.
         return
     if "BO" in name:  # Bayesian Optimization is rarely good, let us save up time.
         return
     optimizer_cls = registry[name]
     if isinstance(optimizer_cls, base.ConfiguredOptimizer):
         assert any(
@@ -420,31 +429,31 @@
 
 
 def test_optimization_discrete_with_one_sample() -> None:
     optimizer = optlib.PortfolioDiscreteOnePlusOne(parametrization=1, budget=10)
     optimizer.minimize(_square)
 
 
-def test_smooth_discrete_one_plus_one() -> None:
-    n = 35
-    d = 35
-    budget = d * d // 2
-    parametrization = ng.p.Array(shape=(d, d), upper=1.0, lower=-1.0)
-    values = []
-    values_smooth = []
-    for _ in range(n):
-        optimizer = xpvariants.SmoothDiscreteOnePlusOne(parametrization=parametrization, budget=budget)
-        recom_smooth = optimizer.minimize(_smooth_target).value
-        optimizer = optlib.DiscreteOnePlusOne(parametrization=parametrization, budget=budget)
-        recom = optimizer.minimize(_smooth_target).value
-        values_smooth += [_smooth_target(recom_smooth)]
-        values += [_smooth_target(recom)]
-    pval = stats.mannwhitneyu(values_smooth, values, alternative="less").pvalue
-    print(f"pval={pval}")
-    assert pval < 0.4, f"P-Value for smooth methods = {pval}."
+# def test_smooth_discrete_one_plus_one() -> None:
+#    n = 35
+#    d = 35
+#    budget = d * d // 2
+#    parametrization = ng.p.Array(shape=(d, d), upper=1.0, lower=-1.0)
+#    values = []
+#    values_smooth = []
+#    for _ in range(n):
+#        optimizer = xpvariants.SmoothDiscreteOnePlusOne(parametrization=parametrization, budget=budget)
+#        recom_smooth = optimizer.minimize(_smooth_target).value
+#        optimizer = optlib.DiscreteOnePlusOne(parametrization=parametrization, budget=budget)
+#        recom = optimizer.minimize(_smooth_target).value
+#        values_smooth += [_smooth_target(recom_smooth)]
+#        values += [_smooth_target(recom)]
+#    pval = stats.mannwhitneyu(values_smooth, values, alternative="less").pvalue
+#    print(f"pval={pval}")
+#    assert pval < 0.4, f"P-Value for smooth methods = {pval}."
 
 
 @pytest.mark.parametrize("name", ["TBPSA", "PSO", "TwoPointsDE", "CMA", "BO"])  # type: ignore
 def test_optim_pickle(name: str) -> None:
     # some generic class can fail to be pickled:
     # example of work around:
     # "self.population = base.utils.Population[DEParticle]([])"
@@ -651,14 +660,16 @@
         optimizer.parametrization.register_cheap_constraint(constraint, as_layer=as_layer)
     recom = optimizer.minimize(_square, verbosity=2)
     np.testing.assert_array_almost_equal([recom.kwargs["x"][0], recom.kwargs["y"]], expected)
 
 
 @pytest.mark.parametrize("name", registry)  # type: ignore
 def test_parametrization_offset(name: str) -> None:
+    if sum([ord(c) for c in name]) % 4 > 0:
+        raise SkipTest("Randomly skipping 75% of these tests.")
     if "PSO" in name or "BO" in name:
         raise SkipTest("PSO and BO have large initial variance")
     if "Cobyla" in name and platform.system() == "Windows":
         raise SkipTest("Cobyla is flaky on Windows for unknown reasons")
     parametrization = ng.p.Instrumentation(ng.p.Array(init=[1e12, 1e12]))
     with testing.suppress_nevergrad_warnings():
         optimizer = registry[name](parametrization, budget=100, num_workers=1)
@@ -671,17 +682,17 @@
         ), f"Candidate value[0] at iteration #{k} is below 100: {candidate.value}"
         optimizer.tell(candidate, 0)
 
 
 def test_optimizer_sequence() -> None:
     budget = 24
     parametrization = ng.p.Tuple(*(ng.p.Scalar(lower=-12, upper=12) for _ in range(2)))
-    optimizer = optlib.LHSSearch(parametrization, budget=24)
+    optimizer = optlib.LHSSearch(parametrization, budget=budget)
     points = [np.array(optimizer.ask().value) for _ in range(budget)]
-    assert sum(any(abs(x) > 11 for x in p) for p in points) > 0
+    assert sum(any(abs(x) > (budget // 2) - 1 for x in p) for p in points) > 0
 
 
 def test_shiwa_dim1() -> None:
     param = ng.p.Log(lower=1, upper=1000).set_integer_casting()
     init = param.value
     optimizer = optlib.Shiwa(param, budget=40)
     recom = optimizer.minimize(np.abs)
@@ -803,14 +814,17 @@
         (66, False),
         (200, False),
         (666, False),
         (2000, False),
     ],
 )
 def test_ngopt_on_simple_realistic_scenario(budget: int, with_int: bool) -> None:
+    if sum([ord(c) for c in f"{budget}-{with_int}"]) % 4 > 0:
+        raise SkipTest("Randomly skipping 75% of these tests.")
+
     def fake_training(learning_rate: float, batch_size: int, architecture: str) -> float:
         # optimal for learning_rate=0.2, batch_size=4, architecture="conv"
         return (learning_rate - 0.2) ** 2 + (batch_size - 4) ** 2 + (0 if architecture == "conv" else 10)
 
     # Instrumentation class is used for functions with multiple inputs
     # (positional and/or keywords)
     parametrization = ng.p.Instrumentation(
@@ -939,7 +953,24 @@
         == x.get_standardized_data(reference=x).shape
     )
     x = ng.p.Array(shape=(5, 5)).set_integer_casting()
     assert (
         optlib.smooth_copy(x).get_standardized_data(reference=x).shape
         == x.get_standardized_data(reference=x).shape
     )
+
+
+def test_weighted_moo_de() -> None:
+    for _ in range(1):  # Yes this is cheaper.
+        D = 2
+        N = 3
+        DE = ng.optimizers.TwoPointsDE(D, budget=600)
+        index = np.random.choice(range(N))
+        w = np.ones(N)
+        w[index] = 30.0
+        DE.set_objective_weights(w)  # type: ignore
+        targ = [np.array([np.cos(2 * np.pi * i / N), np.sin(2 * np.pi * i / N)]) for i in range(N)]
+        DE.minimize(lambda x: [np.linalg.norm(x - xi) for xi in targ])
+        x = np.zeros(N)
+        for u in DE.pareto_front():
+            x = x + u.losses
+        assert index == list(x).index(min(x))
```

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_recaster.py` & `nevergrad-0.7.0/nevergrad/optimization/test_recaster.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_sa.py` & `nevergrad-0.7.0/nevergrad/optimization/test_sa.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_sequences.py` & `nevergrad-0.7.0/nevergrad/optimization/test_sequences.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_special.py` & `nevergrad-0.7.0/nevergrad/optimization/test_special.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_suggest.py` & `nevergrad-0.7.0/nevergrad/optimization/test_suggest.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import pytest
 import numpy as np
 import sys
+from unittest import SkipTest
 import nevergrad as ng
 import nevergrad.common.typing as tp
 from nevergrad.common import testing
 from . import base
 from .optimizerlib import registry
 
 
@@ -52,14 +53,17 @@
 
 
 @skip_win_perf  # type: ignore
 @pytest.mark.parametrize("name", [r for r in registry if suggestable(r)])  # type: ignore
 def test_suggest_optimizers(name: str) -> None:
     """Checks that each optimizer is able to converge when optimum is given"""
 
+    if sum([ord(c) for c in name]) % 4 > 0 and name not in ["CMA", "PSO", "DE"]:
+        raise SkipTest("Too expensive: we randomly skip 3/4 of these tests.")
+
     instrum = ng.p.Array(shape=(100,)).set_bounds(0.0, 1.0)
     instrum.set_integer_casting()
     suggestion = np.asarray([0] * 17 + [1] * 17 + [0] * 66)  # The optimum is the suggestion.
     target = lambda x: 0 if np.all(np.asarray(x, dtype=int) == suggestion) else 1
     suggestion_testing(name, instrum, suggestion, 7, target)
```

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_tabu.py` & `nevergrad-0.7.0/nevergrad/optimization/test_tabu.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 
 
 @skip_win_perf  # type: ignore
 def test_tabu() -> None:
 
     num_tests = 97
-    for o in ["DiscreteOnePlusOne", "DiscreteLenglerOnePlusOne"]:
+    for o in ["DiscreteOnePlusOne"]:
         values = []
         valuesT = []
         for _ in range(num_tests):
             dim = 4
             arity = 7
             budget = (arity**dim) // 50
             domain = ng.p.TransitionChoice(range(arity), ordered=False, repetitions=dim)
@@ -47,15 +47,15 @@
     return sum(x)
 
 
 @skip_win_perf  # type: ignore
 def test_tabu_sum() -> None:
 
     num_tests = 147
-    for o in ["DiscreteOnePlusOne", "DiscreteLenglerOnePlusOne"]:
+    for o in ["DiscreteOnePlusOne"]:
         values = []
         valuesT = []
         for _ in range(num_tests):
             dim = 24
             arity = 3
             budget = 7
             domain = ng.p.TransitionChoice(range(arity), ordered=False, repetitions=dim)
```

### Comparing `nevergrad-0.6.0/nevergrad/optimization/test_utils.py` & `nevergrad-0.7.0/nevergrad/optimization/test_utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/optimization/utils.py` & `nevergrad-0.7.0/nevergrad/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/_datalayers.py` & `nevergrad-0.7.0/nevergrad/parametrization/_datalayers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/_layering.py` & `nevergrad-0.7.0/nevergrad/parametrization/_layering.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/choice.py` & `nevergrad-0.7.0/nevergrad/parametrization/choice.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/container.py` & `nevergrad-0.7.0/nevergrad/parametrization/container.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/core.py` & `nevergrad-0.7.0/nevergrad/parametrization/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/data.py` & `nevergrad-0.7.0/nevergrad/parametrization/data.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/discretization.py` & `nevergrad-0.7.0/nevergrad/parametrization/discretization.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/helpers.py` & `nevergrad-0.7.0/nevergrad/parametrization/helpers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/instantiate.py` & `nevergrad-0.7.0/nevergrad/parametrization/instantiate.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/mutation.py` & `nevergrad-0.7.0/nevergrad/parametrization/mutation.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/parameter.py` & `nevergrad-0.7.0/nevergrad/parametrization/parameter.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_discretization.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_discretization.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_instantiate.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_layers.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_layers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_mutation.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_mutation.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_param_doc.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_param_doc.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_parameter.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_parameter.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_parameters_legacy.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_parameters_legacy.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_transforms.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_transforms.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/test_utils.py` & `nevergrad-0.7.0/nevergrad/parametrization/test_utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/transforms.py` & `nevergrad-0.7.0/nevergrad/parametrization/transforms.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad/parametrization/utils.py` & `nevergrad-0.7.0/nevergrad/parametrization/utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad.egg-info/PKG-INFO` & `nevergrad-0.7.0/nevergrad.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 Metadata-Version: 2.1
 Name: nevergrad
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python toolbox for performing gradient-free optimization
 Home-page: https://github.com/facebookresearch/nevergrad
 Author: Facebook AI Research
 License: MIT
-Description: [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-ukraine) [![CircleCI](https://circleci.com/gh/facebookresearch/nevergrad/tree/main.svg?style=svg)](https://circleci.com/gh/facebookresearch/nevergrad/tree/main)
-        
-        # Nevergrad - A gradient-free optimization platform
-        
-        ![Nevergrad](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.6.0/docs/resources/Nevergrad-LogoMark.png)
-        
-        
-        `nevergrad` is a Python 3.6+ library. It can be installed with:
-        
-        ```
-        pip install nevergrad
-        ```
-        
-        More installation options, including windows installation, and complete instructions are available in the "Getting started" section of the [**documentation**](https://facebookresearch.github.io/nevergrad/).
-        
-        You can join Nevergrad users Facebook group [here](https://www.facebook.com/groups/nevergradusers/).
-        
-        Minimizing a function using an optimizer (here `NGOpt`) is straightforward:
-        
-        ```python
-        import nevergrad as ng
-        
-        def square(x):
-            return sum((x - .5)**2)
-        
-        optimizer = ng.optimizers.NGOpt(parametrization=2, budget=100)
-        recommendation = optimizer.minimize(square)
-        print(recommendation.value)  # recommended value
-        >>> [0.49971112 0.5002944]
-        ```
-        
-        `nevergrad` can also support bounded continuous variables as well as discrete variables, and mixture of those.
-        To do this, one can specify the input space:
-        
-        ```python
-        import nevergrad as ng
-        
-        def fake_training(learning_rate: float, batch_size: int, architecture: str) -> float:
-            # optimal for learning_rate=0.2, batch_size=4, architecture="conv"
-            return (learning_rate - 0.2)**2 + (batch_size - 4)**2 + (0 if architecture == "conv" else 10)
-        
-        # Instrumentation class is used for functions with multiple inputs
-        # (positional and/or keywords)
-        parametrization = ng.p.Instrumentation(
-            # a log-distributed scalar between 0.001 and 1.0
-            learning_rate=ng.p.Log(lower=0.001, upper=1.0),
-            # an integer from 1 to 12
-            batch_size=ng.p.Scalar(lower=1, upper=12).set_integer_casting(),
-            # either "conv" or "fc"
-            architecture=ng.p.Choice(["conv", "fc"])
-        )
-        
-        optimizer = ng.optimizers.NGOpt(parametrization=parametrization, budget=100)
-        recommendation = optimizer.minimize(fake_training)
-        
-        # show the recommended keyword arguments of the function
-        print(recommendation.kwargs)
-        >>> {'learning_rate': 0.1998, 'batch_size': 4, 'architecture': 'conv'}
-        ```
-        
-        Learn more on parametrization in the [**documentation**](https://facebookresearch.github.io/nevergrad/)!
-        
-        ![Example of optimization](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.6.0/docs/resources/TwoPointsDE.gif)
-        
-        *Convergence of a population of points to the minima with two-points DE.*
-        
-        
-        ## Documentation
-        
-        Check out our [**documentation**](https://facebookresearch.github.io/nevergrad/)! It's still a work in progress, don't hesitate to submit issues and/or PR to update it and make it clearer!
-        
-        
-        ## Citing
-        
-        ```bibtex
-        @misc{nevergrad,
-            author = {J. Rapin and O. Teytaud},
-            title = {{Nevergrad - A gradient-free optimization platform}},
-            year = {2018},
-            publisher = {GitHub},
-            journal = {GitHub repository},
-            howpublished = {\url{https://GitHub.com/FacebookResearch/Nevergrad}},
-        }
-        ```
-        
-        ## License
-        
-        `nevergrad` is released under the MIT license. See [LICENSE](https://github.com/facebookresearch/nevergrad/blob/0.6.0/LICENSE) for additional details about it.
-        See also our [Terms of Use](https://opensource.facebook.com/legal/terms) and [Privacy Policy](https://opensource.facebook.com/legal/privacy).
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: benchmark
+License-File: LICENSE
+
+[![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-ukraine) [![CircleCI](https://circleci.com/gh/facebookresearch/nevergrad/tree/main.svg?style=svg)](https://circleci.com/gh/facebookresearch/nevergrad/tree/main)
+
+# Nevergrad - A gradient-free optimization platform
+
+![Nevergrad](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.7.0/docs/resources/Nevergrad-LogoMark.png)
+
+
+`nevergrad` is a Python 3.6+ library. It can be installed with:
+
+```
+pip install nevergrad
+```
+
+More installation options, including windows installation, and complete instructions are available in the "Getting started" section of the [**documentation**](https://facebookresearch.github.io/nevergrad/).
+
+You can join Nevergrad users Facebook group [here](https://www.facebook.com/groups/nevergradusers/).
+
+Minimizing a function using an optimizer (here `NGOpt`) is straightforward:
+
+```python
+import nevergrad as ng
+
+def square(x):
+    return sum((x - .5)**2)
+
+optimizer = ng.optimizers.NGOpt(parametrization=2, budget=100)
+recommendation = optimizer.minimize(square)
+print(recommendation.value)  # recommended value
+>>> [0.49971112 0.5002944]
+```
+
+`nevergrad` can also support bounded continuous variables as well as discrete variables, and mixture of those.
+To do this, one can specify the input space:
+
+```python
+import nevergrad as ng
+
+def fake_training(learning_rate: float, batch_size: int, architecture: str) -> float:
+    # optimal for learning_rate=0.2, batch_size=4, architecture="conv"
+    return (learning_rate - 0.2)**2 + (batch_size - 4)**2 + (0 if architecture == "conv" else 10)
+
+# Instrumentation class is used for functions with multiple inputs
+# (positional and/or keywords)
+parametrization = ng.p.Instrumentation(
+    # a log-distributed scalar between 0.001 and 1.0
+    learning_rate=ng.p.Log(lower=0.001, upper=1.0),
+    # an integer from 1 to 12
+    batch_size=ng.p.Scalar(lower=1, upper=12).set_integer_casting(),
+    # either "conv" or "fc"
+    architecture=ng.p.Choice(["conv", "fc"])
+)
+
+optimizer = ng.optimizers.NGOpt(parametrization=parametrization, budget=100)
+recommendation = optimizer.minimize(fake_training)
+
+# show the recommended keyword arguments of the function
+print(recommendation.kwargs)
+>>> {'learning_rate': 0.1998, 'batch_size': 4, 'architecture': 'conv'}
+```
+
+Learn more on parametrization in the [**documentation**](https://facebookresearch.github.io/nevergrad/)!
+
+![Example of optimization](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.7.0/docs/resources/TwoPointsDE.gif)
+
+*Convergence of a population of points to the minima with two-points DE.*
+
+
+## Documentation
+
+Check out our [**documentation**](https://facebookresearch.github.io/nevergrad/)! It's still a work in progress, don't hesitate to submit issues and/or PR to update it and make it clearer!
+
+
+## Citing
+
+```bibtex
+@misc{nevergrad,
+    author = {J. Rapin and O. Teytaud},
+    title = {{Nevergrad - A gradient-free optimization platform}},
+    year = {2018},
+    publisher = {GitHub},
+    journal = {GitHub repository},
+    howpublished = {\url{https://GitHub.com/FacebookResearch/Nevergrad}},
+}
+```
+
+## License
+
+`nevergrad` is released under the MIT license. See [LICENSE](https://github.com/facebookresearch/nevergrad/blob/0.7.0/LICENSE) for additional details about it.
+See also our [Terms of Use](https://opensource.facebook.com/legal/terms) and [Privacy Policy](https://opensource.facebook.com/legal/privacy).
```

### Comparing `nevergrad-0.6.0/nevergrad.egg-info/SOURCES.txt` & `nevergrad-0.7.0/nevergrad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/nevergrad.egg-info/requires.txt` & `nevergrad-0.7.0/nevergrad.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 matplotlib>=2.2.3
 gym==0.24.1
 gym-anm>=1.0.1
 pygame>=2.1.2
 torch>=1.7.0
 hiplot
 fcmaes>=1.2.7
-pandas>=0.23.4
 openpyxl>=3.0.0
 pyproj>=2.6.1
 Pillow>=8.4.0
 tqdm
 torchvision>=0.11.1
 pyomo==5.7.1
 mixsimulator>=0.3.3
```

### Comparing `nevergrad-0.6.0/requirements/bench.txt` & `nevergrad-0.7.0/requirements/bench.txt`

 * *Files identical despite different names*

### Comparing `nevergrad-0.6.0/setup.py` & `nevergrad-0.7.0/setup.py`

 * *Files identical despite different names*

