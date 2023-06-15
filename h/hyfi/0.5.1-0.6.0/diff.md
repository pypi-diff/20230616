# Comparing `tmp/hyfi-0.5.1.tar.gz` & `tmp/hyfi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.5.1.tar", max compression
+gzip compressed data, was "hyfi-0.6.0.tar", max compression
```

## Comparing `hyfi-0.5.1.tar` & `hyfi-0.6.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0     1071 2023-06-14 02:57:55.744163 hyfi-0.5.1/LICENSE
--rw-r--r--   0        0        0     1632 2023-06-14 02:57:55.744163 hyfi-0.5.1/README.md
--rw-r--r--   0        0        0     4515 2023-06-14 02:58:19.940555 hyfi-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3608 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0      359 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-14 02:58:19.868553 hyfi-0.5.1/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-14 02:58:19.868553 hyfi-0.5.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      320 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      701 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      717 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      123 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      554 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0     1518 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      669 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       29 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    12765 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/config/batch.py
--rw-r--r--   0        0        0     5800 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/config/path.py
--rw-r--r--   0        0        0    24230 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/env.py
--rw-r--r--   0        0        0    12839 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8383 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4318 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2494 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3313 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     6819 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12468 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/io/file.py
--rw-r--r--   0        0        0    28965 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/main.py
--rw-r--r--   0        0        0        0 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    16580 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     1206 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/version.py
--rw-r--r--   0        0        0     6131 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/copier.py
--rw-r--r--   0        0        0     5603 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/env.py
--rw-r--r--   0        0        0     9920 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1064 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3595 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4129 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1986 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9760 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2022 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/pipe.py
--rw-r--r--   0        0        0     5466 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-15 22:03:09.087991 hyfi-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1632 2023-06-15 22:03:09.087991 hyfi-0.6.0/README.md
+-rw-r--r--   0        0        0     4566 2023-06-15 22:03:43.544242 hyfi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3608 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2136 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      359 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-15 22:03:43.444241 hyfi-0.6.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-15 22:03:43.444241 hyfi-0.6.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      320 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      717 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      123 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      604 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      781 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       29 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    12765 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0     5728 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/config/path.py
+-rw-r--r--   0        0        0    25427 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/env.py
+-rw-r--r--   0        0        0    12839 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8383 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4318 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2494 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3313 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     6819 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12468 2023-06-15 22:03:09.091991 hyfi-0.6.0/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    30299 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/main.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    16580 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     1206 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/cached_path/version.py
+-rw-r--r--   0        0        0     6369 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/copier.py
+-rw-r--r--   0        0        0     5603 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0     9920 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1064 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3595 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4129 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1986 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9760 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     2022 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/pipe.py
+-rw-r--r--   0        0        0     5466 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-15 22:03:09.095991 hyfi-0.6.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     2986 1970-01-01 00:00:00.000000 hyfi-0.6.0/PKG-INFO
```

### Comparing `hyfi-0.5.1/LICENSE` & `hyfi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/README.md` & `hyfi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/pyproject.toml` & `hyfi-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.5.1"
+version = "0.6.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
 
 [tool.poetry.scripts]
 hyfi = 'hyfi.__cli__:hydra_main'
+hyfi-run = 'hyfi.__click__:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.12"
 hydra-core = "^1.3.2"
 hydra-colorlog = "^1.2.0"
 pydantic = "^1.10.7"
 chardet = "<=5.1.0"
@@ -29,14 +30,15 @@
 pathspec = ">=0.9.0"
 filelock = ">=3.4,<3.10"
 rich = ">=12.1,<14.0"
 gdown = "<=4.6.6"
 huggingface-hub = ">=0.8.1,<0.13.0"
 # google-cloud-storage = ">=1.32.0,<3.0"
 # boto3 = ">=1.0,<2.0"
+click = "^8.1.3"
 
 [tool.poetry.group.ipython]
 optional = true
 
 [tool.poetry.group.ipython.dependencies]
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
@@ -49,15 +51,15 @@
 
 [tool.poetry.group.mkdocs]
 optional = true
 
 [tool.poetry.group.mkdocs.dependencies]
 mkdocs-material = "^9.1.15"
 markdown-include = "^0.8.1"
-mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocstrings = { extras = ["python"], version = "^0.22.0" }
 mkdocs-material-extensions = ">=1.1"
 pymdown-extensions = ">=9.9.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `hyfi-0.5.1/src/hyfi/__cli__.py` & `hyfi-0.6.0/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.6.0/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.6.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 DOTENV_FILENAME: .env
 DOTENV_DIR: ${oc.select:..path.runtime,.}
 DOTENV_PATH: ${.DOTENV_DIR}/${.DOTENV_FILENAME}
 # Internal
 HYFI_RESOURCE_DIR:
