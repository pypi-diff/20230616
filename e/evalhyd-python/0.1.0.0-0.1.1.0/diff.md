# Comparing `tmp/evalhyd-python-0.1.0.0.tar.gz` & `tmp/evalhyd-python-0.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalhyd-python-0.1.0.0.tar", last modified: Mon May  8 06:52:42 2023, max compression
+gzip compressed data, was "evalhyd-python-0.1.1.0.tar", last modified: Fri Jun 16 15:00:24 2023, max compression
```

## Comparing `evalhyd-python-0.1.0.0.tar` & `evalhyd-python-0.1.1.0.tar`

### file list

```diff
@@ -1,718 +1,716 @@
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.591554 evalhyd-python-0.1.0.0/
--rw-r--r--   0 thibhlln   (501) staff       (20)    35580 2023-04-14 16:46:32.000000 evalhyd-python-0.1.0.0/LICENCE.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)       27 2023-05-06 11:48:25.000000 evalhyd-python-0.1.0.0/MANIFEST.in
--rw-r--r--   0 thibhlln   (501) staff       (20)      562 2023-05-08 06:52:42.591158 evalhyd-python-0.1.0.0/PKG-INFO
--rw-r--r--   0 thibhlln   (501) staff       (20)      113 2023-04-14 16:46:32.000000 evalhyd-python-0.1.0.0/README.md
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.093500 evalhyd-python-0.1.0.0/deps/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.103111 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/
--rw-r--r--   0 thibhlln   (501) staff       (20)       44 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/.git
--rw-r--r--   0 thibhlln   (501) staff       (20)       55 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/.gitignore
--rw-r--r--   0 thibhlln   (501) staff       (20)      406 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/.gitlab-ci.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     3208 2023-04-19 12:01:31.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      224 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/EvalHydConfig.cmake.in
--rw-r--r--   0 thibhlln   (501) staff       (20)    35580 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/LICENCE.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      144 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/README.md
--rw-r--r--   0 thibhlln   (501) staff       (20)      186 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/changelog.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      198 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/environment.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.085170 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.104450 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.107742 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.112477 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/
--rw-r--r--   0 thibhlln   (501) staff       (20)     2135 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/diagnostics.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    34648 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/efficiencies.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    18581 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/errors.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    18929 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/evaluator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11025 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/events.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    18892 2023-04-19 15:42:41.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/masks.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      921 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/maths.hpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.119355 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/
--rw-r--r--   0 thibhlln   (501) staff       (20)    48052 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/brier.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8108 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/cdf.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    22470 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/contingency.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2284 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/diagnostics.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    28442 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/evaluator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    27976 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/intervals.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6786 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/multivariate.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10212 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/quantiles.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    18859 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/ranks.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10005 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/uncertainty.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4649 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/utils.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    21673 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/evald.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    21152 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/evalp.hpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.122703 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/
--rw-r--r--   0 thibhlln   (501) staff       (20)     1839 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.126120 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/
--rw-r--r--   0 thibhlln   (501) staff       (20)     1366 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/q_obs.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     9351 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/q_obs_1yr.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)    69202 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/q_prd.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)   125330 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/q_prd_1yr.csv
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.087152 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.133020 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/
--rw-r--r--   0 thibhlln   (501) staff       (20)     3366 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/CONT_TBL.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      957 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/KGE.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      960 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/KGEPRIME.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     2907 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/KGEPRIME_D.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     2907 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/KGE_D.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     1071 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/MAE.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      969 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/MARE.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     1224 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/MSE.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      963 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/NSE.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      915 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/RMSE.csv
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.142816 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/
--rw-r--r--   0 thibhlln   (501) staff       (20)       16 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/AS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       33 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/AW.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       32 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/AWI.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       32 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/AWN.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       52 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/BS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       52 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/BSS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      156 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/BS_CRD.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      156 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/BS_LBD.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       32 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/CR.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       18 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/CRPS_FROM_BS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       17 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/CRPS_FROM_ECDF.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       18 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/CRPS_FROM_QS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     2704 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/CSI.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       18 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/DS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       18 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/ES.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     2704 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/FAR.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     2704 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/POD.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     2704 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/POFD.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      918 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/QS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)      832 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/RANK_HIST.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)     8122 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/REL_DIAG.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       52 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/ROCSS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       37 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/WS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)       32 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/WSS.csv
--rw-r--r--   0 thibhlln   (501) staff       (20)    25964 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/test_determinist.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    35103 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/test_probabilist.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    28110 2023-04-14 16:08:34.000000 evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/test_uncertainty.cpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.149638 evalhyd-python-0.1.0.0/deps/xtensor/
--rw-r--r--   0 thibhlln   (501) staff       (20)     1681 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.appveyor.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.199202 evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/
--rw-r--r--   0 thibhlln   (501) staff       (20)     1229 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/azure-pipelines-linux-clang.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     1357 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/azure-pipelines-linux-gcc.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      724 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/azure-pipelines-osx.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     2813 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/azure-pipelines-win.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     2291 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/unix-build.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     2671 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.clang-format
--rw-r--r--   0 thibhlln   (501) staff       (20)       40 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.git
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.199730 evalhyd-python-0.1.0.0/deps/xtensor/.github/
--rw-r--r--   0 thibhlln   (501) staff       (20)      426 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.200735 evalhyd-python-0.1.0.0/deps/xtensor/.github/workflows/
--rw-r--r--   0 thibhlln   (501) staff       (20)      836 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.github/workflows/gh-pages.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      225 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.github/workflows/static-analysis.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      660 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/.gitignore
--rw-r--r--   0 thibhlln   (501) staff       (20)     1290 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/.pre-commit-config.yaml
--rw-r--r--   0 thibhlln   (501) staff       (20)    12880 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)    14807 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/README.md
--rw-r--r--   0 thibhlln   (501) staff       (20)      259 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/azure-pipelines.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.213385 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/
--rw-r--r--   0 thibhlln   (501) staff       (20)     6224 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     5457 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_adapter.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8175 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_assign.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     7165 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_builder.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4306 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_container.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1985 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_creation.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2622 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_increment_stepper.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2541 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_lambda_expressions.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    16511 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_math.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2054 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_random.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4212 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_reducer.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    14322 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_view_access.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2549 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_view_adapt.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5634 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_view_assignment.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11595 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_views.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2440 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_xshape.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      973 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/copyGBenchmark.cmake.in
--rw-r--r--   0 thibhlln   (501) staff       (20)     1019 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/downloadGBenchmark.cmake.in
--rw-r--r--   0 thibhlln   (501) staff       (20)     1380 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/benchmark/main.cpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.214011 evalhyd-python-0.1.0.0/deps/xtensor/cmake/
--rw-r--r--   0 thibhlln   (501) staff       (20)    12026 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/cmake/FindTBB.cmake
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.216050 evalhyd-python-0.1.0.0/deps/xtensor/docs/
--rw-r--r--   0 thibhlln   (501) staff       (20)       48 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/ghp_environment.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     7750 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/make.bat
--rw-r--r--   0 thibhlln   (501) staff       (20)       69 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/rtd_environment.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.256527 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.257792 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/_static/
--rw-r--r--   0 thibhlln   (501) staff       (20)      302 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/_static/goatcounter.js
--rw-r--r--   0 thibhlln   (501) staff       (20)       60 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/_static/main_stylesheet.css
--rw-r--r--   0 thibhlln   (501) staff       (20)     7074 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/adaptor.rst
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.301341 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/
--rw-r--r--   0 thibhlln   (501) staff       (20)      539 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/accumulating_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      828 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/basic_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      611 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/classif_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      931 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/container_index.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      509 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/error_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      591 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/exponential_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      612 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/expression_index.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      421 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/function_index.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      705 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/hyperbolic_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      443 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/index_related.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      287 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/io_index.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      468 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/iterator_index.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      887 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/nan_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      604 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/nearint_operations.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1830 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/operators.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      602 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/power_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1731 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/reducing_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      299 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/shape.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      613 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/trigonometric_functions.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      399 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xaccumulator.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      342 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xadapt.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      387 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xarray.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      328 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xarray_adaptor.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      733 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xaxis_iterator.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      806 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xaxis_slice_iterator.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      371 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xbroadcast.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1308 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xbuilder.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      333 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xchunked_array.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      593 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xcontainer.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      346 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xcontainer_semantic.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      369 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xcsv.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      304 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xeval.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      505 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xexpression.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      367 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xfixed.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      394 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xfunction.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      391 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xfunctor_view.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      320 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xgenerator.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1336 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xhistogram.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      489 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xindex_view.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1272 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xio.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      425 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xiterable.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      432 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xjson.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      384 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xmanipulation.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      328 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xmasked_view.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    22382 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xmath.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      540 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xnpy.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      352 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xoptional_assembly.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      376 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xoptional_assembly_adaptor.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      372 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xoptional_assembly_base.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      598 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xpad.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1800 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xrandom.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      367 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xreducer.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      308 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xrepeat.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      331 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xsemantic_base.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      649 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xset_operation.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      342 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xshape.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      338 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xsort.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      595 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xstrided_view.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      350 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xstrides.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      514 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xtensor.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      332 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xtensor_adaptor.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      676 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xview.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      331 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xview_semantic.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     3232 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/binder-logo.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     9734 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/bindings.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     4943 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/build-options.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     5723 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/builder.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    97913 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/changelog.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    11665 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/closure-semantics.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    17753 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/cmake.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     6850 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/compilers.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1806 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/conda.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     1309 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/conf.py
--rw-r--r--   0 thibhlln   (501) staff       (20)    10261 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/container.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     7481 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/debian.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     4342 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/dev-build-options.rst
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.318008 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/
--rw-r--r--   0 thibhlln   (501) staff       (20)    14790 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/assign_xexpression.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     8285 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/assignment.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    12540 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/computed_assign.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    10299 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/concepts.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     7948 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/expression_tree.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    12444 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/extended_copy_semantic.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    10146 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/implementation_classes.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     9866 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/iterating_expression.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    26079 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/iteration.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    22373 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/stepper_basic.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    23161 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/stepper_broadcasting.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    17381 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/stepper_iterating.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    23695 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/stepper_to_end.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    17684 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xarray_uml.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    10216 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xcontainer_classes.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     7800 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xfunction_tree.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     8745 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xsemantic_classes.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)      764 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xtensor_internals.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    10234 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/expression.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    15686 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/external-structures.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     3155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/file_loading.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     6137 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/getting_started.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2705 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/histogram.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2787 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/index.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     8157 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/indices.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2896 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/installation.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     4176 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/missing.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     4203 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/numpy-differences.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    64585 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/numpy.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)   487166 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/numpy.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    13200 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/operator.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     4965 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/pitfall.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     5023 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quantstack-white.svg
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.323090 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/
--rw-r--r--   0 thibhlln   (501) staff       (20)     6173 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/basic.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     6111 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/builder.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2609 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/chunked_arrays.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     6364 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/iterator.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2610 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/manipulation.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     3546 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/math.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2204 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/operator.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     3491 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/reducer.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     3497 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/random.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     3235 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/rank.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    13334 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/related.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1860 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/releasing.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     4054 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/scalar.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2489 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/spack.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    14644 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/view.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)   198081 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xeus-cling-screenshot.png
--rw-r--r--   0 thibhlln   (501) staff       (20)     5268 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xframe.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     4209 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xsimd-small.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     2976 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xsimd.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     5385 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-blas-small.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     5386 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-blas.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)   475924 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-cookiecutter.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     7789 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-fftw.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     7065 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-io-small.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     7065 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-io.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     6178 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-julia-small.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     6184 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-julia.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     6266 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-python-small.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     6273 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-python.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     4528 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-r-small.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     4536 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-r.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)    10906 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-ros.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     3478 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     4511 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtl.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)      132 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/environment-dev.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      111 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/environment.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.092102 evalhyd-python-0.1.0.0/deps/xtensor/include/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.396302 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/
--rw-r--r--   0 thibhlln   (501) staff       (20)    11676 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xaccessible.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    14104 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xaccumulator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    36156 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xadapt.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    24640 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xarray.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    49134 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xassign.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10591 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xaxis_iterator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11290 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xaxis_slice_iterator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    38555 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xblockwise_reducer.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    17724 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xblockwise_reducer_functors.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    14970 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xbroadcast.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    41449 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xbuffer_adaptor.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    42455 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xbuilder.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    24351 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xchunked_array.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11386 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xchunked_assign.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8851 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xchunked_view.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8407 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xcomplex.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    41731 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xcontainer.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8597 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xcsv.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    28975 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xdynamic_view.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5808 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xeval.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    13184 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xexception.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    24760 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xexpression.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     7640 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xexpression_holder.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5748 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xexpression_traits.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    37637 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xfixed.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    39903 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xfunction.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    57648 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xfunctor_view.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    17080 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xgenerator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    21613 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xhistogram.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    26749 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xindex_view.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3914 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xinfo.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    26832 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xio.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    52665 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xiterable.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    35923 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xiterator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6722 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xjson.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3452 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xlayout.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    38079 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmanipulation.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    24021 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmasked_view.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)   120621 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmath.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    12998 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmime.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3729 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmultiindex_iterator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6196 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xnoalias.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    31209 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xnorm.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    27263 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xnpy.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3286 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoffset_view.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    34576 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoperation.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    48774 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoptional.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    27116 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoptional_assembly.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    37733 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoptional_assembly_base.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    19544 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoptional_assembly_storage.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10799 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xpad.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    40536 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xrandom.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    64806 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xreducer.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    23264 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xrepeat.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    34142 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xscalar.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    24660 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xsemantic.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     7366 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xset_operation.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    16921 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xshape.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    49258 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xslice.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    48051 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xsort.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    59022 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xstorage.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    29524 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xstrided_view.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    34210 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xstrided_view_base.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    31463 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xstrides.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    35939 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xtensor.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4138 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xtensor_config.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     7842 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xtensor_forward.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8203 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xtensor_simd.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    28368 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xutils.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xvectorize.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    83925 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xview.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8366 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xview_utils.hpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.396954 evalhyd-python-0.1.0.0/deps/xtensor/notebooks/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.398451 evalhyd-python-0.1.0.0/deps/xtensor/notebooks/images/
--rw-r--r--   0 thibhlln   (501) staff       (20)    19420 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/notebooks/images/xtensor-blas.png
--rw-r--r--   0 thibhlln   (501) staff       (20)    15734 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/notebooks/images/xtensor.png
--rw-r--r--   0 thibhlln   (501) staff       (20)    10473 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/notebooks/xtensor.ipynb
--rw-r--r--   0 thibhlln   (501) staff       (20)       40 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/readthedocs.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.469624 evalhyd-python-0.1.0.0/deps/xtensor/test/
--rw-r--r--   0 thibhlln   (501) staff       (20)    11009 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/CMakeLists.txt
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.472050 evalhyd-python-0.1.0.0/deps/xtensor/test/files/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.476507 evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/
--rw-r--r--   0 thibhlln   (501) staff       (20)     5964 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_broadcast_view.cppy
--rw-r--r--   0 thibhlln   (501) staff       (20)     1985 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_xhistogram.cppy
--rw-r--r--   0 thibhlln   (501) staff       (20)     1191 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_xmath_interp.cppy
--rw-r--r--   0 thibhlln   (501) staff       (20)     2742 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_xmath_reducers.cppy
--rw-r--r--   0 thibhlln   (501) staff       (20)    10274 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_xsort.cppy
--rw-r--r--   0 thibhlln   (501) staff       (20)      384 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/generate.py
--rw-r--r--   0 thibhlln   (501) staff       (20)     3387 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/preprocess.py
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.489880 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/
--rw-r--r--   0 thibhlln   (501) staff       (20)      335 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/big_exp.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      190 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/bool_fn.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     2190 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/complex_numbers.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     2190 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/complex_zero_erasing.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)       86 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/custom_formatter_result.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     6426 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/cut_4d.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      162 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/cut_both.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)       42 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/cut_high.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      130 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/cut_long.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     1150 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/float_leading_zero.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)       81 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/long_strings.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      355 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/precision.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     6206 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/print_options_result.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     4580 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/random_nan_inf.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      102 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/random_strings.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      195 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/threed_double.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)       81 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/twod_double.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)    25341 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results.hpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.499321 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/
--rw-r--r--   0 thibhlln   (501) staff       (20)      155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/bool.be.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/bool.le.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/bool_fortran.be.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/bool_fortran.le.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      344 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/double.be.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      344 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/double.le.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      344 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/double_fortran.be.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      344 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/double_fortran.le.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      148 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/int.be.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      148 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/int.le.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      168 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/unsignedlong.be.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      168 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/unsignedlong.le.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      168 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/unsignedlong_fortran.be.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      168 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/files/xnpy_files/unsignedlong_fortran.le.npy
--rw-r--r--   0 thibhlln   (501) staff       (20)      156 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/main.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2272 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/set_compiler_flag.cmake
--rw-r--r--   0 thibhlln   (501) staff       (20)    36747 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_common.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2309 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_common_macros.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    34696 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_broadcast_view.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    12934 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_xhistogram.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5271 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_xmath_interp.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    96615 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_xmath_reducers.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    45383 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_xsort.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5025 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_sfinae.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     9714 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_strided_assign.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2744 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_utils.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6966 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xaccumulator.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    17890 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xadapt.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10473 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xadaptor_semantic.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    12587 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xarray.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5419 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xarray_adaptor.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3699 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xassign.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     7411 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xaxis_iterator.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11048 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xaxis_slice_iterator.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    14023 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xblockwise_reducer.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6271 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xbroadcast.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6426 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xbuffer_adaptor.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    22869 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xbuilder.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4761 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xchunked_array.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2226 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xchunked_view.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    12402 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xcomplex.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    18690 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xcontainer_semantic.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1972 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xcsv.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3305 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xdatesupport.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     9462 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xdynamic_view.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11400 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xeval.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1961 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xexception.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4674 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xexpression.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2315 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xexpression_holder.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3057 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xexpression_traits.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11596 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xfixed.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3447 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xfunc_on_xexpression.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    15395 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xfunction.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6001 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xfunctor_adaptor.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4020 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xhistogram.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5850 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xindex_view.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1179 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xinfo.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     9495 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xio.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    24624 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xiterator.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1717 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xjson.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     7164 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xlayout.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    21276 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmanipulation.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8514 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmasked_view.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    27470 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmath.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    13599 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmath_result_type.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2006 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmime.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1090 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmultiindex_iterator.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    15346 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xnan_functions.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11242 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xnoalias.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     7880 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xnorm.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6674 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xnpy.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    32637 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoperation.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    19755 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoptional.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    18388 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoptional_assembly.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    14479 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoptional_assembly_adaptor.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6078 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoptional_assembly_storage.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8877 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xpad.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8888 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xrandom.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    40571 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xreducer.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10260 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xrepeat.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3357 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xscalar.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     9959 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xscalar_semantic.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4661 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xsemantic.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1980 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xset_operation.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2482 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xshape.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2192 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xsimd.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1231 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xsimd8.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    17712 2023-03-24 12:52:57.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xsort.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     9643 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xstorage.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    32413 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xstrided_view.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10749 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xstrides.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    15248 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xtensor.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5868 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xtensor_adaptor.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2598 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xtensor_semantic.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8025 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xutils.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2270 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xvectorize.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    57076 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xview.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    16538 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/test/test_xview_semantic.cpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.500046 evalhyd-python-0.1.0.0/deps/xtensor/tools/
--rwxr-xr-x   0 thibhlln   (501) staff       (20)     1028 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/tools/check_circular.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      234 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/xtensor.pc.in
--rw-r--r--   0 thibhlln   (501) staff       (20)     2789 2023-02-01 09:15:55.000000 evalhyd-python-0.1.0.0/deps/xtensor/xtensorConfig.cmake.in
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.155256 evalhyd-python-0.1.0.0/deps/xtensor-python/
--rw-r--r--   0 thibhlln   (501) staff       (20)     1253 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/.appveyor.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.157968 evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/
--rw-r--r--   0 thibhlln   (501) staff       (20)     1263 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-linux-clang.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      895 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-linux-gcc.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      784 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-osx.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     2063 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/unix-build.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)       47 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/.git
--rw-r--r--   0 thibhlln   (501) staff       (20)      606 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/.gitignore
--rw-r--r--   0 thibhlln   (501) staff       (20)     5918 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     7128 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/README.md
--rw-r--r--   0 thibhlln   (501) staff       (20)      213 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/azure-pipelines.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.163219 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/
--rw-r--r--   0 thibhlln   (501) staff       (20)     4191 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      215 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/benchmark_pyarray.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      236 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/benchmark_pybind_array.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      247 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/benchmark_pybind_vectorize.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      240 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/benchmark_pytensor.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      226 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/benchmark_pyvectorize.py
--rw-r--r--   0 thibhlln   (501) staff       (20)     1624 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/main.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3387 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/setup.py
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.163819 evalhyd-python-0.1.0.0/deps/xtensor-python/cmake/
--rw-r--r--   0 thibhlln   (501) staff       (20)     3644 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/cmake/FindNumPy.cmake
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.165120 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/
--rw-r--r--   0 thibhlln   (501) staff       (20)       80 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/environment.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     7285 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/make.bat
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.177952 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.178574 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/_static/
--rw-r--r--   0 thibhlln   (501) staff       (20)       60 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/_static/main_stylesheet.css
--rw-r--r--   0 thibhlln   (501) staff       (20)      399 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/api_reference.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1219 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/array_tensor.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2527 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/basic_usage.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    17753 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/cmake.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)      806 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/compilers.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1805 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/conda.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)      861 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/conf.py
--rw-r--r--   0 thibhlln   (501) staff       (20)     2091 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/cookiecutter.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     6863 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/debian.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     1193 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/dev_build_options.rst
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.089532 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.180406 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/copy_cast/
--rw-r--r--   0 thibhlln   (501) staff       (20)      407 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/copy_cast/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      201 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/copy_cast/example.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      874 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/copy_cast/main.cpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.182486 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/readme_example_1/
--rw-r--r--   0 thibhlln   (501) staff       (20)      432 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/readme_example_1/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      124 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/readme_example_1/example.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      511 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/readme_example_1/main.cpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.185000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/sfinae/
--rw-r--r--   0 thibhlln   (501) staff       (20)      512 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/sfinae/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      197 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/sfinae/example.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      222 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/sfinae/main.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      600 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/sfinae/mymodule.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      314 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/sfinae/python.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6348 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2951 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/index.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1784 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/installation.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     3030 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/numpy_capi.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      283 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/pyarray.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      286 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/pytensor.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      285 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/pyvectorize.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     5022 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/quantstack-white.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     1415 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/releasing.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     5970 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/xtensor-python.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)      198 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/environment-dev.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.089800 evalhyd-python-0.1.0.0/deps/xtensor-python/include/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.189531 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/
--rw-r--r--   0 thibhlln   (501) staff       (20)    19952 2023-02-01 08:29:46.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pyarray.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10631 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pyarray_backstrides.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    16852 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pycontainer.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2331 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pynative_casters.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8683 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pystrides_adaptor.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    19005 2023-02-01 08:29:46.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pytensor.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2060 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pyvectorize.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      813 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/xtensor_python_config.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11257 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/xtensor_type_caster_base.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)       38 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/readthedocs.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.193842 evalhyd-python-0.1.0.0/deps/xtensor-python/test/
--rw-r--r--   0 thibhlln   (501) staff       (20)     3953 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     1027 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/copyGTest.cmake.in
--rw-r--r--   0 thibhlln   (501) staff       (20)     1086 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/downloadGTest.cmake.in
--rw-r--r--   0 thibhlln   (501) staff       (20)     1146 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/main.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    26762 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_common.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     9110 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_pyarray.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6246 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_pyarray_traits.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     8549 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_pytensor.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1913 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_pyvectorize.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1914 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_sfinae.cpp
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.195543 evalhyd-python-0.1.0.0/deps/xtensor-python/test_python/
--rw-r--r--   0 thibhlln   (501) staff       (20)    12267 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test_python/main.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4021 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test_python/setup.py
--rw-r--r--   0 thibhlln   (501) staff       (20)    11447 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/test_python/test_pyarray.py
--rw-r--r--   0 thibhlln   (501) staff       (20)     1115 2023-02-01 08:29:29.000000 evalhyd-python-0.1.0.0/deps/xtensor-python/xtensor-pythonConfig.cmake.in
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.507280 evalhyd-python-0.1.0.0/deps/xtl/
--rw-r--r--   0 thibhlln   (501) staff       (20)     1437 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.appveyor.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.512076 evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/
--rw-r--r--   0 thibhlln   (501) staff       (20)     1263 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/azure-pipelines-linux-clang.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      905 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/azure-pipelines-linux-gcc.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      697 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/azure-pipelines-osx.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     2939 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/azure-pipelines-win.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)      726 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/unix-build.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)       36 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.git
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.512835 evalhyd-python-0.1.0.0/deps/xtl/.github/
--rw-r--r--   0 thibhlln   (501) staff       (20)      268 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 thibhlln   (501) staff       (20)      536 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.gitignore
--rw-r--r--   0 thibhlln   (501) staff       (20)      712 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/.releash.py
--rw-r--r--   0 thibhlln   (501) staff       (20)     6019 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)     1947 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/README.md
--rw-r--r--   0 thibhlln   (501) staff       (20)      270 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/azure-pipelines.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.514463 evalhyd-python-0.1.0.0/deps/xtl/docs/
--rw-r--r--   0 thibhlln   (501) staff       (20)       77 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/environment.yml
--rw-r--r--   0 thibhlln   (501) staff       (20)     7285 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/make.bat
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.528226 evalhyd-python-0.1.0.0/deps/xtl/docs/source/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.528962 evalhyd-python-0.1.0.0/deps/xtl/docs/source/_static/
--rw-r--r--   0 thibhlln   (501) staff       (20)       60 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/_static/main_stylesheet.css
--rw-r--r--   0 thibhlln   (501) staff       (20)     3074 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/basic_types.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1126 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/build-options.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     7674 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/changelog.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)    17753 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/cmake.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     1805 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/conda.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)      828 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/conf.py
--rw-r--r--   0 thibhlln   (501) staff       (20)      445 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/containers.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     6863 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/debian.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)      349 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/design_patterns.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1065 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/index.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     1730 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/installation.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      336 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/meta_programming.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)      436 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/miscellaneous.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     5022 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/quantstack-white.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     1342 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/releasing.rst
--rw-r--r--   0 thibhlln   (501) staff       (20)     2489 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/spack.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)     4505 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/docs/source/xtl.svg
--rw-r--r--   0 thibhlln   (501) staff       (20)       90 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/environment-dev.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.094698 evalhyd-python-0.1.0.0/deps/xtl/include/
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.558037 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/
--rw-r--r--   0 thibhlln   (501) staff       (20)    17320 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xany.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2337 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xbase64.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)   100835 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xbasic_fixed_string.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    12658 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xclosure.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4665 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xcompare.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    47661 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xcomplex.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    18183 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xcomplex_sequence.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    42230 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xdynamic_bitset.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1346 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xfunctional.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1135 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xhalf_float.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)   197648 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xhalf_float_impl.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6518 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xhash.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2394 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xhierarchy_generator.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    13096 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xiterator_base.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3024 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xjson.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    27810 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xmasked_value.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1354 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xmasked_value_meta.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    16807 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xmeta_utils.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    12987 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xmultimethods.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    54666 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xoptional.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4846 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xoptional_meta.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    21055 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xoptional_sequence.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1207 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xplatform.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1527 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xproxy_wrapper.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6318 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xsequence.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      798 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xspan.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    23074 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xspan_impl.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2925 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xsystem.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1365 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xtl_config.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    12217 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xtype_traits.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6534 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xvariant.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)   102860 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xvariant_impl.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5388 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xvisitor.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)       38 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/readthedocs.yml
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.584315 evalhyd-python-0.1.0.0/deps/xtl/test/
--rw-r--r--   0 thibhlln   (501) staff       (20)     4471 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/CMakeLists.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      152 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/main.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2475 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_common_macros.hpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1471 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xbase64.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    38902 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xbasic_fixed_string.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4040 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xclosure.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1386 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xcompare.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    10028 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xcomplex.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4494 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xcomplex_sequence.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    16153 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xdynamic_bitset.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      872 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xfunctional.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1588 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xhalf_float.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     5524 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xhash.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     2874 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xhierarchy_generator.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     7702 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xiterator_base.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    16357 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xmasked_value.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     9999 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xmeta_utils.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)    11344 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xmultimethods.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     9016 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xoptional.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      993 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xplatform.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1830 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xproxy_wrapper.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     3873 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xsequence.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     1242 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xsystem.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4678 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xtype_traits.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     6284 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xvariant.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)     4681 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/test/test_xvisitor.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)      202 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/xtl.pc.in
--rw-r--r--   0 thibhlln   (501) staff       (20)      976 2023-02-01 08:28:36.000000 evalhyd-python-0.1.0.0/deps/xtl/xtlConfig.cmake.in
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.586563 evalhyd-python-0.1.0.0/evalhyd/
--rw-r--r--   0 thibhlln   (501) staff       (20)      163 2023-05-03 15:52:55.000000 evalhyd-python-0.1.0.0/evalhyd/__init__.py
--rw-r--r--   0 thibhlln   (501) staff       (20)     2348 2023-04-14 16:46:32.000000 evalhyd-python-0.1.0.0/evalhyd/evald.py
--rw-r--r--   0 thibhlln   (501) staff       (20)     1947 2023-04-14 16:46:32.000000 evalhyd-python-0.1.0.0/evalhyd/evalp.py
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.586919 evalhyd-python-0.1.0.0/evalhyd/src/
--rw-r--r--   0 thibhlln   (501) staff       (20)     4558 2023-04-14 16:46:32.000000 evalhyd-python-0.1.0.0/evalhyd/src/evalhyd.cpp
--rw-r--r--   0 thibhlln   (501) staff       (20)       26 2023-04-14 16:46:49.000000 evalhyd-python-0.1.0.0/evalhyd/version.py
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.589323 evalhyd-python-0.1.0.0/evalhyd_python.egg-info/
--rw-r--r--   0 thibhlln   (501) staff       (20)      562 2023-05-08 06:52:42.000000 evalhyd-python-0.1.0.0/evalhyd_python.egg-info/PKG-INFO
--rw-r--r--   0 thibhlln   (501) staff       (20)    28475 2023-05-08 06:52:42.000000 evalhyd-python-0.1.0.0/evalhyd_python.egg-info/SOURCES.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)        1 2023-05-08 06:52:42.000000 evalhyd-python-0.1.0.0/evalhyd_python.egg-info/dependency_links.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)        1 2023-05-08 06:52:42.000000 evalhyd-python-0.1.0.0/evalhyd_python.egg-info/not-zip-safe
--rw-r--r--   0 thibhlln   (501) staff       (20)       21 2023-05-08 06:52:42.000000 evalhyd-python-0.1.0.0/evalhyd_python.egg-info/requires.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)        8 2023-05-08 06:52:42.000000 evalhyd-python-0.1.0.0/evalhyd_python.egg-info/top_level.txt
--rw-r--r--   0 thibhlln   (501) staff       (20)      193 2023-04-14 16:46:32.000000 evalhyd-python-0.1.0.0/pyproject.toml
--rw-r--r--   0 thibhlln   (501) staff       (20)       38 2023-05-08 06:52:42.591657 evalhyd-python-0.1.0.0/setup.cfg
--rw-r--r--   0 thibhlln   (501) staff       (20)     1956 2023-05-08 06:49:05.000000 evalhyd-python-0.1.0.0/setup.py
-drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-05-08 06:52:42.590364 evalhyd-python-0.1.0.0/tests/
--rw-r--r--   0 thibhlln   (501) staff       (20)    11937 2023-05-03 15:52:55.000000 evalhyd-python-0.1.0.0/tests/test_determinist.py
--rw-r--r--   0 thibhlln   (501) staff       (20)    18711 2023-05-03 15:52:55.000000 evalhyd-python-0.1.0.0/tests/test_probabilist.py
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.845971 evalhyd-python-0.1.1.0/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    35580 2023-04-14 16:46:32.000000 evalhyd-python-0.1.1.0/LICENCE.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)       27 2023-06-16 13:41:33.000000 evalhyd-python-0.1.1.0/MANIFEST.in
+-rw-r--r--   0 thibhlln   (501) staff       (20)      801 2023-06-16 15:00:24.845552 evalhyd-python-0.1.1.0/PKG-INFO
+-rw-r--r--   0 thibhlln   (501) staff       (20)      113 2023-04-14 16:46:32.000000 evalhyd-python-0.1.1.0/README.md
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.433772 evalhyd-python-0.1.1.0/deps/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.447257 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/
+-rw-r--r--   0 thibhlln   (501) staff       (20)       44 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/.git
+-rw-r--r--   0 thibhlln   (501) staff       (20)       55 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/.gitignore
+-rw-r--r--   0 thibhlln   (501) staff       (20)      406 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/.gitlab-ci.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3208 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      224 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/EvalHydConfig.cmake.in
+-rw-r--r--   0 thibhlln   (501) staff       (20)    35580 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/LICENCE.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      144 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/README.md
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1239 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/changelog.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      198 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/environment.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.423093 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.449022 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.452100 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.456003 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2135 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/diagnostics.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    34649 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/efficiencies.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    18582 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/errors.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    18929 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/evaluator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11025 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/events.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    20942 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/masks.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      921 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/maths.hpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.462620 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    48052 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/brier.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8109 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/cdf.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    22471 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/contingency.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2284 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/diagnostics.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    27130 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/evaluator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17560 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/intervals.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6786 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/multivariate.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10212 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/quantiles.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    18863 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/ranks.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10414 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/uncertainty.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4649 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/utils.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    21913 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/evald.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    21085 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/evalp.hpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.465843 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1839 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.469154 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1366 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/q_obs.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9351 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/q_obs_1yr.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)    69202 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/q_prd.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)   125330 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/q_prd_1yr.csv
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.424200 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.475459 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3366 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/CONT_TBL.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      957 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/KGE.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      960 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/KGEPRIME.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2907 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/KGEPRIME_D.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2907 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/KGE_D.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1071 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/MAE.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      969 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/MARE.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1224 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/MSE.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      963 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/NSE.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      915 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/RMSE.csv
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.487563 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/
+-rw-r--r--   0 thibhlln   (501) staff       (20)       16 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/AS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       33 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/AW.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       32 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/AWN.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       52 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/BS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       52 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/BSS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      156 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/BS_CRD.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      156 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/BS_LBD.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       32 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/CR.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       18 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/CRPS_FROM_BS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       17 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/CRPS_FROM_ECDF.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       18 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/CRPS_FROM_QS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2704 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/CSI.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       18 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/DS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       18 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/ES.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2704 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/FAR.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2704 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/POD.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2704 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/POFD.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      918 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/QS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)      832 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/RANK_HIST.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8122 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/REL_DIAG.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       52 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/ROCSS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)       37 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/WS.csv
+-rw-r--r--   0 thibhlln   (501) staff       (20)    25964 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/test_determinist.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    35061 2023-06-16 12:55:23.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/test_probabilist.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    28110 2023-04-14 16:08:34.000000 evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/test_uncertainty.cpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.494290 evalhyd-python-0.1.1.0/deps/xtensor/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1681 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.appveyor.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.530424 evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1229 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/azure-pipelines-linux-clang.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1357 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/azure-pipelines-linux-gcc.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      724 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/azure-pipelines-osx.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2813 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/azure-pipelines-win.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2291 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/unix-build.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2671 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.clang-format
+-rw-r--r--   0 thibhlln   (501) staff       (20)       40 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.git
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.531019 evalhyd-python-0.1.1.0/deps/xtensor/.github/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      426 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.532642 evalhyd-python-0.1.1.0/deps/xtensor/.github/workflows/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      836 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.github/workflows/gh-pages.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      225 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.github/workflows/static-analysis.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      660 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/.gitignore
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1290 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/.pre-commit-config.yaml
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12880 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)    14807 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/README.md
+-rw-r--r--   0 thibhlln   (501) staff       (20)      259 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/azure-pipelines.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.545363 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6224 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5457 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_adapter.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8175 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_assign.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7165 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_builder.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4306 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_container.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1985 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_creation.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2622 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_increment_stepper.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2541 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_lambda_expressions.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    16511 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_math.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2054 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_random.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4212 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_reducer.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    14322 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_view_access.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2549 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_view_adapt.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5634 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_view_assignment.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11595 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_views.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2440 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_xshape.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      973 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/copyGBenchmark.cmake.in
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1019 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/downloadGBenchmark.cmake.in
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1380 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/benchmark/main.cpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.546108 evalhyd-python-0.1.1.0/deps/xtensor/cmake/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12026 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/cmake/FindTBB.cmake
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.549946 evalhyd-python-0.1.1.0/deps/xtensor/docs/
+-rw-r--r--   0 thibhlln   (501) staff       (20)       48 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/ghp_environment.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7750 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/make.bat
+-rw-r--r--   0 thibhlln   (501) staff       (20)       69 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/rtd_environment.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.591835 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.593399 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/_static/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      302 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/_static/goatcounter.js
+-rw-r--r--   0 thibhlln   (501) staff       (20)       60 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/_static/main_stylesheet.css
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7074 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/adaptor.rst
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.628676 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      539 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/accumulating_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      828 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/basic_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      611 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/classif_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      931 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/container_index.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      509 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/error_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      591 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/exponential_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      612 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/expression_index.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      421 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/function_index.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      705 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/hyperbolic_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      443 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/index_related.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      287 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/io_index.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      468 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/iterator_index.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      887 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/nan_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      604 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/nearint_operations.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1830 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/operators.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      602 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/power_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1731 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/reducing_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      299 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/shape.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      613 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/trigonometric_functions.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      399 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xaccumulator.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      342 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xadapt.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      387 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xarray.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      328 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xarray_adaptor.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      733 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xaxis_iterator.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      806 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xaxis_slice_iterator.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      371 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xbroadcast.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1308 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xbuilder.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      333 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xchunked_array.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      593 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xcontainer.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      346 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xcontainer_semantic.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      369 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xcsv.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      304 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xeval.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      505 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xexpression.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      367 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xfixed.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      394 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xfunction.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      391 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xfunctor_view.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      320 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xgenerator.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1336 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xhistogram.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      489 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xindex_view.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1272 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xio.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      425 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xiterable.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      432 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xjson.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      384 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xmanipulation.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      328 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xmasked_view.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    22382 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xmath.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      540 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xnpy.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      352 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xoptional_assembly.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      376 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xoptional_assembly_adaptor.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      372 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xoptional_assembly_base.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      598 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xpad.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1800 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xrandom.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      367 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xreducer.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      308 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xrepeat.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      331 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xsemantic_base.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      649 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xset_operation.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      342 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xshape.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      338 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xsort.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      595 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xstrided_view.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      350 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xstrides.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      514 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xtensor.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      332 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xtensor_adaptor.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      676 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xview.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      331 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xview_semantic.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3232 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/binder-logo.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9734 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/bindings.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4943 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/build-options.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5723 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/builder.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    97913 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/changelog.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11665 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/closure-semantics.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17753 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/cmake.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6850 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/compilers.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1806 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/conda.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1309 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/conf.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10261 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/container.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7481 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/debian.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4342 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/dev-build-options.rst
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.643151 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    14790 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/assign_xexpression.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8285 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/assignment.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12540 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/computed_assign.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10299 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/concepts.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7948 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/expression_tree.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12444 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/extended_copy_semantic.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10146 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/implementation_classes.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9866 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/iterating_expression.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    26079 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/iteration.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    22373 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/stepper_basic.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    23161 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/stepper_broadcasting.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17381 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/stepper_iterating.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    23695 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/stepper_to_end.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17684 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xarray_uml.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10216 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xcontainer_classes.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7800 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xfunction_tree.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8745 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xsemantic_classes.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)      764 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xtensor_internals.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10234 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/expression.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    15686 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/external-structures.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/file_loading.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6137 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/getting_started.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2705 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/histogram.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2787 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/index.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8157 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/indices.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2896 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/installation.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4176 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/missing.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4203 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/numpy-differences.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    64585 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/numpy.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)   487166 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/numpy.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    13200 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/operator.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4965 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/pitfall.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5023 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quantstack-white.svg
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.647509 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6173 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/basic.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6111 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/builder.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2609 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/chunked_arrays.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6364 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/iterator.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2610 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/manipulation.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3546 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/math.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2204 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/operator.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3491 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/reducer.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3497 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/random.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3235 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/rank.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    13334 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/related.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1860 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/releasing.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4054 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/scalar.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2489 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/spack.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    14644 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/view.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)   198081 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xeus-cling-screenshot.png
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5268 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xframe.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4209 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xsimd-small.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2976 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xsimd.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5385 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-blas-small.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5386 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-blas.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)   475924 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-cookiecutter.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7789 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-fftw.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7065 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-io-small.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7065 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-io.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6178 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-julia-small.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6184 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-julia.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6266 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-python-small.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6273 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-python.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4528 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-r-small.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4536 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-r.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10906 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-ros.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3478 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4511 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtl.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)      132 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/environment-dev.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      111 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/environment.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.431456 evalhyd-python-0.1.1.0/deps/xtensor/include/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.701294 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11676 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xaccessible.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    14104 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xaccumulator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    36156 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xadapt.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    24640 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xarray.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    49134 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xassign.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10591 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xaxis_iterator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11290 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xaxis_slice_iterator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    38555 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xblockwise_reducer.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17724 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xblockwise_reducer_functors.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    14970 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xbroadcast.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    41449 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xbuffer_adaptor.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    42455 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xbuilder.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    24351 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xchunked_array.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11386 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xchunked_assign.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8851 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xchunked_view.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8407 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xcomplex.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    41731 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xcontainer.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8597 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xcsv.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    28975 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xdynamic_view.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5808 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xeval.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    13184 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xexception.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    24760 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xexpression.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7640 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xexpression_holder.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5748 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xexpression_traits.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    37637 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xfixed.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    39903 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xfunction.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    57648 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xfunctor_view.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17080 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xgenerator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    21613 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xhistogram.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    26749 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xindex_view.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3914 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xinfo.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    26832 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xio.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    52665 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xiterable.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    35923 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xiterator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6722 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xjson.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3452 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xlayout.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    38079 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmanipulation.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    24021 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmasked_view.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)   120621 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmath.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12998 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmime.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3729 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmultiindex_iterator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6196 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xnoalias.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    31209 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xnorm.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    27263 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xnpy.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3286 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoffset_view.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    34576 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoperation.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    48774 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoptional.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    27116 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoptional_assembly.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    37733 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoptional_assembly_base.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    19544 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoptional_assembly_storage.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10799 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xpad.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    40536 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xrandom.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    64806 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xreducer.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    23264 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xrepeat.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    34142 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xscalar.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    24660 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xsemantic.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7366 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xset_operation.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    16921 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xshape.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    49258 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xslice.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    48051 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xsort.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    59022 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xstorage.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    29524 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xstrided_view.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    34210 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xstrided_view_base.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    31463 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xstrides.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    35939 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xtensor.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4138 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xtensor_config.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7842 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xtensor_forward.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8203 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xtensor_simd.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    28368 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xutils.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xvectorize.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    83925 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xview.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8366 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xview_utils.hpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.701772 evalhyd-python-0.1.1.0/deps/xtensor/notebooks/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.702913 evalhyd-python-0.1.1.0/deps/xtensor/notebooks/images/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    19420 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/notebooks/images/xtensor-blas.png
+-rw-r--r--   0 thibhlln   (501) staff       (20)    15734 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/notebooks/images/xtensor.png
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10473 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/notebooks/xtensor.ipynb
+-rw-r--r--   0 thibhlln   (501) staff       (20)       40 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/readthedocs.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.751663 evalhyd-python-0.1.1.0/deps/xtensor/test/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11009 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/CMakeLists.txt
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.753445 evalhyd-python-0.1.1.0/deps/xtensor/test/files/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.756226 evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5964 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_broadcast_view.cppy
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1985 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_xhistogram.cppy
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1191 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_xmath_interp.cppy
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2742 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_xmath_reducers.cppy
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10274 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_xsort.cppy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      384 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/generate.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3387 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/preprocess.py
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.764109 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      335 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/big_exp.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      190 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/bool_fn.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2190 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/complex_numbers.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2190 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/complex_zero_erasing.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)       86 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/custom_formatter_result.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6426 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/cut_4d.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      162 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/cut_both.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)       42 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/cut_high.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      130 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/cut_long.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1150 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/float_leading_zero.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)       81 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/long_strings.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      355 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/precision.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6206 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/print_options_result.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4580 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/random_nan_inf.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      102 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/random_strings.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      195 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/threed_double.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)       81 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/twod_double.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)    25341 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results.hpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.771077 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/bool.be.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/bool.le.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/bool_fortran.be.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      155 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/bool_fortran.le.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      344 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/double.be.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      344 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/double.le.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      344 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/double_fortran.be.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      344 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/double_fortran.le.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      148 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/int.be.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      148 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/int.le.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      168 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/unsignedlong.be.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      168 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/unsignedlong.le.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      168 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/unsignedlong_fortran.be.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      168 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/files/xnpy_files/unsignedlong_fortran.le.npy
+-rw-r--r--   0 thibhlln   (501) staff       (20)      156 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/main.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2272 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/set_compiler_flag.cmake
+-rw-r--r--   0 thibhlln   (501) staff       (20)    36747 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_common.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2309 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_common_macros.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    34696 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_broadcast_view.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12934 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_xhistogram.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5271 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_xmath_interp.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    96615 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_xmath_reducers.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    45383 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_xsort.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5025 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_sfinae.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9714 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_strided_assign.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2744 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_utils.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6966 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xaccumulator.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17890 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xadapt.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10473 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xadaptor_semantic.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12587 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xarray.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5419 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xarray_adaptor.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3699 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xassign.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7411 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xaxis_iterator.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11048 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xaxis_slice_iterator.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    14023 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xblockwise_reducer.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6271 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xbroadcast.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6426 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xbuffer_adaptor.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    22869 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xbuilder.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4761 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xchunked_array.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2226 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xchunked_view.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12402 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xcomplex.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    18690 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xcontainer_semantic.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1972 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xcsv.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3305 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xdatesupport.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9462 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xdynamic_view.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11400 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xeval.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1961 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xexception.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4674 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xexpression.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2315 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xexpression_holder.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3057 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xexpression_traits.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11596 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xfixed.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3447 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xfunc_on_xexpression.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    15395 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xfunction.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6001 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xfunctor_adaptor.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4020 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xhistogram.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5850 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xindex_view.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1179 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xinfo.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9495 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xio.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    24624 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xiterator.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1717 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xjson.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7164 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xlayout.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    21276 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmanipulation.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8514 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmasked_view.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    27470 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmath.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    13599 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmath_result_type.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2006 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmime.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1090 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmultiindex_iterator.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    15346 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xnan_functions.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11242 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xnoalias.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7880 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xnorm.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6674 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xnpy.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    32637 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoperation.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    19755 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoptional.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    18388 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoptional_assembly.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    14479 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoptional_assembly_adaptor.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6078 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoptional_assembly_storage.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8877 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xpad.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8888 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xrandom.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    40571 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xreducer.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10260 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xrepeat.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3357 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xscalar.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9959 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xscalar_semantic.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4661 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xsemantic.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1980 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xset_operation.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2482 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xshape.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2192 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xsimd.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1231 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xsimd8.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17712 2023-03-24 12:52:57.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xsort.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9643 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xstorage.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    32413 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xstrided_view.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10749 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xstrides.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    15248 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xtensor.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5868 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xtensor_adaptor.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2598 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xtensor_semantic.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8025 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xutils.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2270 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xvectorize.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    57076 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xview.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    16538 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/test/test_xview_semantic.cpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.771450 evalhyd-python-0.1.1.0/deps/xtensor/tools/
+-rwxr-xr-x   0 thibhlln   (501) staff       (20)     1028 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/tools/check_circular.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      234 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/xtensor.pc.in
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2789 2023-02-01 09:15:55.000000 evalhyd-python-0.1.1.0/deps/xtensor/xtensorConfig.cmake.in
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.498672 evalhyd-python-0.1.1.0/deps/xtensor-python/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1253 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/.appveyor.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.500375 evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1263 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-linux-clang.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      895 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-linux-gcc.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      784 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-osx.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2063 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/unix-build.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)       47 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/.git
+-rw-r--r--   0 thibhlln   (501) staff       (20)      606 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/.gitignore
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5918 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7128 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/README.md
+-rw-r--r--   0 thibhlln   (501) staff       (20)      213 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/azure-pipelines.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.504088 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4191 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      215 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/benchmark_pyarray.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      236 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/benchmark_pybind_array.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      247 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/benchmark_pybind_vectorize.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      240 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/benchmark_pytensor.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      226 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/benchmark_pyvectorize.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1624 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/main.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3387 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/setup.py
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.504497 evalhyd-python-0.1.1.0/deps/xtensor-python/cmake/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3644 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/cmake/FindNumPy.cmake
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.505454 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/
+-rw-r--r--   0 thibhlln   (501) staff       (20)       80 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/environment.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7285 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/make.bat
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.513540 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.513864 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/_static/
+-rw-r--r--   0 thibhlln   (501) staff       (20)       60 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/_static/main_stylesheet.css
+-rw-r--r--   0 thibhlln   (501) staff       (20)      399 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/api_reference.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1219 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/array_tensor.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2527 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/basic_usage.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17753 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/cmake.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)      806 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/compilers.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1805 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/conda.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)      861 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/conf.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2091 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/cookiecutter.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6863 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/debian.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1193 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/dev_build_options.rst
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.427216 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.514993 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/copy_cast/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      407 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/copy_cast/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      201 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/copy_cast/example.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      874 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/copy_cast/main.cpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.515900 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/readme_example_1/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      432 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/readme_example_1/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      124 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/readme_example_1/example.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      511 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/readme_example_1/main.cpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.517538 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/sfinae/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      512 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/sfinae/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      197 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/sfinae/example.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      222 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/sfinae/main.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      600 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/sfinae/mymodule.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      314 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/sfinae/python.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6348 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2951 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/index.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1784 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/installation.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3030 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/numpy_capi.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      283 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/pyarray.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      286 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/pytensor.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      285 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/pyvectorize.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5022 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/quantstack-white.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1415 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/releasing.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5970 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/xtensor-python.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)      198 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/environment-dev.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.427663 evalhyd-python-0.1.1.0/deps/xtensor-python/include/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.521519 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    19952 2023-02-01 08:29:46.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pyarray.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10631 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pyarray_backstrides.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    16852 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pycontainer.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2331 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pynative_casters.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8683 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pystrides_adaptor.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    19005 2023-02-01 08:29:46.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pytensor.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2060 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pyvectorize.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      813 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/xtensor_python_config.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11257 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/xtensor_type_caster_base.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)       38 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/readthedocs.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.525302 evalhyd-python-0.1.1.0/deps/xtensor-python/test/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3953 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1027 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/copyGTest.cmake.in
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1086 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/downloadGTest.cmake.in
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1146 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/main.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    26762 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_common.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9110 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_pyarray.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6246 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_pyarray_traits.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     8549 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_pytensor.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1913 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_pyvectorize.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1914 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_sfinae.cpp
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.527125 evalhyd-python-0.1.1.0/deps/xtensor-python/test_python/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12267 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test_python/main.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4021 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test_python/setup.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11447 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/test_python/test_pyarray.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1115 2023-02-01 08:29:29.000000 evalhyd-python-0.1.1.0/deps/xtensor-python/xtensor-pythonConfig.cmake.in
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.777673 evalhyd-python-0.1.1.0/deps/xtl/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1437 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.appveyor.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.780910 evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1263 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/azure-pipelines-linux-clang.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      905 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/azure-pipelines-linux-gcc.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      697 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/azure-pipelines-osx.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2939 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/azure-pipelines-win.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)      726 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/unix-build.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)       36 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.git
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.781507 evalhyd-python-0.1.1.0/deps/xtl/.github/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      268 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 thibhlln   (501) staff       (20)      536 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.gitignore
+-rw-r--r--   0 thibhlln   (501) staff       (20)      712 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/.releash.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6019 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1947 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/README.md
+-rw-r--r--   0 thibhlln   (501) staff       (20)      270 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/azure-pipelines.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.782669 evalhyd-python-0.1.1.0/deps/xtl/docs/
+-rw-r--r--   0 thibhlln   (501) staff       (20)       77 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/environment.yml
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7285 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/make.bat
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.792794 evalhyd-python-0.1.1.0/deps/xtl/docs/source/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.793618 evalhyd-python-0.1.1.0/deps/xtl/docs/source/_static/
+-rw-r--r--   0 thibhlln   (501) staff       (20)       60 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/_static/main_stylesheet.css
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3074 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/basic_types.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1126 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/build-options.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7674 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/changelog.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17753 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/cmake.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1805 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/conda.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)      828 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/conf.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)      445 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/containers.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6863 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/debian.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)      349 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/design_patterns.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1065 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/index.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1730 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/installation.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      336 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/meta_programming.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)      436 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/miscellaneous.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5022 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/quantstack-white.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1342 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/releasing.rst
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2489 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/spack.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4505 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/docs/source/xtl.svg
+-rw-r--r--   0 thibhlln   (501) staff       (20)       90 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/environment-dev.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.435538 evalhyd-python-0.1.1.0/deps/xtl/include/
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.819462 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    17320 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xany.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2337 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xbase64.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)   100835 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xbasic_fixed_string.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12658 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xclosure.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4665 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xcompare.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    47661 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xcomplex.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    18183 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xcomplex_sequence.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    42230 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xdynamic_bitset.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1346 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xfunctional.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1135 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xhalf_float.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)   197648 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xhalf_float_impl.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6518 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xhash.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2394 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xhierarchy_generator.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    13096 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xiterator_base.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3024 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xjson.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    27810 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xmasked_value.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1354 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xmasked_value_meta.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    16807 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xmeta_utils.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12987 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xmultimethods.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    54666 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xoptional.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4846 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xoptional_meta.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    21055 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xoptional_sequence.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1207 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xplatform.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1527 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xproxy_wrapper.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6318 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xsequence.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      798 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xspan.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    23074 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xspan_impl.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2925 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xsystem.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1365 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xtl_config.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    12217 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xtype_traits.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6534 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xvariant.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)   102860 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xvariant_impl.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5388 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xvisitor.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)       38 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/readthedocs.yml
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.836633 evalhyd-python-0.1.1.0/deps/xtl/test/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4471 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/CMakeLists.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      152 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/main.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2475 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_common_macros.hpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1471 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xbase64.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    38902 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xbasic_fixed_string.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4040 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xclosure.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1386 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xcompare.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    10028 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xcomplex.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4494 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xcomplex_sequence.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    16153 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xdynamic_bitset.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      872 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xfunctional.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1588 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xhalf_float.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     5524 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xhash.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2874 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xhierarchy_generator.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     7702 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xiterator_base.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    16357 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xmasked_value.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9999 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xmeta_utils.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11344 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xmultimethods.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     9016 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xoptional.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      993 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xplatform.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1830 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xproxy_wrapper.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     3873 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xsequence.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1242 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xsystem.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4678 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xtype_traits.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     6284 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xvariant.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4681 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/test/test_xvisitor.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)      202 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/xtl.pc.in
+-rw-r--r--   0 thibhlln   (501) staff       (20)      976 2023-02-01 08:28:36.000000 evalhyd-python-0.1.1.0/deps/xtl/xtlConfig.cmake.in
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.839507 evalhyd-python-0.1.1.0/evalhyd/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      163 2023-05-03 15:52:55.000000 evalhyd-python-0.1.1.0/evalhyd/__init__.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2348 2023-04-14 16:46:32.000000 evalhyd-python-0.1.1.0/evalhyd/evald.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)     1947 2023-04-14 16:46:32.000000 evalhyd-python-0.1.1.0/evalhyd/evalp.py
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.839933 evalhyd-python-0.1.1.0/evalhyd/src/
+-rw-r--r--   0 thibhlln   (501) staff       (20)     4558 2023-05-15 15:15:50.000000 evalhyd-python-0.1.1.0/evalhyd/src/evalhyd.cpp
+-rw-r--r--   0 thibhlln   (501) staff       (20)       26 2023-06-16 13:41:33.000000 evalhyd-python-0.1.1.0/evalhyd/version.py
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.843340 evalhyd-python-0.1.1.0/evalhyd_python.egg-info/
+-rw-r--r--   0 thibhlln   (501) staff       (20)      801 2023-06-16 15:00:24.000000 evalhyd-python-0.1.1.0/evalhyd_python.egg-info/PKG-INFO
+-rw-r--r--   0 thibhlln   (501) staff       (20)    28383 2023-06-16 15:00:24.000000 evalhyd-python-0.1.1.0/evalhyd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)        1 2023-06-16 15:00:24.000000 evalhyd-python-0.1.1.0/evalhyd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)        1 2023-06-16 14:42:44.000000 evalhyd-python-0.1.1.0/evalhyd_python.egg-info/not-zip-safe
+-rw-r--r--   0 thibhlln   (501) staff       (20)       21 2023-06-16 15:00:24.000000 evalhyd-python-0.1.1.0/evalhyd_python.egg-info/requires.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)        8 2023-06-16 15:00:24.000000 evalhyd-python-0.1.1.0/evalhyd_python.egg-info/top_level.txt
+-rw-r--r--   0 thibhlln   (501) staff       (20)      193 2023-04-14 16:46:32.000000 evalhyd-python-0.1.1.0/pyproject.toml
+-rw-r--r--   0 thibhlln   (501) staff       (20)       38 2023-06-16 15:00:24.846079 evalhyd-python-0.1.1.0/setup.cfg
+-rw-r--r--   0 thibhlln   (501) staff       (20)     2221 2023-06-16 13:41:33.000000 evalhyd-python-0.1.1.0/setup.py
+drwxr-xr-x   0 thibhlln   (501) staff       (20)        0 2023-06-16 15:00:24.844483 evalhyd-python-0.1.1.0/tests/
+-rw-r--r--   0 thibhlln   (501) staff       (20)    11937 2023-05-03 15:52:55.000000 evalhyd-python-0.1.1.0/tests/test_determinist.py
+-rw-r--r--   0 thibhlln   (501) staff       (20)    18683 2023-06-16 13:41:33.000000 evalhyd-python-0.1.1.0/tests/test_probabilist.py
```

### Comparing `evalhyd-python-0.1.0.0/LICENCE.rst` & `evalhyd-python-0.1.1.0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/PKG-INFO` & `evalhyd-python-0.1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: evalhyd-python
-Version: 0.1.0.0
+Version: 0.1.1.0
 Summary: Python bindings for EvalHyd
 Download-URL: https://pypi.python.org/pypi/evalhyd-python
 Author: Thibault Hallouin
 Author-email: thibault.hallouin@inrae.fr
