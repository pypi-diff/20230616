# Comparing `tmp/caliban-0.4.1.tar.gz` & `tmp/caliban-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/caliban-0.4.1.tar", last modified: Sat Sep 12 19:41:21 2020, max compression
+gzip compressed data, was "caliban-0.4.2.tar", last modified: Fri Jun 16 17:24:59 2023, max compression
```

## Comparing `caliban-0.4.1.tar` & `caliban-0.4.2.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (116)     2445 2020-09-12 19:41:09.000000 caliban-0.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       50 2020-09-12 19:41:09.000000 caliban-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    66258 2020-09-12 19:41:09.000000 caliban-0.4.1/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/util/
--rw-r--r--   0 runner    (1001) docker     (116)     3089 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/util/argparse.py
--rw-r--r--   0 runner    (1001) docker     (116)     5249 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/util/metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     1975 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/util/auth.py
--rw-r--r--   0 runner    (1001) docker     (116)     5827 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2428 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (116)     2374 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/util/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (116)     9149 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/util/fs.py
--rw-r--r--   0 runner    (1001) docker     (116)      656 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5081 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/history/
--rw-r--r--   0 runner    (1001) docker     (116)    18576 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/history/types.py
--rw-r--r--   0 runner    (1001) docker     (116)    16151 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/history/util.py
--rw-r--r--   0 runner    (1001) docker     (116)    13661 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/history/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1627 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/history/submit.py
--rw-r--r--   0 runner    (1001) docker     (116)    31484 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/platform/
--rw-r--r--   0 runner    (1001) docker     (116)    11267 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/run.py
--rw-r--r--   0 runner    (1001) docker     (116)     2631 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/platform/gke/
--rw-r--r--   0 runner    (1001) docker     (116)     3463 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/gke/types.py
--rw-r--r--   0 runner    (1001) docker     (116)    21855 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/gke/util.py
--rw-r--r--   0 runner    (1001) docker     (116)    16825 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/gke/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     3417 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/gke/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    40460 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/gke/cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)     3691 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/platform/cloud/
--rw-r--r--   0 runner    (1001) docker     (116)    15902 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/cloud/types.py
--rw-r--r--   0 runner    (1001) docker     (116)     3517 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (116)    22685 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/cloud/core.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/resources/
--rw-r--r--   0 runner    (1001) docker     (116)     4792 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/resources/caliban_launcher.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2334 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/resources/cloud_sql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/docker/
--rw-r--r--   0 runner    (1001) docker     (116)     2744 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/docker/push.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22872 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/docker/build.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)      688 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban/config/
--rw-r--r--   0 runner    (1001) docker     (116)     7946 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9760 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/config/experiment.py
--rw-r--r--   0 runner    (1001) docker     (116)     3137 2020-09-12 19:41:09.000000 caliban-0.4.1/caliban/expansion.py
--rw-r--r--   0 runner    (1001) docker     (116)    19676 2020-09-12 19:41:09.000000 caliban-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      950 2020-09-12 19:41:21.000000 caliban-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/util/
--rw-r--r--   0 runner    (1001) docker     (116)     8133 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/util/test_util.py
--rw-r--r--   0 runner    (1001) docker     (116)     1250 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/util/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (116)     6100 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/util/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     2095 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/util/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (116)     5058 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/util/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (116)     1183 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/util/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (116)     1308 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/util/test_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2005 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/history/
--rw-r--r--   0 runner    (1001) docker     (116)     8180 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/history/test_history.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/history/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/platform/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/platform/gke/
--rw-r--r--   0 runner    (1001) docker     (116)    28258 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/platform/gke/test_util.py
--rw-r--r--   0 runner    (1001) docker     (116)     2970 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/platform/gke/test_types.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/platform/gke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/platform/cloud/
--rw-r--r--   0 runner    (1001) docker     (116)     4516 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/platform/cloud/test_util.py
--rw-r--r--   0 runner    (1001) docker     (116)     3117 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/platform/cloud/test_types.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/platform/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/resources/
--rw-r--r--   0 runner    (1001) docker     (116)     3890 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/resources/test_caliban_launcher.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/docker/
--rw-r--r--   0 runner    (1001) docker     (116)     2791 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/docker/test_push.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1376 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/docker/test_build.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/tests/caliban/config/
--rw-r--r--   0 runner    (1001) docker     (116)     7050 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/config/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (116)     6304 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-09-12 19:41:09.000000 caliban-0.4.1/tests/caliban/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    24140 2020-09-12 19:41:21.000000 caliban-0.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2259 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)      297 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       82 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)    24140 2020-09-12 19:41:21.000000 caliban-0.4.1/caliban.egg-info/PKG-INFO
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.357844 caliban-0.4.2/
+-rw-rw----   0 sritchie   (501) staff       (20)    11358 2023-06-16 04:01:07.000000 caliban-0.4.2/LICENSE
+-rw-rw----   0 sritchie   (501) staff       (20)      575 2023-06-16 04:01:07.000000 caliban-0.4.2/LICENSE_SHORT
+-rw-rw----   0 sritchie   (501) staff       (20)       50 2023-06-16 04:01:07.000000 caliban-0.4.2/MANIFEST.in
+-rw-rw----   0 sritchie   (501) staff       (20)    20009 2023-06-16 17:24:59.357927 caliban-0.4.2/PKG-INFO
+-rw-rw----   0 sritchie   (501) staff       (20)    19670 2023-06-16 04:01:07.000000 caliban-0.4.2/README.md
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.358415 caliban-0.4.2/caliban/
+-rw-rw----   0 sritchie   (501) staff       (20)      688 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)      656 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/__main__.py
+-rw-rw----   0 sritchie   (501) staff       (20)      497 2023-06-16 17:24:59.358443 caliban-0.4.2/caliban/_version.py
+-rw-rw----   0 sritchie   (501) staff       (20)    31484 2023-06-16 15:32:51.000000 caliban-0.4.2/caliban/cli.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.346161 caliban-0.4.2/caliban/config/
+-rw-rw----   0 sritchie   (501) staff       (20)     8199 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/config/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     9760 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/config/experiment.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.346860 caliban-0.4.2/caliban/docker/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/docker/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)    22217 2023-06-16 17:24:06.000000 caliban-0.4.2/caliban/docker/build.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2744 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/docker/push.py
+-rw-rw----   0 sritchie   (501) staff       (20)     3137 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/expansion.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.347564 caliban-0.4.2/caliban/history/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/history/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)    13661 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/history/cli.py
+-rw-rw----   0 sritchie   (501) staff       (20)     1627 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/history/submit.py
+-rw-rw----   0 sritchie   (501) staff       (20)    18576 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/history/types.py
+-rw-rw----   0 sritchie   (501) staff       (20)    16151 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/history/util.py
+-rw-rw----   0 sritchie   (501) staff       (20)     5081 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/main.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.348198 caliban-0.4.2/caliban/platform/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/__init__.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.349626 caliban-0.4.2/caliban/platform/cloud/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/cloud/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)    22685 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/cloud/core.py
+-rw-rw----   0 sritchie   (501) staff       (20)    15902 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/cloud/types.py
+-rw-rw----   0 sritchie   (501) staff       (20)     3517 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/cloud/util.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.350789 caliban-0.4.2/caliban/platform/gke/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/gke/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)    16825 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/gke/cli.py
+-rw-rw----   0 sritchie   (501) staff       (20)    40460 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/gke/cluster.py
+-rw-rw----   0 sritchie   (501) staff       (20)     3417 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/gke/constants.py
+-rw-rw----   0 sritchie   (501) staff       (20)     3463 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/gke/types.py
+-rw-rw----   0 sritchie   (501) staff       (20)    21855 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/gke/util.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2631 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/notebook.py
+-rw-rw----   0 sritchie   (501) staff       (20)    11306 2023-06-16 17:24:06.000000 caliban-0.4.2/caliban/platform/run.py
+-rw-rw----   0 sritchie   (501) staff       (20)     3691 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/platform/shell.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.351330 caliban-0.4.2/caliban/resources/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/resources/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     4854 2023-06-16 17:24:06.000000 caliban-0.4.2/caliban/resources/caliban_launcher.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2334 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/resources/cloud_sql_proxy.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.352402 caliban-0.4.2/caliban/util/
+-rw-rw----   0 sritchie   (501) staff       (20)     5827 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/util/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     3089 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/util/argparse.py
+-rw-rw----   0 sritchie   (501) staff       (20)     1975 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/util/auth.py
+-rw-rw----   0 sritchie   (501) staff       (20)     9114 2023-06-16 17:24:06.000000 caliban-0.4.2/caliban/util/fs.py
+-rw-rw----   0 sritchie   (501) staff       (20)     5782 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/util/metrics.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2428 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/util/schema.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2374 2023-06-16 04:01:07.000000 caliban-0.4.2/caliban/util/tqdm.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.345815 caliban-0.4.2/caliban.egg-info/
+-rw-rw----   0 sritchie   (501) staff       (20)    20009 2023-06-16 17:24:59.000000 caliban-0.4.2/caliban.egg-info/PKG-INFO
+-rw-rw----   0 sritchie   (501) staff       (20)     2281 2023-06-16 17:24:59.000000 caliban-0.4.2/caliban.egg-info/SOURCES.txt
+-rw-rw----   0 sritchie   (501) staff       (20)        1 2023-06-16 17:24:59.000000 caliban-0.4.2/caliban.egg-info/dependency_links.txt
+-rw-rw----   0 sritchie   (501) staff       (20)       81 2023-06-16 17:24:59.000000 caliban-0.4.2/caliban.egg-info/entry_points.txt
+-rw-rw----   0 sritchie   (501) staff       (20)      271 2023-06-16 17:24:59.000000 caliban-0.4.2/caliban.egg-info/requires.txt
+-rw-rw----   0 sritchie   (501) staff       (20)       14 2023-06-16 17:24:59.000000 caliban-0.4.2/caliban.egg-info/top_level.txt
+-rw-rw----   0 sritchie   (501) staff       (20)      950 2023-06-16 17:24:59.358288 caliban-0.4.2/setup.cfg
+-rw-rw----   0 sritchie   (501) staff       (20)     2212 2023-06-16 17:24:06.000000 caliban-0.4.2/setup.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.341629 caliban-0.4.2/tests/
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.353636 caliban-0.4.2/tests/caliban/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/__init__.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.354455 caliban-0.4.2/tests/caliban/config/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/config/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     6304 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/config/test_config.py
+-rw-rw----   0 sritchie   (501) staff       (20)     7050 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/config/test_experiment.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.354868 caliban-0.4.2/tests/caliban/docker/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/docker/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     1376 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/docker/test_build.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2791 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/docker/test_push.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.355165 caliban-0.4.2/tests/caliban/history/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/history/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     8180 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/history/test_history.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.355311 caliban-0.4.2/tests/caliban/platform/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/platform/__init__.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.355784 caliban-0.4.2/tests/caliban/platform/cloud/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/platform/cloud/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     3117 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/platform/cloud/test_types.py
+-rw-rw----   0 sritchie   (501) staff       (20)     4516 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/platform/cloud/test_util.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.356253 caliban-0.4.2/tests/caliban/platform/gke/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/platform/gke/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2970 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/platform/gke/test_types.py
+-rw-rw----   0 sritchie   (501) staff       (20)    28263 2023-06-16 17:24:06.000000 caliban-0.4.2/tests/caliban/platform/gke/test_util.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.356548 caliban-0.4.2/tests/caliban/resources/
+-rw-rw----   0 sritchie   (501) staff       (20)        0 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/resources/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     3890 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/resources/test_caliban_launcher.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2005 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/test_cli.py
+drwxrwx---   0 sritchie   (501) staff       (20)        0 2023-06-16 17:24:59.357701 caliban-0.4.2/tests/caliban/util/
+-rw-rw----   0 sritchie   (501) staff       (20)      595 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/util/__init__.py
+-rw-rw----   0 sritchie   (501) staff       (20)     1250 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/util/test_argparse.py
+-rw-rw----   0 sritchie   (501) staff       (20)     2095 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/util/test_auth.py
+-rw-rw----   0 sritchie   (501) staff       (20)     5058 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/util/test_fs.py
+-rw-rw----   0 sritchie   (501) staff       (20)     6226 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/util/test_metrics.py
+-rw-rw----   0 sritchie   (501) staff       (20)     1183 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/util/test_schema.py
+-rw-rw----   0 sritchie   (501) staff       (20)     1308 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/util/test_tqdm.py
+-rw-rw----   0 sritchie   (501) staff       (20)     8133 2023-06-16 04:01:07.000000 caliban-0.4.2/tests/caliban/util/test_util.py
+-rw-rw----   0 sritchie   (501) staff       (20)    66258 2023-06-16 04:01:07.000000 caliban-0.4.2/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `caliban-0.4.1/setup.py` & `caliban-0.4.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,22 +44,18 @@
     'google-api-python-client',
     'pyyaml',
     'tqdm>=4.45.0',
     'kubernetes>=10.0.1',
     'google-auth>=1.19.0',
     'google-cloud-core>=1.0.3',
     'google-cloud-container>=0.3.0',
-    'psycopg2-binary==2.8.5',
+    'psycopg2-binary==2.9.6',
     'schema==0.7.2',
     'urllib3>=1.25.7',
     'yaspin>=0.16.0',
-    # This is not a real dependency of ours, but we need it to override the
-    # dep that commentjson brings in. Delete once this is merged:
-    # https://github.com/vaidik/commentjson/pull/33/files
-    'lark-parser>=0.7.1,<0.8.0',
     'SQLAlchemy==1.3.11',
     'pg8000==1.16.1',
 ]
 
 setup(name='caliban',
       version=with_versioneer(lambda v: v.get_version()),
       cmdclass=with_versioneer(lambda v: v.get_cmdclass(), {}),
```

### Comparing `caliban-0.4.1/versioneer.py` & `caliban-0.4.2/versioneer.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/util/argparse.py` & `caliban-0.4.2/caliban/util/argparse.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/util/metrics.py` & `caliban-0.4.2/caliban/util/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,33 +60,41 @@
   return {
       'services': [],
       'env': {},
   }
 
 
 def _create_mlflow_config(
-    cfg: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
+    mlflow_cfg: Optional[Dict[str, Any]] = None,
+    uv_cfg: Optional[Dict[str, Any]] = None,
+) -> Dict[str, Any]:
   '''generates mlflow configuration dict for launcher script
   Args:
-  cfg: mlflow configuration dict from .calibanconfig.json
+  mlflow_cfg: mlflow configuration dict from .calibanconfig.json
+  uv_cfg: uv configuration dict from .calibanconfig.json
 
   Returns:
   config dict for launcher script with entries needed for mlflow
   '''
 
-  if cfg is None:
+  if mlflow_cfg is None:
     return _default_launcher_config()
 