-HYFI_GLOBAL_WORKSPACE_ROOT:
-HYFI_GLOBAL_DATA_ROOT:
+HYFI_GLOBAL_ROOT:
+HYFI_GLOBAL_WORKSPACE_NAME:
 HYFI_PROJECT_NAME:
 HYFI_TASK_NAME:
+HYFI_PROJECT_DESC:
 HYFI_PROJECT_ROOT:
-HYFI_PROJECT_DATA_ROOT:
+HYFI_PROJECT_WORKSPACE_NAME:
 HYFI_LOG_LEVEL: WARNING
 HYFI_VERBOSE: false
-NUM_WORKERS:
+HYFI_NUM_WORKERS:
 CACHED_PATH_CACHE_ROOT:
 # For other packages
 CUDA_DEVICE_ORDER:
 CUDA_VISIBLE_DEVICES:
 WANDB_PROJECT:
 WANDB_DISABLED:
 WANDB_DIR:
```

### Comparing `hyfi-0.5.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.6.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.6.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.6.0/src/hyfi/conf/path/__default__.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-project_data_root: ${oc.select:..project.project_data_root,${oc.env:HYFI_PROJECT_DATA_ROOT,.}}
+project_workspace_root: ${oc.select:..project.project_workspace_root,${oc.env:HYFI_PROJECT_ROOT,.}/${oc.env:HYFI_PROJECT_WORKSPACE_NAME,.}}
 task_name: ${oc.select:..project.task_name, default-task}
-task_root: ${.project_data_root}/${.task_name}
+task_root: ${.project_workspace_root}/${.task_name}
 
 task_outputs: ${.task_root}/outputs
 task_datasets: ${.task_root}/datasets
 task_library: ${.task_root}/libs
 task_models: ${.task_root}/models
 task_cache: ${oc.select:..project.path.project_cache,${.task_root}/cache}
 task_tmp: ${oc.select:..project.path.project_tmp,${.task_root}/tmp}
```

### Comparing `hyfi-0.5.1/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.6.0/src/hyfi/conf/path/__init__.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 # This file defines the path variables used in the project.
 # internal paths for hyfi
 home: ${__home_path__:}
 hyfi: ${__hyfi_path__:}
 resources: ${alt:${oc.env:HYFI_RESOURCE_DIR,null},${.hyfi}/resources}
 runtime: ${get_original_cwd:}
 # global paths
-global_workspace_root: ${oc.select:..global_workspace_root,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_ROOT,null},${__home_path__:}/.hyfi}}
-global_data_root: ${oc.select:..global_data_root,${alt:${oc.env:HYFI_GLOBAL_DATA_ROOT,null},${.global_workspace_root}/data}}
-global_archive: ${.global_data_root}/archive
-global_datasets: ${.global_data_root}/datasets
-global_models: ${.global_data_root}/models
-global_modules: ${.global_data_root}/modules
-global_library: ${.global_data_root}/libs
-global_logs: ${.global_data_root}/logs
+global_hyfi_root: ${oc.select:..global_hyfi_root,${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}}
+global_workspace_name: ${oc.select:..global_workspace_name,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}}
+global_workspace_root: ${.global_hyfi_root}/${.global_workspace_name}
+global_archive: ${.global_workspace_root}/archive
+global_datasets: ${.global_workspace_root}/datasets
+global_models: ${.global_workspace_root}/models
+global_modules: ${.global_workspace_root}/modules
+global_library: ${.global_workspace_root}/libs
+global_logs: ${.global_workspace_root}/logs
 global_cache: ${.global_workspace_root}/.cache
 global_tmp: ${.global_workspace_root}/.tmp
 # project specific paths
 project_root: ${oc.select:..project_root,${alt:${oc.env:HYFI_PROJECT_ROOT,null},${get_original_cwd:}}}
-project_data_root: ${oc.select:..project_data_root,${alt:${oc.env:HYFI_PROJECT_DATA_ROOT,null},${.project_root}/workspace}}
-project_archive: ${.project_data_root}/archive
-project_datasets: ${.project_data_root}/datasets
-project_models: ${.project_data_root}/models
-project_modules: ${.project_data_root}/modules
-project_outputs: ${.project_data_root}/outputs
-project_logs: ${.project_data_root}/logs
-project_library: ${.project_data_root}/libs
-project_cache: ${.project_data_root}/.cache
-project_tmp: ${.project_data_root}/.tmp
+project_workspace_name: ${oc.select:..project_workspace_name,${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}}
+project_workspace_root: ${.project_root}/${.project_workspace_name}
+project_archive: ${.project_workspace_root}/archive
+project_datasets: ${.project_workspace_root}/datasets
+project_models: ${.project_workspace_root}/models
+project_modules: ${.project_workspace_root}/modules
+project_outputs: ${.project_workspace_root}/outputs
+project_logs: ${.project_workspace_root}/logs
+project_library: ${.project_workspace_root}/libs
+project_cache: ${.project_workspace_root}/.cache
+project_tmp: ${.project_workspace_root}/.tmp
```

### Comparing `hyfi-0.5.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.6.0/src/hyfi/conf/project/__init__.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
 project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
 task_name: ${alt:${oc.env:HYFI_TASK_NAME,null},default-task}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
