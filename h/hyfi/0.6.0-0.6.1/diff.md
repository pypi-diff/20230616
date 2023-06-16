# Comparing `tmp/hyfi-0.6.0.tar.gz` & `tmp/hyfi-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.6.0.tar", max compression
+gzip compressed data, was "hyfi-0.6.1.tar", max compression
```

## Comparing `hyfi-0.6.0.tar` & `hyfi-0.6.1.tar`

### file list

```diff
@@ -1,72 +1,78 @@
--rw-r--r--   0        0        0     1071 2023-06-15 22:03:09.087991 hyfi-0.6.0/LICENSE
--rw-r--r--   0        0        0     1632 2023-06-15 22:03:09.087991 hyfi-0.6.0/README.md
--rw-r--r--   0        0        0     4566 2023-06-15 22:03:43.544242 hyfi-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3608 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2136 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      359 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-15 22:03:43.444241 hyfi-0.6.0/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-15 22:03:43.444241 hyfi-0.6.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      320 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      717 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      123 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      604 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0     1719 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      781 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       29 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    12765 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/config/batch.py
--rw-r--r--   0        0        0     5728 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/config/path.py
--rw-r--r--   0        0        0    25427 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/env.py
--rw-r--r--   0        0        0    12839 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8383 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4318 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2494 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3313 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     6819 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12468 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/io/file.py
--rw-r--r--   0        0        0    30299 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/main.py
--rw-r--r--   0        0        0        0 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    16580 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     1206 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/version.py
--rw-r--r--   0        0        0     6369 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/copier.py
--rw-r--r--   0        0        0     5603 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/env.py
--rw-r--r--   0        0        0     9920 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1064 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3595 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4129 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1986 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9760 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2022 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/pipe.py
--rw-r--r--   0        0        0     5466 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     2986 1970-01-01 00:00:00.000000 hyfi-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 04:14:25.157391 hyfi-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-16 04:14:25.157391 hyfi-0.6.1/README.md
+-rw-r--r--   0        0        0     4592 2023-06-16 04:14:48.186760 hyfi-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3661 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2216 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      598 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     5379 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      417 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-16 04:14:48.118757 hyfi-0.6.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0      777 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0    12718 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-16 04:14:48.118757 hyfi-0.6.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      320 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-16 04:14:25.161391 hyfi-0.6.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      717 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      123 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      604 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      781 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0     6369 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     5886 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0    12832 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8393 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4327 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2497 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3326 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     6825 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12472 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/io/file.py
+-rw-r--r--   0        0        0     3479 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0    30375 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0     2903 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     5743 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     5566 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    16580 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     1206 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/cached_path/version.py
+-rw-r--r--   0        0        0     5665 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0     9920 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1114 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3699 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4142 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1986 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9763 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     2084 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/pipe.py
+-rw-r--r--   0        0        0     5476 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-16 04:14:25.165392 hyfi-0.6.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.6.1/PKG-INFO
```

### Comparing `hyfi-0.6.0/LICENSE` & `hyfi-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/README.md` & `hyfi-0.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # HyFI: Hydra Fast Interface
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 
 
 <!-- Links: -->
+[codecov-image]: https://codecov.io/gh/entelecheia/hyfi/branch/main/graph/badge.svg?token=HCYTYW1WVF
+[codecov-url]: https://codecov.io/gh/entelecheia/hyfi
 [pypi-image]: https://img.shields.io/pypi/v/hyfi
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi
 [license-url]: https://github.com/entelecheia/hyfi/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi
 [release-url]: https://github.com/entelecheia/hyfi/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

### Comparing `hyfi-0.6.0/pyproject.toml` & `hyfi-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.6.0"
+version = "0.6.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
@@ -109,14 +109,15 @@
     "docs",
     "tests",
     "venv",
     ".copier-template",
     ".refs",
     "cached_path",
 ]
+ignore = ["E501", "W503"]
 per-file-ignores = [
     '__init__.py:F401,F403',
     '_version.py:W292',
     '*:E501,E203',
     'notebook.py:F821,E501',
     'motion.py:W605,E501',
 ]