-  user = cfg['user']
-  pw = cfg['password']
-  db = cfg['db']
-  project = cfg['project']
-  region = cfg['region']
-  artifact_root = cfg['artifact_root']
-  debug = cfg.get('debug', False)
+  uv_cfg = uv_cfg or {}
+  uv_mlflow_cfg = uv_cfg.get('mlflow') or {}
+
+  user = mlflow_cfg['user']
+  pw = mlflow_cfg['password']
+  db = mlflow_cfg['db']
+  project = mlflow_cfg['project']
+  region = mlflow_cfg['region']
+  artifact_root = mlflow_cfg['artifact_root']
+  debug = mlflow_cfg.get('debug', False)
+  pubsub_project = uv_mlflow_cfg.get('pubsub_project', project)
+  pubsub_topic = uv_mlflow_cfg.get('pubsub_topic') or 'mlflow'
 
   socket_path = '/tmp/cloudsql'
   proxy_path = os.path.join(os.sep, 'usr', 'bin', 'cloud_sql_proxy')
 
   proxy_config = json.dumps({
       'proxy': proxy_path,
       'path': socket_path,
@@ -106,15 +114,17 @@
       f'postgresql+pg8000://{user}:{pw}@/{db}?unix_sock={socket_path}/'
       f'{project}:{region}:{db}/.s.PGSQL.5432')
 
   return {
       'services': [proxy_cmd],
       'env': {
           'MLFLOW_TRACKING_URI': tracking_uri,
-          'MLFLOW_ARTIFACT_ROOT': artifact_root
+          'MLFLOW_ARTIFACT_ROOT': artifact_root,
+          'UV_MLFLOW_PUBSUB_PROJECT': pubsub_project,
+          'UV_MLFLOW_PUBSUB_TOPIC': pubsub_topic,
       }
   }
 
 
 @contextmanager
 def launcher_config_file(
     path: str,
@@ -140,15 +150,17 @@
   '''
 
   caliban_config = caliban_config or {}
 
   config = _default_launcher_config()
   config_file_path = os.path.join(path, LAUNCHER_CONFIG_FILE)
 
-  mlflow_config = _create_mlflow_config(caliban_config.get('mlflow_config'))
+  mlflow_config = _create_mlflow_config(
+      mlflow_cfg=caliban_config.get('mlflow_config'),
+      uv_cfg=caliban_config.get('uv'))
 
   config['services'] += mlflow_config['services']
   config['env'].update(mlflow_config['env'])
 
   with open(config_file_path, 'w') as f:
     json.dump(config, f, indent=2)
```

### Comparing `caliban-0.4.1/caliban/util/auth.py` & `caliban-0.4.2/caliban/util/auth.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/util/__init__.py` & `caliban-0.4.2/caliban/util/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/util/schema.py` & `caliban-0.4.2/caliban/util/schema.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/util/tqdm.py` & `caliban-0.4.2/caliban/util/tqdm.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/util/fs.py` & `caliban-0.4.2/caliban/util/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,16 +250,15 @@
   buf = io.StringIO()
   ret_code = None
 
   with subprocess.Popen(cmd,
                         stdin=subprocess.PIPE,
                         stdout=subprocess.PIPE,
                         stderr=subprocess.STDOUT,
-                        universal_newlines=False,
-                        bufsize=1) as p:
+                        universal_newlines=False) as p:
     if input_str:
       p.stdin.write(input_str.encode('utf-8'))
     p.stdin.close()
 
     out = io.TextIOWrapper(p.stdout, newline='')
 
     for line in out:
```

### Comparing `caliban-0.4.1/caliban/__main__.py` & `caliban-0.4.2/caliban/__main__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/main.py` & `caliban-0.4.2/caliban/main.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/history/types.py` & `caliban-0.4.2/caliban/history/types.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/history/util.py` & `caliban-0.4.2/caliban/history/util.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/history/cli.py` & `caliban-0.4.2/caliban/history/cli.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/history/__init__.py` & `caliban-0.4.2/caliban/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/history/submit.py` & `caliban-0.4.2/caliban/history/submit.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/cli.py` & `caliban-0.4.2/caliban/cli.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/run.py` & `caliban-0.4.2/caliban/platform/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,16 @@
   - run_args: list of args to pass to docker run.
 
   """
   if run_args is None:
     run_args = []
 
   runtime = ["--runtime", "nvidia"] if c.gpu(job_mode) else []
-  return ["docker", "run"] + runtime + ["--ipc", "host"] + run_args
+  return ["docker", "run", "--platform", "linux/amd64"
+         ] + runtime + ["--ipc", "host"] + run_args
 
 
 def log_job_spec_instance(job_spec: JobSpec, i: int) -> JobSpec:
   """Prints logging as a side effect for the supplied sequence of job specs
   generated from an experiment definition; returns the input job spec.
 
   """
```

### Comparing `caliban-0.4.1/caliban/platform/notebook.py` & `caliban-0.4.2/caliban/platform/notebook.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/gke/types.py` & `caliban-0.4.2/caliban/platform/gke/types.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/gke/util.py` & `caliban-0.4.2/caliban/platform/gke/util.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/gke/cli.py` & `caliban-0.4.2/caliban/platform/gke/cli.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/gke/constants.py` & `caliban-0.4.2/caliban/platform/gke/constants.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/gke/__init__.py` & `caliban-0.4.2/caliban/history/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/gke/cluster.py` & `caliban-0.4.2/caliban/platform/gke/cluster.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/shell.py` & `caliban-0.4.2/caliban/platform/shell.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/cloud/types.py` & `caliban-0.4.2/caliban/platform/cloud/types.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/cloud/util.py` & `caliban-0.4.2/caliban/platform/cloud/util.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/cloud/core.py` & `caliban-0.4.2/caliban/platform/cloud/core.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/cloud/__init__.py` & `caliban-0.4.2/caliban/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/platform/__init__.py` & `caliban-0.4.2/caliban/platform/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/resources/caliban_launcher.py` & `caliban-0.4.2/caliban/resources/caliban_launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,20 @@
   Returns:
   possibly modified env dictionary
   '''
 
   if 'GOOGLE_CLOUD_PROJECT' in env:
     return env
 
-  _, project_id = google.auth.default()
+  project_id = None
+  try:
+    _, project_id = google.auth.default()
+  except:
+    project_id = None
+
   if project_id is not None:
     return env
 
   new_env = copy.copy(env)
   new_env['GOOGLE_CLOUD_PROJECT'] = 'placeholder'
   return new_env
```

### Comparing `caliban-0.4.1/caliban/resources/__init__.py` & `caliban-0.4.2/caliban/platform/gke/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/resources/cloud_sql_proxy.py` & `caliban-0.4.2/caliban/resources/cloud_sql_proxy.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/docker/push.py` & `caliban-0.4.2/caliban/docker/push.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/docker/__init__.py` & `caliban-0.4.2/caliban/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/docker/build.py` & `caliban-0.4.2/caliban/docker/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 """
 
 from __future__ import absolute_import, division, print_function
 
 import json
 import os
 import subprocess
+import tempfile
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, NamedTuple, NewType, Optional, Union
 
 from absl import logging
 from blessings import Terminal
 
@@ -42,16 +43,16 @@
 DEFAULT_CPU_TAG = "cpu-ubuntu1804-py37"
 TF_VERSIONS = {"2.2.0", "1.12.3", "1.14.0", "1.15.0"}
 DEFAULT_WORKDIR = "/usr/app"
 CREDS_DIR = "/.creds"
 RESOURCE_DIR = "/.resources"
 CONDA_BIN = "/opt/conda/bin/conda"
 
-ImageId = NewType('ImageId', str)
-ArgSeq = NewType('ArgSeq', List[str])
+ImageId = NewType("ImageId", str)
+ArgSeq = NewType("ArgSeq", List[str])
 
 
 class DockerError(Exception):
   """Exception that passes info on a failed Docker command."""
 
   def __init__(self, message, cmd, ret_code):
     super().__init__(message)
@@ -62,26 +63,28 @@
   @property
   def command(self):
     return " ".join(self.cmd)
 
 
 class NotebookInstall(Enum):
   """Flag to decide what to do ."""
-  none = 'none'
-  lab = 'lab'
-  jupyter = 'jupyter'
+
+  none = "none"
+  lab = "lab"
+  jupyter = "jupyter"
 
   def __str__(self) -> str:
     return self.value
 
 
 class Shell(Enum):
   """Add new shells here and below, in SHELL_DICT."""
-  bash = 'bash'
-  zsh = 'zsh'
+
+  bash = "bash"
+  zsh = "zsh"
 
   def __str__(self) -> str:
     return self.value
 
 
 # Tuple to track the information required to install and execute some custom
 # shell into a container.
@@ -89,34 +92,36 @@
                                      ("packages", List[str])])
 
 
 def apt_install(*packages: str) -> str:
   """Returns a command that will install the supplied list of packages without
   requiring confirmation or any user interaction.
   """
-  package_str = ' '.join(packages)
+  package_str = " ".join(packages)
   no_prompt = "DEBIAN_FRONTEND=noninteractive"
   return f"{no_prompt} apt-get install --yes --no-install-recommends {package_str}"
 
 
 def apt_command(commands: List[str]) -> List[str]:
   """Pre-and-ap-pends the supplied commands with the appropriate in-container and
   cleanup command for aptitude.
 
   """
   update = ["apt-get update"]
   cleanup = ["apt-get clean", "rm -rf /var/lib/apt/lists/*"]
   return update + commands + cleanup
 
 
-def copy_command(user_id: int,
-                 user_group: int,
-                 from_path: str,
-                 to_path: str,
-                 comment: Optional[str] = None) -> str:
+def copy_command(
+    user_id: int,
+    user_group: int,
+    from_path: str,
+    to_path: str,
+    comment: Optional[str] = None,
+) -> str:
   """Generates a Dockerfile entry that will copy the file at the directory-local
   from_path into the container at to_path.
 
   If you supply a relative path, Docker will copy the file into the current
   working directory, where it will be overwritten in any interactive mode. We
   recommend using an absolute path!
 
@@ -132,15 +137,15 @@
 
 # Dict linking a particular supported shell to the data required to run and
 # install the shell inside a container.
 #
 # : Dict[Shell, ShellData]
 SHELL_DICT = {
     Shell.bash: ShellData("/bin/bash", []),
-    Shell.zsh: ShellData("/bin/zsh", ["zsh"])
+    Shell.zsh: ShellData("/bin/zsh", ["zsh"]),
 }
 
 
 def default_shell() -> Shell:
   """Returns the shell to load into the container. Defaults to Shell.bash, but if
   the user's SHELL variable refers to a supported sub-shell, returns that
   instead.
@@ -205,15 +210,15 @@
   setup.py and target a specific set of extras_require dependencies.
 
     Args:
         extras: (potentially empty) list of extra_requires deps.
   """
   ret = "."
   if len(extras) > 0:
-    ret += "[{}]".format(','.join(extras))
+    ret += "[{}]".format(",".join(extras))
   return ret
 
 
 def base_extras(job_mode: c.JobMode, path: str,
                 extras: Optional[List[str]]) -> Optional[List[str]]:
   """Returns None if the supplied path doesn't exist (it's assumed it points to a
   setup.py file).
@@ -222,26 +227,28 @@
   always added to the beginning of the list, depending on the mode.
 
   """
   ret = None
 
   if os.path.exists(path):
     base = extras or []
-    extra = 'gpu' if c.gpu(job_mode) else 'cpu'
+    extra = "gpu" if c.gpu(job_mode) else "cpu"
     ret = base if extra in base else [extra] + base
 
   return ret
 
 
-def _dependency_entries(workdir: str,
-                        user_id: int,
-                        user_group: int,
-                        requirements_path: Optional[str] = None,
-                        conda_env_path: Optional[str] = None,
-                        setup_extras: Optional[List[str]] = None) -> str:
+def _dependency_entries(
+    workdir: str,
+    user_id: int,
+    user_group: int,
+    requirements_path: Optional[str] = None,
+    conda_env_path: Optional[str] = None,
+    setup_extras: Optional[List[str]] = None,
+) -> str:
   """Returns the Dockerfile entries required to install dependencies from either:
 
   - a requirements.txt file, path supplied by requirements_path
   - a conda environment.yml file, path supplied by conda_env_path.
   - a setup.py file, if some sequence of dependencies is supplied.
 
   An empty list for setup_extras means, run `pip install -c .` with no extras.
@@ -291,15 +298,15 @@
 
   Returns:
   string with Dockerfile directives to install cloud_sql_proxy as root
   and reset the user to the specified user_id:user_group.
 
   """
   caliban_config = caliban_config or {}
-  mlflow_cfg = caliban_config.get('mlflow_config')
+  mlflow_cfg = caliban_config.get("mlflow_config")
 
   if mlflow_cfg is None:
     return ""
 
   return f"""
 USER root
 
@@ -319,17 +326,18 @@
   executable: string of main executable
 
   Returns:
   string with Dockerfile directives to set ENTRYPOINT
 
   """
   launcher_cmd = json.dumps([
-      'python',
-      os.path.join(RESOURCE_DIR, um.LAUNCHER_SCRIPT), '--caliban_command',
-      executable
+      "python",
+      os.path.join(RESOURCE_DIR, um.LAUNCHER_SCRIPT),
+      "--caliban_command",
+      executable,
   ])
 
   return f"""
 ENTRYPOINT {launcher_cmd}
 """
 
 
@@ -359,15 +367,16 @@
                                           caliban_config=caliban_config)
 
   copy_code = copy_command(
       user_id,
       user_group,
       package_path,
       f"{workdir}/{package_path}",
-      comment="Copy project code into the docker container.")
+      comment="Copy project code into the docker container.",
+  )
 
   # This needs to use json so that quotes print as double quotes, not single
   # quotes.
   executable_s = json.dumps(package.executable + [arg])
   entrypoint_code = _generate_entrypoint(executable_s)
 
   return f"""
@@ -375,17 +384,21 @@
 
   {copy_code}
 
   {entrypoint_code}
 """
 
 
-def _service_account_entry(user_id: int, user_group: int, credentials_path: str,
-                           docker_credentials_dir: str,
-                           write_adc_placeholder: bool):
+def _service_account_entry(
+    user_id: int,
+    user_group: int,
+    credentials_path: str,
+    docker_credentials_dir: str,
+    write_adc_placeholder: bool,
+):
   """Generates the Dockerfile entries required to transfer a set of Cloud service
   account credentials into the Docker container.
 
   NOTE the write_adc_placeholder variable is here because the "ctpu" script
   that we use to interact with TPUs has a bug in it, as of 1/21/2020, where the
   script will fail if the application_default_credentials.json file isn't
   present, EVEN THOUGH it properly uses the service account credentials
@@ -421,19 +434,21 @@
   directory.
 
   """
   return copy_command(user_id, user_group, adc_path,
                       adc_location(container_home()))
 
 
-def _credentials_entries(user_id: int,
-                         user_group: int,
-                         adc_path: Optional[str],
-                         credentials_path: Optional[str],
-                         docker_credentials_dir: Optional[str] = None) -> str:
+def _credentials_entries(
+    user_id: int,
+    user_group: int,
+    adc_path: Optional[str],
+    credentials_path: Optional[str],
+    docker_credentials_dir: Optional[str] = None,
+) -> str:
   """Returns the Dockerfile entries necessary to copy a user's Cloud credentials
   into the Docker container.
 
   - adc_path is the relative path inside the current directory to an
     application_default_credentials.json file containing... well, you get it.
   - credentials_path is the relative path inside the current directory to a
     JSON credentials file.
@@ -442,19 +457,21 @@
 
   """
   if docker_credentials_dir is None:
     docker_credentials_dir = CREDS_DIR
 
   ret = ""
   if credentials_path is not None:
-    ret += _service_account_entry(user_id,
-                                  user_group,
-                                  credentials_path,
-                                  docker_credentials_dir,
-                                  write_adc_placeholder=adc_path is None)
+    ret += _service_account_entry(
+        user_id,
+        user_group,
+        credentials_path,
+        docker_credentials_dir,
+        write_adc_placeholder=adc_path is None,
+    )
 
   if adc_path is not None:
     ret += _adc_entry(user_id, user_group, adc_path)
 
   return ret
 
 
@@ -503,31 +520,33 @@
 
 RUN {commands}
 
 USER {user_id}:{user_group}
 """.format_map({
         "commands": " && ".join(commands),
         "user_id": user_id,
-        "user_group": user_group
+        "user_group": user_group,
     })
 
   return ret
 
 
 def _copy_dir_entry(workdir: str, user_id: int, user_group: int,
                     dirname: str) -> str:
   """Returns the Dockerfile entry necessary to copy a single extra subdirectory
   from the current directory into a docker container during build.
 
   """
-  return copy_command(user_id,
-                      user_group,
-                      dirname,
-                      f"{workdir}/{dirname}",
-                      comment=f"Copy {dirname} into the Docker container.")
+  return copy_command(
+      user_id,
+      user_group,
+      dirname,
+      f"{workdir}/{dirname}",
+      comment=f"Copy {dirname} into the Docker container.",
+  )
 
 
 def _extra_dir_entries(workdir: str,
                        user_id: int,
                        user_group: int,
                        extra_dirs: Optional[List[str]] = None) -> str:
   """Returns the Dockerfile entries necessary to copy all directories in the
@@ -539,18 +558,20 @@
 
   def copy(d):
     return _copy_dir_entry(workdir, user_id, user_group, d)
 
   return "\n\n".join(map(copy, extra_dirs)) + "\n"
 
 