-project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${get_original_cwd:}}
-project_data_root: ${alt:${oc.env:HYFI_PROJECT_DATA_ROOT,null},${.project_root}/workspace}
-global_workspace_root: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_ROOT,null},${__home_path__:}/.hyfi}
-global_data_root: ${alt:${oc.env:HYFI_GLOBAL_DATA_ROOT,null},${.global_workspace_root}/data}
+project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
+project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
+global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
+global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
+num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
 use_huggingface_hub: false
 use_wandb: false
-verbose: false
+verbose: ${alt:${oc.env:HYFI_VERBOSE,null},false}
```

### Comparing `hyfi-0.5.1/src/hyfi/config/batch.py` & `hyfi-0.6.0/src/hyfi/config/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/config/path.py` & `hyfi-0.6.0/src/hyfi/config/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 logger = getLogger(__name__)
 
 
 class PathConfig(BaseModel):
     config_name: str = "__batch__"
 
-    project_data_root = ""
+    project_workspace_root = ""
     batch_name: str = "demo"
     batch_output: str = ""
     task_name: str = "default-task"
     task_root: str = ""
     task_outputs: str = ""
     task_datasets: str = ""
     task_library: str = ""
@@ -42,36 +42,36 @@
                 "There are no arguments to initilize a config, using default config %s",
                 config_name,
             )
             data = _compose(f"path={config_name}")
         super().__init__(**data)
 
     @property
-    def project_data_dir(self) -> Path:
+    def project_workspace_dir(self) -> Path:
         """
-        Get the path to the project data directory. It is assumed that the user has checked the existence of the project data directory before calling this method.
+        Get the path to the project workspace directory.
 
 
         Returns:
-                absolute path to the project data directory or None if not set by the user ( in which case a default is used )
+                absolute path to the project workspace directory or None if not set by the user ( in which case a default is used )
         """
-        self.project_data_root = self.project_data_root or "./workspace"
-        return Path(self.project_data_root).absolute()
+        self.project_workspace_root = self.project_workspace_root or "./workspace"
+        return Path(self.project_workspace_root).absolute()
 
     @property
     def root_dir(self) -> Path:
         """
         Returns the absolute path to the task root directory. If the task_root attribute is set it is used as the path to the task's data directory. Otherwise the task name is used as the path to the project's data directory.
 
 
         Returns:
                 an absolute path to the task root directory or None if it doesn't exist or cannot be converted to a path object
         """
         self.task_root = (
-            self.task_root or (self.project_data_dir / self.task_name).as_posix()
+            self.task_root or (self.project_workspace_dir / self.task_name).as_posix()
         )
         # return as an absolute path
         return Path(self.task_root).absolute()
 
     @property
     def output_dir(self) -> Path:
         """
```

### Comparing `hyfi-0.5.1/src/hyfi/env.py` & `hyfi-0.6.0/src/hyfi/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,34 +111,33 @@
     verbose: int = 10
 
 
 class JobLibConfig(BaseModel):
     """JobLib Configuration"""
 
     config_name: str = "__init__"
+    num_workers: int = 1
     distributed_framework: DistFramwork = DistFramwork()
     batcher: BatcherConfig = BatcherConfig()
     __initilized__: bool = False
 
     class Config:
         extra = "allow"
         underscore_attrs_are_private = True
 
     def __init__(
         self,
         config_name: str = "__init__",
         **data: Any,
     ):
-        if not data:
-            logger.debug(
-                "There are no arguments to initilize a config, using default config."
-            )
-            data = _compose(
-                f"joblib={config_name}", config_module=__about__.config_module
-            )  # type: ignore
+        data = _compose(
+            f"joblib={config_name}",
+            config_data=data,
+            config_module=__about__.config_module,
+        )  # type: ignore
         super().__init__(config_name=config_name, **data)
 
     def init_backend(
         self,
     ):
         """Initialize the backend for joblib"""
         if self.distributed_framework.initialize:
@@ -201,26 +200,28 @@
     config_name: str = "__init__"
     # internal paths for hyfi
     home: str = ""
     hyfi: str = ""
     resources: str = ""
     runtime: str = ""
     # global paths
+    global_hyfi_root: str = ""
+    global_workspace_name: str = "workspace"
     global_workspace_root: str = ""
-    global_data_root: str = ""
     global_archive: str = ""
     global_datasets: str = ""
     global_models: str = ""
     global_modules: str = ""
     global_library: str = ""
     global_cache: str = ""
     global_tmp: str = ""
     # project specific paths
     project_root: str = ""
-    project_data_root: str = ""
+    project_workspace_name: str = "workspace"
+    project_workspace_root: str = ""
     project_archive: str = ""
     project_datasets: str = ""
     project_models: str = ""
     project_modules: str = ""
     project_outputs: str = ""
     project_logs: str = ""
     project_library: str = ""
@@ -240,22 +241,19 @@
         Initialize the config. This is the base implementation of __init__. You can override this in your own subclass if you want to customize the initilization of a config by passing a keyword argument ` data `.
 
         Args:
                 config_name: The name of the config to initialize
                 data: The data to initialize
         """
         # Initialize the config module.