+License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.irstea.fr/HYCAR-Hydro/evalhyd/evalhyd-python/-/issues
 Project-URL: Documentation, https://hydrogr.github.io/evalhyd/python
 Project-URL: Source Code, https://gitlab.irstea.fr/hycar-hydro/evalhyd/evalhyd-python
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides-Extra: tests
 License-File: LICENCE.rst
 
 An evaluator for streamflow predictions.
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # The full licence is in the file LICENCE, distributed with this software.
 
 cmake_minimum_required(VERSION 3.15)
 
 project(
         EvalHyd
         LANGUAGES CXX
-        VERSION 0.1.0
+        VERSION 0.1.1
         DESCRIPTION "Utility to evaluate streamflow predictions"
 )
 
 # ------------------------------------------------------------------------------
 # dependencies
 # ------------------------------------------------------------------------------
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/LICENCE.rst` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/diagnostics.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/diagnostics.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/efficiencies.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/efficiencies.hpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -805,8 +805,8 @@
 
                 return KGENP_D;
             }
         }
     }
 }
 
-#endif //EVALHYD_DETERMINIST_EFFICIENCIES_HPP
+#endif //EVALHYD_DETERMINIST_EFFICIENCIES_HPP
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/errors.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/errors.hpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -474,8 +474,8 @@
 
                 return RMSE;
             }
         }
     }
 }
 
-#endif //EVALHYD_DETERMINIST_ERRORS_HPP
+#endif //EVALHYD_DETERMINIST_ERRORS_HPP
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/evaluator.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/evaluator.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/events.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/determinist/events.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/masks.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/masks.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,18 @@
         {
             msk_tree subset;
 
             // pattern supported to specify conditions to generate masks on
             // observed or predicted (median or mean for probabilist) streamflow
             // e.g. q{>9.} q{<9} q{>=99.0} q{<=99} q{>9,<99} q{==9} q{!=9}
             std::regex exp_q (
-                    R"((q_obs|q_prd_median|q_prd_mean)\{(((<|>|<=|>=|==|!=)(mean,?|median,?|qtl[0-1]\.[0-9]+,?|[0-9]+\.?[0-9]*,?))+)\})"
+                    R"((q_obs|q_prd_median|q_prd_mean)\{(((<|>|<=|>=|==|!=)(mean,?|median,?|qtl(0|1)\.(0|1|2|3|4|5|6|7|8|9)+,?|(0|1|2|3|4|5|6|7|8|9)+\.?(0|1|2|3|4|5|6|7|8|9)*,?))+)\})"
+                    // NOTE: this should be `R"((q_obs|q_prd_median|q_prd_mean)\{(((<|>|<=|>=|==|!=)(mean,?|median,?|qtl[0-1]\.[0-9]+,?|[0-9]+\.?[0-9]*,?))+)\})"`
+                    //       but there is a bug in the building chain for R packages
+                    //       https://gitlab.irstea.fr/HYCAR-Hydro/evalhyd/evalhyd-r/-/issues/6
             );
 
             for (std::sregex_iterator i =
                     std::sregex_iterator(msk_str.begin(), msk_str.end(), exp_q);
                  i != std::sregex_iterator(); i++)
             {
                 const std::smatch & mtc = *i;
@@ -47,15 +50,20 @@
                 std::string var = mtc[1];
                 std::string str = mtc[2];
 
                 // process masking conditions on streamflow
                 std::vector<std::vector<std::string>> conditions;
 
                 // pattern supported to specify masking conditions based on streamflow
-                std::regex ex (R"((<|>|<=|>=|==|!=)(mean|median|qtl[0-1]\.[0-9]+|[0-9]+\.?[0-9]*))");
+                std::regex ex (
+                        R"((<|>|<=|>=|==|!=)(mean|median|qtl(0|1)\.(0|1|2|3|4|5|6|7|8|9)+|(0|1|2|3|4|5|6|7|8|9)+\.?(0|1|2|3|4|5|6|7|8|9)*))"
+                        // NOTE: this should be `R"((<|>|<=|>=|==|!=)(mean|median|qtl[0-1]\.[0-9]+|[0-9]+\.?[0-9]*))"`
+                        //       but there is a bug in the building chain for R packages
+                        //       https://gitlab.irstea.fr/HYCAR-Hydro/evalhyd/evalhyd-r/-/issues/6
+                );
 
                 for (std::sregex_iterator j =
                         std::sregex_iterator(str.begin(), str.end(), ex);
                      j != std::sregex_iterator(); j++)
                 {
                     const std::smatch & mt = *j;
 
@@ -88,15 +96,20 @@
                 }
 
                 subset[var] = conditions;
             }
 
             // pattern supported to specify conditions to generate masks on time index
             // e.g. t{0:10} t{0:10,20:30} t{0,1,2,3} t{0:10,30,40,50} t{:}
-            std::regex exp_t (R"((t)\{(:|([0-9]+:[0-9]+,?|[0-9]+,?)+)\})");
+            std::regex exp_t (
+                    R"((t)\{(:|((0|1|2|3|4|5|6|7|8|9)+:(0|1|2|3|4|5|6|7|8|9)+,?|(0|1|2|3|4|5|6|7|8|9)+,?)+)\})"
+                    // NOTE: this should be `R"((t)\{(:|([0-9]+:[0-9]+,?|[0-9]+,?)+)\})"`
+                    //       but there is a bug in the building chain for R packages
+                    //       https://gitlab.irstea.fr/HYCAR-Hydro/evalhyd/evalhyd-r/-/issues/6
+            );
 
             for (std::sregex_iterator i =
                     std::sregex_iterator(msk_str.begin(), msk_str.end(), exp_t);
                  i != std::sregex_iterator(); i++)
             {
                 const std::smatch & mtc = *i;
 
@@ -110,15 +123,20 @@
                 if (s == ":")
                 {
                     condition.emplace_back();
                 }
                 else
                 {
                     // pattern supported to specify masking conditions based on time index
-                    std::regex e (R"([0-9]+:[0-9]+|[0-9]+)");
+                    std::regex e (
+                            R"((0|1|2|3|4|5|6|7|8|9)+:(0|1|2|3|4|5|6|7|8|9)+|(0|1|2|3|4|5|6|7|8|9)+)"
+                            // NOTE: this should be `R"([0-9]+:[0-9]+|[0-9]+)"`
+                            //       but there is a bug in the building chain for R packages
+                            //       https://gitlab.irstea.fr/HYCAR-Hydro/evalhyd/evalhyd-r/-/issues/6
+                    );
 
                     for (std::sregex_iterator j =
                             std::sregex_iterator(s.begin(), s.end(), e);
                          j != std::sregex_iterator(); j++)
                     {
                         const std::smatch & m = *j;
 
@@ -228,25 +246,37 @@
                     auto get_val =
                             [&](const std::string& str, const std::string& num)
                     {
                         if (str.empty())  // it is a simple numerical value
                         {
                             return std::stod(num);
                         }
-                        else if (str == "median")
-                        {
-                            return xt::median(q);
-                        }
-                        else if (str == "mean")
-                        {
-                            return xt::mean(q)();
-                        }
-                        else  // (str == "qtl")
+                        else
                         {
-                            return xt::quantile(q, {std::stod(num)})();
+                            auto q_filtered = xt::filter(q, !xt::isnan(q));
+
+                            if (q_filtered.size() > 0)
+                            {
+                                if (str == "median")
+                                {
+                                    return xt::median(q_filtered);
+                                }
+                                else if (str == "mean")
+                                {
+                                    return xt::mean(q_filtered)();
+                                }
+                                else  // (str == "qtl")
+                                {
+                                    return xt::quantile(q_filtered, {std::stod(num)})();
+                                }
+                            }
+                            else
+                            {
+                                return double(NAN);
+                            }
                         }
                     };
 
                     // preprocess conditions to identify special cases
                     // within/without
                     bool within = false;
                     bool without = false;
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/maths.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/maths.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/brier.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/brier.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/cdf.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/cdf.hpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
                 return CRPS_FROM_ECDF;
             }
         }
     }
 }
 
-#endif //EVALHYD_PROBABILIST_CDF_HPP
+#endif //EVALHYD_PROBABILIST_CDF_HPP
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/contingency.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/contingency.hpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -537,8 +537,8 @@
 
                 return ROCSS;
             }
         }
     }
 }
 
-#endif //EVALHYD_PROBABILIST_CONTINGENCY_HPP
+#endif //EVALHYD_PROBABILIST_CONTINGENCY_HPP
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/diagnostics.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/diagnostics.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/evaluator.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/evaluator.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
             // > Ranks-based
             xtl::xoptional<xt::xtensor<double, 3>, bool> r_k;
             xtl::xoptional<xt::xtensor<double, 5>, bool> o_j;
             // > Intervals-based
             xtl::xoptional<xt::xtensor<double, 5>, bool> itv_bnds;
             xtl::xoptional<xt::xtensor<double, 4>, bool> obs_in_itv;
             xtl::xoptional<xt::xtensor<double, 4>, bool> itv_width;
-            xtl::xoptional<xt::xtensor<double, 6>, bool> clim_bnds;
 
             // members for intermediate evaluation metrics
             // (i.e. before the reduction along the temporal axis)
             // > Brier-based
             xtl::xoptional<xt::xtensor<double, 4>, bool> bs;
             // > CDF-based
             xtl::xoptional<xt::xtensor<double, 3>, bool> crps_from_ecdf;
@@ -120,17 +119,15 @@
             xtl::xoptional<xt::xtensor<double, 5>, bool> RANK_HIST;
             xtl::xoptional<xt::xtensor<double, 4>, bool> DS;
             xtl::xoptional<xt::xtensor<double, 4>, bool> AS;
             // > Intervals-based
             xtl::xoptional<xt::xtensor<double, 5>, bool> CR;
             xtl::xoptional<xt::xtensor<double, 5>, bool> AW;
             xtl::xoptional<xt::xtensor<double, 5>, bool> AWN;
-            xtl::xoptional<xt::xtensor<double, 5>, bool> AWI;
             xtl::xoptional<xt::xtensor<double, 5>, bool> WS;
-            xtl::xoptional<xt::xtensor<double, 5>, bool> WSS;
             // > Multi-variate
             xtl::xoptional<xt::xtensor<double, 4>, bool> ES;
 
             // methods to get optional parameters
             auto get_q_thr()
             {
                 if (_q_thr.size() < 1)
@@ -363,27 +360,14 @@
                     itv_width = elements::calc_itv_width(
                             get_itv_bnds()
                     );
                 }
                 return itv_width.value();
             };
 
-
-            xt::xtensor<double, 6> get_clim_bnds()
-            {
-                if (!clim_bnds.has_value())
-                {
-                    clim_bnds = elements::calc_clim_bnds(
-                            q_obs, get_c_lvl(), t_msk, b_exp,
-                            n_sit, n_ldt, n_itv, n_msk, n_exp
-                    );
-                }
-                return clim_bnds.value();
-            };
-
             // methods to compute intermediate metrics
             xt::xtensor<double, 4> get_bs()
             {
                 if (!bs.has_value())
                 {
                     bs = intermediate::calc_bs(
                             get_o_k(), get_y_k()
@@ -794,49 +778,26 @@
                             q_obs, get_AW(), t_msk, b_exp,
                             n_sit, n_ldt, n_msk, n_exp
                     );
                 }
                 return AWN.value();
             };
 
-            xt::xtensor<double, 5> get_AWI()
-            {
-                if (!AWI.has_value())
-                {
-                    AWI = metrics::calc_AWI(
-                            get_AW(), get_clim_bnds()
-                    );
-                }
-                return AWI.value();
-            };
-
             xt::xtensor<double, 5> get_WS()
             {
                 if (!WS.has_value())
                 {
                     WS = metrics::calc_WS(
                             get_ws(), t_msk, b_exp,
                             n_sit, n_ldt, n_itv, n_msk, n_exp
                     );
                 }
                 return WS.value();
             };
 
-            xt::xtensor<double, 5> get_WSS()
-            {
-                if (!WSS.has_value())
-                {
-                    WSS = metrics::calc_WSS(
-                            q_obs, get_c_lvl(), get_clim_bnds(), get_WS(),
-                            t_msk, b_exp, n_sit, n_ldt, n_itv, n_msk, n_exp
-                    );
-                }
-                return WSS.value();
-            };
-
             xt::xtensor<double, 4> get_ES()
             {
                 if (!ES.has_value())
                 {
                     ES = metrics::calc_ES(
                             get_es(), t_msk, b_exp, n_ldt, n_msk, n_exp
                     );
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/intervals.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/intervals.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -119,127 +119,14 @@
                 // https://doi.org/10.1198/016214506000001437
 
                 auto l = xt::view(itv_bnds, xt::all(), xt::all(), xt::all(), 0, xt::all());
                 auto u = xt::view(itv_bnds, xt::all(), xt::all(), xt::all(), 1, xt::all());
 
                 return (u - l);
             }
-
-            /// Compute the bounds of the climatology corresponding to the
-            /// confidence levels.
-            ///
-            /// \param q_obs
-            ///     Streamflow predictions.
-            ///     shape: (sites, time)
-            /// \param c_lvl
-            ///     Confidence levels for the predictive intervals.
-            ///     shape: (intervals,)
-            /// \param t_msk
-            ///     Temporal subsets of the whole record.
-            ///     shape: (sites, lead times, subsets, time)
-            /// \param b_exp
-            ///     Boostrap samples.
-            ///     shape: (samples, time slice)
-            /// \param n_sit
-            ///     Number of sites.
-            /// \param n_ldt
-            ///     Number of lead times.
-            /// \param n_itv
-            ///     Number of predictive intervals.
-            /// \param n_msk
-            ///     Number of temporal subsets.
-            /// \param n_exp
-            ///     Number of bootstrap samples.
-            /// \return
-            ///     Climatology bounds.
-            ///     shape: (sites, lead times, subsets, samples, intervals, bounds)
-            template <class XD2>
-            inline xt::xtensor<double, 6> calc_clim_bnds(
-                    const XD2& q_obs,
-                    const xt::xtensor<double, 1>& c_lvl,
-                    const xt::xtensor<bool, 4>& t_msk,
-                    const std::vector<xt::xkeep_slice<int>>& b_exp,
-                    std::size_t n_sit,
-                    std::size_t n_ldt,
-                    std::size_t n_itv,
-                    std::size_t n_msk,
-                    std::size_t n_exp
-            )
-            {
-                // compute "climatology" average width
-                xt::xtensor<double, 6> clim_bnds =
-                        xt::zeros<double>({n_sit, n_ldt, n_msk, n_exp,
-                                           n_itv, std::size_t {2}});
-
-                // determine quantiles forming the predictive intervals
-                // from the confidence levels
-                xt::xtensor<double, 2> quantiles =
-                        xt::zeros<double>({n_itv, std::size_t {2}});
-                xt::col(quantiles, 0) = 0.5 - c_lvl / 200.;
-                xt::col(quantiles, 1) = 0.5 + c_lvl / 200.;
-
-                // compute variable one mask at a time to minimise memory imprint
-                for (std::size_t m = 0; m < n_msk; m++)
-                {
-                    // apply the mask
-                    // (using NaN workaround until reducers work on masked_view)
-                    auto q_obs_masked = xt::where(
-                            xt::view(t_msk, xt::all(), xt::all(), m, xt::all()),
-                            xt::view(q_obs, xt::all(), xt::newaxis(), xt::all()),
-                            NAN
-                    );
-
-                    // compute variable one sample at a time
-                    for (std::size_t e = 0; e < n_exp; e++)
-                    {
-                        // apply the bootstrap sampling
-                        auto q_obs_masked_sampled =
-                                xt::view(q_obs_masked, xt::all(), xt::all(), b_exp[e]);
-
-                        // compute "climatology" interval
-                        for (std::size_t s = 0; s < n_sit; s++)
-                        {
-                            for (std::size_t l = 0; l < n_ldt; l++)
-                            {
-                                for (std::size_t i = 0; i < n_itv; i++)
-                                {
-                                    auto obs = xt::view(q_obs_masked_sampled,
-                                                        s, l, xt::all());
-                                    auto obs_filtered =
-                                            xt::filter(obs, !xt::isnan(obs));
-
-                                    if (obs_filtered.size() > 0)
-                                    {
-                                        // lower bound
-                                        xt::view(clim_bnds, s, l, m, e, i, 0) =
-                                                xt::quantile(
-                                                        obs_filtered,
-                                                        {quantiles(i, 0)}
-                                                )();
-                                        // upper bound
-                                        xt::view(clim_bnds, s, l, m, e, i, 1) =
-                                                xt::quantile(
-                                                        obs_filtered,
-                                                        {quantiles(i, 1)}
-                                                )();
-                                    }
-                                    else
-                                    {
-                                        xt::view(clim_bnds, s, l, m, e, i, xt::all()) =
-                                                NAN;
-                                    }
-
-                                }
-                            }
-                        }
-                    }
-                }
-
-                return clim_bnds;
-            }
         }
 
         namespace intermediate
         {
             /// Compute the Winkler score for each time step.
             ///
             /// \param q_obs
@@ -483,42 +370,14 @@
                 }
 
                 return xt::where(mean_obs > 0,
                                  AW / mean_obs,
                                  - std::numeric_limits<double>::infinity());
             }
 
-            /// Compute the Average Width Index (AWI).
-            ///
-            /// \param AW
-            ///     Average widths.
-            ///     shape: (sites, lead times, subsets, samples, intervals)
-            /// \param clim_bnds
-            ///     Climatology bounds.
-            ///     shape: (sites, lead times, subsets, samples, intervals, bounds)
-            /// \return
-            ///     Average width indices.
-            ///     shape: (sites, lead times, subsets, samples, intervals)
-            inline xt::xtensor<double, 5> calc_AWI(
-                    const xt::xtensor<double, 5>& AW,
-                    const xt::xtensor<double, 6>& clim_bnds
-            )
-            {
-                // compute "climatology" average width
-                auto AW_clim =
-                        xt::view(clim_bnds, xt::all(), xt::all(), xt::all(),
-                                 xt::all(), xt::all(), 1)
-                        - xt::view(clim_bnds, xt::all(), xt::all(), xt::all(),
-                                   xt::all(), xt::all(), 0);
-
-                return xt::where(AW_clim > 0,
-                                 1 - (AW / AW_clim),
-                                 - std::numeric_limits<double>::infinity());
-            }
-
             /// Compute the Winkler scores (WS), also known as interval score.
             ///
             /// \param ws
             ///     Winkler scores for each time step.
             ///     shape: (sites, lead times, intervals, time)
             /// \param t_msk
             ///     Temporal subsets of the whole record.
@@ -550,101 +409,12 @@
                     std::size_t n_exp
             )
             {
                 return detail::calc_METRIC_from_metric(
                         ws, t_msk, b_exp, n_sit, n_ldt, n_itv, n_msk, n_exp
                 );
             }
-
-            /// Compute the Winkler skill scores (WSS).
-            ///
-            /// \param q_obs
-            ///     Streamflow predictions.
-            ///     shape: (sites, time)
-            /// \param c_lvl
-            ///     Confidence levels for the predictive intervals.
-            ///     shape: (intervals,)
-            /// \param clim_bnds
-            ///     Climatology bounds.
-            ///     shape: (sites, lead times, subsets, samples, intervals, bounds)
-            /// \param WS
-            ///     Winkler scores.
-            ///     shape: (sites, lead times, subsets, samples, intervals)
-            /// \param t_msk
-            ///     Temporal subsets of the whole record.
-            ///     shape: (sites, lead times, subsets, time)
-            /// \param b_exp
-            ///     Boostrap samples.
-            ///     shape: (samples, time slice)
-            /// \param n_sit
-            ///     Number of sites.
-            /// \param n_ldt
-            ///     Number of lead times.
-            /// \param n_itv
-            ///     Number of predictive intervals.
-            /// \param n_msk
-            ///     Number of temporal subsets.
-            /// \param n_exp
-            ///     Number of bootstrap samples.
-            /// \return
-            ///     Winkler skill scores.
-            ///     shape: (sites, lead times, subsets, samples, intervals)
-            template <class XD2>
-            inline xt::xtensor<double, 5> calc_WSS(
-                    const XD2& q_obs,
-                    const xt::xtensor<double, 1>& c_lvl,
-                    const xt::xtensor<double, 6>& clim_bnds,
-                    const xt::xtensor<double, 5>& WS,
-                    const xt::xtensor<bool, 4>& t_msk,
-                    const std::vector<xt::xkeep_slice<int>>& b_exp,
-                    std::size_t n_sit,
-                    std::size_t n_ldt,
-                    std::size_t n_itv,
-                    std::size_t n_msk,
-                    std::size_t n_exp
-            )
-            {
-                // compute "climatology" Winkler score
-                xt::xtensor<double, 5> WS_clim =
-                        xt::zeros<double>({n_sit, n_ldt, n_msk, n_exp, n_itv});
-
-                for (std::size_t l = 0; l < n_ldt; l++)
-                {
-                    for (std::size_t m = 0; m < n_msk; m++)
-                    {
-                        for (std::size_t e = 0; e < n_exp; e++)
-                        {
-                            auto ws_clim = intermediate::calc_ws(
-                                    q_obs, c_lvl,
-                                    xt::view(clim_bnds, xt::all(), l, xt::newaxis(),
-                                             m, e, xt::all(), xt::all(),
-                                             xt::newaxis())
-                            );
-
-                            // apply the mask
-                            // (using NaN workaround until reducers work on masked_view)
-                            auto ws_clim_masked = xt::where(
-                                    xt::view(t_msk, xt::all(), l, m, xt::newaxis(), xt::all()),
-                                    xt::view(ws_clim, xt::all(), l, xt::all(), xt::all()),
-                                    NAN
-                            );
-
-                            // apply the bootstrap sampling
-                            auto ws_clim_masked_sampled =
-                                    xt::view(ws_clim_masked, xt::all(), xt::all(), b_exp[e]);
-
-                            xt::view(WS_clim, xt::all(), l, m, e, xt::all()) =
-                                    xt::nanmean(ws_clim_masked_sampled, -1);
-                        }
-                    }
-                }
-
-                // compute the Winkler skill score
-                return xt::where(WS_clim > 0,
-                                 1 - (WS / WS_clim),
-                                 - std::numeric_limits<double>::infinity());
-            }
         }
     }
 }
 
 #endif //EVALHYD_PROBABILIST_INTERVALS_HPP
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/multivariate.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/multivariate.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/quantiles.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/quantiles.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/ranks.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/probabilist/ranks.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
                     std::size_t n_ldt,
                     std::size_t n_mbr,
                     std::size_t n_msk,
                     std::size_t n_exp
             )
             {
                 // initialise output variable
-                xt::xtensor<double, 5> REL_DIAG =
+                xt::xtensor<double, 5> RANK_HIST =
                         xt::zeros<double>({n_sit, n_ldt, n_msk, n_exp, n_mbr + 1});
 
                 // compute variable one mask at a time to minimise memory imprint
                 for (std::size_t m = 0; m < n_msk; m++)
                 {
                     // compute variable one sample at a time
                     for (std::size_t e = 0; e < n_exp; e++)
@@ -242,23 +242,23 @@
 
                         // calculate length of subset
                         auto l = xt::eval(
                                 xt::sum(t_msk_sampled, -1, xt::keep_dims)
                         );
 
                         // compute the rank diagram
-                        xt::view(REL_DIAG, xt::all(), xt::all(), m, e, xt::all()) =
+                        xt::view(RANK_HIST, xt::all(), xt::all(), m, e, xt::all()) =
                                 xt::view(o_j, xt::all(), xt::all(),
                                          m, e, xt::all())
                                 / l
                         ;
                     }
                 }
 
-                return REL_DIAG;
+                return RANK_HIST;
             }
 
             /// Compute the Delta score.
             ///
             /// \param o_j
             ///     Tallies of streamflow observations for all possible ranks.
             ///     shape: (sites, lead times, subsets, samples, ranks)
@@ -445,8 +445,8 @@
 
                 return AS;
             }
         }
     }
 }
 
-#endif //EVALHYD_PROBABILIST_RANKS_HPP
+#endif //EVALHYD_PROBABILIST_RANKS_HPP
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/uncertainty.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/uncertainty.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,24 @@
                 }
             }
 
             // identify start and end years for period
             int start_yr = v_tm.front().tm_year + 1900;
             int end_yr = v_tm.back().tm_year + 1900;
 
-            // assume start of year block as start of time series
+            // deal with special case with a start on 1st of January
+            // (note: use string rather than *tm_yday* member of time_point
+            //  because *tm_yday* is not set when using `std::get_time`)
+            if (datetimes[0].substr(5, 5) == "01-01")
+            {
+                // add one year to make sure last year is included in loop
+                end_yr += 1;
+            }
+
+            // take start of year block as start of time series
             std::tm start_hy = v_tm.front();
 
             xt::xtensor<int, 1> year_blocks = xt::zeros<int>({v_tm.size()});
             for (int y = start_yr; y < end_yr; y++)
             {
                 // define window for year blocks
                 start_hy.tm_year = y - 1900;
@@ -96,15 +105,15 @@
                         (x_timepoints >= start) && (x_timepoints < end);
 
                 // check that year is complete (without a rigorous leap year check)
                 int n_days = xt::sum(wdw)();
                 if ((n_days != 365) && (n_days != 366))
                 {
                     throw std::runtime_error(
-                            "year starting in " + std::to_string(y)
+                            "year starting in " + std::to_string(y - 400)
                             + " is incomplete"
                     );
                 }
 
                 // determine corresponding year block for each time step
                 year_blocks = xt::where(wdw, y, year_blocks);
             }
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/detail/utils.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/detail/utils.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/evald.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/evald.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -206,27 +206,33 @@
             const std::vector<std::string>& dts = {},
             xtl::xoptional<const int, bool> seed =
                     xtl::missing<const int>(),
             xtl::xoptional<const std::vector<std::string>, bool> diagnostics =
                     xtl::missing<const std::vector<std::string>>()
     )
     {
-        // check ranks of tensors
-        if (xt::get_rank<XD2>::value != 2)
+        // check ranks of expressions if they are tensors
+        if (xt::get_rank<XD2>::value != SIZE_MAX)
         {
-            throw std::runtime_error(
-                    "observations and/or predictions and/or thresholds "
-                    "are not two-dimensional"
-            );
+            if (xt::get_rank<XD2>::value != 2)
+            {
+                throw std::runtime_error(
+                        "observations and/or predictions and/or thresholds "
+                        "are not two-dimensional"
+                );
+            }
         }
-        if (xt::get_rank<XB3>::value != 3)
+        if (xt::get_rank<XB3>::value != SIZE_MAX)
         {
-            throw std::runtime_error(
-                    "temporal masks are not three-dimensional"
-            );
+            if (xt::get_rank<XB3>::value != 3)
+            {
+                throw std::runtime_error(
+                        "temporal masks are not three-dimensional"
+                );
+            }
         }
 
         // retrieve real types of the expressions
         const XD2& q_obs_ = q_obs.derived_cast();
         const XD2& q_prd_ = q_prd.derived_cast();
         const XD2& q_thr_ = q_thr.derived_cast();
 
@@ -362,15 +368,15 @@
                     }
                 }
 
                 return c_msk;
             }
             else
             {
-                return XB3({});
+                return XB3(xt::zeros<bool>({0, 0, 0}));
             }
         };
         const XB3 c_msk = gen_msk();
 
         // apply streamflow transformation if requested
         auto q_transform = [&](const XD2& q)
         {
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/include/evalhyd/evalp.hpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/include/evalhyd/evalp.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     ///
     ///       xt::xtensor<bool, 3> msk = {{{ false, true, true, false, true }}};
     ///
     ///       evalhyd::evalp(obs, prd, {"BS"}, thr, msk);
     ///
     ///    .. code-block:: c++
     ///
-    ///       evalhyd::evalp(obs, prd, {"CRPS"});
+    ///       evalhyd::evalp(obs, prd, {"CRPS_FROM_QS"});
     ///
     /// \endrst
     template <class XD2, class XD4, class XB4 = xt::xtensor<bool, 4>,
               class XS2 = xt::xtensor<std::array<char, 32>, 2>>
     std::vector<xt::xarray<double>> evalp(
             const xt::xexpression<XD2>& q_obs,
             const xt::xexpression<XD4>& q_prd,
@@ -186,32 +186,43 @@
             const std::vector<std::string>& dts = {},
             xtl::xoptional<const int, bool> seed =
                     xtl::missing<const int>(),
             xtl::xoptional<const std::vector<std::string>, bool> diagnostics =
                     xtl::missing<const std::vector<std::string>>()
     )
     {
-        // check ranks of tensors
-        if (xt::get_rank<XD2>::value != 2)
+        // check ranks of expressions if they are tensors
+        if (xt::get_rank<XD2>::value != SIZE_MAX)
         {
-            throw std::runtime_error(
-                    "observations and/or thresholds are not two-dimensional"
-            );
+            if (xt::get_rank<XD2>::value != 2)
+            {
+                throw std::runtime_error(
+                        "observations and/or thresholds are not two-dimensional"
+                );
+            }
         }
-        if (xt::get_rank<XD4>::value != 4)
+
+        if (xt::get_rank<XD4>::value != SIZE_MAX)
         {
-            throw std::runtime_error(
-                    "predictions are not four-dimensional"
-            );
+            if (xt::get_rank<XD4>::value != 4)
+            {
+                throw std::runtime_error(
+                        "predictions are not four-dimensional"
+                );
+            }
         }
-        if (xt::get_rank<XB4>::value != 4)
+
+        if (xt::get_rank<XB4>::value != SIZE_MAX)
         {
-            throw std::runtime_error(
-                    "temporal masks are not four-dimensional"
-            );
+            if (xt::get_rank<XB4>::value != 4)
+            {
+                throw std::runtime_error(
+                        "temporal masks are not four-dimensional"
+                );
+            }
         }
 
         // retrieve real types of the expressions
         const XD2& q_obs_ = q_obs.derived_cast();
         const XD4& q_prd_ = q_prd.derived_cast();
         const XD2& q_thr_ = q_thr.derived_cast();
 
@@ -225,15 +236,15 @@
         utils::check_metrics(
                 metrics,
                 {"BS", "BSS", "BS_CRD", "BS_LBD", "REL_DIAG", "CRPS_FROM_BS",
                  "CRPS_FROM_ECDF",
                  "QS", "CRPS_FROM_QS",
                  "POD", "POFD", "FAR", "CSI", "ROCSS",
                  "RANK_HIST", "DS", "AS",
-                 "CR", "AW", "AWN", "AWI", "WS", "WSS",
+                 "CR", "AW", "AWN", "WS",
                  "ES"}
         );
 
         if ( diagnostics.has_value() )
         {
             utils::check_diags(
                     diagnostics.value(),
@@ -364,15 +375,15 @@
                     }
                 }
 
                 return c_msk;
             }
             else
             {
-                return XB4({});
+                return XB4(xt::zeros<bool>({0, 0, 0, 0}));
             }
         };
         const XB4 c_msk = gen_msk();
 
         // generate bootstrap experiment if requested
         std::vector<xt::xkeep_slice<int>> b_exp;
         int summary;
@@ -532,32 +543,20 @@
             }
             else if ( metric == "AWN" )
             {
                 r.emplace_back(
                         uncertainty::summarise_p(evaluator.get_AWN(), summary)
                 );
             }
-            else if ( metric == "AWI" )
-            {
-                r.emplace_back(
-                        uncertainty::summarise_p(evaluator.get_AWI(), summary)
-                );
-            }
             else if ( metric == "WS" )
             {
                 r.emplace_back(
                         uncertainty::summarise_p(evaluator.get_WS(), summary)
                 );
             }
-            else if ( metric == "WSS" )
-            {
-                r.emplace_back(
-                        uncertainty::summarise_p(evaluator.get_WSS(), summary)
-                );
-            }
             else if ( metric == "ES" )
             {
                 r.emplace_back(
                         uncertainty::summarise_p(evaluator.get_ES(), summary)
                 );
             }
         }
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/q_obs.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/q_obs.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/q_obs_1yr.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/q_obs_1yr.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/q_prd.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/q_prd.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/data/q_prd_1yr.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/data/q_prd_1yr.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/CONT_TBL.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/CONT_TBL.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/KGE.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/KGE.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/KGEPRIME.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/KGEPRIME.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/KGEPRIME_D.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/KGEPRIME_D.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/KGE_D.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/KGE_D.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/MAE.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/MAE.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/MARE.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/MARE.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/MSE.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/MSE.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/NSE.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/NSE.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evald/RMSE.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evald/RMSE.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/CSI.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/CSI.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/FAR.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/FAR.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/POD.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/POD.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/POFD.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/POFD.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/QS.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/QS.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/RANK_HIST.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/RANK_HIST.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/expected/evalp/REL_DIAG.csv` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/expected/evalp/REL_DIAG.csv`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/test_determinist.cpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/test_determinist.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/test_probabilist.cpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/test_probabilist.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 std::vector<std::string> all_metrics_p = {
         "BS", "BSS", "BS_CRD", "BS_LBD", "REL_DIAG", "CRPS_FROM_BS",
         "CRPS_FROM_ECDF",
         "QS", "CRPS_FROM_QS",
         "POD", "POFD", "FAR", "CSI", "ROCSS",
         "RANK_HIST", "DS", "AS",
-        "CR", "AW", "AWN", "AWI", "WS", "WSS",
+        "CR", "AW", "AWN", "WS",
         "ES"
 };
 
 std::tuple<xt::xtensor<double, 1>, xt::xtensor<double, 2>> load_data_p()
 {
     // read in data
     std::ifstream ifs;
@@ -259,23 +259,23 @@
     xt::xtensor<double, 2> predicted;
     std::tie(observed, predicted) = load_data_p();
 
     // read in expected results
     auto expected = load_expected_p();
 
     // compute scores
-    std::vector<std::string> metrics = {"CR", "AW", "AWN", "AWI", "WS", "WSS"};
+    std::vector<std::string> metrics = {"CR", "AW", "AWN", "WS"};
 
     std::vector<xt::xarray<double>> results =
             evalhyd::evalp(
                     // shape: (sites [1], time [t])
                     xt::eval(xt::view(observed, xt::newaxis(), xt::all())),
                     // shape: (sites [1], lead times [1], members [m], time [t])
                     xt::eval(xt::view(predicted, xt::newaxis(), xt::newaxis(), xt::all(), xt::all())),
-                    {"CR", "AW", "AWN", "AWI", "WS", "WSS"},
+                    {"CR", "AW", "AWN", "WS"},
                     xt::xtensor<double, 2>({}),
                     "",  // events
                     {30., 80.}  // c_lvl
             );
 
     // check results
     for (std::size_t m = 0; m < metrics.size(); m++)
```