-def _resource_entries(uid: int,
-                      gid: int,
-                      resource_files: Optional[List[str]] = None,
-                      resource_dir: str = RESOURCE_DIR) -> str:
+def _resource_entries(
+    uid: int,
+    gid: int,
+    resource_files: Optional[List[str]] = None,
+    resource_dir: str = RESOURCE_DIR,
+) -> str:
   """Returns Dockerfile entries necessary to copy miscellaneous resource files
   into container. Usually these files are staged in the working directory, so
   that Docker's build context can access them.
 
   Args:
   uid: user id in container for files
   gid: user group id in container for files
@@ -582,15 +603,16 @@
     adc_path: Optional[str] = None,
     credentials_path: Optional[str] = None,
     jupyter_version: Optional[str] = None,
     inject_notebook: NotebookInstall = NotebookInstall.none,
     shell: Optional[Shell] = None,
     extra_dirs: Optional[List[str]] = None,
     resource_files: Optional[List[str]] = None,
-    caliban_config: Optional[Dict[str, Any]] = None) -> str:
+    caliban_config: Optional[Dict[str, Any]] = None,
+) -> str:
   """Returns a Dockerfile that builds on a local CPU or GPU base image (depending
   on the value of job_mode) to create a container that:
 
   - installs any dependency specified in a requirements.txt file living at
     requirements_path, a conda environment at conda_env_path, or any
     dependencies in a setup.py file, including extra dependencies, if
     setup_extras isn't None
@@ -644,100 +666,102 @@
 
   dockerfile += _custom_packages(uid,
                                  gid,
                                  packages=c.apt_packages(
                                      caliban_config, job_mode),
                                  shell=shell)
 
-  dockerfile += _dependency_entries(workdir,
-                                    uid,
-                                    gid,
-                                    requirements_path=requirements_path,
-                                    conda_env_path=conda_env_path,
-                                    setup_extras=setup_extras)
+  dockerfile += _dependency_entries(
+      workdir,
+      uid,
+      gid,
+      requirements_path=requirements_path,
+      conda_env_path=conda_env_path,
+      setup_extras=setup_extras,
+  )
 
-  if inject_notebook.value != 'none':
+  if inject_notebook.value != "none":
     install_lab = inject_notebook == NotebookInstall.lab
     dockerfile += _notebook_entries(lab=install_lab, version=jupyter_version)
 
   dockerfile += _extra_dir_entries(workdir, uid, gid, extra_dirs)
 
   dockerfile += _resource_entries(uid, gid, resource_files)
 
   if package is not None:
     # The actual entrypoint and final copied code.
     dockerfile += _package_entries(workdir, uid, gid, package, caliban_config)
 
   return dockerfile
 
 
-def docker_image_id(output: str) -> ImageId:
-  """Accepts a string containing the output of a successful `docker build`
-  command and parses the Docker image ID from the stream.
-
-  NOTE this is probably quite brittle! I can imagine this breaking quite easily
-  on a Docker upgrade.
-
-  """
-  return ImageId(output.splitlines()[-1].split()[-1])
-
-
-def build_image(job_mode: c.JobMode,
-                build_path: str,
-                credentials_path: Optional[str] = None,
-                adc_path: Optional[str] = None,
-                no_cache: bool = False,
-                **kwargs) -> str:
+def build_image(
+    job_mode: c.JobMode,
+    build_path: str,
+    credentials_path: Optional[str] = None,
+    adc_path: Optional[str] = None,
+    no_cache: bool = False,
+    **kwargs,
+) -> str:
   """Builds a Docker image by generating a Dockerfile and passing it to `docker
   build` via stdin. All output from the `docker build` process prints to
   stdout.
 
   Returns the image ID of the new docker container; if the command fails,
   throws on error with information about the command and any issues that caused
   the problem.
 
   """
-  caliban_config = kwargs.get('caliban_config', {})
+  caliban_config = kwargs.get("caliban_config", {})
 
   # Paths for resource files.
   sql_proxy_path = um.cloud_sql_proxy_path()
   launcher_path = um.launcher_path()
 
   with ufs.TempCopy({
       credentials_path: ".caliban_default_creds.json",
       adc_path: ".caliban_adc_creds.json",
       sql_proxy_path: um.CLOUD_SQL_WRAPPER_SCRIPT,
       launcher_path: um.LAUNCHER_SCRIPT,
   }) as creds:
 
-    # generate our launcher configuration file
-    with um.launcher_config_file(
-        path='.', caliban_config=caliban_config) as launcher_config:
-
-      cache_args = ["--no-cache"] if no_cache else []
-      cmd = ["docker", "build"] + cache_args + ["--rm", "-f-", build_path]
-
-      dockerfile = _dockerfile_template(
-          job_mode,
-          credentials_path=creds.get(credentials_path),
-          adc_path=creds.get(adc_path),
-          resource_files=[
-              creds.get(sql_proxy_path),
-              creds.get(launcher_path),
-              launcher_config,
-          ],
-          **kwargs)
-
-      joined_cmd = " ".join(cmd)
-      logging.info("Running command: {}".format(joined_cmd))
-
-      try:
-        output, ret_code = ufs.capture_stdout(cmd, input_str=dockerfile)
-        if ret_code == 0:
-          return docker_image_id(output)
-        else:
-          error_msg = "Docker failed with error code {}.".format(ret_code)
-          raise DockerError(error_msg, cmd, ret_code)
-
-      except subprocess.CalledProcessError as e:
-        logging.error(e.output)
-        logging.error(e.stderr)
+    with tempfile.NamedTemporaryFile() as id_file:
+
+      # generate our launcher configuration file
+      with um.launcher_config_file(
+          path=".", caliban_config=caliban_config) as launcher_config:
+
+        cache_args = ["--no-cache"] if no_cache else []
+        cmd = ["docker", "build", "--platform", "linux/amd64"] + cache_args + \
+          ["--iidfile", id_file.name] + \
+          ["--rm", "-f-", build_path]
+
+        dockerfile = _dockerfile_template(
+            job_mode,
+            credentials_path=creds.get(credentials_path),
+            adc_path=creds.get(adc_path),
+            resource_files=[
+                creds.get(sql_proxy_path),
+                creds.get(launcher_path),
+                launcher_config,
+            ],
+            **kwargs,
+        )
+
+        joined_cmd = " ".join(cmd)
+        logging.info("Running command: {}".format(joined_cmd))
+
+        try:
+          _, ret_code = ufs.capture_stdout(cmd, input_str=dockerfile)
+          if ret_code == 0:
+            image_id = None
+            with open(id_file.name) as f:
+              image_id = f.read()
+            return image_id
+
+          else:
+            error_msg = "Docker failed with error code {}.".format(ret_code)
+            raise DockerError(error_msg, cmd, ret_code)
+
+        except subprocess.CalledProcessError as e:
+          logging.error(e.output)
+          logging.error(e.stderr)
```

### Comparing `caliban-0.4.1/caliban/__init__.py` & `caliban-0.4.2/caliban/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/config/__init__.py` & `caliban-0.4.2/caliban/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,23 @@
     'db': str,
     'user': str,
     'password': str,
     'artifact_root': str,
     s.Optional('debug'): bool,
 }
 