-        if not data:
-            logger.debug(
-                "There are no arguments to initilize a config, using default config %s",
-                config_name,
-            )
-            data = _compose(
-                f"path={config_name}", config_module=__about__.config_module
-            )  # type: ignore
+        data = _compose(
+            f"path={config_name}",
+            config_data=data,
+            config_module=__about__.config_module,
+        )  # type: ignore
         super().__init__(config_name=config_name, **data)
 
     @property
     def log_dir(self):
         """
         Create and return the path to the log directory. This is a convenience method for use in unit tests that want to ensure that the log directory exists and is accessible to the user.
 
@@ -285,23 +283,24 @@
     config_name: str = "__init__"
 
     DOTENV_FILENAME: Optional[str] = ".env"
     DOTENV_DIR: Optional[str] = ""
     DOTENV_PATH: Optional[str] = ""
     # Internal
     HYFI_RESOURCE_DIR: Optional[str] = ""
-    HYFI_GLOBAL_WORKSPACE_ROOT: Optional[str] = ""
-    HYFI_GLOBAL_DATA_ROOT: Optional[str] = ""
+    HYFI_GLOBAL_ROOT: Optional[str] = ""
+    HYFI_GLOBAL_WORKSPACE_NAME: Optional[str] = "workspace"
     HYFI_PROJECT_NAME: Optional[str] = ""
     HYFI_TASK_NAME: Optional[str] = ""
+    HYFI_PROJECT_DESC: Optional[str] = ""
     HYFI_PROJECT_ROOT: Optional[str] = ""
-    HYFI_PROJECT_DATA_ROOT: Optional[str] = ""
+    HYFI_PROJECT_WORKSPACE_NAME: Optional[str] = "workspace"
     HYFI_LOG_LEVEL: Optional[str] = "WARNING"
     HYFI_VERBOSE: Optional[Union[bool, str, int]] = False
-    NUM_WORKERS: Optional[int] = 1
+    HYFI_NUM_WORKERS: Optional[int] = 1
     CACHED_PATH_CACHE_ROOT: Optional[str] = ""
     # For other packages
     CUDA_DEVICE_ORDER: Optional[str] = "PCI_BUS_ID"
     CUDA_VISIBLE_DEVICES: Optional[str] = ""
     WANDB_PROJECT: Optional[str] = ""
     WANDB_DISABLED: Optional[str] = ""
     WANDB_DIR: Optional[str] = ""
@@ -337,36 +336,14 @@
             file_secret_settings: SettingsSourceCallable,
         ) -> Tuple[SettingsSourceCallable, ...]:
             load_dotenv()
             return env_settings, file_secret_settings, init_settings
 
     @root_validator()
     def _check_and_set_values(cls, values):
-        global_workspace_root = values.get("HYFI_GLOBAL_WORKSPACE_ROOT")
-        global_data_root = values.get("HYFI_GLOBAL_DATA_ROOT")
-        if global_workspace_root and not global_data_root:
-            global_data_root = os.path.join(global_workspace_root, "data")
-            values["HYFI_GLOBAL_DATA_ROOT"] = global_data_root
-        project_name = values.get("HYFI_PROJECT_NAME")
-        project_root = values.get("HYFI_PROJECT_ROOT")
-        dotenv_dir = values.get("DOTENV_DIR")
-        if not project_root:
-            if global_workspace_root and project_name:
-                project_root = os.path.join(
-                    global_workspace_root, "projects", project_name
-                )
-                values["HYFI_PROJECT_ROOT"] = project_root
-            elif dotenv_dir and Path(dotenv_dir).is_dir():
-                project_root = dotenv_dir
-                values["HYFI_PROJECT_ROOT"] = project_root
-        project_data_root = values.get("HYFI_PROJECT_DATA_ROOT")
-        if project_root and not project_data_root:
-            project_data_root = os.path.join(project_root, "workspace")
-            values["HYFI_PROJECT_DATA_ROOT"] = project_data_root
-
         for k, v in values.items():
             if v is not None:
                 old_value = os.getenv(k.upper())
                 if old_value is None or old_value != str(v):
                     os.environ[k.upper()] = str(v)
                     logger.debug(f"Set environment variable {k.upper()}={v}")
         return values
@@ -376,80 +353,75 @@
     """Project Config"""
 
     config_name: str = "__init__"
     project_name: str = "hyfi-project"
     task_name: str = ""
     project_description: str = ""
     project_root: str = ""
-    project_data_root: str = ""
-    global_workspace_root: str = ""
-    global_data_root: str = ""
+    project_workspace_name: str = "workspace"
+    global_hyfi_root: str = ""
+    global_workspace_name: str = "workspace"
+    num_workers: int = 1
     use_huggingface_hub: bool = False
     use_wandb: bool = False
     verbose: Union[bool, int] = False
     # Config Classes
     dotenv: DotEnvConfig = None  # type: ignore
     joblib: JobLibConfig = None  # type: ignore
     path: PathConfig = None  # type: ignore
 
     class Config:
         extra = "allow"
         arbitrary_types_allowed = True
 
-    def __init__(
-        self,
-        config_name: str = "__init__",
-        **data: Any,
-    ):
-        if not data:
-            logger.debug(
-                "There are no arguments to initilize a config, using default config."
-            )
-            data = _compose(
-                f"project={config_name}", config_module=__about__.config_module
-            )  # type: ignore
-        super().__init__(config_name=config_name, **data)
-
     @validator("project_name", allow_reuse=True)
     def _validate_project_name(cls, v):
         if v is None:
             raise ValueError("Project name must be specified.")
         return v
 
-    @property
-    def environ(self):
-        return os.environ
-
-    @property
-    def project_data_dir(self):
-        if self.path is None:
-            raise ValueError("Path object not initialized")
-        _p = Path(self.path.project_data_root)
-        _p.mkdir(parents=True, exist_ok=True)
-        return _p.absolute()
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
 
-    @property
-    def project_dir(self):
-        if self.path is None:
-            raise ValueError("Path object not initialized")
-        _p = Path(self.path.project_root)
-        _p.mkdir(parents=True, exist_ok=True)
-        return _p.absolute()
+    def __init__(
+        self,
+        config_name: str = "__init__",
+        **data: Any,
+    ):
+        data = _compose(
+            f"project={config_name}",
+            config_data=data,
+            config_module=__about__.config_module,
+        )  # type: ignore
+        super().__init__(config_name=config_name, **data)
 
     def init_project(self):
         self.dotenv = DotEnvConfig()
         if self.path is None:
             self.path = PathConfig()
         if self.joblib is None:
             self.joblib = JobLibConfig()
 
-        if self.dotenv.HYFI_VERBOSE is not None:
-            self.verbose = int(self.dotenv.HYFI_VERBOSE)
-        self.dotenv.HYFI_GLOBAL_WORKSPACE_ROOT = str(self.path.global_workspace_root)
-        self.dotenv.HYFI_GLOBAL_DATA_ROOT = str(self.path.global_data_root)
+        self.dotenv.HYFI_PROJECT_NAME = self.project_name
+        self.dotenv.HYFI_TASK_NAME = self.task_name
+        self.dotenv.HYFI_PROJECT_DESC = self.project_description
+        self.dotenv.HYFI_PROJECT_ROOT = self.project_root
+        self.dotenv.HYFI_PROJECT_WORKSPACE_NAME = self.project_workspace_name
+        self.dotenv.HYFI_GLOBAL_ROOT = self.global_hyfi_root
+        self.dotenv.HYFI_GLOBAL_WORKSPACE_NAME = self.global_workspace_name
+        self.dotenv.HYFI_NUM_WORKERS = self.num_workers
+        self.dotenv.HYFI_VERBOSE = self.verbose
         self.dotenv.CACHED_PATH_CACHE_ROOT = str(self.path.cache_dir / "cached_path")
         self.init_wandb()
         if self.use_huggingface_hub:
             self.init_huggingface_hub()
 
     def init_wandb(self):
         if self.path is None:
@@ -499,14 +471,34 @@
                 notebook_login()
             else:
                 logger.info(
                     "huggingface_hub.notebook_login() is only available in notebook,"
                     "set HUGGING_FACE_HUB_TOKEN manually"
                 )
 
+    @property
+    def environ(self):
+        return os.environ
+
+    @property
+    def project_workspace_dir(self):
+        if self.path is None:
+            raise ValueError("Path object not initialized")
+        _p = Path(self.path.project_workspace_root)
+        _p.mkdir(parents=True, exist_ok=True)
+        return _p.absolute()
+
+    @property
+    def project_dir(self):
+        if self.path is None:
+            raise ValueError("Path object not initialized")
+        _p = Path(self.path.project_root)
+        _p.mkdir(parents=True, exist_ok=True)
+        return _p.absolute()
+
 
 class HyfiConfig(BaseModel):
     """HyFI config primary class"""
 
     hyfi_config_path: str = __about__.config_path
     hyfi_config_module: str = __about__.config_module
     hyfi_user_config_path: str = ""
@@ -558,37 +550,43 @@
         super().__init__(**data)
         # self.about = __about__
 
     def init_workspace(
         self,
         project_name: str = "",
         task_name: str = "",
+        project_description: str = "",
         project_root: str = "",
-        project_data_root: str = "",
-        global_workspace_root: str = "",
-        global_data_root: str = "",
+        project_workspace_name: str = "",
+        global_hyfi_root: str = "",
+        global_workspace_name: str = "",
+        num_workers: int = -1,
         log_level: str = "",
         autotime: bool = True,
         retina: bool = True,
         verbose: Union[bool, int] = False,
         **kwargs,
     ):
         envs = DotEnvConfig(HYFI_VERBOSE=verbose)
         if project_name:
             envs.HYFI_PROJECT_NAME = expand_posix_vars(project_name)
         if task_name:
             envs.HYFI_TASK_NAME = expand_posix_vars(task_name)
+        if project_description:
+            envs.HYFI_PROJECT_DESC = expand_posix_vars(project_description)
         if project_root:
             envs.HYFI_PROJECT_ROOT = expand_posix_vars(project_root)
-        if project_data_root:
-            envs.HYFI_PROJECT_DATA_ROOT = expand_posix_vars(project_data_root)
-        if global_workspace_root:
-            envs.HYFI_GLOBAL_WORKSPACE_ROOT = expand_posix_vars(global_workspace_root)
-        if global_data_root:
-            envs.HYFI_GLOBAL_DATA_ROOT = expand_posix_vars(global_data_root)
+        if project_workspace_name:
+            envs.HYFI_PROJECT_WORKSPACE_NAME = expand_posix_vars(project_workspace_name)
+        if global_hyfi_root:
+            envs.HYFI_GLOBAL_ROOT = expand_posix_vars(global_hyfi_root)
+        if global_workspace_name:
+            envs.HYFI_GLOBAL_WORKSPACE_NAME = expand_posix_vars(global_workspace_name)
+        if num_workers:
+            envs.HYFI_NUM_WORKERS = num_workers
         if log_level:
             envs.HYFI_LOG_LEVEL = log_level
             setLogger(log_level)
             logger.setLevel(log_level)
         if autotime:
             load_extentions(exts=["autotime"])
         if retina:
@@ -642,88 +640,116 @@
     def __call__(self, *args, **kwargs):
         return Dummy()
 
 
 def _compose(
     config_group: Union[str, None] = None,
     overrides: Union[List[str], None] = None,
+    config_data: Union[Dict[str, Any], DictConfig, None] = None,
     *,
-    return_as_dict: bool = False,
+    return_as_dict: bool = True,
     throw_on_resolution_failure: bool = True,
     throw_on_missing: bool = False,
     config_name: Union[str, None] = None,
     config_module: Union[str, None] = None,
+    global_package: bool = False,
     verbose: bool = False,
 ) -> Union[DictConfig, Dict]:  # sourcery skip: low-code-quality
     """
