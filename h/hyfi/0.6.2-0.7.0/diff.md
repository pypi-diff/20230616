# Comparing `tmp/hyfi-0.6.2.tar.gz` & `tmp/hyfi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.6.2.tar", max compression
+gzip compressed data, was "hyfi-0.7.0.tar", max compression
```

## Comparing `hyfi-0.6.2.tar` & `hyfi-0.7.0.tar`

### file list

```diff
@@ -1,77 +1,85 @@
--rw-r--r--   0        0        0     1071 2023-06-16 06:31:48.645149 hyfi-0.6.2/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-16 06:31:48.645149 hyfi-0.6.2/README.md
--rw-r--r--   0        0        0     4592 2023-06-16 06:32:13.366097 hyfi-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3661 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2544 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__click__.py
--rw-r--r--   0        0        0      598 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9559 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      417 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-16 06:32:13.298094 hyfi-0.6.2/src/hyfi/_version.py
--rw-r--r--   0        0        0      777 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0    12718 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     6832 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/version.py
--rw-r--r--   0        0        0        0 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-16 06:32:13.302094 hyfi-0.6.2/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      320 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      717 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      123 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      604 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0     1719 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      781 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0     6369 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     5886 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0    12854 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0        0 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8393 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4330 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2497 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3329 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/utils.py
--rw-r--r--   0        0        0     3480 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    16589 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0     2086 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/pipe.py
--rw-r--r--   0        0        0    30671 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0     2903 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     5743 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     5566 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     5668 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    12472 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/file.py
--rw-r--r--   0        0        0     9920 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1114 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3699 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4145 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1986 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9766 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     5476 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 11:04:36.665550 hyfi-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-16 11:04:36.665550 hyfi-0.7.0/README.md
+-rw-r--r--   0        0        0     4592 2023-06-16 11:05:00.213687 hyfi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3804 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2544 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      598 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9601 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      417 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-16 11:05:00.145686 hyfi-0.7.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0      777 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     3182 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/version.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-16 11:05:00.145686 hyfi-0.7.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      407 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      967 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0      120 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      609 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      806 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      121 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      130 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0     6369 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/__init__.py
+-rw-r--r--   0        0        0     8395 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/collage.py
+-rw-r--r--   0        0        0     4330 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/motion.py
+-rw-r--r--   0        0        0     2497 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/plot.py
+-rw-r--r--   0        0        0     3331 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/utils.py
+-rw-r--r--   0        0        0     5886 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0    12854 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0     3480 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    16589 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0     2086 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/pipe.py
+-rw-r--r--   0        0        0    30681 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     2903 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     5743 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     5566 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/tasks/__init__.py
+-rw-r--r--   0        0        0     4920 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/tasks/base.py
+-rw-r--r--   0        0        0     5289 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/tasks/batch.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     5668 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    12472 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/file.py
+-rw-r--r--   0        0        0     9920 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1114 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3699 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4145 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1986 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9766 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     5476 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.7.0/PKG-INFO
```

### Comparing `hyfi-0.6.2/LICENSE` & `hyfi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/README.md` & `hyfi-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/pyproject.toml` & `hyfi-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.6.2"
+version = "0.7.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.6.2/src/hyfi/__cli__.py` & `hyfi-0.7.0/src/hyfi/__cli__.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,26 @@
 
 
 def run_copy(**args):
     """
     Copy all config files to the current working directory.
     This is a wrapper around HyfiConfig to allow us to pass arguments to it.
     """
-    cfg = HyfiConfig(**args)
-    cfg = HyFI.to_dict(cfg.copier)
+    if "copier" not in args:
+        raise ValueError("No copier configuration found")
+    cfg = HyFI.to_dict(args["copier"])
+    print(type(cfg), cfg)
     with Copier(**cfg) as worker:
         worker.run_copy()
 
 