### Comparing `evalhyd-python-0.1.0.0/deps/evalhyd-cpp/tests/test_uncertainty.cpp` & `evalhyd-python-0.1.1.0/deps/evalhyd-cpp/tests/test_uncertainty.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.appveyor.yml` & `evalhyd-python-0.1.1.0/deps/xtensor/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/azure-pipelines-linux-clang.yml` & `evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/azure-pipelines-linux-clang.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/azure-pipelines-linux-gcc.yml` & `evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/azure-pipelines-linux-gcc.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/azure-pipelines-osx.yml` & `evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/azure-pipelines-osx.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/azure-pipelines-win.yml` & `evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/azure-pipelines-win.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.azure-pipelines/unix-build.yml` & `evalhyd-python-0.1.1.0/deps/xtensor/.azure-pipelines/unix-build.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.clang-format` & `evalhyd-python-0.1.1.0/deps/xtensor/.clang-format`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.github/workflows/gh-pages.yml` & `evalhyd-python-0.1.1.0/deps/xtensor/.github/workflows/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.gitignore` & `evalhyd-python-0.1.1.0/deps/xtensor/.gitignore`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/.pre-commit-config.yaml` & `evalhyd-python-0.1.1.0/deps/xtensor/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/README.md` & `evalhyd-python-0.1.1.0/deps/xtensor/README.md`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_adapter.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_adapter.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_assign.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_assign.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_builder.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_builder.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_container.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_container.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_creation.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_creation.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_increment_stepper.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_increment_stepper.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_lambda_expressions.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_lambda_expressions.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_math.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_math.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_random.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_random.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_reducer.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_reducer.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_view_access.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_view_access.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_view_adapt.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_view_adapt.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_view_assignment.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_view_assignment.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_views.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_views.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/benchmark_xshape.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/benchmark_xshape.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/copyGBenchmark.cmake.in` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/copyGBenchmark.cmake.in`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/downloadGBenchmark.cmake.in` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/downloadGBenchmark.cmake.in`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/benchmark/main.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/benchmark/main.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/cmake/FindTBB.cmake` & `evalhyd-python-0.1.1.0/deps/xtensor/cmake/FindTBB.cmake`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/make.bat` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/make.bat`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/adaptor.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/adaptor.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/accumulating_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/accumulating_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/basic_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/basic_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/classif_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/classif_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/container_index.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/container_index.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/exponential_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/exponential_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/expression_index.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/expression_index.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/hyperbolic_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/hyperbolic_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/nan_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/nan_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/nearint_operations.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/nearint_operations.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/operators.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/operators.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/power_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/power_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/reducing_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/reducing_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/trigonometric_functions.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/trigonometric_functions.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xaxis_iterator.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xaxis_iterator.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xaxis_slice_iterator.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xaxis_slice_iterator.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xbuilder.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xbuilder.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xcontainer.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xcontainer.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xhistogram.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xhistogram.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xio.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xio.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xmath.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xmath.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xnpy.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xnpy.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xpad.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xpad.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xrandom.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xrandom.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xset_operation.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xset_operation.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xstrided_view.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xstrided_view.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xtensor.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xtensor.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/api/xview.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/api/xview.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/binder-logo.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/binder-logo.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/bindings.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/bindings.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/build-options.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/build-options.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/builder.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/builder.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/changelog.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/closure-semantics.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/closure-semantics.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/cmake.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/cmake.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/compilers.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/compilers.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/conda.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/conda.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/conf.py` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/container.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/container.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/debian.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/debian.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/dev-build-options.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/dev-build-options.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/assign_xexpression.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/assign_xexpression.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/assignment.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/assignment.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/computed_assign.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/computed_assign.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/concepts.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/concepts.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/expression_tree.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/expression_tree.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/extended_copy_semantic.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/extended_copy_semantic.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/implementation_classes.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/implementation_classes.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/iterating_expression.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/iterating_expression.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/iteration.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/iteration.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/stepper_basic.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/stepper_basic.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/stepper_broadcasting.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/stepper_broadcasting.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/stepper_iterating.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/stepper_iterating.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/stepper_to_end.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/stepper_to_end.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xarray_uml.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xarray_uml.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xcontainer_classes.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xcontainer_classes.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xfunction_tree.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xfunction_tree.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xsemantic_classes.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xsemantic_classes.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/developer/xtensor_internals.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/developer/xtensor_internals.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/expression.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/expression.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/external-structures.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/external-structures.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/file_loading.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/file_loading.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/getting_started.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/histogram.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/histogram.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/index.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/indices.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/indices.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/installation.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/missing.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/missing.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/numpy-differences.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/numpy-differences.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/numpy.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/numpy.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/numpy.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/numpy.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/operator.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/operator.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/pitfall.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/pitfall.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quantstack-white.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quantstack-white.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/basic.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/basic.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/builder.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/builder.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/chunked_arrays.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/chunked_arrays.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/iterator.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/iterator.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/manipulation.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/manipulation.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/math.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/math.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/operator.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/operator.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/quickref/reducer.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/quickref/reducer.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/random.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/random.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/rank.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/rank.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/related.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/related.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/releasing.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/releasing.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/scalar.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/scalar.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/spack.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/spack.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/view.rst` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/view.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xeus-cling-screenshot.png` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xeus-cling-screenshot.png`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xframe.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xframe.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xsimd-small.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xsimd-small.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xsimd.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xsimd.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-blas-small.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-blas-small.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-blas.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-blas.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-cookiecutter.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-cookiecutter.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-fftw.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-fftw.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-io-small.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-io-small.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-io.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-io.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-julia-small.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-julia-small.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-julia.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-julia.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-python-small.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-python-small.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-python.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-python.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-r-small.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-r-small.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-r.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-r.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor-ros.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor-ros.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtensor.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtensor.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/docs/source/xtl.svg` & `evalhyd-python-0.1.1.0/deps/xtensor/docs/source/xtl.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xaccessible.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xaccessible.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xaccumulator.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xaccumulator.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xadapt.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xadapt.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xarray.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xarray.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xassign.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xassign.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xaxis_iterator.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xaxis_iterator.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xaxis_slice_iterator.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xaxis_slice_iterator.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xblockwise_reducer.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xblockwise_reducer.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xblockwise_reducer_functors.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xblockwise_reducer_functors.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xbroadcast.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xbroadcast.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xbuffer_adaptor.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xbuffer_adaptor.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xbuilder.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xbuilder.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xchunked_array.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xchunked_array.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xchunked_assign.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xchunked_assign.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xchunked_view.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xchunked_view.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xcomplex.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xcomplex.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xcontainer.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xcontainer.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xcsv.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xcsv.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xdynamic_view.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xdynamic_view.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xeval.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xeval.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xexception.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xexception.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xexpression.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xexpression.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xexpression_holder.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xexpression_holder.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xexpression_traits.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xexpression_traits.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xfixed.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xfixed.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xfunction.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xfunction.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xfunctor_view.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xfunctor_view.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xgenerator.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xgenerator.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xhistogram.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xhistogram.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xindex_view.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xindex_view.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xinfo.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xinfo.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xio.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xio.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xiterable.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xiterable.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xiterator.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xiterator.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xjson.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xjson.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xlayout.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xlayout.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmanipulation.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmanipulation.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmasked_view.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmasked_view.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmath.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmath.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmime.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmime.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xmultiindex_iterator.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xmultiindex_iterator.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xnoalias.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xnoalias.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xnorm.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xnorm.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xnpy.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xnpy.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoffset_view.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoffset_view.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoperation.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoperation.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoptional.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoptional.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoptional_assembly.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoptional_assembly.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoptional_assembly_base.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoptional_assembly_base.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xoptional_assembly_storage.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xoptional_assembly_storage.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xpad.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xpad.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xrandom.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xrandom.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xreducer.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xreducer.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xrepeat.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xrepeat.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xscalar.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xscalar.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xsemantic.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xsemantic.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xset_operation.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xset_operation.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xshape.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xshape.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xslice.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xslice.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xsort.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xsort.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xstorage.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xstorage.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xstrided_view.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xstrided_view.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xstrided_view_base.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xstrided_view_base.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xstrides.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xstrides.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xtensor.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xtensor.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xtensor_config.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xtensor_config.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xtensor_forward.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xtensor_forward.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xtensor_simd.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xtensor_simd.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xutils.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xutils.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xvectorize.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xvectorize.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xview.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xview.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/include/xtensor/xview_utils.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/include/xtensor/xview_utils.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/notebooks/images/xtensor-blas.png` & `evalhyd-python-0.1.1.0/deps/xtensor/notebooks/images/xtensor-blas.png`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/notebooks/images/xtensor.png` & `evalhyd-python-0.1.1.0/deps/xtensor/notebooks/images/xtensor.png`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/notebooks/xtensor.ipynb` & `evalhyd-python-0.1.1.0/deps/xtensor/notebooks/xtensor.ipynb`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_broadcast_view.cppy` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_broadcast_view.cppy`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_xhistogram.cppy` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_xhistogram.cppy`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_xmath_interp.cppy` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_xmath_interp.cppy`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_xmath_reducers.cppy` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_xmath_reducers.cppy`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/cppy_source/test_extended_xsort.cppy` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/cppy_source/test_extended_xsort.cppy`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/preprocess.py` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/preprocess.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/complex_numbers.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/complex_numbers.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/complex_zero_erasing.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/complex_zero_erasing.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/cut_4d.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/cut_4d.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/float_leading_zero.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/float_leading_zero.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/print_options_result.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/print_options_result.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results/random_nan_inf.txt` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results/random_nan_inf.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/files/xio_expected_results.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/files/xio_expected_results.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/set_compiler_flag.cmake` & `evalhyd-python-0.1.1.0/deps/xtensor/test/set_compiler_flag.cmake`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_common.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_common.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_common_macros.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_common_macros.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_broadcast_view.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_broadcast_view.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_xhistogram.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_xhistogram.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_xmath_interp.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_xmath_interp.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_xmath_reducers.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_xmath_reducers.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_extended_xsort.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_extended_xsort.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_sfinae.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_sfinae.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_strided_assign.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_strided_assign.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_utils.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_utils.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xaccumulator.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xaccumulator.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xadapt.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xadapt.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xadaptor_semantic.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xadaptor_semantic.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xarray.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xarray.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xarray_adaptor.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xarray_adaptor.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xassign.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xassign.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xaxis_iterator.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xaxis_iterator.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xaxis_slice_iterator.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xaxis_slice_iterator.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xblockwise_reducer.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xblockwise_reducer.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xbroadcast.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xbroadcast.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xbuffer_adaptor.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xbuffer_adaptor.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xbuilder.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xbuilder.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xchunked_array.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xchunked_array.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xchunked_view.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xchunked_view.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xcomplex.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xcomplex.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xcontainer_semantic.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xcontainer_semantic.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xcsv.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xcsv.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xdatesupport.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xdatesupport.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xdynamic_view.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xdynamic_view.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xeval.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xeval.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xexception.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xexception.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xexpression.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xexpression.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xexpression_holder.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xexpression_holder.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xexpression_traits.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xexpression_traits.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xfixed.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xfixed.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xfunc_on_xexpression.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xfunc_on_xexpression.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xfunction.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xfunction.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xfunctor_adaptor.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xfunctor_adaptor.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xhistogram.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xhistogram.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xindex_view.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xindex_view.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xinfo.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xinfo.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xio.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xio.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xiterator.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xiterator.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xjson.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xjson.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xlayout.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xlayout.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmanipulation.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmanipulation.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmasked_view.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmasked_view.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmath.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmath.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmath_result_type.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmath_result_type.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmime.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmime.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xmultiindex_iterator.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xmultiindex_iterator.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xnan_functions.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xnan_functions.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xnoalias.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xnoalias.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xnorm.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xnorm.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xnpy.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xnpy.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoperation.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoperation.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoptional.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoptional.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoptional_assembly.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoptional_assembly.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoptional_assembly_adaptor.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoptional_assembly_adaptor.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xoptional_assembly_storage.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xoptional_assembly_storage.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xpad.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xpad.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xrandom.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xrandom.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xreducer.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xreducer.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xrepeat.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xrepeat.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xscalar.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xscalar.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xscalar_semantic.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xscalar_semantic.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xsemantic.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xsemantic.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xset_operation.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xset_operation.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xshape.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xshape.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xsimd.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xsimd.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xsimd8.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xsimd8.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xsort.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xsort.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xstorage.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xstorage.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xstrided_view.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xstrided_view.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xstrides.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xstrides.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xtensor.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xtensor.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xtensor_adaptor.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xtensor_adaptor.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xtensor_semantic.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xtensor_semantic.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xutils.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xutils.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xvectorize.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xvectorize.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xview.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xview.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/test/test_xview_semantic.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor/test/test_xview_semantic.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/tools/check_circular.py` & `evalhyd-python-0.1.1.0/deps/xtensor/tools/check_circular.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor/xtensorConfig.cmake.in` & `evalhyd-python-0.1.1.0/deps/xtensor/xtensorConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/.appveyor.yml` & `evalhyd-python-0.1.1.0/deps/xtensor-python/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-linux-clang.yml` & `evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-linux-clang.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-linux-gcc.yml` & `evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-linux-gcc.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-osx.yml` & `evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/azure-pipelines-osx.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/.azure-pipelines/unix-build.yml` & `evalhyd-python-0.1.1.0/deps/xtensor-python/.azure-pipelines/unix-build.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/.gitignore` & `evalhyd-python-0.1.1.0/deps/xtensor-python/.gitignore`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtensor-python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/README.md` & `evalhyd-python-0.1.1.0/deps/xtensor-python/README.md`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/main.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/main.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/benchmark/setup.py` & `evalhyd-python-0.1.1.0/deps/xtensor-python/benchmark/setup.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/cmake/FindNumPy.cmake` & `evalhyd-python-0.1.1.0/deps/xtensor-python/cmake/FindNumPy.cmake`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/make.bat` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/array_tensor.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/array_tensor.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/basic_usage.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/cmake.svg` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/cmake.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/compilers.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/compilers.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/conda.svg` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/conda.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/conf.py` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/cookiecutter.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/cookiecutter.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/debian.svg` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/debian.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/dev_build_options.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/dev_build_options.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/copy_cast/main.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/copy_cast/main.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/sfinae/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/sfinae/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples/sfinae/mymodule.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples/sfinae/mymodule.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/examples.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/index.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/installation.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/numpy_capi.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/numpy_capi.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/quantstack-white.svg` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/quantstack-white.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/releasing.rst` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/releasing.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/docs/source/xtensor-python.svg` & `evalhyd-python-0.1.1.0/deps/xtensor-python/docs/source/xtensor-python.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pyarray.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pyarray.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pyarray_backstrides.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pyarray_backstrides.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pycontainer.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pycontainer.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pynative_casters.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pynative_casters.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pystrides_adaptor.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pystrides_adaptor.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pytensor.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pytensor.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/pyvectorize.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/pyvectorize.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/xtensor_python_config.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/xtensor_python_config.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/include/xtensor-python/xtensor_type_caster_base.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/include/xtensor-python/xtensor_type_caster_base.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/copyGTest.cmake.in` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/copyGTest.cmake.in`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/downloadGTest.cmake.in` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/downloadGTest.cmake.in`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/main.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/main.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_common.hpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_common.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_pyarray.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_pyarray.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_pyarray_traits.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_pyarray_traits.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_pytensor.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_pytensor.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_pyvectorize.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_pyvectorize.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test/test_sfinae.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test/test_sfinae.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test_python/main.cpp` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test_python/main.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test_python/setup.py` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test_python/setup.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/test_python/test_pyarray.py` & `evalhyd-python-0.1.1.0/deps/xtensor-python/test_python/test_pyarray.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtensor-python/xtensor-pythonConfig.cmake.in` & `evalhyd-python-0.1.1.0/deps/xtensor-python/xtensor-pythonConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/.appveyor.yml` & `evalhyd-python-0.1.1.0/deps/xtl/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/azure-pipelines-linux-clang.yml` & `evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/azure-pipelines-linux-clang.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/azure-pipelines-linux-gcc.yml` & `evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/azure-pipelines-linux-gcc.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/azure-pipelines-osx.yml` & `evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/azure-pipelines-osx.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/azure-pipelines-win.yml` & `evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/azure-pipelines-win.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/.azure-pipelines/unix-build.yml` & `evalhyd-python-0.1.1.0/deps/xtl/.azure-pipelines/unix-build.yml`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/.gitignore` & `evalhyd-python-0.1.1.0/deps/xtl/.gitignore`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/.releash.py` & `evalhyd-python-0.1.1.0/deps/xtl/.releash.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/README.md` & `evalhyd-python-0.1.1.0/deps/xtl/README.md`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/make.bat` & `evalhyd-python-0.1.1.0/deps/xtl/docs/make.bat`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/basic_types.rst` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/basic_types.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/build-options.rst` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/build-options.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/changelog.rst` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/cmake.svg` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/cmake.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/conda.svg` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/conda.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/conf.py` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/debian.svg` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/debian.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/index.rst` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/installation.rst` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/quantstack-white.svg` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/quantstack-white.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/releasing.rst` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/releasing.rst`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/spack.svg` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/spack.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/docs/source/xtl.svg` & `evalhyd-python-0.1.1.0/deps/xtl/docs/source/xtl.svg`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xany.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xany.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xbase64.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xbase64.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xbasic_fixed_string.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xbasic_fixed_string.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xclosure.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xclosure.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xcompare.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xcompare.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xcomplex.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xcomplex.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xcomplex_sequence.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xcomplex_sequence.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xdynamic_bitset.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xdynamic_bitset.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xfunctional.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xfunctional.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xhalf_float.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xhalf_float.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xhalf_float_impl.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xhalf_float_impl.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xhash.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xhash.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xhierarchy_generator.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xhierarchy_generator.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xiterator_base.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xiterator_base.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xjson.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xjson.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xmasked_value.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xmasked_value.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xmasked_value_meta.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xmasked_value_meta.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xmeta_utils.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xmeta_utils.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xmultimethods.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xmultimethods.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xoptional.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xoptional.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xoptional_meta.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xoptional_meta.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xoptional_sequence.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xoptional_sequence.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xplatform.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xplatform.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xproxy_wrapper.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xproxy_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xsequence.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xsequence.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xspan.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xspan.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xspan_impl.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xspan_impl.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xsystem.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xsystem.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xtl_config.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xtl_config.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xtype_traits.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xtype_traits.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xvariant.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xvariant.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xvariant_impl.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xvariant_impl.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/include/xtl/xvisitor.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/include/xtl/xvisitor.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/CMakeLists.txt` & `evalhyd-python-0.1.1.0/deps/xtl/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_common_macros.hpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_common_macros.hpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xbase64.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xbase64.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xbasic_fixed_string.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xbasic_fixed_string.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xclosure.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xclosure.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xcompare.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xcompare.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xcomplex.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xcomplex.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xcomplex_sequence.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xcomplex_sequence.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xdynamic_bitset.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xdynamic_bitset.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xfunctional.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xfunctional.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xhalf_float.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xhalf_float.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xhash.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xhash.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xhierarchy_generator.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xhierarchy_generator.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xiterator_base.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xiterator_base.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xmasked_value.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xmasked_value.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xmeta_utils.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xmeta_utils.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xmultimethods.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xmultimethods.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xoptional.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xoptional.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xplatform.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xplatform.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xproxy_wrapper.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xproxy_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xsequence.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xsequence.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xsystem.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xsystem.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xtype_traits.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xtype_traits.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xvariant.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xvariant.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/test/test_xvisitor.cpp` & `evalhyd-python-0.1.1.0/deps/xtl/test/test_xvisitor.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/deps/xtl/xtlConfig.cmake.in` & `evalhyd-python-0.1.1.0/deps/xtl/xtlConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/evalhyd/evald.py` & `evalhyd-python-0.1.1.0/evalhyd/evald.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/evalhyd/evalp.py` & `evalhyd-python-0.1.1.0/evalhyd/evalp.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/evalhyd/src/evalhyd.cpp` & `evalhyd-python-0.1.1.0/evalhyd/src/evalhyd.cpp`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/evalhyd_python.egg-info/PKG-INFO` & `evalhyd-python-0.1.1.0/evalhyd_python.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: evalhyd-python
-Version: 0.1.0.0
+Version: 0.1.1.0
 Summary: Python bindings for EvalHyd
 Download-URL: https://pypi.python.org/pypi/evalhyd-python
 Author: Thibault Hallouin
 Author-email: thibault.hallouin@inrae.fr