-    Compose your configuration from config groups and overrides (overrides=["override_name"])
+    Compose a configuration by applying overrides
 
-    :param overrides: List of overrides to apply
-    :param config_group: Config group name to select ('config_group=name')
-    :param return_as_dict: Return the composed config as a dict
-    :param throw_on_resolution_failure: Throw if resolution fails
-    :param throw_on_missing: Throw if a config is missing
-    :param config_name: Name of the config to compose
-    :param verbose: Print the composed config
+    Args:
+        config_group: Name of the config group to compose (`config_group=name`)
+        overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
+        config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group.key=value`)
+        return_as_dict: Return the result as a dict
+        throw_on_resolution_failure: If True throw an exception if resolution fails
+        throw_on_missing: If True throw an exception if config_group doesn't exist
+        config_name: Name of the root config to be used (e.g. `hconf`)
+        config_module: Module of the config to be used (e.g. `hyfi.conf`)
+        global_package: If True, the config assumed to be a global package
+        verbose: If True print configuration to stdout
 
-    :return: The composed config
+    Returns:
+        A config object or a dictionary with the composed config
     """
+    if isinstance(config_data, DictConfig):
+        logger.debug("returning config_group_kwargs without composing")
+        return (
+            _to_dict(config_data)
+            if return_as_dict and isinstance(config_data, DictConfig)
+            else config_data
+        )
+    # Set overrides to the empty list if None
     if overrides is None:
         overrides = []
     config_module = config_module or __global_config__.hyfi_config_module
     # if verbose:
-    logger.info("config_module: %s", config_module)
+    logger.debug("config_module: %s", config_module)
     is_initialized = hydra.core.global_hydra.GlobalHydra.instance().is_initialized()  # type: ignore
+    # Set the group key and value of the config group.
     if config_group:
-        _task = config_group.split("=")
-        if len(_task) == 2:
-            key, value = _task
+        group_ = config_group.split("=")
+        # group_key group_value group_key group_value group_key group_value default
+        if len(group_) == 2:
+            group_key, group_value = group_
         else:
-            key = _task[0]
-            value = "default"
-        config_group = f"{key}={value}"
+            group_key = group_[0]
+            group_value = "default"
+        config_group = f"{group_key}={group_value}"
     else:
-        key = None
-        value = None
-    if key and value:
+        group_key = None
+        group_value = None
+    # If group_key and group_value are specified in the configuration file.
+    if group_key and group_value:
+        # Initialize hydra configuration module.
         if is_initialized:
             cfg = hydra.compose(config_name=config_name, overrides=overrides)
         else:
             with hydra.initialize_config_module(
                 config_module=config_module, version_base=__hydra_version_base__
             ):
                 cfg = hydra.compose(config_name=config_name, overrides=overrides)
         cfg = _select(
             cfg,
-            key=key,
+            key=group_key,
             default=None,
             throw_on_missing=False,
             throw_on_resolution_failure=False,
         )
         override = config_group if cfg is not None else f"+{config_group}"
+        # Add override to overrides list.
         if isinstance(override, str):
             if overrides:
                 overrides.append(override)
             else:
                 overrides = [override]
+    # Add config group overrides to overrides list.
+    if config_data:
+        for k, v in config_data.items():
+            if isinstance(v, (str, int)):
+                overrides.append(f"{group_key}.{k}={v}")
     # if verbose:
-    logger.info(f"compose config with overrides: {overrides}")
+    logger.debug(f"compose config with overrides: {overrides}")
+    # Initialize hydra and return the configuration.
     if is_initialized:
+        # Hydra is already initialized.
         if verbose:
-            logger.info("Hydra is already initialized")
+            logger.debug("Hydra is already initialized")
         cfg = hydra.compose(config_name=config_name, overrides=overrides)
     else:
         with hydra.initialize_config_module(
             config_module=config_module, version_base=__hydra_version_base__
         ):
             cfg = hydra.compose(config_name=config_name, overrides=overrides)
 
-    if key and key != "task":
+    # Select the group_key from the configuration.
+    if group_key and not global_package:
         cfg = _select(
             cfg,
-            key=key,
+            key=group_key,
             default=None,
             throw_on_missing=throw_on_missing,
             throw_on_resolution_failure=throw_on_resolution_failure,
         )
-    logger.debug("Composed config: %s", OmegaConf.to_yaml(cfg))
+    logger.debug("Composed config: %s", OmegaConf.to_yaml(_to_dict(cfg)))
     return _to_dict(cfg) if return_as_dict and isinstance(cfg, DictConfig) else cfg
```