+def run_task(**args):
+    print(args["task"].keys())
+
+
 def cli_main(cfg: DictConfig) -> None:
     """
     Main function for the command line interface.
     Initializes Hydra and instantiates the class.
     Prints the configuration to standard out if verbose is set to True
 
     Args:
```

### Comparing `hyfi-0.6.2/src/hyfi/__click__.py` & `hyfi-0.7.0/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/__global__/__init__.py` & `hyfi-0.7.0/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/__global__/config.py` & `hyfi-0.7.0/src/hyfi/__global__/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     from hyfi._version import __version__
 
     return __version__
 
 
 class HyfiConfig(BaseModel):
-    """HyFI config primary class"""
+    """HyFI root config class.  This class is used to store the configuration"""
 
     hyfi_config_path: str = __about__.config_path
     hyfi_config_module: str = __about__.config_module
     hyfi_user_config_path: str = ""
 
     debug_mode: bool = False
     print_config: bool = False
@@ -218,15 +218,15 @@
             config = _compose(
                 overrides=["+project=__init__"], config_module=__about__.config_module
             )
             logger.debug("Using default config.")
 
         # Skip project config initialization.
         if "project" not in config:
-            logger.warning(
+            logger.info(
                 "No project config found, skip project config initialization."
             )
             return
         self.project = ProjectConfig(**config["project"])
         self.project.init_project()
         # Initialize joblib backend if joblib is not set.
         if self.project.joblib:
```

### Comparing `hyfi-0.6.2/src/hyfi/about/__init__.py` & `hyfi-0.7.0/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/__init__.py` & `hyfi-0.7.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/__init__.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/_cached_path.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/cache_file.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/common.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/file_lock.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/meta.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/progress.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/hf.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/http.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/testing.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/util.py` & `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.7.0/src/hyfi/conf/copier/conf.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Source path where to find the template.
 src_path: conf
 # Destination path where to render the template.
-dst_path: .
+dst_path: tmp/conf
 # Filetypes to copy.
 filetypes:
   - yaml
   - yml
   - py
 # User-chosen additional file exclusion patterns.
 exclude:
```

### Comparing `hyfi-0.6.2/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.7.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.7.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.7.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # @package _global_
 debug_mode: false
 print_config: false
 print_resolved_config: true
 verbose: false
 ignore_warnings: true
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
+project_name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}}
+log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}}
 
 hydra:
   job:
-    name: ${project.project_name}
+    name: ${project_name}
     chdir: true
   run:
-    dir: ${project.path.project_logs}/hydra/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${log_dir}/hydra/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
   sweep:
-    dir: ${project.path.project_logs}/hydra/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${log_dir}/hydra/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
     subdir: ${hydra.job.num}
   verbose: false
   job_logging:
     handlers:
       console:
         level: ${hydra.job_logging.root.level}
       file:
```

### Comparing `hyfi-0.6.2/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.7.0/src/hyfi/conf/path/__task__.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-project_workspace_root: ${oc.select:..project.project_workspace_root,${oc.env:HYFI_PROJECT_ROOT,.}/${oc.env:HYFI_PROJECT_WORKSPACE_NAME,.}}
+project_workspace_root: ${oc.select:..project.path.project_workspace_root,${oc.env:HYFI_PROJECT_ROOT,.}/${oc.env:HYFI_PROJECT_WORKSPACE_NAME,.}}
 task_name: ${oc.select:..project.task_name, default-task}
 task_root: ${.project_workspace_root}/${.task_name}
 
 task_outputs: ${.task_root}/outputs
 task_datasets: ${.task_root}/datasets
 task_library: ${.task_root}/libs
 task_models: ${.task_root}/models
```

### Comparing `hyfi-0.6.2/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.7.0/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.7.0/src/hyfi/conf/project/__init__.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
 project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
-task_name: ${alt:${oc.env:HYFI_TASK_NAME,null},default-task}
+task_name: ${oc.select:..task_name,${alt:${oc.env:HYFI_TASK_NAME,null},default-task}}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
 project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
 project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
 global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
 global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
 num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
 use_huggingface_hub: false
```

### Comparing `hyfi-0.6.2/src/hyfi/copier/__init__.py` & `hyfi-0.7.0/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/dotenv/__init__.py` & `hyfi-0.7.0/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/hydra/__init__.py` & `hyfi-0.7.0/src/hyfi/hydra/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/hydra/main.py` & `hyfi-0.7.0/src/hyfi/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/image/collage.py` & `hyfi-0.7.0/src/hyfi/graphic/collage.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List
 
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image, ImageDraw
 from pydantic import BaseModel
 
-from hyfi.image.utils import get_image_font, load_image, load_images, scale_image
+from hyfi.graphic.utils import get_image_font, load_image, load_images, scale_image
 
 log = logging.getLogger(__name__)
 
 
 class Collage(BaseModel):
     """Collage of images."""
```

### Comparing `hyfi-0.6.2/src/hyfi/image/motion.py` & `hyfi-0.7.0/src/hyfi/graphic/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/image/plot.py` & `hyfi-0.7.0/src/hyfi/graphic/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/image/utils.py` & `hyfi-0.7.0/src/hyfi/graphic/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Image utils."""
 import io
 
 import numpy as np
 from PIL import Image, ImageFont
 