+License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.irstea.fr/HYCAR-Hydro/evalhyd/evalhyd-python/-/issues
 Project-URL: Documentation, https://hydrogr.github.io/evalhyd/python
 Project-URL: Source Code, https://gitlab.irstea.fr/hycar-hydro/evalhyd/evalhyd-python
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides-Extra: tests
 License-File: LICENCE.rst
 
 An evaluator for streamflow predictions.
```

### Comparing `evalhyd-python-0.1.0.0/evalhyd_python.egg-info/SOURCES.txt` & `evalhyd-python-0.1.1.0/evalhyd_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 deps/evalhyd-cpp/tests/expected/evald/MAE.csv
 deps/evalhyd-cpp/tests/expected/evald/MARE.csv
 deps/evalhyd-cpp/tests/expected/evald/MSE.csv
 deps/evalhyd-cpp/tests/expected/evald/NSE.csv
 deps/evalhyd-cpp/tests/expected/evald/RMSE.csv
 deps/evalhyd-cpp/tests/expected/evalp/AS.csv
 deps/evalhyd-cpp/tests/expected/evalp/AW.csv
-deps/evalhyd-cpp/tests/expected/evalp/AWI.csv
 deps/evalhyd-cpp/tests/expected/evalp/AWN.csv
 deps/evalhyd-cpp/tests/expected/evalp/BS.csv
 deps/evalhyd-cpp/tests/expected/evalp/BSS.csv
 deps/evalhyd-cpp/tests/expected/evalp/BS_CRD.csv
 deps/evalhyd-cpp/tests/expected/evalp/BS_LBD.csv
 deps/evalhyd-cpp/tests/expected/evalp/CR.csv
 deps/evalhyd-cpp/tests/expected/evalp/CRPS_FROM_BS.csv