### Comparing `hyfi-0.5.1/src/hyfi/hydra.py` & `hyfi-0.6.0/src/hyfi/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/image/collage.py` & `hyfi-0.6.0/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/image/motion.py` & `hyfi-0.6.0/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/image/plot.py` & `hyfi-0.6.0/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/image/utils.py` & `hyfi-0.6.0/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/io/cached_path.py` & `hyfi-0.6.0/src/hyfi/io/cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/io/file.py` & `hyfi-0.6.0/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/main.py` & `hyfi-0.6.0/src/hyfi/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,32 +141,52 @@
         """Get the value of an environment variable or return the default value"""
         return get_osenv(key, default=default)
 
     @staticmethod
     def compose(
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
+        config_data: Union[Dict[str, Any], DictConfig, None] = None,
         *,
-        return_as_dict: bool = False,
+        return_as_dict: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
         config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
+        global_package: bool = False,
         verbose: bool = False,
     ) -> Union[DictConfig, Dict]:
-        if overrides is None:
-            overrides = []
+        """
+        Compose a configuration by applying overrides
+
+        Args:
+            config_group: Name of the config group to compose (`config_group=name`)
+            overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
+            config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group.key=value`)
+            return_as_dict: Return the result as a dict
+            throw_on_resolution_failure: If True throw an exception if resolution fails
+            throw_on_missing: If True throw an exception if config_group doesn't exist
+            config_name: Name of the root config to be used (e.g. `hconf`)
+            config_module: Module of the config to be used (e.g. `hyfi.conf`)
+            global_package: If True, the config assumed to be a global package
+            verbose: If True print configuration to stdout
+
+        Returns:
+            A config object or a dictionary with the composed config
+        """
         return _compose(
             config_group=config_group,
             overrides=overrides,
+            config_data=config_data,
             return_as_dict=return_as_dict,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
             config_name=config_name,
             config_module=config_module,
+            global_package=global_package,
             verbose=verbose,
         )
 
     @staticmethod
     def select(
         cfg: Any,
         key: str,
@@ -957,31 +977,35 @@
             **kwargs,
         )
 
     @staticmethod
     def init_workspace(
         project_name: str = "",
         task_name: str = "",
+        project_description: str = "",
         project_root: str = "",
-        project_data_root: str = "",
-        global_workspace_root: str = "",
-        global_data_root: str = "",
+        project_workspace_name: str = "",
+        global_hyfi_root: str = "",
+        global_workspace_name: str = "",
+        num_workers: int = -1,
         log_level: str = "",
         autotime: bool = True,
         retina: bool = True,
         verbose: Union[bool, int] = False,
         **kwargs,
     ) -> ProjectConfig:
         __global_config__.init_workspace(
             project_name=project_name,
             task_name=task_name,
+            project_description=project_description,
             project_root=project_root,
-            project_data_root=project_data_root,
-            global_workspace_root=global_workspace_root,
-            global_data_root=global_data_root,
+            project_workspace_name=project_workspace_name,
+            global_hyfi_root=global_hyfi_root,
+            global_workspace_name=global_workspace_name,
+            num_workers=num_workers,
             log_level=log_level,
             autotime=autotime,
             retina=retina,
             verbose=verbose,
             **kwargs,
         )
         if __global_config__.project:
```

### Comparing `hyfi-0.5.1/src/hyfi/utils/batch/apply.py` & `hyfi-0.6.0/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.6.0/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/batch/batcher.py` & `hyfi-0.6.0/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/__init__.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/_cached_path.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/cache_file.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/common.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/file_lock.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/meta.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/progress.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/__init__.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/beaker.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/hf.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/http.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/scheme_client.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/testing.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/cached_path/util.py` & `hyfi-0.6.0/src/hyfi/utils/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/copier.py` & `hyfi-0.6.0/src/hyfi/utils/copier.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from pathlib import Path
 from shutil import copy2, rmtree
 from typing import List
 
 from pathspec import PathSpec
 from pydantic.dataclasses import dataclass
 
-from ..hydra import getcwd
-from .tools import Style, printf
+from hyfi.utils.env import getcwd
+from hyfi.utils.tools import Style, printf
 
 
 @dataclass()
 class Copier:
     """Copier process state manager.
 
     This class represents the state of a copier work and contains methods to
@@ -71,15 +71,15 @@
         dry_run:
             When `True`, produce no real rendering.
 
         verbose:
             When `True`, show all output.
     """
 
-    src_path: Path = field(default=Path("config"))
+    src_path: Path = field(default=Path("conf"))
     dst_path: Path = field(default=Path("."))
     filetypes: List = field(default_factory=list)
     exclude: List = field(default_factory=list)
     skip_if_exists: bool = False
     cleanup_on_error: bool = True
     overwrite: bool = False
     dry_run: bool = False