```

### Comparing `hyfi-0.6.0/src/hyfi/__cli__.py` & `hyfi-0.6.1/src/hyfi/__cli__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Command line interface for HyFI"""
 import os
 from typing import Optional
 
 import hydra
+from omegaconf import DictConfig
 
-from hyfi.env import HyfiConfig, __about__, __hydra_version_base__
-from hyfi.main import DictConfig, HyFI, _about, getLogger
-from hyfi.utils.copier import Copier
+from hyfi.__global__ import __about__, __hydra_version_base__
+from hyfi.__global__.config import HyfiConfig
+from hyfi.copier import Copier
+from hyfi.main import HyFI, _about
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 __config_path__ = "conf"
 __config_name__ = "config"
 
@@ -50,15 +53,16 @@
     Initializes Hydra and instantiates the class.
     Prints the configuration to standard out if verbose is set to True
 
     Args:
         cfg: Configuration dictionary to be used for instantiation
 
     Returns:
-        None if everything went fine otherwise an error is raised to indicate the reason for the failure ( s )
+        None if everything went fine otherwise an error is raised
+        to indicate the reason for the failure
     """
     hyfi = HyfiConfig(**cfg)  # type: ignore
     verbose = hyfi.verbose
     app_name = hyfi.about.name
     print_config = hyfi.print_config
     print_resolved_config = hyfi.print_resolved_config
 
@@ -75,16 +79,16 @@
             HyFI.pprint(cfg)
         else:
             logger.info("## hydra configuration ##")
             print(HyFI.to_yaml(cfg))
 
     # Prints out the working directory and original working directory.
     if verbose:
-        logger.info(f"Hydra working directory : {os.getcwd()}")
-        logger.info(f"Orig working directory  : {hydra.utils.get_original_cwd()}")
+        logger.info("Hydra working directory : %s", {os.getcwd()})
+        logger.info("Orig working directory  : %s", {hydra.utils.get_original_cwd()})
 
     HyFI.instantiate(cfg)
 
     HyFI.terminate()
 
 
 def hydra_main(
@@ -111,9 +115,8 @@
         config_name=config_name,
         version_base=__hydra_version_base__,
     )(cli_main)()
 
 
 # Run the command line interface
 if __name__ == "__main__":
-    """Run the command line interface"""
     hydra_main()