@@ -69,15 +68,14 @@
 deps/evalhyd-cpp/tests/expected/evalp/POD.csv
 deps/evalhyd-cpp/tests/expected/evalp/POFD.csv
 deps/evalhyd-cpp/tests/expected/evalp/QS.csv
 deps/evalhyd-cpp/tests/expected/evalp/RANK_HIST.csv
 deps/evalhyd-cpp/tests/expected/evalp/REL_DIAG.csv
 deps/evalhyd-cpp/tests/expected/evalp/ROCSS.csv
 deps/evalhyd-cpp/tests/expected/evalp/WS.csv
-deps/evalhyd-cpp/tests/expected/evalp/WSS.csv
 deps/xtensor/.appveyor.yml
 deps/xtensor/.clang-format
 deps/xtensor/.git
 deps/xtensor/.gitignore
 deps/xtensor/.pre-commit-config.yaml
 deps/xtensor/CMakeLists.txt
 deps/xtensor/README.md
```

### Comparing `evalhyd-python-0.1.0.0/setup.py` & `evalhyd-python-0.1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,13 +48,20 @@
     project_urls={
         'Bug Tracker': 'https://gitlab.irstea.fr/HYCAR-Hydro/evalhyd/evalhyd-python/-/issues',
         'Documentation': 'https://hydrogr.github.io/evalhyd/python',
         'Source Code': 'https://gitlab.irstea.fr/hycar-hydro/evalhyd/evalhyd-python',
     },
     description='Python bindings for EvalHyd',
     long_description='An evaluator for streamflow predictions.',
