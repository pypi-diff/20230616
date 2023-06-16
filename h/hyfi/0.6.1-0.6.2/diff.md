# Comparing `tmp/hyfi-0.6.1.tar.gz` & `tmp/hyfi-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.6.1.tar", max compression
+gzip compressed data, was "hyfi-0.6.2.tar", max compression
```

## Comparing `hyfi-0.6.1.tar` & `hyfi-0.6.2.tar`

### file list

```diff
@@ -1,78 +1,77 @@
--rw-r--r--   0        0        0     1071 2023-06-16 04:14:25.157391 hyfi-0.6.1/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-16 04:14:25.157391 hyfi-0.6.1/README.md
--rw-r--r--   0        0        0     4592 2023-06-16 04:14:48.186760 hyfi-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3661 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2216 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__click__.py
--rw-r--r--   0        0        0      598 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     5379 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      417 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-16 04:14:48.118757 hyfi-0.6.1/src/hyfi/_version.py
--rw-r--r--   0        0        0      777 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0    12718 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-16 04:14:48.118757 hyfi-0.6.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      320 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      717 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      123 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      604 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0     1719 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      781 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0     6369 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     5886 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0    12832 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0        0 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8393 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4327 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2497 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3326 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     6825 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12472 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/io/file.py
--rw-r--r--   0        0        0     3479 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0    30375 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0     2903 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     5743 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     5566 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    16580 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     1206 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/version.py
--rw-r--r--   0        0        0     5665 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/env.py
--rw-r--r--   0        0        0     9920 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1114 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3699 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4142 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1986 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9763 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2084 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/pipe.py
--rw-r--r--   0        0        0     5476 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 06:31:48.645149 hyfi-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-16 06:31:48.645149 hyfi-0.6.2/README.md
+-rw-r--r--   0        0        0     4592 2023-06-16 06:32:13.366097 hyfi-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3661 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2544 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      598 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9559 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      417 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-16 06:32:13.298094 hyfi-0.6.2/src/hyfi/_version.py
+-rw-r--r--   0        0        0      777 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0    12718 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/cached_path/_cached_path/version.py
+-rw-r--r--   0        0        0        0 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-16 06:32:13.302094 hyfi-0.6.2/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      320 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      717 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      123 2023-06-16 06:31:48.649150 hyfi-0.6.2/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      604 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      781 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0     6369 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     5886 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0    12854 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8393 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4330 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2497 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3329 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0     3480 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    16589 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0     2086 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/joblib/pipe.py
+-rw-r--r--   0        0        0    30671 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0     2903 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     5743 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     5566 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     5668 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    12472 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/file.py
+-rw-r--r--   0        0        0     9920 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1114 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3699 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4145 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1986 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9766 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     5476 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-16 06:31:48.653150 hyfi-0.6.2/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.6.2/PKG-INFO
```

### Comparing `hyfi-0.6.1/LICENSE` & `hyfi-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/README.md` & `hyfi-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/pyproject.toml` & `hyfi-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.6.1"
+version = "0.6.2"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.6.1/src/hyfi/__cli__.py` & `hyfi-0.6.2/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/__click__.py` & `hyfi-0.6.2/src/hyfi/__click__.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,27 +16,51 @@
 @click.version_option(__version__)
 def cli():
     pass
 
 
 @cli.command()
 @click.option(
-    "--src_path", default=f"{__hyfi_path__()}/conf", help="Source path to copy from"
+    "--src_path",
+    show_default=True,
+    default=f"{__hyfi_path__()}/conf",
+    help="Source path to copy from",
 )
 @click.option(
     "--dst_path",
     show_default=True,
     default="./tmp/conf",
     help="Destination path to copy to",
 )