+UVMLFlowConfig = {
+    s.Optional('pubsub_project'): str,  # default = mlflow_config.project
+    s.Optional('pubsub_topic', default='mlflow'): str,
+}
+
+UVConfig = {
+    s.Optional('mlflow'): UVMLFlowConfig,
+}
+
 # Config items that are project-specific, and don't belong in a global
 # .calibanconfig shared between projects.
 ProjectConfig = {
     s.Optional("build_time_credentials", default=False):
         bool,
     s.Optional("base_image", default=None):
         BaseImage,
@@ -155,14 +164,15 @@
 
 # Elements of calibanconfig that are fair game to share between projects.
 #
 SystemConfig = {
     s.Optional("default_mode", default=JobMode.CPU): s.Use(JobMode.parse),
     s.Optional("gcloud", default={}): GCloudConfig,
     s.Optional("mlflow_config", default=None): MLFlowConfig,
+    s.Optional("uv", default={}): UVConfig,
 }
 
 # The final, parsed calibanconfig.
 CalibanConfig = s.Schema({**ProjectConfig, **SystemConfig})
 
 # Accessors
```

### Comparing `caliban-0.4.1/caliban/config/experiment.py` & `caliban-0.4.2/caliban/config/experiment.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/caliban/expansion.py` & `caliban-0.4.2/caliban/expansion.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/README.md` & `caliban-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -491,28 +491,30 @@
 here: [COMMITTERS.md](COMMITTERS.md)
 
 A list of contributors to the project can be found at the project's
 [Contributors](https://github.com/google/caliban/graphs/contributors) page.
 
 ## Citing Caliban
 
-If Caliban helps you in your research, please consider citing the repository:
+If Caliban helps you in your research, please consider citing Caliban's
+associated academic paper:
 
 ```
-@software{caliban2020github,
-  author = {Sam Ritchie and Ambrose Slone and Vinay Ramasesh},
-  title = {{Caliban}: Docker-based job manager for reproducible workflows},
-  url = {http://github.com/google/caliban},
-  version = {0.2.5},
+@article{Ritchie2020,
+  doi = {10.21105/joss.02403},
+  url = {https://doi.org/10.21105/joss.02403},
   year = {2020},
+  publisher = {The Open Journal},
+  volume = {5},
+  number = {53},
+  pages = {2403},
+  author = {Sam Ritchie and Ambrose Slone and Vinay Ramasesh},
+  title = {Caliban: Docker-based job manager for reproducible workflows},
+  journal = {Journal of Open Source Software}
 }
 ```
 
-In the above bibtex entry, the version number is intended to be that of the
-latest tag on github, and the year corresponds to the project's open-source
-release.
-
 ## License
 
 Copyright 2020 Google LLC.
 
 Licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
```

### Comparing `caliban-0.4.1/setup.cfg` & `caliban-0.4.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [run]
 omit = 
 	*/tests/*
 	*/test_*
 	*/_version.py
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = caliban/_version.py
 versionfile_build = caliban/_version.py
 tag_prefix = 
 
 [mypy-tqdm.*]
 ignore_missing_imports = True
```

### Comparing `caliban-0.4.1/tests/caliban/util/test_util.py` & `caliban-0.4.2/tests/caliban/util/test_util.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/util/test_argparse.py` & `caliban-0.4.2/tests/caliban/util/test_argparse.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/util/test_metrics.py` & `caliban-0.4.2/tests/caliban/util/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,19 @@
                 'project': project,
                 'region': region,
                 'db': db,
                 'user': user,
                 'password': password,
                 'artifact_root': artifact_root,
             },
+            'uv': {
+                'mlflow': {
+                    'pubsub_topic': 'mlflow',
+                }
+            }
         },
     }
 
     proxy_config = {
         'proxy': os.path.join(os.sep, 'usr', 'bin', 'cloud_sql_proxy'),
         'path': '/tmp/cloudsql',
         'project': project,
```

### Comparing `caliban-0.4.1/tests/caliban/util/test_auth.py` & `caliban-0.4.2/tests/caliban/util/test_auth.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/util/test_fs.py` & `caliban-0.4.2/tests/caliban/util/test_fs.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/util/test_schema.py` & `caliban-0.4.2/tests/caliban/util/test_schema.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/util/test_tqdm.py` & `caliban-0.4.2/tests/caliban/util/test_tqdm.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/util/__init__.py` & `caliban-0.4.2/tests/caliban/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/test_cli.py` & `caliban-0.4.2/tests/caliban/test_cli.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/history/test_history.py` & `caliban-0.4.2/tests/caliban/history/test_history.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/history/__init__.py` & `caliban-0.4.2/tests/caliban/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/platform/gke/test_util.py` & `caliban-0.4.2/tests/caliban/platform/gke/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
       x = json.load(f)
     assert x == nnd
 
     fname = os.path.join(tmpdir, 'foo.yaml')
     assert util.export_job(j, fname)
     assert os.path.exists(fname)
     with open(fname, 'r') as f:
-      x = yaml.load(f)
+      x = yaml.safe_load(f)
     assert x == nnd
 
     fname = os.path.join(tmpdir, 'foo.xyz')
     assert not util.export_job(j, fname)
 
 
 # ----------------------------------------------------------------------------
```

### Comparing `caliban-0.4.1/tests/caliban/platform/gke/test_types.py` & `caliban-0.4.2/tests/caliban/platform/gke/test_types.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/platform/gke/__init__.py` & `caliban-0.4.2/tests/caliban/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/platform/cloud/test_util.py` & `caliban-0.4.2/tests/caliban/platform/cloud/test_util.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/platform/cloud/test_types.py` & `caliban-0.4.2/tests/caliban/platform/cloud/test_types.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/platform/cloud/__init__.py` & `caliban-0.4.2/tests/caliban/history/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/platform/__init__.py` & `caliban-0.4.2/tests/caliban/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/resources/test_caliban_launcher.py` & `caliban-0.4.2/tests/caliban/resources/test_caliban_launcher.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/docker/test_push.py` & `caliban-0.4.2/tests/caliban/docker/test_push.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/docker/__init__.py` & `caliban-0.4.2/tests/caliban/platform/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/docker/test_build.py` & `caliban-0.4.2/tests/caliban/docker/test_build.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/__init__.py` & `caliban-0.4.2/tests/caliban/platform/gke/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/config/test_experiment.py` & `caliban-0.4.2/tests/caliban/config/test_experiment.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/config/test_config.py` & `caliban-0.4.2/tests/caliban/config/test_config.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/tests/caliban/config/__init__.py` & `caliban-0.4.2/tests/caliban/util/__init__.py`

 * *Files identical despite different names*

### Comparing `caliban-0.4.1/PKG-INFO` & `caliban-0.4.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,530 +1,533 @@
 Metadata-Version: 2.1
 Name: caliban
-Version: 0.4.1
+Version: 0.4.2
 Summary: Docker-based job runner for AI research.
 Home-page: https://github.com/google/caliban
 Author: Caliban Team
 Author-email: samritchie@google.com
 License: Apache-2.0
-Description: # Caliban
-        
-        [![Build status](https://github.com/google/caliban/workflows/build/badge.svg?branch=master)](https://github.com/google/caliban/actions?query=workflow%3Abuild+branch%3Amaster)
-        [![Codecov branch](https://img.shields.io/codecov/c/github/google/caliban/master.svg?maxAge=3600)](https://codecov.io/github/google/caliban)
-        [![JOSS](https://joss.theoj.org/papers/c33c8b464103b2fb3b641878722bf8f3/status.svg)](https://joss.theoj.org/papers/c33c8b464103b2fb3b641878722bf8f3)
-        [![readthedocs](https://img.shields.io/readthedocs/caliban?maxAge=3600)](https://caliban.readthedocs.io/en/latest/?badge=latest)
-        [![caliban version](https://img.shields.io/pypi/v/caliban?maxAge=3600)](https://pypi.org/project/caliban)
-        
-        Caliban is a tool that helps researchers launch and track their numerical
-        experiments in an isolated, reproducible computing environment. It was developed
-        by machine learning researchers and engineers, and makes it easy to go from a
-        simple prototype running on a workstation to thousands of experimental jobs
-        running on Cloud.
-        
-        With Caliban, you can:
-        
-        - Develop your experimental code locally and test it inside an isolated (Docker)
-          environment
-        - Easily sweep over experimental parameters
-        - Submit your experiments as Cloud jobs, where they will run in the same
-          isolated environment
-        - Control and keep track of jobs
-        
-        ## Quickstart
-        
-        [Install Docker](#docker), make sure it's running, then install Caliban (you'll need [Python >= 3.6](#python-36)):
-        
-        ```bash
-        pip install caliban
-        ```
-        
-        Train a simple deep learning model on your local machine:
-        
-        ```bash
-        git clone https://github.com/google/caliban.git && cd caliban/tutorials/basic
-        caliban run --nogpu mnist.py
-        ```
-        
-        Sweep over learning rates to find the best one (flags are specified in JSON format):
-        
-        ```bash
-        echo '{"learning_rate": [0.01, 0.001, 0.0001]}' | caliban run --experiment_config stdin --nogpu mnist.py
-        ```
-        
-        **Next**:
-        
-        - See how to submit the experiment to Cloud and use other Caliban features in ["Getting Started with Caliban"](#getting-started-with-caliban)
-        - See [Installation](#installation-and-prerequisites) for detailed installation instructions
-        - Read the [Command Overview](#command-overview) for info on Caliban commands.
-        
-        Full documentation for Caliban lives at [Read The Docs](https://caliban.readthedocs.io/en/latest).
-        
-        ### Dramatic Interlude
-        
-        <p>
-        <img style="float: right;" align="right" src="https://upload.wikimedia.org/wikipedia/commons/a/ad/Stephano%2C_Trinculo_and_Caliban_dancing_from_The_Tempest_by_Johann_Heinrich_Ramberg.jpg" width="350">
-        
-        > “Be not afeard; the isle is full of noises, \
-        > Sounds, and sweet airs, that give delight and hurt not. \
-        > Sometimes a thousand twangling instruments \
-        > Will hum about mine ears; and sometime voices, \
-        > That, if I then had waked after long sleep, \
-        > Will make me sleep again: and then, in dreaming, \
-        > The clouds methought would open, and show riches \
-        > Ready to drop upon me; that, when I waked, \
-        > I cried to dream again.”
-        >
-        > -- <cite>Shakespeare, The Tempest</cite>
-        </p>
-        
-        ## Installation and Prerequisites
-        
-        Caliban's prequisites are [Docker](#docker) and [Python >= 3.6](#python-36).
-        
-        Make sure your Python is up to date:
-        
-        ```bash
-        $ python --version
-        Python 3.6.9 # should be >=3.6.0
-        ```
-        
-        If not, visit ["Installing Python 3.6"](#python-36) before proceeding.
-        
-        Next, install Caliban via [pip](https://pypi.org/project/caliban/):
-        
-        ```bash
-        pip install -U caliban
-        ```
-        
-        check if your installation worked by navigating to an empty folder and running
-        `caliban --help`. You should see the usage dialogue:
-        
-        ```bash
-        $ caliban --help
-        usage: caliban [-h] [--helpfull] [--version]
-                       {shell,notebook,build,run,cloud,cluster,status,stop,resubmit}
-                       ...
-        ```
-        
-        ### Docker
-        
-        Caliban executes your code inside a "container", managed by
-        [Docker](https://hub.docker.com/editions/community/docker-ce-desktop-mac). To get Docker:
-        
-        - On MacOS, follow the installation instructions at [Docker
-          Desktop](https://hub.docker.com/editions/community/docker-ce-desktop-mac) and
-          start the newly-installed Docker Desktop application.
-        - On Linux, visit the [Docker installation
-          instructions](https://docs.docker.com/engine/install/ubuntu/#installation-methods).
-          (It's important that you configure [sudo-less
-          Docker](https://caliban.readthedocs.io/en/latest/getting_started/prerequisites.html#docker)
-          and start Docker running on your machine.)
-        
-        Make sure Docker is correctly installed, configured and running by executing the
-        following command:
-        
-        ```bash
-        docker run hello-world
-        ```
-        
-        You should see output that looks like this:
-        
-        ```text
-        ...
-        Hello from Docker!
-        This message shows that your installation appears to be working correctly.
-        ...
-        ```
-        
-        ### Python 3.6
-        
-        Make sure your Python version is up to date:
-        
-        ```bash
-        $ python --version
-        Python 3.6.9 # should be >=3.6.0
-        ```
-        
-        If you need to upgrade:
-        
-        - On MacOS, install the latest Python version from
-          [python.org](https://www.python.org/downloads/mac-osx) ([direct
-          link](https://www.python.org/ftp/python/3.8.3/python-3.8.3-macosx10.9.pkg)).
-        - On Linux, run `sudo apt-get update && sudo apt-get install python3.7`.
-        
-        ### Cloud Submission and GPUs
-        
-        Caliban's [Read the Docs](https://caliban.readthedocs.io/) documentation has
-        instructions on:
-        
-        - [Installing the `nvidia-docker2`
-          runtime](https://caliban.readthedocs.io/en/latest/getting_started/prerequisites.html#docker-and-cuda),
-          so you can use Caliban to run jobs that use your Linux machine's GPU.
-        - [Setting up a Google Cloud
-          account](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
-          so you can submit your code to Google's [Cloud AI
-          Platform](https://cloud.google.com/ai-platform) with `caliban cloud`.
-        
-        ## Getting Started with Caliban
-        
-        In this section we will use Caliban to train an image classification network
-        (implemented in
-        [TensorFlow](https://www.tensorflow.org/tutorials/quickstart/beginner)). We
-        will:
-        
-        - Train a neural network on the local machine
-        - Increase the model's accuracy by changing the [learning
-          rate](https://medium.com/octavian-ai/which-optimizer-and-learning-rate-should-i-use-for-deep-learning-5acb418f9b2)
-          with a command-line flag
-        - Sweep across a range of learning rates with Caliban's [experiment
-          broadcasting](https://caliban.readthedocs.io/en/latest/explore/experiment_broadcasting.html)
-          feature
-        - Train the model in the Cloud on Google's [AI
-          Platform](https://cloud.google.com/ai-platform)
-        - Develop code interactively using `caliban shell` in the exact same
-          environment.
-        
-        ### Preparing your Project
-        
-        Create an empty directory and use `curl` to download a [python
-        script](https://github.com/google/caliban/blob/master/tutorials/basic/mnist.py#L16)
-        that trains a basic neural network.
-        
-        ```
-        mkdir demo && cd demo
-        curl --output mnist.py https://raw.githubusercontent.com/google/caliban/master/tutorials/basic/mnist.py
-        ```
-        
-        Create a file called `requirements.txt` to declare `tensorflow-cpu` as a dependency:
-        
-        ```bash
-        echo "tensorflow-cpu" > requirements.txt
-        ```
-        
-        Caliban will automatically make any entry in `requirements.txt` available when
-        you run your code. See ["Declaring
-        Requirements"](https://caliban.readthedocs.io/en/latest/explore/declaring_requirements.html)
-        for more information.
-        
-        ### Training the Network
-        
-        Run this command to train your first ML model:
-        
-        ```bash
-        caliban run --nogpu mnist.py
-        ```
-        
-        You should see a stream of output ending in this:
-        
-        ```text
-        Training model with learning rate=0.1 for 3 epochs.
-        Epoch 1/3
-        1875/1875 - 3s - loss: 2.0989 - accuracy: 0.2506
-        Epoch 2/3
-        1875/1875 - 3s - loss: 1.9222 - accuracy: 0.2273
-        Epoch 3/3
-        1875/1875 - 3s - loss: 2.0777 - accuracy: 0.1938
-        Model performance:
-        313/313 - 0s - loss: 2.0973 - accuracy: 0.1858
-        ```
-        
-        Your model was able to recognize digits from the
-        [MNIST](https://en.wikipedia.org/wiki/MNIST_database) dataset with 18.58%
-        accuracy. Can we do better?
-        
-        ### Improving the Model
-        
-        The default learning rate is `0.1`. Run the code again with a smaller learning
-        rate by passing a command-line flag, separated from your original command by
-        `--`:
-        
-        ```bash
-        $ caliban run --nogpu mnist.py -- --learning_rate 0.01
-        
-        <<elided>>
-        
-        Training model with learning rate=0.01 for 3 epochs.
-        Epoch 1/3
-        1875/1875 - 4s - loss: 0.2676 - accuracy: 0.9221
-        Epoch 2/3
-        1875/1875 - 4s - loss: 0.1863 - accuracy: 0.9506
-        Epoch 3/3
-        1875/1875 - 4s - loss: 0.1567 - accuracy: 0.9585
-        Model performance:
-        313/313 - 0s - loss: 0.1410 - accuracy: 0.9642
-        ```
-        
-        96% accuracy! Much better! Can we do better still?
-        
-        ### Experiment Broadcasting
-        
-        Caliban's [experiment
-        broadcasting](https://caliban.readthedocs.io/en/latest/explore/experiment_broadcasting.html)
-        feature will allow us to run many jobs with different sets of arguments.
-        
-        Create a file called `experiment.json` with a
-        [JSON](https://www.json.org/json-en.html) dictionary of the format
-        `{"flag_name": ["list", "of", "values"]}`:
-        
-        ```bash
-        echo '{"learning_rate": [0.01, 0.001, 0.0001]}' > experiment.json
-        ```
-        
-        Pass the config with `--experiment_config` and run again:
-        
-        ```bash
-        caliban run --experiment_config experiment.json --nogpu mnist.py
-        ```
-        
-        You should see accuracies of roughly `0.9493`, `0.9723` and `0.9537`. Looks like
-        `0.001` is a nice choice.
-        
-        ### Submitting to Cloud AI Platform
-        
-        Now it's time to submit the job to [Cloud AI
-        Platform](https://cloud.google.com/ai-platform).
-        
-        (**NOTE**: This section requires a Google Cloud account. You can create a free
-        account with $300 of credit to get started. Follow Caliban's ["Getting Started
-        with Google
-        Cloud"](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
-        documentation, then come back here to proceed.)
-        
-        Submit the job to AI Platform by changing the word `run` to `cloud`:
-        
-        ```bash
-        caliban cloud --nogpu mnist.py -- --learning_rate 0.01
-        ```
-        
-        You should see output like this:
-        
-        ```bash
-        I0615 19:57:43.354172 4563361216 core.py:161] Job 1 - jobId: caliban_totoro_1, image: gcr.io/research-3141/974a776e6037:latest
-        I0615 19:57:43.354712 4563361216 core.py:161] Job 1 - Accelerator: {'count': 0, 'type': 'ACCELERATOR_TYPE_UNSPECIFIED'}, machine: 'n1-highcpu-32', region: 'us-central1'
-        I0615 19:57:43.355082 4563361216 core.py:161] Job 1 - Experiment arguments: ['--learning_rate', '0.01']
-        I0615 19:57:43.355440 4563361216 core.py:161] Job 1 - labels: {'gpu_enabled': 'false', 'tpu_enabled': 'false', 'job_name': 'caliban_totoro', 'learning_rate': '0_01'}
-        
-        I0615 19:57:43.356621 4563361216 core.py:324] Submitting request!
-        I0615 19:57:45.078382 4563361216 core.py:97] Request for job 'caliban_totoro_20200615_195743_1' succeeded!
-        I0615 19:57:45.078989 4563361216 core.py:98] Job URL: https://console.cloud.google.com/ai-platform/jobs/caliban_totoro_20200615_195743_1?projectId=totoro-project
-        I0615 19:57:45.079524 4563361216 core.py:100] Streaming log CLI command: $ gcloud ai-platform jobs stream-logs caliban_totoro_20200615_195743_1
-        Submitting caliban_totoro_1: 100%|####################################################################################################################################################################################| 1/1 [00:02<00:00,  2.65s/requests]
-        I0615 19:57:45.405600 4563361216 core.py:673]
-        I0615 19:57:45.405819 4563361216 core.py:676] Visit https://console.cloud.google.com/ai-platform/jobs/?projectId=research-3141 to see the status of all jobs.
-        I0615 19:57:45.405959 4563361216 core.py:677]
-        ```
-        
-        This output means that Caliban has:
-        
-        - built a Docker container with all of your code
-        - Pushed that container up to Google Cloud's [Container
-          Registry](https://cloud.google.com/container-registry)
-        - Submitted the job to [AI Platform](https://cloud.google.com/ai-platform).
-        
-        You can now visit the link in the output that looks like:
-        https://console.cloud.google.com/ai-platform/jobs/caliban_totoro_20200615_195743_1?projectId=totoro-project
-        to see all of your job's logs.
-        
-        #### Why do I need Cloud?
-        
-        With Google Cloud, you can use on-demand
-        [GPUs](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html) and
-        [TPUs](https://caliban.readthedocs.io/en/latest/cloud/ai_platform_tpu.html) and
-        train models on large datasets at very high speeds. You can also customize the
-        [machine
-        type](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html#custom-machine-types)
-        that AI Platform uses to run your job. You might need high memory or more CPU,
-        for example.
-        
-        See Caliban's ["Customizing Machines and
-        GPUs"](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html#) for more
-        information.
-        
-        ### Interactive Development with `caliban shell`
-        
-        [`caliban
-        shell`](https://caliban.readthedocs.io/en/latest/cli/caliban_shell.html) lets
-        you develop code interactively inside of the exact same environment that your
-        code will have available, locally during `caliban run` or in the Cloud with
-        `caliban cloud`.
-        
-        Run the following command to activate the shell:
-        
-        ```bash
-        caliban shell --nogpu
-        ```
-        
-        You should see Caliban's terminal:
-        
-        ```
-        I0611 12:33:17.551121 4500135360 docker.py:911] Running command: docker run --ipc host -w /usr/app -u 735994:89939 -v /Users/totoro/code/example:/usr/app -it --entrypoint /bin/bash -v /Users/totoro:/home/totoro ab8a7d7db868
-           _________    __    ________  ___    _   __  __  __
-          / ____/   |  / /   /  _/ __ )/   |  / | / /  \ \ \ \
-         / /   / /| | / /    / // __  / /| | /  |/ /    \ \ \ \
-        / /___/ ___ |/ /____/ // /_/ / ___ |/ /|  /     / / / /
-        \____/_/  |_/_____/___/_____/_/  |_/_/ |_/     /_/ /_/
-        
-        You are running caliban shell as user with ID 735994 and group 89939,
-        which should map to the ID and group for your user on the Docker host. Great!
-        
-        [totoro@6a9b28990757 /usr/app]$
-        ```
-        
-        You're now living in an isolated [Docker
-        container](https://www.docker.com/resources/what-container) with your
-        `tensorflow-cpu` dependency available (and any others [you've
-        declared](https://caliban.readthedocs.io/en/latest/explore/declaring_requirements.html)).
-        
-        Run the `python` command and check that `tensorflow` is installed:
-        
-        ```bash
-        $ python
-        Python 3.6.9 (default, Nov  7 2019, 10:44:02)
-        [GCC 8.3.0] on linux
-        Type "help", "copyright", "credits" or "license" for more information.
-        >>> import tensorflow as tf
-        >>> tf.__version__
-        '2.2.0'
-        ```
-        
-        Your home directory and the folder where you ran the command are both mounted
-        into this isolated environment, so any changes you make to either of those
-        directories will be reflected immediately.
-        
-        Any code you add to the current folder and edit on your computer will be
-        available in this special Caliban shell. Run the example from before like this:
-        
-        ```
-        python mnist.py --learning_rate 0.01
-        ```
-        
-        If your code runs in `caliban shell`, you can be almost certain that your code
-        will execute in a Cloud environment, with potentially many GPUs attached and
-        much larger machines available.
-        
-        ### What next?
-        
-        Read the [Overview](#overview) for more information on Caliban's subcommands,
-        then head over to [Caliban's documentation
-        site](https://caliban.readthedocs.io/en/latest/) and check out the links on the
-        sidebar.
-        
-        If you find anything confusing, please feel free to [create an
-        issue](https://github.com/google/caliban/issues) on our [Github Issues
-        page](https://github.com/google/caliban/issues), and we'll get you sorted out.
-        
-        ## Command Overview
-        
-        Caliban provides seven subcommands that you run inside some project directory on
-        your machine:
-        
-        * [`caliban
-          shell`](https://caliban.readthedocs.io/en/latest/cli/caliban_shell.html)
-          generates a Docker image containing any dependencies you've declared in a
-          `requirements.txt` and/or `setup.py` in the directory and opens an interactive
-          shell in that directory. The `caliban shell` environment is ~identical to the
-          environment that will be available to your code when you submit it to AI
-          Platform; the difference is that your current directory is live-mounted into
-          the container, so you can develop interactively.
-        
-        * [`caliban
-          notebook`](https://caliban.readthedocs.io/en/latest/cli/caliban_notebook.html)
-          starts a Jupyter notebook or lab instance inside of a Docker image containing
-          your dependencies; the guarantee about an environment identical to AI Platform
-          applies here as well.
-        
-        * [`caliban run`](https://caliban.readthedocs.io/en/latest/cli/caliban_run.html)
-          packages your directory's code into the Docker image and executes it locally
-          using `docker run`. If you have a GPU, the instance will attach to it by
-          default - no need to install the CUDA toolkit. The Docker environment takes
-          care of all that. This environment is truly identical to the AI Platform
-          environment. The Docker image that runs locally is the same image that will
-          run in AI Platform.
-        
-        * [`caliban
-          cloud`](https://caliban.readthedocs.io/en/latest/cli/caliban_cloud.html)
-          allows you to [submit jobs to AI
-          Platform](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
-          that will run inside the same Docker image you used with `caliban run`. You
-          can submit hundreds of jobs at once. Any machine type, GPU count, and GPU type
-          combination you specify will be validated client side, so you'll see an
-          immediate error with suggestions, rather than having to debug by submitting
-          jobs over and over.
-        
-        * [`caliban
-          build`](https://caliban.readthedocs.io/en/latest/cli/caliban_build.html) builds
-          the Docker image used in `caliban cloud` and `caliban run` without actually
-          running the container or submitting any code.
-        
-        * [`caliban
-          cluster`](https://caliban.readthedocs.io/en/latest/cli/caliban_cluster.html)
-          creates GKE clusters and submits jobs to GKE clusters.
-        
-        * [`caliban
-          status`](https://caliban.readthedocs.io/en/latest/cli/caliban_status.html)
-          displays information about all jobs submitted by Caliban, and makes it easy to
-          interact with large groups of experiments. Use `caliban status` when you need
-          to cancel pending jobs, or re-build a container and resubmit a batch of
-          experiments after fixing a bug.
-        
-        ## Disclaimer
-        
-        This is a research project, not an official Google product. Expect bugs and
-        sharp edges. Please help by trying out Caliban, [reporting
-        bugs](https://github.com/google/caliban/issues), and letting us know what you
-        think!
-        
-        ## Get Involved + Get Support
-        
-        Pull requests and bug reports are always welcome! Check out our [Contributor's
-        Guide](CONTRIBUTING.md) for information on how to get started contributing to
-        Caliban.
-        
-        The TL;DR; is:
-        
-        - send us a pull request,
-        - iterate on the feedback + discussion, and
-        - get a +1 from a [Committer](COMMITTERS.md)
-        
-        in order to get your PR accepted.
-        
-        Issues should be reported on the [GitHub issue
-        tracker](https://github.com/google/caliban/issues).
-        
-        If you want to discuss an idea for a new feature or ask us a question,
-        discussion occurs primarily in the body of [Github
-        Issues](https://github.com/google/caliban/issues), though the project is growing
-        large enough that we may start a Gitter channel soon.
-        
-        The current list of active committers (who can +1 a pull request) can be found
-        here: [COMMITTERS.md](COMMITTERS.md)
-        
-        A list of contributors to the project can be found at the project's
-        [Contributors](https://github.com/google/caliban/graphs/contributors) page.
-        
-        ## Citing Caliban
-        
-        If Caliban helps you in your research, please consider citing the repository:
-        
-        ```
-        @software{caliban2020github,
-          author = {Sam Ritchie and Ambrose Slone and Vinay Ramasesh},
-          title = {{Caliban}: Docker-based job manager for reproducible workflows},
-          url = {http://github.com/google/caliban},
-          version = {0.2.5},
-          year = {2020},
-        }
-        ```
-        
-        In the above bibtex entry, the version number is intended to be that of the
-        latest tag on github, and the year corresponds to the project's open-source
-        release.
-        
-        ## License
-        
-        Copyright 2020 Google LLC.
-        
-        Licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
-        
-Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_SHORT
+
+# Caliban
+
+[![Build status](https://github.com/google/caliban/workflows/build/badge.svg?branch=master)](https://github.com/google/caliban/actions?query=workflow%3Abuild+branch%3Amaster)
+[![Codecov branch](https://img.shields.io/codecov/c/github/google/caliban/master.svg?maxAge=3600)](https://codecov.io/github/google/caliban)
+[![JOSS](https://joss.theoj.org/papers/c33c8b464103b2fb3b641878722bf8f3/status.svg)](https://joss.theoj.org/papers/c33c8b464103b2fb3b641878722bf8f3)
+[![readthedocs](https://img.shields.io/readthedocs/caliban?maxAge=3600)](https://caliban.readthedocs.io/en/latest/?badge=latest)
+[![caliban version](https://img.shields.io/pypi/v/caliban?maxAge=3600)](https://pypi.org/project/caliban)
+
+Caliban is a tool that helps researchers launch and track their numerical
+experiments in an isolated, reproducible computing environment. It was developed
+by machine learning researchers and engineers, and makes it easy to go from a
+simple prototype running on a workstation to thousands of experimental jobs
+running on Cloud.
+
+With Caliban, you can:
+
+- Develop your experimental code locally and test it inside an isolated (Docker)
+  environment
+- Easily sweep over experimental parameters
+- Submit your experiments as Cloud jobs, where they will run in the same
+  isolated environment
+- Control and keep track of jobs
+
+## Quickstart
+
+[Install Docker](#docker), make sure it's running, then install Caliban (you'll need [Python >= 3.6](#python-36)):
+
+```bash
+pip install caliban
+```
+
+Train a simple deep learning model on your local machine:
+
+```bash
+git clone https://github.com/google/caliban.git && cd caliban/tutorials/basic
+caliban run --nogpu mnist.py
+```
+
+Sweep over learning rates to find the best one (flags are specified in JSON format):
+
+```bash
+echo '{"learning_rate": [0.01, 0.001, 0.0001]}' | caliban run --experiment_config stdin --nogpu mnist.py
+```
+
+**Next**:
+
+- See how to submit the experiment to Cloud and use other Caliban features in ["Getting Started with Caliban"](#getting-started-with-caliban)
+- See [Installation](#installation-and-prerequisites) for detailed installation instructions
+- Read the [Command Overview](#command-overview) for info on Caliban commands.
+
+Full documentation for Caliban lives at [Read The Docs](https://caliban.readthedocs.io/en/latest).
+
+### Dramatic Interlude
+
+<p>
+<img style="float: right;" align="right" src="https://upload.wikimedia.org/wikipedia/commons/a/ad/Stephano%2C_Trinculo_and_Caliban_dancing_from_The_Tempest_by_Johann_Heinrich_Ramberg.jpg" width="350">
+
+> “Be not afeard; the isle is full of noises, \
+> Sounds, and sweet airs, that give delight and hurt not. \
+> Sometimes a thousand twangling instruments \
+> Will hum about mine ears; and sometime voices, \
+> That, if I then had waked after long sleep, \
+> Will make me sleep again: and then, in dreaming, \
+> The clouds methought would open, and show riches \
+> Ready to drop upon me; that, when I waked, \
+> I cried to dream again.”
+>
+> -- <cite>Shakespeare, The Tempest</cite>
+</p>
+
+## Installation and Prerequisites
+
+Caliban's prequisites are [Docker](#docker) and [Python >= 3.6](#python-36).
+
+Make sure your Python is up to date:
+
+```bash
+$ python --version
+Python 3.6.9 # should be >=3.6.0
+```
+
+If not, visit ["Installing Python 3.6"](#python-36) before proceeding.
+
+Next, install Caliban via [pip](https://pypi.org/project/caliban/):
+
+```bash
+pip install -U caliban
+```
+
+check if your installation worked by navigating to an empty folder and running
+`caliban --help`. You should see the usage dialogue:
+
+```bash
+$ caliban --help
+usage: caliban [-h] [--helpfull] [--version]
+               {shell,notebook,build,run,cloud,cluster,status,stop,resubmit}
+               ...
+```
+
+### Docker
+
+Caliban executes your code inside a "container", managed by
+[Docker](https://hub.docker.com/editions/community/docker-ce-desktop-mac). To get Docker:
+
+- On MacOS, follow the installation instructions at [Docker
+  Desktop](https://hub.docker.com/editions/community/docker-ce-desktop-mac) and
+  start the newly-installed Docker Desktop application.
+- On Linux, visit the [Docker installation
+  instructions](https://docs.docker.com/engine/install/ubuntu/#installation-methods).
+  (It's important that you configure [sudo-less
+  Docker](https://caliban.readthedocs.io/en/latest/getting_started/prerequisites.html#docker)
+  and start Docker running on your machine.)
+
+Make sure Docker is correctly installed, configured and running by executing the
+following command:
+
+```bash
+docker run hello-world
+```
+
+You should see output that looks like this:
+
+```text
+...
+Hello from Docker!
+This message shows that your installation appears to be working correctly.
+...
+```
+
+### Python 3.6
+
+Make sure your Python version is up to date:
+
+```bash
+$ python --version
+Python 3.6.9 # should be >=3.6.0
+```
+
+If you need to upgrade:
+
+- On MacOS, install the latest Python version from
+  [python.org](https://www.python.org/downloads/mac-osx) ([direct
+  link](https://www.python.org/ftp/python/3.8.3/python-3.8.3-macosx10.9.pkg)).
+- On Linux, run `sudo apt-get update && sudo apt-get install python3.7`.
+
+### Cloud Submission and GPUs
+
+Caliban's [Read the Docs](https://caliban.readthedocs.io/) documentation has
+instructions on:
+
+- [Installing the `nvidia-docker2`
+  runtime](https://caliban.readthedocs.io/en/latest/getting_started/prerequisites.html#docker-and-cuda),
+  so you can use Caliban to run jobs that use your Linux machine's GPU.
+- [Setting up a Google Cloud
+  account](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
+  so you can submit your code to Google's [Cloud AI
+  Platform](https://cloud.google.com/ai-platform) with `caliban cloud`.
+
+## Getting Started with Caliban
+
+In this section we will use Caliban to train an image classification network
+(implemented in
+[TensorFlow](https://www.tensorflow.org/tutorials/quickstart/beginner)). We
+will:
+
+- Train a neural network on the local machine
+- Increase the model's accuracy by changing the [learning
+  rate](https://medium.com/octavian-ai/which-optimizer-and-learning-rate-should-i-use-for-deep-learning-5acb418f9b2)
+  with a command-line flag
+- Sweep across a range of learning rates with Caliban's [experiment
+  broadcasting](https://caliban.readthedocs.io/en/latest/explore/experiment_broadcasting.html)
+  feature
+- Train the model in the Cloud on Google's [AI
+  Platform](https://cloud.google.com/ai-platform)
+- Develop code interactively using `caliban shell` in the exact same
+  environment.
+
+### Preparing your Project
+
+Create an empty directory and use `curl` to download a [python
+script](https://github.com/google/caliban/blob/master/tutorials/basic/mnist.py#L16)
+that trains a basic neural network.
+
+```
+mkdir demo && cd demo
+curl --output mnist.py https://raw.githubusercontent.com/google/caliban/master/tutorials/basic/mnist.py
+```
+
+Create a file called `requirements.txt` to declare `tensorflow-cpu` as a dependency:
+
+```bash
+echo "tensorflow-cpu" > requirements.txt
+```
+
+Caliban will automatically make any entry in `requirements.txt` available when
+you run your code. See ["Declaring
+Requirements"](https://caliban.readthedocs.io/en/latest/explore/declaring_requirements.html)
+for more information.
+
+### Training the Network
+
+Run this command to train your first ML model:
+
+```bash
+caliban run --nogpu mnist.py
+```
+
+You should see a stream of output ending in this:
+
+```text
+Training model with learning rate=0.1 for 3 epochs.
+Epoch 1/3
+1875/1875 - 3s - loss: 2.0989 - accuracy: 0.2506
+Epoch 2/3
+1875/1875 - 3s - loss: 1.9222 - accuracy: 0.2273
+Epoch 3/3
+1875/1875 - 3s - loss: 2.0777 - accuracy: 0.1938
+Model performance:
+313/313 - 0s - loss: 2.0973 - accuracy: 0.1858
+```
+
+Your model was able to recognize digits from the
+[MNIST](https://en.wikipedia.org/wiki/MNIST_database) dataset with 18.58%
+accuracy. Can we do better?
+
+### Improving the Model
+
+The default learning rate is `0.1`. Run the code again with a smaller learning
+rate by passing a command-line flag, separated from your original command by
+`--`:
+
+```bash
+$ caliban run --nogpu mnist.py -- --learning_rate 0.01
+
+<<elided>>
+
+Training model with learning rate=0.01 for 3 epochs.
+Epoch 1/3
+1875/1875 - 4s - loss: 0.2676 - accuracy: 0.9221
+Epoch 2/3
+1875/1875 - 4s - loss: 0.1863 - accuracy: 0.9506
+Epoch 3/3
+1875/1875 - 4s - loss: 0.1567 - accuracy: 0.9585
+Model performance:
+313/313 - 0s - loss: 0.1410 - accuracy: 0.9642
+```
+
+96% accuracy! Much better! Can we do better still?
+
+### Experiment Broadcasting
+
+Caliban's [experiment
+broadcasting](https://caliban.readthedocs.io/en/latest/explore/experiment_broadcasting.html)
+feature will allow us to run many jobs with different sets of arguments.
+
+Create a file called `experiment.json` with a
+[JSON](https://www.json.org/json-en.html) dictionary of the format
+`{"flag_name": ["list", "of", "values"]}`:
+
+```bash
+echo '{"learning_rate": [0.01, 0.001, 0.0001]}' > experiment.json
+```
+
+Pass the config with `--experiment_config` and run again:
+
+```bash
+caliban run --experiment_config experiment.json --nogpu mnist.py
+```
+
+You should see accuracies of roughly `0.9493`, `0.9723` and `0.9537`. Looks like
+`0.001` is a nice choice.
+
+### Submitting to Cloud AI Platform
+
+Now it's time to submit the job to [Cloud AI
+Platform](https://cloud.google.com/ai-platform).
+
+(**NOTE**: This section requires a Google Cloud account. You can create a free
+account with $300 of credit to get started. Follow Caliban's ["Getting Started
+with Google
+Cloud"](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
+documentation, then come back here to proceed.)
+
+Submit the job to AI Platform by changing the word `run` to `cloud`:
+
+```bash
+caliban cloud --nogpu mnist.py -- --learning_rate 0.01
+```
+
+You should see output like this:
+
+```bash
+I0615 19:57:43.354172 4563361216 core.py:161] Job 1 - jobId: caliban_totoro_1, image: gcr.io/research-3141/974a776e6037:latest
+I0615 19:57:43.354712 4563361216 core.py:161] Job 1 - Accelerator: {'count': 0, 'type': 'ACCELERATOR_TYPE_UNSPECIFIED'}, machine: 'n1-highcpu-32', region: 'us-central1'
+I0615 19:57:43.355082 4563361216 core.py:161] Job 1 - Experiment arguments: ['--learning_rate', '0.01']
+I0615 19:57:43.355440 4563361216 core.py:161] Job 1 - labels: {'gpu_enabled': 'false', 'tpu_enabled': 'false', 'job_name': 'caliban_totoro', 'learning_rate': '0_01'}
+
+I0615 19:57:43.356621 4563361216 core.py:324] Submitting request!
+I0615 19:57:45.078382 4563361216 core.py:97] Request for job 'caliban_totoro_20200615_195743_1' succeeded!
+I0615 19:57:45.078989 4563361216 core.py:98] Job URL: https://console.cloud.google.com/ai-platform/jobs/caliban_totoro_20200615_195743_1?projectId=totoro-project
+I0615 19:57:45.079524 4563361216 core.py:100] Streaming log CLI command: $ gcloud ai-platform jobs stream-logs caliban_totoro_20200615_195743_1
+Submitting caliban_totoro_1: 100%|####################################################################################################################################################################################| 1/1 [00:02<00:00,  2.65s/requests]
+I0615 19:57:45.405600 4563361216 core.py:673]
+I0615 19:57:45.405819 4563361216 core.py:676] Visit https://console.cloud.google.com/ai-platform/jobs/?projectId=research-3141 to see the status of all jobs.
+I0615 19:57:45.405959 4563361216 core.py:677]
+```
+
+This output means that Caliban has:
+
+- built a Docker container with all of your code
+- Pushed that container up to Google Cloud's [Container
+  Registry](https://cloud.google.com/container-registry)
+- Submitted the job to [AI Platform](https://cloud.google.com/ai-platform).
+
+You can now visit the link in the output that looks like:
+https://console.cloud.google.com/ai-platform/jobs/caliban_totoro_20200615_195743_1?projectId=totoro-project
+to see all of your job's logs.
+
+#### Why do I need Cloud?
+
+With Google Cloud, you can use on-demand
+[GPUs](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html) and
+[TPUs](https://caliban.readthedocs.io/en/latest/cloud/ai_platform_tpu.html) and
+train models on large datasets at very high speeds. You can also customize the
+[machine
+type](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html#custom-machine-types)
+that AI Platform uses to run your job. You might need high memory or more CPU,
+for example.
+
+See Caliban's ["Customizing Machines and
+GPUs"](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html#) for more
+information.
+
+### Interactive Development with `caliban shell`
+
+[`caliban
+shell`](https://caliban.readthedocs.io/en/latest/cli/caliban_shell.html) lets
+you develop code interactively inside of the exact same environment that your
+code will have available, locally during `caliban run` or in the Cloud with
+`caliban cloud`.
+
+Run the following command to activate the shell:
+
+```bash
+caliban shell --nogpu
+```
+
+You should see Caliban's terminal:
+
+```
+I0611 12:33:17.551121 4500135360 docker.py:911] Running command: docker run --ipc host -w /usr/app -u 735994:89939 -v /Users/totoro/code/example:/usr/app -it --entrypoint /bin/bash -v /Users/totoro:/home/totoro ab8a7d7db868
+   _________    __    ________  ___    _   __  __  __
+  / ____/   |  / /   /  _/ __ )/   |  / | / /  \ \ \ \
+ / /   / /| | / /    / // __  / /| | /  |/ /    \ \ \ \
+/ /___/ ___ |/ /____/ // /_/ / ___ |/ /|  /     / / / /
+\____/_/  |_/_____/___/_____/_/  |_/_/ |_/     /_/ /_/
+
+You are running caliban shell as user with ID 735994 and group 89939,
+which should map to the ID and group for your user on the Docker host. Great!
+
+[totoro@6a9b28990757 /usr/app]$
+```
+
+You're now living in an isolated [Docker
+container](https://www.docker.com/resources/what-container) with your
+`tensorflow-cpu` dependency available (and any others [you've
+declared](https://caliban.readthedocs.io/en/latest/explore/declaring_requirements.html)).
+
+Run the `python` command and check that `tensorflow` is installed:
+
+```bash
+$ python
+Python 3.6.9 (default, Nov  7 2019, 10:44:02)
+[GCC 8.3.0] on linux
+Type "help", "copyright", "credits" or "license" for more information.
+>>> import tensorflow as tf
+>>> tf.__version__
+'2.2.0'
+```
+
+Your home directory and the folder where you ran the command are both mounted
+into this isolated environment, so any changes you make to either of those
+directories will be reflected immediately.
+
+Any code you add to the current folder and edit on your computer will be
+available in this special Caliban shell. Run the example from before like this:
+
+```
+python mnist.py --learning_rate 0.01
+```
+
+If your code runs in `caliban shell`, you can be almost certain that your code
+will execute in a Cloud environment, with potentially many GPUs attached and
+much larger machines available.
+
+### What next?
+
+Read the [Overview](#overview) for more information on Caliban's subcommands,
+then head over to [Caliban's documentation
+site](https://caliban.readthedocs.io/en/latest/) and check out the links on the
+sidebar.
+
+If you find anything confusing, please feel free to [create an
+issue](https://github.com/google/caliban/issues) on our [Github Issues
+page](https://github.com/google/caliban/issues), and we'll get you sorted out.
+
+## Command Overview
+
+Caliban provides seven subcommands that you run inside some project directory on
+your machine:
+
+* [`caliban
+  shell`](https://caliban.readthedocs.io/en/latest/cli/caliban_shell.html)
+  generates a Docker image containing any dependencies you've declared in a
+  `requirements.txt` and/or `setup.py` in the directory and opens an interactive
+  shell in that directory. The `caliban shell` environment is ~identical to the
+  environment that will be available to your code when you submit it to AI
+  Platform; the difference is that your current directory is live-mounted into
+  the container, so you can develop interactively.
+
+* [`caliban
+  notebook`](https://caliban.readthedocs.io/en/latest/cli/caliban_notebook.html)
+  starts a Jupyter notebook or lab instance inside of a Docker image containing
+  your dependencies; the guarantee about an environment identical to AI Platform
+  applies here as well.
+
+* [`caliban run`](https://caliban.readthedocs.io/en/latest/cli/caliban_run.html)
+  packages your directory's code into the Docker image and executes it locally
+  using `docker run`. If you have a GPU, the instance will attach to it by
+  default - no need to install the CUDA toolkit. The Docker environment takes
+  care of all that. This environment is truly identical to the AI Platform
+  environment. The Docker image that runs locally is the same image that will
+  run in AI Platform.
+
+* [`caliban
+  cloud`](https://caliban.readthedocs.io/en/latest/cli/caliban_cloud.html)
+  allows you to [submit jobs to AI
+  Platform](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
+  that will run inside the same Docker image you used with `caliban run`. You
+  can submit hundreds of jobs at once. Any machine type, GPU count, and GPU type
+  combination you specify will be validated client side, so you'll see an
+  immediate error with suggestions, rather than having to debug by submitting
+  jobs over and over.
+
+* [`caliban
+  build`](https://caliban.readthedocs.io/en/latest/cli/caliban_build.html) builds
+  the Docker image used in `caliban cloud` and `caliban run` without actually
+  running the container or submitting any code.
+
+* [`caliban
+  cluster`](https://caliban.readthedocs.io/en/latest/cli/caliban_cluster.html)
+  creates GKE clusters and submits jobs to GKE clusters.
+
+* [`caliban
+  status`](https://caliban.readthedocs.io/en/latest/cli/caliban_status.html)
+  displays information about all jobs submitted by Caliban, and makes it easy to
+  interact with large groups of experiments. Use `caliban status` when you need
+  to cancel pending jobs, or re-build a container and resubmit a batch of
+  experiments after fixing a bug.
+
+## Disclaimer
+
+This is a research project, not an official Google product. Expect bugs and
+sharp edges. Please help by trying out Caliban, [reporting
+bugs](https://github.com/google/caliban/issues), and letting us know what you
+think!
+
+## Get Involved + Get Support
+
+Pull requests and bug reports are always welcome! Check out our [Contributor's
+Guide](CONTRIBUTING.md) for information on how to get started contributing to
+Caliban.
+
+The TL;DR; is:
+
+- send us a pull request,
+- iterate on the feedback + discussion, and
+- get a +1 from a [Committer](COMMITTERS.md)
+
+in order to get your PR accepted.
+
+Issues should be reported on the [GitHub issue
+tracker](https://github.com/google/caliban/issues).
+
+If you want to discuss an idea for a new feature or ask us a question,
+discussion occurs primarily in the body of [Github
+Issues](https://github.com/google/caliban/issues), though the project is growing
+large enough that we may start a Gitter channel soon.
+
+The current list of active committers (who can +1 a pull request) can be found
+here: [COMMITTERS.md](COMMITTERS.md)
+
+A list of contributors to the project can be found at the project's
+[Contributors](https://github.com/google/caliban/graphs/contributors) page.
+
+## Citing Caliban
+
+If Caliban helps you in your research, please consider citing Caliban's
+associated academic paper:
+
+```
+@article{Ritchie2020,
+  doi = {10.21105/joss.02403},
+  url = {https://doi.org/10.21105/joss.02403},
+  year = {2020},
+  publisher = {The Open Journal},
+  volume = {5},
+  number = {53},
+  pages = {2403},
+  author = {Sam Ritchie and Ambrose Slone and Vinay Ramasesh},
+  title = {Caliban: Docker-based job manager for reproducible workflows},
+  journal = {Journal of Open Source Software}
+}
+```
+
+## License
+
+Copyright 2020 Google LLC.
+
+Licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
```

### Comparing `caliban-0.4.1/caliban.egg-info/SOURCES.txt` & `caliban-0.4.2/caliban.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+LICENSE_SHORT
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 caliban/__init__.py
 caliban/__main__.py
```

### Comparing `caliban-0.4.1/caliban.egg-info/PKG-INFO` & `caliban-0.4.2/caliban.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,530 +1,533 @@
 Metadata-Version: 2.1
 Name: caliban
-Version: 0.4.1
+Version: 0.4.2
 Summary: Docker-based job runner for AI research.
 Home-page: https://github.com/google/caliban
 Author: Caliban Team
 Author-email: samritchie@google.com
 License: Apache-2.0
-Description: # Caliban
-        
-        [![Build status](https://github.com/google/caliban/workflows/build/badge.svg?branch=master)](https://github.com/google/caliban/actions?query=workflow%3Abuild+branch%3Amaster)
-        [![Codecov branch](https://img.shields.io/codecov/c/github/google/caliban/master.svg?maxAge=3600)](https://codecov.io/github/google/caliban)
-        [![JOSS](https://joss.theoj.org/papers/c33c8b464103b2fb3b641878722bf8f3/status.svg)](https://joss.theoj.org/papers/c33c8b464103b2fb3b641878722bf8f3)
-        [![readthedocs](https://img.shields.io/readthedocs/caliban?maxAge=3600)](https://caliban.readthedocs.io/en/latest/?badge=latest)
-        [![caliban version](https://img.shields.io/pypi/v/caliban?maxAge=3600)](https://pypi.org/project/caliban)
-        
-        Caliban is a tool that helps researchers launch and track their numerical
-        experiments in an isolated, reproducible computing environment. It was developed
-        by machine learning researchers and engineers, and makes it easy to go from a
-        simple prototype running on a workstation to thousands of experimental jobs
-        running on Cloud.
-        
-        With Caliban, you can:
-        
-        - Develop your experimental code locally and test it inside an isolated (Docker)
-          environment
-        - Easily sweep over experimental parameters
-        - Submit your experiments as Cloud jobs, where they will run in the same
-          isolated environment
-        - Control and keep track of jobs
-        
-        ## Quickstart
-        
-        [Install Docker](#docker), make sure it's running, then install Caliban (you'll need [Python >= 3.6](#python-36)):
-        
-        ```bash
-        pip install caliban
-        ```
-        
-        Train a simple deep learning model on your local machine:
-        
-        ```bash
-        git clone https://github.com/google/caliban.git && cd caliban/tutorials/basic
-        caliban run --nogpu mnist.py
-        ```
-        
-        Sweep over learning rates to find the best one (flags are specified in JSON format):
-        
-        ```bash
-        echo '{"learning_rate": [0.01, 0.001, 0.0001]}' | caliban run --experiment_config stdin --nogpu mnist.py
-        ```
-        
-        **Next**:
-        
-        - See how to submit the experiment to Cloud and use other Caliban features in ["Getting Started with Caliban"](#getting-started-with-caliban)
-        - See [Installation](#installation-and-prerequisites) for detailed installation instructions
-        - Read the [Command Overview](#command-overview) for info on Caliban commands.
-        
-        Full documentation for Caliban lives at [Read The Docs](https://caliban.readthedocs.io/en/latest).
-        
-        ### Dramatic Interlude
-        
-        <p>
-        <img style="float: right;" align="right" src="https://upload.wikimedia.org/wikipedia/commons/a/ad/Stephano%2C_Trinculo_and_Caliban_dancing_from_The_Tempest_by_Johann_Heinrich_Ramberg.jpg" width="350">
-        
-        > “Be not afeard; the isle is full of noises, \
-        > Sounds, and sweet airs, that give delight and hurt not. \
-        > Sometimes a thousand twangling instruments \
-        > Will hum about mine ears; and sometime voices, \
-        > That, if I then had waked after long sleep, \
-        > Will make me sleep again: and then, in dreaming, \
-        > The clouds methought would open, and show riches \
-        > Ready to drop upon me; that, when I waked, \
-        > I cried to dream again.”
-        >
-        > -- <cite>Shakespeare, The Tempest</cite>
-        </p>
-        
-        ## Installation and Prerequisites
-        
-        Caliban's prequisites are [Docker](#docker) and [Python >= 3.6](#python-36).
-        
-        Make sure your Python is up to date:
-        
-        ```bash
-        $ python --version
-        Python 3.6.9 # should be >=3.6.0
-        ```
-        
-        If not, visit ["Installing Python 3.6"](#python-36) before proceeding.
-        
-        Next, install Caliban via [pip](https://pypi.org/project/caliban/):
-        
-        ```bash
-        pip install -U caliban
-        ```
-        
-        check if your installation worked by navigating to an empty folder and running
-        `caliban --help`. You should see the usage dialogue:
-        
-        ```bash
-        $ caliban --help
-        usage: caliban [-h] [--helpfull] [--version]
-                       {shell,notebook,build,run,cloud,cluster,status,stop,resubmit}
-                       ...
-        ```
-        
-        ### Docker
-        
-        Caliban executes your code inside a "container", managed by
-        [Docker](https://hub.docker.com/editions/community/docker-ce-desktop-mac). To get Docker:
-        
-        - On MacOS, follow the installation instructions at [Docker
-          Desktop](https://hub.docker.com/editions/community/docker-ce-desktop-mac) and
-          start the newly-installed Docker Desktop application.
-        - On Linux, visit the [Docker installation
-          instructions](https://docs.docker.com/engine/install/ubuntu/#installation-methods).
-          (It's important that you configure [sudo-less
-          Docker](https://caliban.readthedocs.io/en/latest/getting_started/prerequisites.html#docker)
-          and start Docker running on your machine.)
-        
-        Make sure Docker is correctly installed, configured and running by executing the
-        following command:
-        
-        ```bash
-        docker run hello-world
-        ```
-        
-        You should see output that looks like this:
-        
-        ```text
-        ...
-        Hello from Docker!
-        This message shows that your installation appears to be working correctly.
-        ...
-        ```
-        
-        ### Python 3.6
-        
-        Make sure your Python version is up to date:
-        
-        ```bash
-        $ python --version
-        Python 3.6.9 # should be >=3.6.0
-        ```
-        
-        If you need to upgrade:
-        
-        - On MacOS, install the latest Python version from
-          [python.org](https://www.python.org/downloads/mac-osx) ([direct
-          link](https://www.python.org/ftp/python/3.8.3/python-3.8.3-macosx10.9.pkg)).
-        - On Linux, run `sudo apt-get update && sudo apt-get install python3.7`.
-        
-        ### Cloud Submission and GPUs
-        
-        Caliban's [Read the Docs](https://caliban.readthedocs.io/) documentation has
-        instructions on:
-        
-        - [Installing the `nvidia-docker2`
-          runtime](https://caliban.readthedocs.io/en/latest/getting_started/prerequisites.html#docker-and-cuda),
-          so you can use Caliban to run jobs that use your Linux machine's GPU.
-        - [Setting up a Google Cloud
-          account](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
-          so you can submit your code to Google's [Cloud AI
-          Platform](https://cloud.google.com/ai-platform) with `caliban cloud`.
-        
-        ## Getting Started with Caliban
-        
-        In this section we will use Caliban to train an image classification network
-        (implemented in
-        [TensorFlow](https://www.tensorflow.org/tutorials/quickstart/beginner)). We
-        will:
-        
-        - Train a neural network on the local machine
-        - Increase the model's accuracy by changing the [learning
-          rate](https://medium.com/octavian-ai/which-optimizer-and-learning-rate-should-i-use-for-deep-learning-5acb418f9b2)
-          with a command-line flag
-        - Sweep across a range of learning rates with Caliban's [experiment
-          broadcasting](https://caliban.readthedocs.io/en/latest/explore/experiment_broadcasting.html)
-          feature
-        - Train the model in the Cloud on Google's [AI
-          Platform](https://cloud.google.com/ai-platform)
-        - Develop code interactively using `caliban shell` in the exact same
-          environment.
-        
-        ### Preparing your Project
-        
-        Create an empty directory and use `curl` to download a [python
-        script](https://github.com/google/caliban/blob/master/tutorials/basic/mnist.py#L16)
-        that trains a basic neural network.
-        
-        ```
-        mkdir demo && cd demo
-        curl --output mnist.py https://raw.githubusercontent.com/google/caliban/master/tutorials/basic/mnist.py
-        ```
-        
-        Create a file called `requirements.txt` to declare `tensorflow-cpu` as a dependency:
-        
-        ```bash
-        echo "tensorflow-cpu" > requirements.txt
-        ```
-        
-        Caliban will automatically make any entry in `requirements.txt` available when
-        you run your code. See ["Declaring
-        Requirements"](https://caliban.readthedocs.io/en/latest/explore/declaring_requirements.html)
-        for more information.
-        
-        ### Training the Network
-        
-        Run this command to train your first ML model:
-        
-        ```bash
-        caliban run --nogpu mnist.py
-        ```
-        
-        You should see a stream of output ending in this:
-        
-        ```text
-        Training model with learning rate=0.1 for 3 epochs.
-        Epoch 1/3
-        1875/1875 - 3s - loss: 2.0989 - accuracy: 0.2506
-        Epoch 2/3
-        1875/1875 - 3s - loss: 1.9222 - accuracy: 0.2273
-        Epoch 3/3
-        1875/1875 - 3s - loss: 2.0777 - accuracy: 0.1938
-        Model performance:
-        313/313 - 0s - loss: 2.0973 - accuracy: 0.1858
-        ```
-        
-        Your model was able to recognize digits from the
-        [MNIST](https://en.wikipedia.org/wiki/MNIST_database) dataset with 18.58%
-        accuracy. Can we do better?
-        
-        ### Improving the Model
-        
-        The default learning rate is `0.1`. Run the code again with a smaller learning
-        rate by passing a command-line flag, separated from your original command by
-        `--`:
-        
-        ```bash
-        $ caliban run --nogpu mnist.py -- --learning_rate 0.01
-        
-        <<elided>>
-        
-        Training model with learning rate=0.01 for 3 epochs.
-        Epoch 1/3
-        1875/1875 - 4s - loss: 0.2676 - accuracy: 0.9221
-        Epoch 2/3
-        1875/1875 - 4s - loss: 0.1863 - accuracy: 0.9506
-        Epoch 3/3
-        1875/1875 - 4s - loss: 0.1567 - accuracy: 0.9585
-        Model performance:
-        313/313 - 0s - loss: 0.1410 - accuracy: 0.9642
-        ```
-        
-        96% accuracy! Much better! Can we do better still?
-        
-        ### Experiment Broadcasting
-        
-        Caliban's [experiment
-        broadcasting](https://caliban.readthedocs.io/en/latest/explore/experiment_broadcasting.html)
-        feature will allow us to run many jobs with different sets of arguments.
-        
-        Create a file called `experiment.json` with a
-        [JSON](https://www.json.org/json-en.html) dictionary of the format
-        `{"flag_name": ["list", "of", "values"]}`:
-        
-        ```bash
-        echo '{"learning_rate": [0.01, 0.001, 0.0001]}' > experiment.json
-        ```
-        
-        Pass the config with `--experiment_config` and run again:
-        
-        ```bash
-        caliban run --experiment_config experiment.json --nogpu mnist.py
-        ```
-        
-        You should see accuracies of roughly `0.9493`, `0.9723` and `0.9537`. Looks like
-        `0.001` is a nice choice.
-        
-        ### Submitting to Cloud AI Platform
-        
-        Now it's time to submit the job to [Cloud AI
-        Platform](https://cloud.google.com/ai-platform).
-        
-        (**NOTE**: This section requires a Google Cloud account. You can create a free
-        account with $300 of credit to get started. Follow Caliban's ["Getting Started
-        with Google
-        Cloud"](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
-        documentation, then come back here to proceed.)
-        
-        Submit the job to AI Platform by changing the word `run` to `cloud`:
-        
-        ```bash
-        caliban cloud --nogpu mnist.py -- --learning_rate 0.01
-        ```
-        
-        You should see output like this:
-        
-        ```bash
-        I0615 19:57:43.354172 4563361216 core.py:161] Job 1 - jobId: caliban_totoro_1, image: gcr.io/research-3141/974a776e6037:latest
-        I0615 19:57:43.354712 4563361216 core.py:161] Job 1 - Accelerator: {'count': 0, 'type': 'ACCELERATOR_TYPE_UNSPECIFIED'}, machine: 'n1-highcpu-32', region: 'us-central1'
-        I0615 19:57:43.355082 4563361216 core.py:161] Job 1 - Experiment arguments: ['--learning_rate', '0.01']
-        I0615 19:57:43.355440 4563361216 core.py:161] Job 1 - labels: {'gpu_enabled': 'false', 'tpu_enabled': 'false', 'job_name': 'caliban_totoro', 'learning_rate': '0_01'}
-        
-        I0615 19:57:43.356621 4563361216 core.py:324] Submitting request!
-        I0615 19:57:45.078382 4563361216 core.py:97] Request for job 'caliban_totoro_20200615_195743_1' succeeded!
-        I0615 19:57:45.078989 4563361216 core.py:98] Job URL: https://console.cloud.google.com/ai-platform/jobs/caliban_totoro_20200615_195743_1?projectId=totoro-project
-        I0615 19:57:45.079524 4563361216 core.py:100] Streaming log CLI command: $ gcloud ai-platform jobs stream-logs caliban_totoro_20200615_195743_1
-        Submitting caliban_totoro_1: 100%|####################################################################################################################################################################################| 1/1 [00:02<00:00,  2.65s/requests]
-        I0615 19:57:45.405600 4563361216 core.py:673]
-        I0615 19:57:45.405819 4563361216 core.py:676] Visit https://console.cloud.google.com/ai-platform/jobs/?projectId=research-3141 to see the status of all jobs.
-        I0615 19:57:45.405959 4563361216 core.py:677]
-        ```
-        
-        This output means that Caliban has:
-        
-        - built a Docker container with all of your code
-        - Pushed that container up to Google Cloud's [Container
-          Registry](https://cloud.google.com/container-registry)
-        - Submitted the job to [AI Platform](https://cloud.google.com/ai-platform).
-        
-        You can now visit the link in the output that looks like:
-        https://console.cloud.google.com/ai-platform/jobs/caliban_totoro_20200615_195743_1?projectId=totoro-project
-        to see all of your job's logs.
-        
-        #### Why do I need Cloud?
-        
-        With Google Cloud, you can use on-demand
-        [GPUs](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html) and
-        [TPUs](https://caliban.readthedocs.io/en/latest/cloud/ai_platform_tpu.html) and
-        train models on large datasets at very high speeds. You can also customize the
-        [machine
-        type](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html#custom-machine-types)
-        that AI Platform uses to run your job. You might need high memory or more CPU,
-        for example.
-        
-        See Caliban's ["Customizing Machines and
-        GPUs"](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html#) for more
-        information.
-        
-        ### Interactive Development with `caliban shell`
-        
-        [`caliban
-        shell`](https://caliban.readthedocs.io/en/latest/cli/caliban_shell.html) lets
-        you develop code interactively inside of the exact same environment that your
-        code will have available, locally during `caliban run` or in the Cloud with
-        `caliban cloud`.
-        
-        Run the following command to activate the shell:
-        
-        ```bash
-        caliban shell --nogpu
-        ```
-        
-        You should see Caliban's terminal:
-        
-        ```
-        I0611 12:33:17.551121 4500135360 docker.py:911] Running command: docker run --ipc host -w /usr/app -u 735994:89939 -v /Users/totoro/code/example:/usr/app -it --entrypoint /bin/bash -v /Users/totoro:/home/totoro ab8a7d7db868
-           _________    __    ________  ___    _   __  __  __
-          / ____/   |  / /   /  _/ __ )/   |  / | / /  \ \ \ \
-         / /   / /| | / /    / // __  / /| | /  |/ /    \ \ \ \
-        / /___/ ___ |/ /____/ // /_/ / ___ |/ /|  /     / / / /
-        \____/_/  |_/_____/___/_____/_/  |_/_/ |_/     /_/ /_/
-        
-        You are running caliban shell as user with ID 735994 and group 89939,
-        which should map to the ID and group for your user on the Docker host. Great!
-        
-        [totoro@6a9b28990757 /usr/app]$
-        ```
-        
-        You're now living in an isolated [Docker
-        container](https://www.docker.com/resources/what-container) with your
-        `tensorflow-cpu` dependency available (and any others [you've
-        declared](https://caliban.readthedocs.io/en/latest/explore/declaring_requirements.html)).
-        
-        Run the `python` command and check that `tensorflow` is installed:
-        
-        ```bash
-        $ python
-        Python 3.6.9 (default, Nov  7 2019, 10:44:02)
-        [GCC 8.3.0] on linux
-        Type "help", "copyright", "credits" or "license" for more information.
-        >>> import tensorflow as tf
-        >>> tf.__version__
-        '2.2.0'
-        ```
-        
-        Your home directory and the folder where you ran the command are both mounted
-        into this isolated environment, so any changes you make to either of those
-        directories will be reflected immediately.
-        
-        Any code you add to the current folder and edit on your computer will be
-        available in this special Caliban shell. Run the example from before like this:
-        
-        ```
-        python mnist.py --learning_rate 0.01
-        ```
-        
-        If your code runs in `caliban shell`, you can be almost certain that your code
-        will execute in a Cloud environment, with potentially many GPUs attached and
-        much larger machines available.
-        
-        ### What next?
-        
-        Read the [Overview](#overview) for more information on Caliban's subcommands,
-        then head over to [Caliban's documentation
-        site](https://caliban.readthedocs.io/en/latest/) and check out the links on the
-        sidebar.
-        
-        If you find anything confusing, please feel free to [create an
-        issue](https://github.com/google/caliban/issues) on our [Github Issues
-        page](https://github.com/google/caliban/issues), and we'll get you sorted out.
-        
-        ## Command Overview
-        
-        Caliban provides seven subcommands that you run inside some project directory on
-        your machine:
-        
-        * [`caliban
-          shell`](https://caliban.readthedocs.io/en/latest/cli/caliban_shell.html)
-          generates a Docker image containing any dependencies you've declared in a
-          `requirements.txt` and/or `setup.py` in the directory and opens an interactive
-          shell in that directory. The `caliban shell` environment is ~identical to the
-          environment that will be available to your code when you submit it to AI
-          Platform; the difference is that your current directory is live-mounted into
-          the container, so you can develop interactively.
-        
-        * [`caliban
-          notebook`](https://caliban.readthedocs.io/en/latest/cli/caliban_notebook.html)
-          starts a Jupyter notebook or lab instance inside of a Docker image containing
-          your dependencies; the guarantee about an environment identical to AI Platform
-          applies here as well.
-        
-        * [`caliban run`](https://caliban.readthedocs.io/en/latest/cli/caliban_run.html)
-          packages your directory's code into the Docker image and executes it locally
-          using `docker run`. If you have a GPU, the instance will attach to it by
-          default - no need to install the CUDA toolkit. The Docker environment takes
-          care of all that. This environment is truly identical to the AI Platform
-          environment. The Docker image that runs locally is the same image that will
-          run in AI Platform.
-        
-        * [`caliban
-          cloud`](https://caliban.readthedocs.io/en/latest/cli/caliban_cloud.html)
-          allows you to [submit jobs to AI
-          Platform](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
-          that will run inside the same Docker image you used with `caliban run`. You
-          can submit hundreds of jobs at once. Any machine type, GPU count, and GPU type
-          combination you specify will be validated client side, so you'll see an
-          immediate error with suggestions, rather than having to debug by submitting
-          jobs over and over.
-        
-        * [`caliban
-          build`](https://caliban.readthedocs.io/en/latest/cli/caliban_build.html) builds
-          the Docker image used in `caliban cloud` and `caliban run` without actually
-          running the container or submitting any code.
-        
-        * [`caliban
-          cluster`](https://caliban.readthedocs.io/en/latest/cli/caliban_cluster.html)
-          creates GKE clusters and submits jobs to GKE clusters.
-        
-        * [`caliban
-          status`](https://caliban.readthedocs.io/en/latest/cli/caliban_status.html)
-          displays information about all jobs submitted by Caliban, and makes it easy to
-          interact with large groups of experiments. Use `caliban status` when you need
-          to cancel pending jobs, or re-build a container and resubmit a batch of
-          experiments after fixing a bug.
-        
-        ## Disclaimer
-        
-        This is a research project, not an official Google product. Expect bugs and
-        sharp edges. Please help by trying out Caliban, [reporting
-        bugs](https://github.com/google/caliban/issues), and letting us know what you
-        think!
-        
-        ## Get Involved + Get Support
-        
-        Pull requests and bug reports are always welcome! Check out our [Contributor's
-        Guide](CONTRIBUTING.md) for information on how to get started contributing to
-        Caliban.
-        
-        The TL;DR; is:
-        
-        - send us a pull request,
-        - iterate on the feedback + discussion, and
-        - get a +1 from a [Committer](COMMITTERS.md)
-        
-        in order to get your PR accepted.
-        
-        Issues should be reported on the [GitHub issue
-        tracker](https://github.com/google/caliban/issues).
-        
-        If you want to discuss an idea for a new feature or ask us a question,
-        discussion occurs primarily in the body of [Github
-        Issues](https://github.com/google/caliban/issues), though the project is growing
-        large enough that we may start a Gitter channel soon.
-        
-        The current list of active committers (who can +1 a pull request) can be found
-        here: [COMMITTERS.md](COMMITTERS.md)
-        
-        A list of contributors to the project can be found at the project's
-        [Contributors](https://github.com/google/caliban/graphs/contributors) page.
-        
-        ## Citing Caliban
-        
-        If Caliban helps you in your research, please consider citing the repository:
-        
-        ```
-        @software{caliban2020github,
-          author = {Sam Ritchie and Ambrose Slone and Vinay Ramasesh},
-          title = {{Caliban}: Docker-based job manager for reproducible workflows},
-          url = {http://github.com/google/caliban},
-          version = {0.2.5},
-          year = {2020},
-        }
-        ```
-        
-        In the above bibtex entry, the version number is intended to be that of the
-        latest tag on github, and the year corresponds to the project's open-source
-        release.
-        
-        ## License
-        
-        Copyright 2020 Google LLC.
-        
-        Licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
-        
-Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_SHORT
+
+# Caliban
+
+[![Build status](https://github.com/google/caliban/workflows/build/badge.svg?branch=master)](https://github.com/google/caliban/actions?query=workflow%3Abuild+branch%3Amaster)
+[![Codecov branch](https://img.shields.io/codecov/c/github/google/caliban/master.svg?maxAge=3600)](https://codecov.io/github/google/caliban)
+[![JOSS](https://joss.theoj.org/papers/c33c8b464103b2fb3b641878722bf8f3/status.svg)](https://joss.theoj.org/papers/c33c8b464103b2fb3b641878722bf8f3)
+[![readthedocs](https://img.shields.io/readthedocs/caliban?maxAge=3600)](https://caliban.readthedocs.io/en/latest/?badge=latest)
+[![caliban version](https://img.shields.io/pypi/v/caliban?maxAge=3600)](https://pypi.org/project/caliban)
+
+Caliban is a tool that helps researchers launch and track their numerical
+experiments in an isolated, reproducible computing environment. It was developed
+by machine learning researchers and engineers, and makes it easy to go from a
+simple prototype running on a workstation to thousands of experimental jobs
+running on Cloud.
+
+With Caliban, you can:
+
+- Develop your experimental code locally and test it inside an isolated (Docker)
+  environment
+- Easily sweep over experimental parameters
+- Submit your experiments as Cloud jobs, where they will run in the same
+  isolated environment
+- Control and keep track of jobs
+
+## Quickstart
+
+[Install Docker](#docker), make sure it's running, then install Caliban (you'll need [Python >= 3.6](#python-36)):
+
+```bash
+pip install caliban
+```
+
+Train a simple deep learning model on your local machine:
+
+```bash
+git clone https://github.com/google/caliban.git && cd caliban/tutorials/basic
+caliban run --nogpu mnist.py
+```
+
+Sweep over learning rates to find the best one (flags are specified in JSON format):
+
+```bash
+echo '{"learning_rate": [0.01, 0.001, 0.0001]}' | caliban run --experiment_config stdin --nogpu mnist.py
+```
+
+**Next**:
+
+- See how to submit the experiment to Cloud and use other Caliban features in ["Getting Started with Caliban"](#getting-started-with-caliban)
+- See [Installation](#installation-and-prerequisites) for detailed installation instructions
+- Read the [Command Overview](#command-overview) for info on Caliban commands.
+
+Full documentation for Caliban lives at [Read The Docs](https://caliban.readthedocs.io/en/latest).
+
+### Dramatic Interlude
+
+<p>
+<img style="float: right;" align="right" src="https://upload.wikimedia.org/wikipedia/commons/a/ad/Stephano%2C_Trinculo_and_Caliban_dancing_from_The_Tempest_by_Johann_Heinrich_Ramberg.jpg" width="350">
+
+> “Be not afeard; the isle is full of noises, \
+> Sounds, and sweet airs, that give delight and hurt not. \
+> Sometimes a thousand twangling instruments \
+> Will hum about mine ears; and sometime voices, \
+> That, if I then had waked after long sleep, \
+> Will make me sleep again: and then, in dreaming, \
+> The clouds methought would open, and show riches \
+> Ready to drop upon me; that, when I waked, \
+> I cried to dream again.”
+>
+> -- <cite>Shakespeare, The Tempest</cite>
+</p>
+
+## Installation and Prerequisites
+
+Caliban's prequisites are [Docker](#docker) and [Python >= 3.6](#python-36).
+
+Make sure your Python is up to date:
+
+```bash
+$ python --version
+Python 3.6.9 # should be >=3.6.0
+```
+
+If not, visit ["Installing Python 3.6"](#python-36) before proceeding.
+
+Next, install Caliban via [pip](https://pypi.org/project/caliban/):
+
+```bash
+pip install -U caliban
+```
+
+check if your installation worked by navigating to an empty folder and running
+`caliban --help`. You should see the usage dialogue:
+
+```bash
+$ caliban --help
+usage: caliban [-h] [--helpfull] [--version]
+               {shell,notebook,build,run,cloud,cluster,status,stop,resubmit}
+               ...
+```
+
+### Docker
+
+Caliban executes your code inside a "container", managed by
+[Docker](https://hub.docker.com/editions/community/docker-ce-desktop-mac). To get Docker:
+
+- On MacOS, follow the installation instructions at [Docker
+  Desktop](https://hub.docker.com/editions/community/docker-ce-desktop-mac) and
+  start the newly-installed Docker Desktop application.
+- On Linux, visit the [Docker installation
+  instructions](https://docs.docker.com/engine/install/ubuntu/#installation-methods).
+  (It's important that you configure [sudo-less
+  Docker](https://caliban.readthedocs.io/en/latest/getting_started/prerequisites.html#docker)
+  and start Docker running on your machine.)
+
+Make sure Docker is correctly installed, configured and running by executing the
+following command:
+
+```bash
+docker run hello-world
+```
+
+You should see output that looks like this:
+
+```text
+...
+Hello from Docker!
+This message shows that your installation appears to be working correctly.
+...
+```
+
+### Python 3.6
+
+Make sure your Python version is up to date:
+
+```bash
+$ python --version
+Python 3.6.9 # should be >=3.6.0
+```
+
+If you need to upgrade:
+
+- On MacOS, install the latest Python version from
+  [python.org](https://www.python.org/downloads/mac-osx) ([direct
+  link](https://www.python.org/ftp/python/3.8.3/python-3.8.3-macosx10.9.pkg)).
+- On Linux, run `sudo apt-get update && sudo apt-get install python3.7`.
+
+### Cloud Submission and GPUs
+
+Caliban's [Read the Docs](https://caliban.readthedocs.io/) documentation has
+instructions on:
+
+- [Installing the `nvidia-docker2`
+  runtime](https://caliban.readthedocs.io/en/latest/getting_started/prerequisites.html#docker-and-cuda),
+  so you can use Caliban to run jobs that use your Linux machine's GPU.
+- [Setting up a Google Cloud
+  account](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
+  so you can submit your code to Google's [Cloud AI
+  Platform](https://cloud.google.com/ai-platform) with `caliban cloud`.
+
+## Getting Started with Caliban
+
+In this section we will use Caliban to train an image classification network
+(implemented in
+[TensorFlow](https://www.tensorflow.org/tutorials/quickstart/beginner)). We
+will:
+
+- Train a neural network on the local machine
+- Increase the model's accuracy by changing the [learning
+  rate](https://medium.com/octavian-ai/which-optimizer-and-learning-rate-should-i-use-for-deep-learning-5acb418f9b2)
+  with a command-line flag
+- Sweep across a range of learning rates with Caliban's [experiment
+  broadcasting](https://caliban.readthedocs.io/en/latest/explore/experiment_broadcasting.html)
+  feature
+- Train the model in the Cloud on Google's [AI
+  Platform](https://cloud.google.com/ai-platform)
+- Develop code interactively using `caliban shell` in the exact same
+  environment.
+
+### Preparing your Project
+
+Create an empty directory and use `curl` to download a [python
+script](https://github.com/google/caliban/blob/master/tutorials/basic/mnist.py#L16)
+that trains a basic neural network.
+
+```
+mkdir demo && cd demo
+curl --output mnist.py https://raw.githubusercontent.com/google/caliban/master/tutorials/basic/mnist.py
+```
+
+Create a file called `requirements.txt` to declare `tensorflow-cpu` as a dependency:
+
+```bash
+echo "tensorflow-cpu" > requirements.txt
+```
+
+Caliban will automatically make any entry in `requirements.txt` available when
+you run your code. See ["Declaring
+Requirements"](https://caliban.readthedocs.io/en/latest/explore/declaring_requirements.html)
+for more information.
+
+### Training the Network
+
+Run this command to train your first ML model:
+
+```bash
+caliban run --nogpu mnist.py
+```
+
+You should see a stream of output ending in this:
+
+```text
+Training model with learning rate=0.1 for 3 epochs.
+Epoch 1/3
+1875/1875 - 3s - loss: 2.0989 - accuracy: 0.2506
+Epoch 2/3
+1875/1875 - 3s - loss: 1.9222 - accuracy: 0.2273
+Epoch 3/3
+1875/1875 - 3s - loss: 2.0777 - accuracy: 0.1938
+Model performance:
+313/313 - 0s - loss: 2.0973 - accuracy: 0.1858
+```
+
+Your model was able to recognize digits from the
+[MNIST](https://en.wikipedia.org/wiki/MNIST_database) dataset with 18.58%
+accuracy. Can we do better?
+
+### Improving the Model
+
+The default learning rate is `0.1`. Run the code again with a smaller learning
+rate by passing a command-line flag, separated from your original command by
+`--`:
+
+```bash
+$ caliban run --nogpu mnist.py -- --learning_rate 0.01
+
+<<elided>>
+
+Training model with learning rate=0.01 for 3 epochs.
+Epoch 1/3
+1875/1875 - 4s - loss: 0.2676 - accuracy: 0.9221
+Epoch 2/3
+1875/1875 - 4s - loss: 0.1863 - accuracy: 0.9506
+Epoch 3/3
+1875/1875 - 4s - loss: 0.1567 - accuracy: 0.9585
+Model performance:
+313/313 - 0s - loss: 0.1410 - accuracy: 0.9642
+```
+
+96% accuracy! Much better! Can we do better still?
+
+### Experiment Broadcasting
+
+Caliban's [experiment
+broadcasting](https://caliban.readthedocs.io/en/latest/explore/experiment_broadcasting.html)
+feature will allow us to run many jobs with different sets of arguments.
+
+Create a file called `experiment.json` with a
+[JSON](https://www.json.org/json-en.html) dictionary of the format
+`{"flag_name": ["list", "of", "values"]}`:
+
+```bash
+echo '{"learning_rate": [0.01, 0.001, 0.0001]}' > experiment.json
+```
+
+Pass the config with `--experiment_config` and run again:
+
+```bash
+caliban run --experiment_config experiment.json --nogpu mnist.py
+```
+
+You should see accuracies of roughly `0.9493`, `0.9723` and `0.9537`. Looks like
+`0.001` is a nice choice.
+
+### Submitting to Cloud AI Platform
+
+Now it's time to submit the job to [Cloud AI
+Platform](https://cloud.google.com/ai-platform).
+
+(**NOTE**: This section requires a Google Cloud account. You can create a free
+account with $300 of credit to get started. Follow Caliban's ["Getting Started
+with Google
+Cloud"](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
+documentation, then come back here to proceed.)
+
+Submit the job to AI Platform by changing the word `run` to `cloud`:
+
+```bash
+caliban cloud --nogpu mnist.py -- --learning_rate 0.01
+```
+
+You should see output like this:
+
+```bash
+I0615 19:57:43.354172 4563361216 core.py:161] Job 1 - jobId: caliban_totoro_1, image: gcr.io/research-3141/974a776e6037:latest
+I0615 19:57:43.354712 4563361216 core.py:161] Job 1 - Accelerator: {'count': 0, 'type': 'ACCELERATOR_TYPE_UNSPECIFIED'}, machine: 'n1-highcpu-32', region: 'us-central1'
+I0615 19:57:43.355082 4563361216 core.py:161] Job 1 - Experiment arguments: ['--learning_rate', '0.01']
+I0615 19:57:43.355440 4563361216 core.py:161] Job 1 - labels: {'gpu_enabled': 'false', 'tpu_enabled': 'false', 'job_name': 'caliban_totoro', 'learning_rate': '0_01'}
+
+I0615 19:57:43.356621 4563361216 core.py:324] Submitting request!
+I0615 19:57:45.078382 4563361216 core.py:97] Request for job 'caliban_totoro_20200615_195743_1' succeeded!
+I0615 19:57:45.078989 4563361216 core.py:98] Job URL: https://console.cloud.google.com/ai-platform/jobs/caliban_totoro_20200615_195743_1?projectId=totoro-project
+I0615 19:57:45.079524 4563361216 core.py:100] Streaming log CLI command: $ gcloud ai-platform jobs stream-logs caliban_totoro_20200615_195743_1
+Submitting caliban_totoro_1: 100%|####################################################################################################################################################################################| 1/1 [00:02<00:00,  2.65s/requests]
+I0615 19:57:45.405600 4563361216 core.py:673]
+I0615 19:57:45.405819 4563361216 core.py:676] Visit https://console.cloud.google.com/ai-platform/jobs/?projectId=research-3141 to see the status of all jobs.
+I0615 19:57:45.405959 4563361216 core.py:677]
+```
+
+This output means that Caliban has:
+
+- built a Docker container with all of your code
+- Pushed that container up to Google Cloud's [Container
+  Registry](https://cloud.google.com/container-registry)
+- Submitted the job to [AI Platform](https://cloud.google.com/ai-platform).
+
+You can now visit the link in the output that looks like:
+https://console.cloud.google.com/ai-platform/jobs/caliban_totoro_20200615_195743_1?projectId=totoro-project
+to see all of your job's logs.
+
+#### Why do I need Cloud?
+
+With Google Cloud, you can use on-demand
+[GPUs](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html) and
+[TPUs](https://caliban.readthedocs.io/en/latest/cloud/ai_platform_tpu.html) and
+train models on large datasets at very high speeds. You can also customize the
+[machine
+type](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html#custom-machine-types)
+that AI Platform uses to run your job. You might need high memory or more CPU,
+for example.
+
+See Caliban's ["Customizing Machines and
+GPUs"](https://caliban.readthedocs.io/en/latest/cloud/gpu_specs.html#) for more
+information.
+
+### Interactive Development with `caliban shell`
+
+[`caliban
+shell`](https://caliban.readthedocs.io/en/latest/cli/caliban_shell.html) lets
+you develop code interactively inside of the exact same environment that your
+code will have available, locally during `caliban run` or in the Cloud with
+`caliban cloud`.
+
+Run the following command to activate the shell:
+
+```bash
+caliban shell --nogpu
+```
+
+You should see Caliban's terminal:
+
+```
+I0611 12:33:17.551121 4500135360 docker.py:911] Running command: docker run --ipc host -w /usr/app -u 735994:89939 -v /Users/totoro/code/example:/usr/app -it --entrypoint /bin/bash -v /Users/totoro:/home/totoro ab8a7d7db868
+   _________    __    ________  ___    _   __  __  __
+  / ____/   |  / /   /  _/ __ )/   |  / | / /  \ \ \ \
+ / /   / /| | / /    / // __  / /| | /  |/ /    \ \ \ \
+/ /___/ ___ |/ /____/ // /_/ / ___ |/ /|  /     / / / /
+\____/_/  |_/_____/___/_____/_/  |_/_/ |_/     /_/ /_/
+
+You are running caliban shell as user with ID 735994 and group 89939,
+which should map to the ID and group for your user on the Docker host. Great!
+
+[totoro@6a9b28990757 /usr/app]$
+```
+
+You're now living in an isolated [Docker
+container](https://www.docker.com/resources/what-container) with your
+`tensorflow-cpu` dependency available (and any others [you've
+declared](https://caliban.readthedocs.io/en/latest/explore/declaring_requirements.html)).
+
+Run the `python` command and check that `tensorflow` is installed:
+
+```bash
+$ python
+Python 3.6.9 (default, Nov  7 2019, 10:44:02)
+[GCC 8.3.0] on linux
+Type "help", "copyright", "credits" or "license" for more information.
+>>> import tensorflow as tf
+>>> tf.__version__
+'2.2.0'
+```
+
+Your home directory and the folder where you ran the command are both mounted
+into this isolated environment, so any changes you make to either of those
+directories will be reflected immediately.
+
+Any code you add to the current folder and edit on your computer will be
+available in this special Caliban shell. Run the example from before like this:
+
+```
+python mnist.py --learning_rate 0.01
+```
+
+If your code runs in `caliban shell`, you can be almost certain that your code
+will execute in a Cloud environment, with potentially many GPUs attached and
+much larger machines available.
+
+### What next?
+
+Read the [Overview](#overview) for more information on Caliban's subcommands,
+then head over to [Caliban's documentation
+site](https://caliban.readthedocs.io/en/latest/) and check out the links on the
+sidebar.
+
+If you find anything confusing, please feel free to [create an
+issue](https://github.com/google/caliban/issues) on our [Github Issues
+page](https://github.com/google/caliban/issues), and we'll get you sorted out.
+
+## Command Overview
+
+Caliban provides seven subcommands that you run inside some project directory on
+your machine:
+
+* [`caliban
+  shell`](https://caliban.readthedocs.io/en/latest/cli/caliban_shell.html)
+  generates a Docker image containing any dependencies you've declared in a
+  `requirements.txt` and/or `setup.py` in the directory and opens an interactive
+  shell in that directory. The `caliban shell` environment is ~identical to the
+  environment that will be available to your code when you submit it to AI
+  Platform; the difference is that your current directory is live-mounted into
+  the container, so you can develop interactively.
+
+* [`caliban
+  notebook`](https://caliban.readthedocs.io/en/latest/cli/caliban_notebook.html)
+  starts a Jupyter notebook or lab instance inside of a Docker image containing
+  your dependencies; the guarantee about an environment identical to AI Platform
+  applies here as well.
+
+* [`caliban run`](https://caliban.readthedocs.io/en/latest/cli/caliban_run.html)
+  packages your directory's code into the Docker image and executes it locally
+  using `docker run`. If you have a GPU, the instance will attach to it by
+  default - no need to install the CUDA toolkit. The Docker environment takes
+  care of all that. This environment is truly identical to the AI Platform
+  environment. The Docker image that runs locally is the same image that will
+  run in AI Platform.
+
+* [`caliban
+  cloud`](https://caliban.readthedocs.io/en/latest/cli/caliban_cloud.html)
+  allows you to [submit jobs to AI
+  Platform](https://caliban.readthedocs.io/en/latest/getting_started/cloud.html)
+  that will run inside the same Docker image you used with `caliban run`. You
+  can submit hundreds of jobs at once. Any machine type, GPU count, and GPU type
+  combination you specify will be validated client side, so you'll see an
+  immediate error with suggestions, rather than having to debug by submitting
+  jobs over and over.
+
+* [`caliban
+  build`](https://caliban.readthedocs.io/en/latest/cli/caliban_build.html) builds
+  the Docker image used in `caliban cloud` and `caliban run` without actually
+  running the container or submitting any code.
+
+* [`caliban
+  cluster`](https://caliban.readthedocs.io/en/latest/cli/caliban_cluster.html)
+  creates GKE clusters and submits jobs to GKE clusters.
+
+* [`caliban
+  status`](https://caliban.readthedocs.io/en/latest/cli/caliban_status.html)
+  displays information about all jobs submitted by Caliban, and makes it easy to
+  interact with large groups of experiments. Use `caliban status` when you need
+  to cancel pending jobs, or re-build a container and resubmit a batch of
+  experiments after fixing a bug.
+
+## Disclaimer
+
+This is a research project, not an official Google product. Expect bugs and
+sharp edges. Please help by trying out Caliban, [reporting
+bugs](https://github.com/google/caliban/issues), and letting us know what you
+think!
+
+## Get Involved + Get Support
+
+Pull requests and bug reports are always welcome! Check out our [Contributor's
+Guide](CONTRIBUTING.md) for information on how to get started contributing to
+Caliban.
+
+The TL;DR; is:
+
+- send us a pull request,
+- iterate on the feedback + discussion, and
+- get a +1 from a [Committer](COMMITTERS.md)
+
+in order to get your PR accepted.
+
+Issues should be reported on the [GitHub issue
+tracker](https://github.com/google/caliban/issues).
+
+If you want to discuss an idea for a new feature or ask us a question,
+discussion occurs primarily in the body of [Github
+Issues](https://github.com/google/caliban/issues), though the project is growing
+large enough that we may start a Gitter channel soon.
+
+The current list of active committers (who can +1 a pull request) can be found
+here: [COMMITTERS.md](COMMITTERS.md)
+
+A list of contributors to the project can be found at the project's
+[Contributors](https://github.com/google/caliban/graphs/contributors) page.
+
+## Citing Caliban
+
+If Caliban helps you in your research, please consider citing Caliban's
+associated academic paper:
+
+```
+@article{Ritchie2020,
+  doi = {10.21105/joss.02403},
+  url = {https://doi.org/10.21105/joss.02403},
+  year = {2020},
+  publisher = {The Open Journal},
+  volume = {5},
+  number = {53},
+  pages = {2403},
+  author = {Sam Ritchie and Ambrose Slone and Vinay Ramasesh},
+  title = {Caliban: Docker-based job manager for reproducible workflows},
+  journal = {Journal of Open Source Software}
+}
+```
+
+## License
+
+Copyright 2020 Google LLC.
+
+Licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
```