```

### Comparing `hyfi-0.6.0/src/hyfi/__click__.py` & `hyfi-0.6.1/src/hyfi/__click__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Command line interface for HyFI"""
 
 import click
 
+from hyfi.__global__ import __hyfi_path__
+from hyfi.__global__.config import HyfiConfig
 from hyfi._version import __version__
-from hyfi.env import HyfiConfig
-from hyfi.hydra import __hyfi_path__
+from hyfi.copier import Copier
 from hyfi.main import _about
-from hyfi.utils.copier import Copier
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 @click.group()
 @click.version_option(__version__)
@@ -19,15 +19,18 @@
 
 
 @cli.command()
 @click.option(
     "--src_path", default=f"{__hyfi_path__()}/conf", help="Source path to copy from"
 )
 @click.option(
-    "--dst_path", show_default=True, default="conf", help="Destination path to copy to"
+    "--dst_path",
+    show_default=True,
+    default="./tmp/conf",
+    help="Destination path to copy to",
 )
 @click.option("--exclude", default=None, help="Exclude files matching this pattern")
 @click.option("--skip_if_exists", default=False, help="Skip if destination exists")
 @click.option("--overwrite", default=False, help="Overwrite destination")
 @click.option("--dry_run", default=False, help="Dry run")
 @click.option("--verbose", is_flag=True, default=False, help="Verbose output")
 def cc(**args):
@@ -42,22 +45,23 @@
 
 @cli.command()
 def about():
     """
     Print the about information for Hyfi.
     """
     cfg = HyfiConfig()
+    cfg.about.version = __version__
     _about(cfg)
 
 
 @cli.command()
 @click.option(
-    "--uninstall", is_flag=True, default=False, help="Uninstall shell completion"
+    "--uninstall", "-u", is_flag=True, default=False, help="Uninstall shell completion"
 )
-@click.option("--shell", default="zsh", help="Shell to install completion for")
+@click.option("--shell", "-s", default="zsh", help="Shell to install completion for")
 def sc(uninstall, shell):
     """
     Install or Uninstall shell completion for Hyfi.
     """
     if uninstall:
         click.echo(f"Uninstall shell completion for {shell}:")
         click.echo(
```

### Comparing `hyfi-0.6.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.6.1/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.6.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.6.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.6.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.6.1/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.6.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.6.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/config/batch.py` & `hyfi-0.6.1/src/hyfi/batch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import random
 from pathlib import Path
 from typing import Optional, Union
 
 from omegaconf import DictConfig
 from pydantic import BaseModel, validator
 
-from hyfi.config.path import PathConfig
-from hyfi.env import ProjectConfig, _to_config, _to_dict, getLogger
-from hyfi.hydra import _compose, _load, _merge, _methods, _print, _save, _save_json
+from hyfi.hydra import _compose, _to_config, _to_dict
+from hyfi.hydra.main import _load, _merge, _methods, _print, _save, _save_json
+from hyfi.path.batch import BatchPathConfig
+from hyfi.project import ProjectConfig
 from hyfi.utils.lib import ensure_import_module
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 class BaseBatchConfig(BaseModel):
     batch_name: str
     batch_num: int = None
@@ -31,17 +33,14 @@
     config_json = "config.json"
     config_dirname = "configs"
     verbose: Union[bool, int] = False
 
     def __init__(self, **data):
         if not data:
             data = _compose("batch")
-            logger.info(
-                f"There is no batch in the config, using default batch: {data.batch_name}"
-            )
         super().__init__(**data)
         self.init_batch_num()
 
     def init_batch_num(self):
         if self.batch_num is None:
             num_files = len(list(self.config_dir.glob(self.config_filepattern)))
             self.batch_num = num_files - 1 if self.resume_latest else num_files
@@ -108,15 +107,15 @@
         return self.config_dir / self.config_jsonfile
 
 
 class BaseConfigModel(BaseModel):
     config_name: str = None
     config_group: str = None
     name: str
-    path: PathConfig = None
+    path: BatchPathConfig = None
     project: ProjectConfig = None
     module: DictConfig = None
     auto: Union[DictConfig, str] = None
     force: Union[DictConfig, str] = None
     autoload: bool = False
     version: str = "0.0.0"
     _config_: DictConfig = None
@@ -172,15 +171,15 @@
             path = _compose("path=_batch_")
             logger.info(
                 f"There is no path in the config, using default path: {path.root}"
             )
             self._config_.path = path
         if root_dir is not None:
             path.root = str(root_dir)
-        self.path = PathConfig(**path)
+        self.path = BatchPathConfig(**path)
 
     def set_name(self, val):
         self._config_.name = val
         if self.name is None or self.name != val:
             self.name = val
 
     def initialize_configs(self, root_dir=None, **kwargs):
@@ -204,15 +203,15 @@
 
     @property
     def project_dir(self):
         return Path(self.project.project_dir)
 
     @property
     def workspace_dir(self):
-        return Path(self.project.workspace_dir)
+        return Path(self.project.project_workspace_dir)
 
     @property
     def model_dir(self):
         return self.path.model_dir
 
     @property
     def log_dir(self):
```

### Comparing `hyfi-0.6.0/src/hyfi/config/path.py` & `hyfi-0.6.1/src/hyfi/path/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path
 from typing import Any
 
 from pydantic import BaseModel
 
-from hyfi.env import getLogger
 from hyfi.hydra import _compose
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
-class PathConfig(BaseModel):
+class BatchPathConfig(BaseModel):
     config_name: str = "__batch__"
 
     project_workspace_root = ""
     batch_name: str = "demo"
     batch_output: str = ""
     task_name: str = "default-task"
     task_root: str = ""
```

### Comparing `hyfi-0.6.0/src/hyfi/hydra.py` & `hyfi-0.6.1/src/hyfi/hydra/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 from enum import Enum
 from pathlib import Path
 from typing import IO, Any, Dict, List, Tuple, Union
 
 import hydra
 from omegaconf import DictConfig, ListConfig, OmegaConf, SCMode
 
-from .env import __global_config__, _compose, _select, _to_dict
-from .io.cached_path import cached_path
-from .io.file import check_path, exists, join_path, mkdir
-from .utils.env import dotenv_values, getcwd
-from .utils.func import lower_case_with_underscores, strptime, today
-from .utils.logging import getLogger
+from hyfi.__global__ import __home_path__, __hyfi_path__
+from hyfi.__global__.config import __global_config__
+from hyfi.hydra import _compose, _select, _to_dict
+from hyfi.io.cached_path import cached_path
+from hyfi.io.file import check_path, exists, join_path, mkdir
+from hyfi.utils.env import dotenv_values, getcwd
+from hyfi.utils.func import lower_case_with_underscores, strptime, today
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 DictKeyType = Union[str, int, Enum, float, bool]
 
 
@@ -316,22 +318,14 @@
             logger.info(f"Function {_name_} not callable")
             return None
     else:
         logger.info(f"Skipping execute of {fn}")
         return None
 
 
-def __hyfi_path__():
-    return Path(__file__).parent.as_posix()
-
-
-def __home_path__():
-    return Path.home().as_posix()
-
-
 def __search_package_path__():
     return __global_config__.hyfi_config_path
 
 
 OmegaConf.register_new_resolver("__hyfi_path__", __hyfi_path__)
 OmegaConf.register_new_resolver("__search_package_path__", __search_package_path__)
 OmegaConf.register_new_resolver("__home_path__", __home_path__)
```

### Comparing `hyfi-0.6.0/src/hyfi/image/collage.py` & `hyfi-0.6.1/src/hyfi/image/collage.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List
 
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image, ImageDraw
 from pydantic import BaseModel
 
-from .utils import get_image_font, load_image, load_images, scale_image
+from hyfi.image.utils import get_image_font, load_image, load_images, scale_image
 
 log = logging.getLogger(__name__)
 
 
 class Collage(BaseModel):
     """Collage of images."""
```

### Comparing `hyfi-0.6.0/src/hyfi/image/motion.py` & `hyfi-0.6.1/src/hyfi/image/motion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Motion image processing functions."""
 import os
 import subprocess
 from pathlib import Path
 