-@click.option("--exclude", default=None, help="Exclude files matching this pattern")
-@click.option("--skip_if_exists", default=False, help="Skip if destination exists")
-@click.option("--overwrite", default=False, help="Overwrite destination")
-@click.option("--dry_run", default=False, help="Dry run")
-@click.option("--verbose", is_flag=True, default=False, help="Verbose output")
+@click.option(
+    "--exclude",
+    show_default=True,
+    default=None,
+    help="Exclude files matching this pattern",
+)
+@click.option(
+    "--skip_if_exists",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Skip if destination exists",
+)
+@click.option(
+    "--overwrite",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Overwrite destination",
+)
+@click.option(
+    "--dry_run", is_flag=True, show_default=True, default=False, help="Dry run"
+)
+@click.option(
+    "--verbose", is_flag=True, show_default=True, default=False, help="Verbose output"
+)
 def cc(**args):
     """
     Copy all config files to the destination directory.
     """
     click.echo("Copying configuration files")
     # click.echo(f"args : {args}")
     with Copier(**args) as worker:
@@ -51,17 +75,28 @@
     cfg = HyfiConfig()
     cfg.about.version = __version__
     _about(cfg)
 
 
 @cli.command()
 @click.option(
-    "--uninstall", "-u", is_flag=True, default=False, help="Uninstall shell completion"
+    "--uninstall",
+    "-u",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Uninstall shell completion",
+)
+@click.option(
+    "--shell",
+    "-s",
+    show_default=True,
+    default="zsh",
+    help="Shell to install completion for",
 )