+    license="GPLv3",
+    classifiers=[
+        'Natural Language :: English',
+        'Intended Audience :: Science/Research',
+        'Topic :: Scientific/Engineering :: Hydrology',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)'
+    ],
     packages=["evalhyd"],
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     extras_require={'tests': 'numpy>=1.16'},
     zip_safe=False,
 )
```

### Comparing `evalhyd-python-0.1.0.0/tests/test_determinist.py` & `evalhyd-python-0.1.1.0/tests/test_determinist.py`

 * *Files identical despite different names*

### Comparing `evalhyd-python-0.1.0.0/tests/test_probabilist.py` & `evalhyd-python-0.1.1.0/tests/test_probabilist.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     # quantile-based
     'QS', 'CRPS_FROM_QS',
     # contingency table-based
     'POD', 'POFD', 'FAR', 'CSI', 'ROCSS',
     # ranks-based
     'RANK_HIST', 'DS', 'AS',
     # intervals
-    'CR', 'AW', 'AWN', 'AWI', 'WS', 'WSS',
+    'CR', 'AW', 'AWN', 'WS',
     # multivariate
     'ES'
 )
 
 # list all available deterministic diagnostics
 _all_diags = (
     'completeness'
@@ -78,15 +78,15 @@
         ) for metric in ('RANK_HIST', 'DS', 'AS')
     }
 
     expected_itv = {
         metric: (
             numpy.genfromtxt(f"./expected/evalp/{metric}.csv", delimiter=',')
             [numpy.newaxis, numpy.newaxis, numpy.newaxis, numpy.newaxis, ...]
-        ) for metric in ('CR', 'AW', 'AWN', 'AWI', 'WS', 'WSS')
+        ) for metric in ('CR', 'AW', 'AWN', 'WS')
     }
 
     expected_mvr = {
         metric: (
             numpy.genfromtxt(f"./expected/evalp/{metric}.csv", delimiter=',')
             [numpy.newaxis, numpy.newaxis, numpy.newaxis, numpy.newaxis, ...]
         ) for metric in ('ES',)
```