@@ -125,14 +125,21 @@
 
     def run_copy(self):
         """Execute the copy process.
 
         Walk through the source directory, compare YAML files with the destination
         directory, and copy files based on the specified settings.
         """
+        if not Path(self.src_path).is_dir():
+            printf(
+                "ERROR",
+                f"Source path {self.src_path} does not exist.",
+                style=Style.DANGER,
+            )
+            return
         for root, _, files in os.walk(self.src_path):
             for filename in files:
                 if not any(filename.endswith(filetype) for filetype in self.filetypes):
                     continue
 
                 src_file = Path(root, filename)
                 dst_file = self.dst_path / src_file.relative_to(self.src_path)
```

### Comparing `hyfi-0.5.1/src/hyfi/utils/env.py` & `hyfi-0.6.0/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/func.py` & `hyfi-0.6.0/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/google.py` & `hyfi-0.6.0/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/gpu.py` & `hyfi-0.6.0/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/lib.py` & `hyfi-0.6.0/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/logging.py` & `hyfi-0.6.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/notebook.py` & `hyfi-0.6.0/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/pipe.py` & `hyfi-0.6.0/src/hyfi/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/src/hyfi/utils/tools.py` & `hyfi-0.6.0/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.1/PKG-INFO` & `hyfi-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.5.1
+Version: 0.6.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ipython
 Requires-Dist: chardet (<=5.1.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
 Requires-Dist: filelock (>=3.4,<3.10)
 Requires-Dist: gdown (<=4.6.6)
 Requires-Dist: huggingface-hub (>=0.8.1,<0.13.0)
 Requires-Dist: hydra-colorlog (>=1.2.0,<2.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
```