-from ..io.file import get_filepaths
-from ..utils.logging import getLogger
-from ..utils.notebook import display_image
+from hyfi.io.file import get_filepaths
+from hyfi.utils.logging import getLogger
+from hyfi.utils.notebook import display_image
 
 logger = getLogger(__name__)
 
 
 def make_gif(
     image_filepaths=None,
     filename_patterns=None,
```

### Comparing `hyfi-0.6.0/src/hyfi/image/plot.py` & `hyfi-0.6.1/src/hyfi/image/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import platform
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 from matplotlib import font_manager, rc
 
-from ..utils.logging import getLogger
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def get_plot_font(
     set_font_for_matplot=True, fontpath=None, fontname=None, verbose=False
 ):
```

### Comparing `hyfi-0.6.0/src/hyfi/image/utils.py` & `hyfi-0.6.1/src/hyfi/image/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Image utils."""
 import io
 
 import numpy as np
 from PIL import Image, ImageFont
 
-from ..io.file import read
-from .plot import get_plot_font
+from hyfi.image.plot import get_plot_font
+from hyfi.io.file import read
 
 
 def scale_image(
     image: Image.Image,
     max_width: int = None,
     max_height: int = None,
     max_pixels: int = None,
```

### Comparing `hyfi-0.6.0/src/hyfi/io/cached_path.py` & `hyfi-0.6.1/src/hyfi/io/cached_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 import gdown
 
-from ..utils.cached_path import _cached_path as _cpath
-from ..utils.logging import getLogger
+from hyfi.utils.cached_path import _cached_path as _cpath
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def cached_path(
     url_or_filename,
     extract_archive: bool = False,
```

### Comparing `hyfi-0.6.0/src/hyfi/io/file.py` & `hyfi-0.6.1/src/hyfi/io/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import re
 from glob import glob
 from pathlib import Path, PosixPath, WindowsPath
 from typing import List, Union
 
 import pandas as pd
 
-from ..utils.func import elapsed_timer
-from ..utils.logging import getLogger
+from hyfi.utils.func import elapsed_timer
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def is_valid_regex(expr: str) -> bool:
     """Check if a string is a valid regular expression"""
     try:
@@ -29,15 +29,15 @@
 def glob_re(pattern: str, base_dir: str, recursive: bool = False) -> list:
     """Glob files matching a regular expression"""
     if is_valid_regex(pattern):
         pattern = pattern[2:]
         pattern = re.compile(pattern)
         files = []
         if recursive:
-            for (dirpath, dirnames, filenames) in os.walk(base_dir):
+            for dirpath, dirnames, filenames in os.walk(base_dir):
                 files += [
                     os.path.join(dirpath, file)
                     for file in filenames
                     if pattern.search(file)
                 ]
         else:
             files = [
```

### Comparing `hyfi-0.6.0/src/hyfi/main.py` & `hyfi-0.6.1/src/hyfi/main/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from pathlib import Path
 from typing import IO, Any, Dict, List, Tuple, Union
 
 from omegaconf import DictConfig, ListConfig, SCMode
 
-from hyfi.env import DotEnvConfig, ProjectConfig, __global_config__, _to_config
-from hyfi.hydra import (
+from hyfi.__global__.config import __global_config__
+from hyfi.dotenv import DotEnvConfig
+from hyfi.hydra import _compose, _select, _to_config, _to_dict
+from hyfi.hydra.main import (
     DictKeyType,
     SpecialKeys,
     __home_path__,
     __hyfi_path__,
-    _compose,
     _ensure_kwargs,
     _ensure_list,
     _function,
     _getsource,
     _instantiate,
     _is_config,
     _is_instantiatable,
@@ -23,23 +24,22 @@
     _merge,
     _methods,
     _partial,
     _print,
     _run,
     _save,
     _save_json,
-    _select,
     _to_container,
-    _to_dict,
     _to_yaml,
     _update,
     _viewsource,
 )
 from hyfi.io.cached_path import cached_path
 from hyfi.io.file import exists, is_dir, is_file, join_path, mkdir
+from hyfi.project import ProjectConfig
 from hyfi.utils.env import expand_posix_vars, get_osenv, load_dotenv, set_osenv
 from hyfi.utils.func import (
     dict_product,
     dict_to_dataframe,
     records_to_dataframe,
     to_dateparm,
     to_datetime,
```

### Comparing `hyfi-0.6.0/src/hyfi/utils/batch/apply.py` & `hyfi-0.6.1/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.6.1/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/batch/batcher.py` & `hyfi-0.6.1/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/__init__.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/_cached_path.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/cache_file.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/common.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/file_lock.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/meta.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/progress.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/__init__.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/beaker.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/hf.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/http.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/scheme_client.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/testing.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/cached_path/util.py` & `hyfi-0.6.1/src/hyfi/utils/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/copier.py` & `hyfi-0.6.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/env.py` & `hyfi-0.6.1/src/hyfi/utils/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from pathlib import Path
 from string import Template
 from typing import Any, Union
 
 import dotenv
 import hydra
 
-from ..io.file import is_dir
-from .logging import getLogger
+from hyfi.io.file import is_dir
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def getcwd():
     """Get the original working directory before Hydra changed it.
 
@@ -29,14 +29,15 @@
     try:
         return hydra.utils.get_original_cwd()
     except ValueError:
         return os.getcwd()
 
 
 def expand_posix_vars(posix_expr: str, context: dict = None) -> str:  # type: ignore
+    # sourcery skip: dict-assign-update-to-union
     """
     Expand POSIX variables in a string.
 
     Args:
         posix_expr (str): The string containing POSIX variables to be expanded.
         context (dict, optional): A dictionary containing additional variables to be used in the expansion.
             Defaults to None.
```

### Comparing `hyfi-0.6.0/src/hyfi/utils/func.py` & `hyfi-0.6.1/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/google.py` & `hyfi-0.6.1/src/hyfi/utils/google.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Google Colab utilities."""
 import os
 
-from .env import set_osenv
-from .logging import getLogger
+from hyfi.utils.env import set_osenv
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def mount_google_drive(
     project_root: str = "",
     project_name: str = "",
@@ -17,15 +17,17 @@
     """Mount Google Drive to Colab."""
     try:
         from google.colab import drive  # type: ignore
 
         drive.mount(mountpoint, force_remount=force_remount, timeout_ms=timeout_ms)
 
         if project_root:
-            if not project_root.startswith(os.path.sep) and not project_root.startswith(".."):
+            if not project_root.startswith(os.path.sep) and not project_root.startswith(
+                ".."
+            ):
                 project_root = os.path.join(mountpoint, project_root)
             set_osenv("HYFI_PROJECT_ROOT", project_root)
             logger.info(f"Setting HYFI_PROJECT_ROOT to {project_root}")
         if project_name:
             set_osenv("HYFI_PROJECT_NAME", project_name)
             logger.info(f"Setting HYFI_PROJECT_NAME to {project_name}")
     except ImportError:
```

### Comparing `hyfi-0.6.0/src/hyfi/utils/gpu.py` & `hyfi-0.6.1/src/hyfi/utils/gpu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """GPU utilities"""
+
+import contextlib
 import gc
 import os
 import time
 from threading import Thread
 
-from .logging import getLogger
-from .notebook import clear_output
+from hyfi.utils.logging import getLogger
+from hyfi.utils.notebook import clear_output
 
 logger = getLogger(__name__)
 
 try:
-    import GPUtil
+    import GPUtil  # type: ignore
 except ImportError:
     logger.info("GPUtil not found. Please install it to use GPU utilities.")
 
 
 class GPUMon(Thread):
     """Monitor GPU usage in a separate thread"""
 
@@ -84,55 +86,53 @@
             excludeID=excludeID,
             excludeUUID=excludeUUID,
         )
 
     @staticmethod
     def release_gpu_memory():
         gc.collect()
-        try:
-            import torch
+        with contextlib.suppress(ImportError):
+            import torch  # type: ignore
 
             torch.cuda.empty_cache()
-        except ImportError:
-            pass
 
 
 def nvidia_smi():
     """Run nvidia-smi and return the output as a string"""
     import subprocess
 
-    return subprocess.run(
-        ["nvidia-smi", "-L"], stdout=subprocess.PIPE
-    ).stdout.decode("utf-8")
+    return subprocess.run(["nvidia-smi", "-L"], stdout=subprocess.PIPE).stdout.decode(
+        "utf-8"
+    )
 
 
 def is_cuda_available():
     """Check if cuda is available"""
     try:
-        import torch
+        import torch  # type: ignore
 
         return torch.cuda.is_available()
     except ImportError:
         return False
 
 
 def set_cuda(device=0):
     """Set cuda device to use"""
     try:
-        import torch
+        import torch  # type: ignore
 
         _names = []
         if isinstance(device, str):
             device = device.replace("cuda:", "")
             ids = device.split(",")
         else:
             ids = [str(device)]
         for id in ids:
             _device_name = torch.cuda.get_device_name(int(id))
             _names.append(f"{_device_name} (id:{id})")
         logger.info(f"Setting cuda device to {_names}")
         device = ", ".join(ids)
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = device
-    except ImportError:
+    except ImportError as e:
         os.environ["CUDA_VISIBLE_DEVICES"] = ""
-        raise Exception("Cuda device not found")
+        raise Exception("Cuda device not found") from e
```

### Comparing `hyfi-0.6.0/src/hyfi/utils/lib.py` & `hyfi-0.6.1/src/hyfi/utils/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Utilities for loading libraries and dependencies."""
 import importlib
 import os
 import subprocess
 import sys
 from pathlib import Path
 
-from ..io.file import is_dir, is_file
-from .logging import getLogger
+from hyfi.io.file import is_dir, is_file
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def gitclone(
     url: str,
     targetdir: str = "",
```

### Comparing `hyfi-0.6.0/src/hyfi/utils/logging.py` & `hyfi-0.6.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.6.0/src/hyfi/utils/notebook.py` & `hyfi-0.6.1/src/hyfi/utils/notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utilities for working with notebooks.""" ""
 import logging
 import os
 import sys
 
-from ..io.file import read
+from hyfi.io.file import read
 
 logger = logging.getLogger(__name__)
 
 
 def is_notebook():
     """Check if the code is running in a notebook."""
     try:
```

### Comparing `hyfi-0.6.0/src/hyfi/utils/pipe.py` & `hyfi-0.6.1/src/hyfi/utils/pipe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from tqdm.auto import tqdm
 
-from ..hydra import SpecialKeys, _partial
-from .batch import batcher, decorator_apply
-from .logging import getLogger
+from hyfi.hydra.main import SpecialKeys, _partial
+from hyfi.utils.batch import batcher
+from hyfi.utils.batch.apply import decorator_apply
+from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def _pipe(data, pipe):
     _func_ = pipe.get(SpecialKeys.FUNC)
     _fn = _partial(_func_)
```

### Comparing `hyfi-0.6.0/src/hyfi/utils/tools.py` & `hyfi-0.6.1/src/hyfi/utils/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pathlib import Path
 from types import TracebackType
 from typing import Any, Callable, Optional, TextIO, Tuple, Union
 
 import colorama
 from pydantic import StrictBool
 
-from .types import IntSeq
+from hyfi.utils.types import IntSeq
 
 colorama.init()
 
 
 class Style:
     """Common color styles."""
```

### Comparing `hyfi-0.6.0/PKG-INFO` & `hyfi-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.6.0
+Version: 0.6.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -36,17 +36,20 @@
 
 # HyFI: Hydra Fast Interface
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 
 
 <!-- Links: -->
+[codecov-image]: https://codecov.io/gh/entelecheia/hyfi/branch/main/graph/badge.svg?token=HCYTYW1WVF
+[codecov-url]: https://codecov.io/gh/entelecheia/hyfi
 [pypi-image]: https://img.shields.io/pypi/v/hyfi
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi
 [license-url]: https://github.com/entelecheia/hyfi/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi
 [release-url]: https://github.com/entelecheia/hyfi/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