-@click.option("--shell", "-s", default="zsh", help="Shell to install completion for")
 def sc(uninstall, shell):
     """
     Install or Uninstall shell completion for Hyfi.
     """
     if uninstall:
         click.echo(f"Uninstall shell completion for {shell}:")
         click.echo(
```

### Comparing `hyfi-0.6.1/src/hyfi/__global__/__init__.py` & `hyfi-0.6.2/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/__global__/config.py` & `hyfi-0.6.2/src/hyfi/project/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,167 +1,162 @@
-from typing import Any, Dict, Optional, Union
+import os
+from pathlib import Path
+from typing import Any, Union
 
-from omegaconf import DictConfig
-from pydantic import BaseModel, root_validator, validator
+from pydantic import BaseModel, validator
 
-from hyfi.__global__ import __about__, __hydra_config__
-from hyfi.about import AboutConfig
+from hyfi.__global__ import __about__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.hydra import _compose
-from hyfi.project import ProjectConfig
-from hyfi.utils.env import _check_and_set_value, expand_posix_vars
-from hyfi.utils.logging import getLogger, setLogger
-from hyfi.utils.notebook import load_extentions, set_matplotlib_formats
+from hyfi.joblib import JobLibConfig
+from hyfi.path import PathConfig
+from hyfi.utils.logging import getLogger
+from hyfi.utils.notebook import is_notebook
 
 logger = getLogger(__name__)
 
 
-def __version__():
-    """Returns the version of HyFI"""
-    from hyfi._version import __version__
+class ProjectConfig(BaseModel):
+    """Project Config"""
 
-    return __version__
-
-
-class HyfiConfig(BaseModel):
-    """HyFI config primary class"""
-
-    hyfi_config_path: str = __about__.config_path
-    hyfi_config_module: str = __about__.config_module
-    hyfi_user_config_path: str = ""
-
-    debug_mode: bool = False
-    print_config: bool = False
-    print_resolved_config: bool = False
-    verbose: bool = False
-    logging_level: str = "WARNING"
-
-    hydra: Optional[DictConfig] = None
-
-    about: AboutConfig = AboutConfig()
-    project: Optional[ProjectConfig] = None
-    copier: Optional[DictConfig] = None
-
-    __version__: str = __version__()
-    __initilized__: bool = False
+    config_name: str = "__init__"
+    project_name: str = "hyfi-project"
+    task_name: str = ""
+    project_description: str = ""
+    project_root: str = ""
+    project_workspace_name: str = "workspace"
+    global_hyfi_root: str = ""
+    global_workspace_name: str = "workspace"
+    num_workers: int = 1
+    use_huggingface_hub: bool = False
+    use_wandb: bool = False
+    verbose: Union[bool, int] = False
+    # Config Classes
+    dotenv: DotEnvConfig = None  # type: ignore
+    joblib: JobLibConfig = None  # type: ignore
+    path: PathConfig = None  # type: ignore
 
     class Config:
-        arbitrary_types_allowed = True
-        underscore_attrs_are_private = True
-        validate_assignment = True
         extra = "allow"
+        arbitrary_types_allowed = True
 
-    @root_validator()
-    def _check_and_set_values(cls, values):
-        key = "hyfi_config_path"
-        val = _check_and_set_value(key, values.get(key))
-        values[key] = val
-        if val is not None:
-            key = "hyfi_config_module"
-            values[key] = _check_and_set_value(key, val.replace("pkg://", ""))
-        return values
-
-    @validator("hyfi_user_config_path")
-    def _validate_hyfi_user_config_path(cls, v):
-        return _check_and_set_value("hyfi_user_config_path", v)
-
-    @validator("logging_level")
-    def _validate_logging_level(cls, v, values):
-        verbose = values.get("verbose", False)
-        if verbose and v == "WARNING":
-            v = "INFO"
-        logger.setLevel(v)
+    @validator("project_name", allow_reuse=True)
+    def _validate_project_name(cls, v):
+        if v is None:
+            raise ValueError("Project name must be specified.")
         return v
 
-    def __init__(self, **data: Any):
-        super().__init__(**data)
-        # self.about = __about__
+    @validator("verbose", allow_reuse=True)
+    def _validate_verbose(cls, v):
+        if isinstance(v, str):
+            if v.lower() in {"true", "1"}:
+                v = True
+            elif v.lower() in {"false", "0"}:
+                v = False
+            else:
+                raise ValueError("verbose must be a boolean or a string of 0 or 1")
+        return v
 
-    def init_workspace(
+    def __init__(
         self,
-        project_name: str = "",
-        task_name: str = "",
-        project_description: str = "",
-        project_root: str = "",
-        project_workspace_name: str = "",
-        global_hyfi_root: str = "",
-        global_workspace_name: str = "",
-        num_workers: int = -1,
-        log_level: str = "",
-        autotime: bool = True,
-        retina: bool = True,
-        verbose: Union[bool, int] = False,
-        **kwargs,
+        config_name: str = "__init__",
+        **data: Any,
     ):
-        envs = DotEnvConfig(HYFI_VERBOSE=verbose)
-        if project_name:
-            envs.HYFI_PROJECT_NAME = expand_posix_vars(project_name)
-        if task_name:
-            envs.HYFI_TASK_NAME = expand_posix_vars(task_name)
-        if project_description:
-            envs.HYFI_PROJECT_DESC = expand_posix_vars(project_description)
-        if project_root:
-            envs.HYFI_PROJECT_ROOT = expand_posix_vars(project_root)
-        if project_workspace_name:
-            envs.HYFI_PROJECT_WORKSPACE_NAME = expand_posix_vars(project_workspace_name)
-        if global_hyfi_root:
-            envs.HYFI_GLOBAL_ROOT = expand_posix_vars(global_hyfi_root)
-        if global_workspace_name:
-            envs.HYFI_GLOBAL_WORKSPACE_NAME = expand_posix_vars(global_workspace_name)
-        if num_workers:
-            envs.HYFI_NUM_WORKERS = num_workers
-        if log_level:
-            envs.HYFI_LOG_LEVEL = log_level
-            setLogger(log_level)
-            logger.setLevel(log_level)
-        if autotime:
-            load_extentions(exts=["autotime"])
-        if retina:
-            set_matplotlib_formats("retina")
-        self.initialize()
-
-    def initialize(self, config: Union[DictConfig, Dict, None] = None):
-        """Initialize hyfi config"""
-        if self.__initilized__:
-            return
-        __hydra_config__.hyfi_config_module = self.hyfi_config_module
-        __hydra_config__.hyfi_config_path = self.hyfi_config_path
-        __hydra_config__.hyfi_user_config_path = self.hyfi_user_config_path
-
-        if config is None:
-            config = _compose(
-                overrides=["+project=__init__"], config_module=__about__.config_module
-            )
-            logger.debug("Using default config.")
-
-        if "project" not in config:
+        data = _compose(
+            f"project={config_name}",
+            config_data=data,
+            config_module=__about__.config_module,
+        )  # type: ignore
+        super().__init__(config_name=config_name, **data)
+
+    def init_project(self):
+        self.dotenv = DotEnvConfig()
+        if self.path is None:
+            self.path = PathConfig()
+        if self.joblib is None:
+            self.joblib = JobLibConfig()
+
+        self.dotenv.HYFI_PROJECT_NAME = self.project_name
+        self.dotenv.HYFI_TASK_NAME = self.task_name
+        self.dotenv.HYFI_PROJECT_DESC = self.project_description
+        self.dotenv.HYFI_PROJECT_ROOT = self.project_root
+        self.dotenv.HYFI_PROJECT_WORKSPACE_NAME = self.project_workspace_name
+        self.dotenv.HYFI_GLOBAL_ROOT = self.global_hyfi_root
+        self.dotenv.HYFI_GLOBAL_WORKSPACE_NAME = self.global_workspace_name
+        self.dotenv.HYFI_NUM_WORKERS = self.num_workers
+        self.dotenv.HYFI_VERBOSE = self.verbose
+        self.dotenv.CACHED_PATH_CACHE_ROOT = str(self.path.cache_dir / "cached_path")
+        self.init_wandb()
+        if self.use_huggingface_hub:
+            self.init_huggingface_hub()
+
+    def init_wandb(self):
+        if self.path is None:
+            raise ValueError("Path object not initialized")
+        if self.dotenv is None:
+            raise ValueError("DotEnv object not initialized")
+
+        self.dotenv.WANDB_DIR = str(self.path.log_dir)
+        project_name = self.project_name.replace("/", "-").replace("\\", "-")
+        self.dotenv.WANDB_PROJECT = project_name
+        task_name = self.task_name.replace("/", "-").replace("\\", "-")
+        notebook_name = self.path.log_dir / f"{task_name}-nb"
+        notebook_name.mkdir(parents=True, exist_ok=True)
+        self.dotenv.WANDB_NOTEBOOK_NAME = str(notebook_name)
+        self.dotenv.WANDB_SILENT = str(not self.verbose)
+        if self.use_wandb:
+            try:
+                import wandb  # type: ignore
+
+                wandb.init(project=self.project_name)
+            except ImportError:
+                logger.warning(
+                    "wandb is not installed, please install it to use wandb."
+                )
+
+    def init_huggingface_hub(self):
+        """Initialize huggingface_hub"""
+        try:
+            from huggingface_hub import notebook_login  # type: ignore
+            from huggingface_hub.hf_api import HfFolder  # type: ignore
+        except ImportError:
             logger.warning(
-                "No project config found, skip project config initialization."
+                "huggingface_hub is not installed, please install it to use huggingface_hub."
             )
             return
-        self.project = ProjectConfig(**config["project"])
-        self.project.init_project()
-        if self.project.joblib:
-            self.project.joblib.init_backend()
-
-        self.__initilized__ = True
-
-    def terminate(self):
-        """Terminate hyfi config"""
-        if not self.__initilized__:
-            return
-        if self.project and self.project.joblib:
-            self.project.joblib.stop_backend()
-        self.__initilized__ = False
-
-    def __repr__(self):
-        return f"HyFIConfig(project={self.project})"
 
-    def __str__(self):
-        return self.__repr__()
+        self.dotenv = DotEnvConfig()
+        if (
+            self.dotenv.HUGGING_FACE_HUB_TOKEN is None
+            and self.dotenv.HF_USER_ACCESS_TOKEN is not None
+        ):
+            self.dotenv.HUGGING_FACE_HUB_TOKEN = self.dotenv.HF_USER_ACCESS_TOKEN
+
+        local_token = HfFolder.get_token()
+        if local_token is None:
+            if is_notebook():
+                notebook_login()
+            else:
+                logger.info(
+                    "huggingface_hub.notebook_login() is only available in notebook,"
+                    "set HUGGING_FACE_HUB_TOKEN manually"
+                )
 
     @property
-    def app_version(self):
-        return self.about.version
+    def environ(self):
+        return os.environ
 
+    @property
+    def project_workspace_dir(self):
+        if self.path is None:
+            raise ValueError("Path object not initialized")
+        _p = Path(self.path.project_workspace_root)
+        _p.mkdir(parents=True, exist_ok=True)
+        return _p.absolute()
 
-__global_config__ = HyfiConfig()
+    @property
+    def project_dir(self):
+        if self.path is None:
+            raise ValueError("Path object not initialized")
+        _p = Path(self.path.project_root)
+        _p.mkdir(parents=True, exist_ok=True)
+        return _p.absolute()
```

### Comparing `hyfi-0.6.1/src/hyfi/about/__init__.py` & `hyfi-0.6.2/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/batch/__init__.py` & `hyfi-0.6.2/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.6.2/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.6.2/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.6.2/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.6.2/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.6.2/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.6.2/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.6.2/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/copier/__init__.py` & `hyfi-0.6.2/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/dotenv/__init__.py` & `hyfi-0.6.2/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/hydra/__init__.py` & `hyfi-0.6.2/src/hyfi/hydra/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/hydra/main.py` & `hyfi-0.6.2/src/hyfi/hydra/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from typing import IO, Any, Dict, List, Tuple, Union
 
 import hydra
 from omegaconf import DictConfig, ListConfig, OmegaConf, SCMode
 
 from hyfi.__global__ import __home_path__, __hyfi_path__
 from hyfi.__global__.config import __global_config__
+from hyfi.cached_path import cached_path
 from hyfi.hydra import _compose, _select, _to_dict
-from hyfi.io.cached_path import cached_path
-from hyfi.io.file import check_path, exists, join_path, mkdir
 from hyfi.utils.env import dotenv_values, getcwd
+from hyfi.utils.file import check_path, exists, join_path, mkdir
 from hyfi.utils.func import lower_case_with_underscores, strptime, today
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 DictKeyType = Union[str, int, Enum, float, bool]
@@ -36,14 +36,15 @@
     FUNC = "_func_"
     METHOD = "_method_"
     METHOD_NAME = "_name_"
     NAME = "name"
     PARTIAL = "_partial_"
     rcPARAMS = "rcParams"
     RECURSIVE = "_recursive_"
+    SUFFIX = "suffix"
     TARGET = "_target_"
     VERBOSE = "verbose"
 
 
 _config_ = _compose().copy()
```

### Comparing `hyfi-0.6.1/src/hyfi/image/collage.py` & `hyfi-0.6.2/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/image/motion.py` & `hyfi-0.6.2/src/hyfi/image/motion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Motion image processing functions."""
 import os
 import subprocess
 from pathlib import Path
 
-from hyfi.io.file import get_filepaths
+from hyfi.utils.file import get_filepaths
 from hyfi.utils.logging import getLogger
 from hyfi.utils.notebook import display_image
 
 logger = getLogger(__name__)
 
 
 def make_gif(
```

### Comparing `hyfi-0.6.1/src/hyfi/image/plot.py` & `hyfi-0.6.2/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/image/utils.py` & `hyfi-0.6.2/src/hyfi/image/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Image utils."""
 import io
 
 import numpy as np
 from PIL import Image, ImageFont
 
 from hyfi.image.plot import get_plot_font
-from hyfi.io.file import read
+from hyfi.utils.file import read
 
 
 def scale_image(
     image: Image.Image,
     max_width: int = None,
     max_height: int = None,
     max_pixels: int = None,
```

### Comparing `hyfi-0.6.1/src/hyfi/io/cached_path.py` & `hyfi-0.6.2/src/hyfi/cached_path/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pathlib import Path
 
 import gdown
 
-from hyfi.utils.cached_path import _cached_path as _cpath
+from hyfi.cached_path._cached_path import _cached_path as _cpath
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def cached_path(
     url_or_filename,
```

### Comparing `hyfi-0.6.1/src/hyfi/io/file.py` & `hyfi-0.6.2/src/hyfi/utils/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/joblib/__init__.py` & `hyfi-0.6.2/src/hyfi/joblib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 
 from pydantic import BaseModel
 
 from hyfi.__global__ import __about__
 from hyfi.hydra import _compose
-from hyfi.utils.batch import batcher
+from hyfi.joblib.batch import batcher
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 class DistFramwork(BaseModel):
     """Distributed Framework Configuration"""
```

### Comparing `hyfi-0.6.1/src/hyfi/main/__init__.py` & `hyfi-0.6.2/src/hyfi/main/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+"""
+    This module contains the primary class for the hyfi config package, HyFI,
+    as well as various utility functions and imports.
+"""
 from pathlib import Path
 from typing import IO, Any, Dict, List, Tuple, Union
 
 from omegaconf import DictConfig, ListConfig, SCMode
 
+from hyfi.__global__ import __home_path__, __hyfi_path__
 from hyfi.__global__.config import __global_config__
+from hyfi.cached_path import cached_path
 from hyfi.dotenv import DotEnvConfig
 from hyfi.hydra import _compose, _select, _to_config, _to_dict
 from hyfi.hydra.main import (
     DictKeyType,
     SpecialKeys,
-    __home_path__,
-    __hyfi_path__,
     _ensure_kwargs,
     _ensure_list,
     _function,
     _getsource,
     _instantiate,
     _is_config,
     _is_instantiatable,
@@ -29,18 +33,18 @@
     _save,
     _save_json,
     _to_container,
     _to_yaml,
     _update,
     _viewsource,
 )
-from hyfi.io.cached_path import cached_path
-from hyfi.io.file import exists, is_dir, is_file, join_path, mkdir
+from hyfi.joblib.pipe import _apply, _pipe
 from hyfi.project import ProjectConfig
 from hyfi.utils.env import expand_posix_vars, get_osenv, load_dotenv, set_osenv
+from hyfi.utils.file import exists, is_dir, is_file, join_path, mkdir
 from hyfi.utils.func import (
     dict_product,
     dict_to_dataframe,
     records_to_dataframe,
     to_dateparm,
     to_datetime,
     to_numeric,
@@ -60,15 +64,14 @@
     display,
     display_image,
     get_display,
     hide_code_in_slideshow,
     is_colab,
     is_notebook,
 )
-from hyfi.utils.pipe import _apply, _pipe
 
 logger = getLogger(__name__)
 
 
 def _about(cfg):
     pkg_name = cfg.about.__package_name__
     name = cfg.about.name
@@ -78,15 +81,15 @@
             continue
         print(f"{k:11} : {v}")
     if pkg_name:
         print(f"\nExecute `{pkg_name} --help` to see what you can do with {name}")
 
 
 class HyFI:
-    """hyfi config primary class"""
+    """Primary class for the hyfi config package"""
 
     config = __global_config__
     SpeicialKeys = SpecialKeys
     __version__ = __global_config__.__version__
     __hyfi_path__ = __hyfi_path__()
     __home_path__ = __home_path__()
 
@@ -343,75 +346,39 @@
             override=override,
             dotenv_filename=dotenv_filename,
             dotenv_dir=dotenv_dir,
             verbose=verbose,
         )
 
     @staticmethod
-    def path(
+    def cached_path(
         url_or_filename,
         extract_archive: bool = False,
         force_extract: bool = False,
         return_parent_dir: bool = False,
         cache_dir=None,
         verbose: bool = False,
     ):
         """
-        Given something that might be a URL or local path, determine which.
-        If it's a remote resource, download the file and cache it, and
-        then return the path to the cached file. If it's already a local path,
-        make sure the file exists and return the path.
+        Attempts to cache a file or URL and return the path to the cached file.
+        If required libraries 'cached_path' and 'gdown' are not installed, raises an ImportError.
 
-        For URLs, the following schemes are all supported out-of-the-box:
-
-        * ``http`` and ``https``,
-        * ``gd`` for objects on `Google Drive`_, and
-        * ``hf`` for objects or repositories on `HuggingFace Hub`_.
-
-        Parameters
-        ----------
-
-        url_or_filename :
-            A URL or path to parse and possibly download.
-
-        extract_archive :
-            If ``True``, then zip or tar.gz archives will be automatically extracted.
-            In which case the directory is returned.
-
-        force_extract :
-            If ``True`` and the file is an archive file, it will be extracted regardless
-            of whether or not the extracted directory already exists.
-
-            .. caution::
-                Use this flag with caution! This can lead to race conditions if used
-                from multiple processes on the same file.
-
-        cache_dir :
-            The directory to cache downloads. If not specified, the global default cache directory
-            will be used (``~/.cache/cached_path``). This can be set to something else with
-            :func:`set_cache_dir()`.
-
-        Returns
-        -------
-        :class:`pathlib.Path`
-            The local path to the (potentially cached) resource.
-
-        Raises
-        ------
-        ``FileNotFoundError``
-
-            If the resource cannot be found locally or remotely.
-
-        ``ValueError``
-            When the URL is invalid.
+        Args:
+            url_or_filename (str): The URL or filename to be cached.
+            extract_archive (bool, optional): Whether to extract the file if it's an archive. Defaults to False.
+            force_extract (bool, optional): Whether to force extraction even if the destination already exists. Defaults to False.
+            return_parent_dir (bool, optional): If True, returns the parent directory of the cached file. Defaults to False.
+            cache_dir (str, optional): Directory to store cached files. Defaults to None.
+            verbose (bool, optional): Whether to print informative messages during the process. Defaults to False.
 
-        ``Other errors``
-            Other error types are possible as well depending on the client used to fetch
-            the resource.
+        Raises:
+            ImportError: If the required libraries 'cached_path' and 'gdown' are not imported.
 
+        Returns:
+            str: Path to the cached file or its parent directory, depending on the 'return_parent_dir' parameter.
         """
         return cached_path(
             url_or_filename,
             extract_archive=extract_archive,
             force_extract=force_extract,
             return_parent_dir=return_parent_dir,
             cache_dir=cache_dir,
@@ -484,15 +451,15 @@
         columns=None,
         index=False,
         filetype="parquet",
         suffix=None,
         verbose=False,
         **kwargs,
     ):
-        from hyfi.io.file import save_data
+        from hyfi.utils.file import save_data
 
         if filename is None:
             raise ValueError("filename must be specified")
         save_data(
             data,
             filename,
             base_dir=base_dir,
@@ -502,15 +469,15 @@
             suffix=suffix,
             verbose=verbose,
             **kwargs,
         )
 
     @staticmethod
     def load_data(filename=None, base_dir=None, filetype=None, verbose=False, **kwargs):
-        from hyfi.io.file import load_data
+        from hyfi.utils.file import load_data
 
         if filename is not None:
             filename = str(filename)
         if SpecialKeys.TARGET in kwargs:
             return _instantiate(
                 kwargs,
                 filename=filename,
@@ -528,15 +495,15 @@
             **kwargs,
         )
 
     @staticmethod
     def get_filepaths(
         filename_patterns=None, base_dir=None, recursive=True, verbose=True, **kwargs
     ):
-        from hyfi.io.file import get_filepaths
+        from hyfi.utils.file import get_filepaths
 
         if filename_patterns is None:
             raise ValueError("filename must be specified")
         return get_filepaths(
             filename_patterns,
             base_dir=base_dir,
             recursive=recursive,
@@ -550,29 +517,29 @@
         columns=None,
         add_key_as_name=False,
         name_column="_name_",
         ignore_index=True,
         verbose=False,
         **kwargs,
     ):
-        from hyfi.io.file import concat_data
+        from hyfi.utils.file import concat_data
 
         return concat_data(
             data,
             columns=columns,
             add_key_as_name=add_key_as_name,
             name_column=name_column,
             ignore_index=ignore_index,
             verbose=verbose,
             **kwargs,
         )
 
     @staticmethod
     def is_dataframe(data):
-        from hyfi.io.file import is_dataframe
+        from hyfi.utils.file import is_dataframe
 
         return is_dataframe(data)
 
     @staticmethod
     def is_colab():
         return is_colab()
 
@@ -943,15 +910,15 @@
     def get_image_font(fontname=None, fontsize=12):
         from hyfi.image.collage import get_image_font
 
         return get_image_font(fontname, fontsize)
 
     @staticmethod
     def read(uri, mode="rb", encoding=None, head=None, **kwargs):
-        from hyfi.io.file import read as _read
+        from hyfi.utils.file import read as _read
 
         return _read(uri, mode, encoding, head, **kwargs)
 
     @staticmethod
     def load_image(
         image_or_uri,
         max_width: int = None,
@@ -989,14 +956,31 @@
         num_workers: int = -1,
         log_level: str = "",
         autotime: bool = True,
         retina: bool = True,
         verbose: Union[bool, int] = False,
         **kwargs,
     ) -> ProjectConfig:
+        """
+        Initialize and start hyfi.
+
+        Args:
+                project_name: Name of the project to use.
+                task_name: Name of the task to use.
+                project_description: Description of the project that will be used.
+                project_root: Root directory of the project.
+                project_workspace_name: Name of the project's workspace directory.
+                global_hyfi_root: Root directory of the global hyfi.
+                global_workspace_name: Name of the global hierachical workspace directory.
+                num_workers: Number of workers to run.
+                log_level: Log level for the log.
+                autotime: Whether to automatically set time and / or keep track of run times.
+                retina: Whether to use retina or not.
+                verbose: Enables or disables logging
+        """
         __global_config__.init_workspace(
             project_name=project_name,
             task_name=task_name,
             project_description=project_description,
             project_root=project_root,
             project_workspace_name=project_workspace_name,
             global_hyfi_root=global_hyfi_root,
```

### Comparing `hyfi-0.6.1/src/hyfi/path/__init__.py` & `hyfi-0.6.2/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/path/batch.py` & `hyfi-0.6.2/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/batch/apply.py` & `hyfi-0.6.2/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.6.2/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/batch/batcher.py` & `hyfi-0.6.2/src/hyfi/joblib/batch/batcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from contextlib import closing
 from math import ceil
 
 import pandas as pd
 import scipy.sparse as ssp
 from tqdm.auto import tqdm
 
-from ..logging import getLogger
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 class Batcher(object):
     """Scheduler to handle parallel jobs on minibatches
```

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/__init__.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/_cached_path.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/cache_file.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/common.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/file_lock.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/meta.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/progress.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/__init__.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/beaker.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/hf.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/http.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/scheme_client.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/testing.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/cached_path/util.py` & `hyfi-0.6.2/src/hyfi/cached_path/_cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/env.py` & `hyfi-0.6.2/src/hyfi/utils/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from string import Template
 from typing import Any, Union
 
 import dotenv
 import hydra
 
-from hyfi.io.file import is_dir
+from hyfi.utils.file import is_dir
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def getcwd():
     """Get the original working directory before Hydra changed it.
```

### Comparing `hyfi-0.6.1/src/hyfi/utils/func.py` & `hyfi-0.6.2/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/google.py` & `hyfi-0.6.2/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/gpu.py` & `hyfi-0.6.2/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/lib.py` & `hyfi-0.6.2/src/hyfi/utils/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utilities for loading libraries and dependencies."""
 import importlib
 import os
 import subprocess
 import sys
 from pathlib import Path
 
-from hyfi.io.file import is_dir, is_file
+from hyfi.utils.file import is_dir, is_file
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def gitclone(
     url: str,
```

### Comparing `hyfi-0.6.1/src/hyfi/utils/logging.py` & `hyfi-0.6.2/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/src/hyfi/utils/notebook.py` & `hyfi-0.6.2/src/hyfi/utils/notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utilities for working with notebooks.""" ""
 import logging
 import os
 import sys
 
-from hyfi.io.file import read
+from hyfi.utils.file import read
 
 logger = logging.getLogger(__name__)
 
 
 def is_notebook():
     """Check if the code is running in a notebook."""
     try:
```

### Comparing `hyfi-0.6.1/src/hyfi/utils/pipe.py` & `hyfi-0.6.2/src/hyfi/joblib/pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tqdm.auto import tqdm
 
 from hyfi.hydra.main import SpecialKeys, _partial
-from hyfi.utils.batch import batcher
-from hyfi.utils.batch.apply import decorator_apply
+from hyfi.joblib.batch import batcher
+from hyfi.joblib.batch.apply import decorator_apply
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def _pipe(data, pipe):
     _func_ = pipe.get(SpecialKeys.FUNC)
```

### Comparing `hyfi-0.6.1/src/hyfi/utils/tools.py` & `hyfi-0.6.2/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.1/PKG-INFO` & `hyfi-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.6.1
+Version: 0.6.2
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