-from hyfi.image.plot import get_plot_font
+from hyfi.graphic.plot import get_plot_font
 from hyfi.utils.file import read
 
 
 def scale_image(
     image: Image.Image,
     max_width: int = None,
     max_height: int = None,
```

### Comparing `hyfi-0.6.2/src/hyfi/joblib/__init__.py` & `hyfi-0.7.0/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/joblib/batch/apply.py` & `hyfi-0.7.0/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-0.7.0/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/joblib/batch/batcher.py` & `hyfi-0.7.0/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/joblib/pipe.py` & `hyfi-0.7.0/src/hyfi/joblib/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/main/__init__.py` & `hyfi-0.7.0/src/hyfi/main/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,15 +578,15 @@
         show_filename=False,
         filename_offset=(5, 5),
         fontname=None,
         fontsize=12,
         fontcolor="#000",
         **kwargs,
     ):
-        from hyfi.image.collage import collage as _collage
+        from hyfi.graphic.collage import collage as _collage
 
         return _collage(
             images_or_uris,
             collage_filepath=collage_filepath,
             ncols=ncols,
             max_images=max_images,
             collage_width=collage_width,
@@ -612,15 +612,15 @@
         width=None,
         optimize=True,
         quality=50,
         show=False,
         force=False,
         **kwargs,
     ):
-        from hyfi.image.motion import make_gif as _make_gif
+        from hyfi.graphic.motion import make_gif as _make_gif
 
         return _make_gif(
             image_filepaths=image_filepaths,
             filename_patterns=filename_patterns,
             base_dir=base_dir,
             output_filepath=output_filepath,
             duration=duration,
@@ -904,15 +904,15 @@
             style,
             layout,
             **kwargs,
         )
 
     @staticmethod
     def get_image_font(fontname=None, fontsize=12):
-        from hyfi.image.collage import get_image_font
+        from hyfi.graphic.collage import get_image_font
 
         return get_image_font(fontname, fontsize)
 
     @staticmethod
     def read(uri, mode="rb", encoding=None, head=None, **kwargs):
         from hyfi.utils.file import read as _read
 
@@ -926,15 +926,15 @@
         max_pixels: int = None,
         scale: float = 1.0,
         resize_to_multiple_of: int = None,
         crop_box=None,
         mode="RGB",
         **kwargs,
     ):
-        from hyfi.image.utils import load_image as _load_image
+        from hyfi.graphic.utils import load_image as _load_image
 
         return _load_image(
             image_or_uri,
             max_width,
             max_height,
             max_pixels,
             scale,
@@ -1009,15 +1009,15 @@
     ):
         """
         Scale an image to a maximum width, height, or number of pixels.
 
         resample:   Image.NEAREST (0), Image.LANCZOS (1), Image.BILINEAR (2),
                     Image.BICUBIC (3), Image.BOX (4) or Image.HAMMING (5)
         """
-        from hyfi.image.utils import scale_image as _scale_image
+        from hyfi.graphic.utils import scale_image as _scale_image
 
         return _scale_image(
             image,
             max_width,
             max_height,
             max_pixels,
             scale,
```

### Comparing `hyfi-0.6.2/src/hyfi/path/__init__.py` & `hyfi-0.7.0/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/path/batch.py` & `hyfi-0.7.0/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/project/__init__.py` & `hyfi-0.7.0/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/env.py` & `hyfi-0.7.0/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/file.py` & `hyfi-0.7.0/src/hyfi/utils/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/func.py` & `hyfi-0.7.0/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/google.py` & `hyfi-0.7.0/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/gpu.py` & `hyfi-0.7.0/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/lib.py` & `hyfi-0.7.0/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/logging.py` & `hyfi-0.7.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/notebook.py` & `hyfi-0.7.0/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/src/hyfi/utils/tools.py` & `hyfi-0.7.0/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.2/PKG-INFO` & `hyfi-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.6.2
+Version: 0.7.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

