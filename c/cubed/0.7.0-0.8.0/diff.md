# Comparing `tmp/cubed-0.7.0.tar.gz` & `tmp/cubed-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubed-0.7.0.tar", last modified: Thu May 25 11:02:26 2023, max compression
+gzip compressed data, was "cubed-0.8.0.tar", last modified: Fri Jun 16 11:03:06 2023, max compression
```

## Comparing `cubed-0.7.0.tar` & `cubed-0.8.0.tar`

### file list

```diff
@@ -1,103 +1,111 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.278348 cubed-0.7.0/
--rw-r--r--   0 tom        (501) staff       (20)    11358 2023-05-16 07:59:53.000000 cubed-0.7.0/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     1843 2023-05-25 11:02:26.278428 cubed-0.7.0/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      939 2023-02-21 09:42:15.000000 cubed-0.7.0/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.262299 cubed-0.7.0/cubed/
--rw-r--r--   0 tom        (501) staff       (20)      846 2023-05-05 10:22:49.000000 cubed-0.7.0/cubed/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.266378 cubed-0.7.0/cubed/array_api/
--rw-r--r--   0 tom        (501) staff       (20)     3578 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/array_api/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    12924 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/array_api/array_object.py
--rw-r--r--   0 tom        (501) staff       (20)       81 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/constants.py
--rw-r--r--   0 tom        (501) staff       (20)     8762 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/array_api/creation_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      751 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/data_type_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      471 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/dtypes.py
--rw-r--r--   0 tom        (501) staff       (20)    11395 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/elementwise_functions.py
--rw-r--r--   0 tom        (501) staff       (20)       83 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/array_api/indexing_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     4016 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/linear_algebra_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     9144 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/array_api/manipulation_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     1010 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/searching_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     3693 2023-03-17 17:46:35.000000 cubed-0.7.0/cubed/array_api/statistical_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      479 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/utility_functions.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.267608 cubed-0.7.0/cubed/core/
--rw-r--r--   0 tom        (501) staff       (20)      431 2023-02-17 17:56:56.000000 cubed-0.7.0/cubed/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    12389 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/core/array.py
--rw-r--r--   0 tom        (501) staff       (20)     5532 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/core/gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)    26890 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/core/ops.py
--rw-r--r--   0 tom        (501) staff       (20)    11664 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/core/plan.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.268300 cubed-0.7.0/cubed/extensions/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/extensions/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3230 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/extensions/history.py
--rw-r--r--   0 tom        (501) staff       (20)     2738 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/extensions/timeline.py
--rw-r--r--   0 tom        (501) staff       (20)     1439 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/extensions/tqdm.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.268982 cubed-0.7.0/cubed/primitive/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/primitive/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    11045 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/primitive/blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)     2031 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/primitive/rechunk.py
--rw-r--r--   0 tom        (501) staff       (20)      356 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/primitive/types.py
--rw-r--r--   0 tom        (501) staff       (20)     1401 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/random.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.269852 cubed-0.7.0/cubed/runtime/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/runtime/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      953 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/runtime/backup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.271328 cubed-0.7.0/cubed/runtime/executors/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/runtime/executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     8292 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/runtime/executors/beam.py
--rw-r--r--   0 tom        (501) staff       (20)     9240 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/runtime/executors/lithops.py
--rw-r--r--   0 tom        (501) staff       (20)     3538 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/runtime/executors/modal.py
--rw-r--r--   0 tom        (501) staff       (20)     6193 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/runtime/executors/modal_async.py
--rw-r--r--   0 tom        (501) staff       (20)     1279 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/runtime/executors/python.py
--rw-r--r--   0 tom        (501) staff       (20)     4241 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/runtime/executors/python_async.py
--rw-r--r--   0 tom        (501) staff       (20)     3632 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/runtime/pipeline.py
--rw-r--r--   0 tom        (501) staff       (20)      251 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/runtime/types.py
--rw-r--r--   0 tom        (501) staff       (20)      118 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/runtime/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.273375 cubed-0.7.0/cubed/tests/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.273887 cubed-0.7.0/cubed/tests/primitive/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/primitive/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6787 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/primitive/test_blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)     2893 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/primitive/test_rechunk.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.274635 cubed-0.7.0/cubed/tests/runtime/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/runtime/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      860 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/runtime/test_backup.py
--rw-r--r--   0 tom        (501) staff       (20)     4014 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/runtime/test_lithops.py
--rw-r--r--   0 tom        (501) staff       (20)     4691 2023-03-27 13:45:10.000000 cubed-0.7.0/cubed/tests/runtime/test_modal_async.py
--rw-r--r--   0 tom        (501) staff       (20)    16663 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_array_api.py
--rw-r--r--   0 tom        (501) staff       (20)    14506 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_core.py
--rw-r--r--   0 tom        (501) staff       (20)     3028 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)     1454 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_indexing.py
--rw-r--r--   0 tom        (501) staff       (20)     5287 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_mem_utilization.py
--rw-r--r--   0 tom        (501) staff       (20)     2397 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_optimization.py
--rw-r--r--   0 tom        (501) staff       (20)     1225 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_random.py
--rw-r--r--   0 tom        (501) staff       (20)     2310 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/tests/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     2867 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/tests/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     4508 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.274872 cubed-0.7.0/cubed/vendor/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.275682 cubed-0.7.0/cubed/vendor/dask/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.276741 cubed-0.7.0/cubed/vendor/dask/array/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    17366 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/core.py
--rw-r--r--   0 tom        (501) staff       (20)     1685 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)     4670 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/reshape.py
--rw-r--r--   0 tom        (501) staff       (20)      543 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    14901 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)      608 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/core.py
--rw-r--r--   0 tom        (501) staff       (20)     2221 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.277809 cubed-0.7.0/cubed/vendor/rechunker/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    13197 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/algorithm.py
--rw-r--r--   0 tom        (501) staff       (20)    12312 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/rechunker/api.py
--rw-r--r--   0 tom        (501) staff       (20)      309 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/compat.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.278167 cubed-0.7.0/cubed/vendor/rechunker/executors/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      923 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/executors/python.py
--rw-r--r--   0 tom        (501) staff       (20)     3421 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/types.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.263122 cubed-0.7.0/cubed.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     1843 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2506 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      369 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)     1611 2023-05-25 11:01:22.000000 cubed-0.7.0/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)     1195 2023-05-25 11:02:26.279006 cubed-0.7.0/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      289 2023-05-16 07:59:53.000000 cubed-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-16 11:02:53.000000 cubed-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-16 11:03:06.533476 cubed-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-16 11:02:53.000000 cubed-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.517476 cubed-0.8.0/cubed/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.521476 cubed-0.8.0/cubed/array_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/array_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/creation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/data_type_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/elementwise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/indexing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/linear_algebra_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/manipulation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/searching_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/statistical_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.521476 cubed-0.8.0/cubed/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/gufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/extensions/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/extensions/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/extensions/tqdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/primitive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/primitive/blockwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/primitive/rechunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/primitive/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/runtime/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/beam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/lithops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/modal_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/python_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/storage/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.529476 cubed-0.8.0/cubed/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.529476 cubed-0.8.0/cubed/tests/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/primitive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/primitive/test_blockwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/primitive/test_rechunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.529476 cubed-0.8.0/cubed/tests/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/test_lithops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/test_modal_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/test_python_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/storage/test_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_array_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_gufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_mem_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/dask/array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17366 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/gufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/blockwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/rechunker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/rechunker/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/executors/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.517476 cubed-0.8.0/cubed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-16 11:02:53.000000 cubed-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-16 11:03:06.537476 cubed-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 11:02:53.000000 cubed-0.8.0/setup.py
```

### Comparing `cubed-0.7.0/LICENSE` & `cubed-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/PKG-INFO` & `cubed-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed
-Version: 0.7.0
+Version: 0.8.0
 Summary: Bounded-memory serverless distributed N-dimensional array processing
 Author-email: Tom White <tom.e.white@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/tomwhite/cubed
 Project-URL: documentation, https://tomwhite.github.io/cubed
 Project-URL: repository, https://github.com/tomwhite/cubed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cubed-0.7.0/README.md` & `cubed-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/__init__.py` & `cubed-0.8.0/cubed/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from .array_api import Array
 from .core.array import (
     Callback,
     Spec,
     TaskEndEvent,
     compute,
+    measure_reserved_mem,
     measure_reserved_memory,
     visualize,
 )
 from .core.gufunc import apply_gufunc
 from .core.ops import from_array, from_zarr, map_blocks, store, to_zarr
 
 __all__ = [
@@ -31,12 +32,13 @@
     "Spec",
     "TaskEndEvent",
     "apply_gufunc",
     "compute",
     "from_array",
     "from_zarr",
     "map_blocks",
+    "measure_reserved_mem",
     "measure_reserved_memory",
     "store",
     "to_zarr",
     "visualize",
 ]
```

### Comparing `cubed-0.7.0/cubed/array_api/__init__.py` & `cubed-0.8.0/cubed/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/array_api/array_object.py` & `cubed-0.8.0/cubed/array_api/array_object.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/array_api/creation_functions.py` & `cubed-0.8.0/cubed/array_api/creation_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import TYPE_CHECKING, Iterable, List
 
 import numpy as np
-import zarr
 from zarr.util import normalize_shape
 
-from cubed.core import Plan, gensym, map_blocks, new_temp_store, new_temp_zarr
+from cubed.core import Plan, gensym, map_blocks
 from cubed.core.ops import map_direct
+from cubed.core.plan import new_temp_path
+from cubed.storage.zarr import lazy_from_array, lazy_full
 from cubed.utils import to_chunksize
 from cubed.vendor.dask.array.core import normalize_chunks
 
 if TYPE_CHECKING:
     from .array_object import Array
 
 
@@ -65,17 +66,16 @@
         a = np.asarray(a, dtype=dtype)
     if dtype is None:
         dtype = a.dtype
 
     # write to zarr
     chunksize = to_chunksize(normalize_chunks(chunks, shape=a.shape, dtype=dtype))
     name = gensym()
-    target = new_temp_zarr(a.shape, dtype, chunksize, name=name, spec=spec)
-    if a.size > 0:
-        target[...] = a
+    zarr_path = new_temp_path(name=name, spec=spec)
+    target = lazy_from_array(a, dtype=dtype, chunks=chunksize, store=zarr_path)
 
     plan = Plan._new(name, "asarray", target)
     return Array(name, target, spec, plan)
 
 
 def empty(shape, *, dtype=None, device=None, chunks="auto", spec=None) -> "Array":
     if dtype is None:
@@ -133,21 +133,21 @@
             dtype = np.float64
         elif isinstance(fill_value, bool):
             dtype = np.bool_
         else:
             raise TypeError("Invalid input to full")
     chunksize = to_chunksize(normalize_chunks(chunks, shape=shape, dtype=dtype))
     name = gensym()
-    store = new_temp_store(name=name, spec=spec)
-    target = zarr.full(
+    zarr_path = new_temp_path(name=name, spec=spec)
+    target = lazy_full(
         shape,
         fill_value,
-        store=store,
         dtype=dtype,
         chunks=chunksize,
+        store=zarr_path,
         write_empty_chunks=False,
     )
 
     from .array_object import Array
 
     plan = Plan._new(name, "full", target)
     return Array(name, target, spec, plan)
```

### Comparing `cubed-0.7.0/cubed/array_api/data_type_functions.py` & `cubed-0.8.0/cubed/array_api/data_type_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/array_api/elementwise_functions.py` & `cubed-0.8.0/cubed/array_api/elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/array_api/linear_algebra_functions.py` & `cubed-0.8.0/cubed/array_api/linear_algebra_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/array_api/manipulation_functions.py` & `cubed-0.8.0/cubed/array_api/manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/array_api/searching_functions.py` & `cubed-0.8.0/cubed/array_api/searching_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/array_api/statistical_functions.py` & `cubed-0.8.0/cubed/array_api/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/core/array.py` & `cubed-0.8.0/cubed/core/array.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass
 from operator import mul
-from typing import Optional, TypeVar
+from typing import Optional, TypeVar, Union
 from warnings import warn
 
 import numpy as np
 from toolz import map, reduce
 
 from cubed.runtime.pipeline import already_computed
 from cubed.runtime.types import Executor
-from cubed.utils import chunk_memory
+from cubed.storage.zarr import open_if_lazy_zarr_array
+from cubed.utils import chunk_memory, convert_to_bytes
 from cubed.vendor.dask.array.core import normalize_chunks
 
 from .plan import arrays_to_plan
 
 sym_counter = 0
 
 
@@ -32,28 +33,38 @@
 
     This class has the basic array attributes (``dtype``, ``shape``, ``chunks``, etc).
     The other array methods and attributes are provided in a subclass.
     """
 
     def __init__(self, name, zarray, spec, plan):
         self.name = name
-        self.zarray = zarray
+        self._zarray = zarray
         self._shape = zarray.shape
         self._dtype = zarray.dtype
         self._chunks = normalize_chunks(
             zarray.chunks, shape=self.shape, dtype=self.dtype
         )
         # if no spec is supplied, use a default with local temp dir,
         # and a modest amount of memory (200MB, of which 100MB is reserved)
         self.spec = spec or Spec(
             None, allowed_mem=200_000_000, reserved_mem=100_000_000
         )
         self.plan = plan
 
     @property
+    def zarray_maybe_lazy(self):
+        """The underlying Zarr array or LazyZarrArray. Use this during planning, before the computation has started."""
+        return self._zarray
+
+    @property
+    def zarray(self):
+        """The underlying Zarr array. May only be used during the computation once the array has been created."""
+        return open_if_lazy_zarr_array(self._zarray)
+
+    @property
     def chunkmem(self):
         """Amount of memory in bytes that a single chunk uses."""
         return chunk_memory(self.dtype, self.chunksize)
 
     @property
     def chunksize(self):
         """A tuple indicating the chunk size of each corresponding array dimension."""
@@ -105,22 +116,24 @@
 
     def compute(
         self,
         *,
         executor=None,
         callbacks=None,
         optimize_graph=True,
+        resume=None,
         **kwargs,
     ):
         """Compute this array, and any arrays that it depends on."""
         result = compute(
             self,
             executor=executor,
             callbacks=callbacks,
             optimize_graph=optimize_graph,
+            resume=resume,
             **kwargs,
         )
         if result:
             return result[0]
 
     def rechunk(self: T_ChunkedArray, chunks) -> T_ChunkedArray:
         """Change the chunking of this array without changing its shape or data.
@@ -182,56 +195,126 @@
 
         self.zarray.__setitem__(key, value)
 
     def __repr__(self):
         return f"cubed.core.CoreArray<{self.name}, shape={self.shape}, dtype={self.dtype}, chunks={self.chunks}>"
 
 
-@dataclass
 class Spec:
     """Specification of resources available to run a computation."""
 
-    work_dir: Optional[str] = None
-    """The directory path (specified as an fsspec URL) used for storing intermediate data."""
+    def __init__(
+        self,
+        work_dir: Union[str, None] = None,
+        max_mem: Union[int, None] = None,
+        allowed_mem: Union[int, str, None] = None,
+        reserved_mem: Union[int, str, None] = 0,
+        executor: Union[Executor, None] = None,
+        storage_options: Union[dict, None] = None,
+    ):
+        """
+        Specify resources available to run a computation.
 
-    max_mem: Optional[int] = None
-    """**Deprecated**. The maximum memory available to a worker for data use for the computation, in bytes."""
+        Parameters
+        ----------
+        work_dir : str or None
+            The directory path (specified as an fsspec URL) used for storing intermediate data.
+        max_mem : int, optional
+            **Deprecated**. The maximum memory available to a worker for data use for the computation, in bytes.
+        allowed_mem : int or str, optional
+            The total memory available to a worker for running a task, in bytes.
+
+            If int it should be >=0. If str it should be of form <value><unit> where unit can be kB, MB, GB, TB etc.
+            This includes any ``reserved_mem`` that has been set.
+        reserved_mem : int or str, optional
+            The memory reserved on a worker for non-data use when running a task, in bytes.
+
+            If int it should be >=0. If str it should be of form <value><unit> where unit can be kB, MB, GB, TB etc.
+        executor : Executor, optional
+            The default executor for running computations.
+        storage_options : dict, optional
+            Storage options to be passed to fsspec.
+        """
 
-    allowed_mem: Optional[int] = None
-    """The total memory available to a worker for running a task, in bytes.
+        if max_mem is not None:
+            warn(
+                "`max_mem` is deprecated, please use `allowed_mem` instead",
+                DeprecationWarning,
+                stacklevel=2,
+            )
 
-    This includes any ``reserved_mem`` that has been set."""
+        self._work_dir = work_dir
 
-    reserved_mem: int = 0
-    """The memory reserved on a worker for non-data use when running a task, in bytes.
+        self._reserved_mem = convert_to_bytes(reserved_mem)
+        if allowed_mem is None:
+            self._allowed_mem = (max_mem or 0) + self.reserved_mem
+        else:
+            self._allowed_mem = convert_to_bytes(allowed_mem)
 
-    See ``cubed.measure_reserved_memory``.
-    """
+        self._executor = executor
+        self._storage_options = storage_options
 
-    executor: Executor = None
-    """The default executor for running computations."""
+    @property
+    def work_dir(self) -> str:
+        """The directory path (specified as an fsspec URL) used for storing intermediate data."""
+        return self._work_dir
 
-    storage_options: dict = None  # type: ignore[assignment]
-    """Storage options to be passed to fsspec"""
+    @property
+    def allowed_mem(self) -> int:
+        """
+        The total memory available to a worker for running a task, in bytes.
 
-    def __post_init__(self):
-        if self.max_mem is not None:
-            warn(
-                "`max_mem` is deprecated, please use `allowed_mem` instead",
-                DeprecationWarning,
-                stacklevel=2,
+        This includes any ``reserved_mem`` that has been set.
+        """
+        return self._allowed_mem
+
+    @property
+    def reserved_mem(self) -> int:
+        """
+        The memory reserved on a worker for non-data use when running a task, in bytes.
+
+        See Also
+        --------
+        cubed.measure_reserved_mem
+        """
+        return self._reserved_mem
+
+    @property
+    def executor(self) -> Executor:
+        """The default executor for running computations."""
+        return self._executor
+
+    @property
+    def storage_options(self) -> dict:
+        """Storage options to be passed to fsspec."""
+        return self._storage_options
+
+    def __repr__(self) -> str:
+        return (
+            f"cubed.Spec(work_dir={self._work_dir}, allowed_mem={self._allowed_mem}, "
+            f"reserved_mem={self._reserved_mem}, executor={self._executor}, storage_options={self._storage_options})"
+        )
+
+    def __eq__(self, other):
+        if isinstance(other, Spec):
+            return (
+                self.work_dir == other.work_dir
+                and self.allowed_mem == other.allowed_mem
+                and self.reserved_mem == other.reserved_mem
+                and self.executor == other.executor
+                and self.storage_options == other.storage_options
             )
-        if self.allowed_mem is None:
-            self.allowed_mem = (self.max_mem or 0) + self.reserved_mem
+        else:
+            return False
 
 
 class Callback:
     """Object to receive callback events during array computation."""
 
-    def on_compute_start(self, dag):
+    def on_compute_start(self, dag, resume):
         """Called when the computation is about to start.
 
         Parameters
         ----------
         dag : networkx.MultiDiGraph
             The computation DAG.
         """
@@ -297,14 +380,15 @@
 
 
 def compute(
     *arrays,
     executor=None,
     callbacks=None,
     optimize_graph=True,
+    resume=None,
     **kwargs,
 ):
     """Compute multiple arrays at once."""
     plan = arrays_to_plan(*arrays)  # guarantees all arrays have same spec
     if executor is None:
         executor = arrays[0].spec.executor
         if executor is None:
@@ -313,14 +397,15 @@
             executor = PythonDagExecutor()
 
     _return_in_memory_array = kwargs.pop("_return_in_memory_array", True)
     plan.execute(
         executor=executor,
         callbacks=callbacks,
         optimize_graph=optimize_graph,
+        resume=resume,
         array_names=[a.name for a in arrays],
         **kwargs,
     )
 
     if _return_in_memory_array:
         return tuple(a._read_stored() for a in arrays)
 
@@ -354,15 +439,28 @@
 
 
 class PeakMeasuredMemoryCallback(Callback):
     def on_task_end(self, event):
         self.peak_measured_mem = event.peak_measured_mem_end
 
 
-def measure_reserved_memory(executor):
+def measure_reserved_memory(
+    executor: Executor, work_dir: Optional[str] = None, **kwargs
+) -> int:
+    warn(
+        "`measure_reserved_memory` is deprecated, please use `measure_reserved_mem` instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return measure_reserved_mem(executor, work_dir=work_dir, **kwargs)
+
+
+def measure_reserved_mem(
+    executor: Executor, work_dir: Optional[str] = None, **kwargs
+) -> int:
     """Measures the reserved memory use for a given executor runtime.
 
     This is the memory used by the Python process for running a task,
     excluding any memory used for data for the computation. It can vary by
     operating system, Python version, executor runtime, and installed package
     versions.
 
@@ -373,19 +471,27 @@
 
     Parameters
     ----------
     executor : cubed.runtime.types.Executor
         The executor to use to run the computation. It must be an executor that
         reports peak memory, such as Lithops or Modal.
 
+    work_dir : str or None, optional
+        The directory path (specified as an fsspec URL) used for storing intermediate data.
+        This is required when using a cloud runtime.
+
+    kwargs
+        Keyword arguments to pass to the ``compute`` function.
+
     Returns
     -------
     int
         The memory used by the runtime in bytes.
     """
     import cubed.array_api as xp
 
-    a = xp.ones((1,))
+    # give a generous memory allowance
+    a = xp.ones((1,), spec=Spec(work_dir, allowed_mem="500MB"))
     b = xp.negative(a)
     peak_measured_mem_callback = PeakMeasuredMemoryCallback()
-    b.compute(executor=executor, callbacks=[peak_measured_mem_callback])
+    b.compute(executor=executor, callbacks=[peak_measured_mem_callback], **kwargs)
     return peak_measured_mem_callback.peak_measured_mem
```

### Comparing `cubed-0.7.0/cubed/core/gufunc.py` & `cubed-0.8.0/cubed/core/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/core/ops.py` & `cubed-0.8.0/cubed/core/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     OrthogonalIndexer,
     is_integer_list,
     is_slice,
     replace_ellipsis,
 )
 
 from cubed.core.array import CoreArray, check_array_specs, compute, gensym
-from cubed.core.plan import Plan, new_temp_store
+from cubed.core.plan import Plan, new_temp_path
 from cubed.primitive.blockwise import blockwise as primitive_blockwise
 from cubed.primitive.rechunk import rechunk as primitive_rechunk
 from cubed.utils import chunk_memory, get_item, to_chunksize
 from cubed.vendor.dask.array.core import common_blockdim, normalize_chunks
 from cubed.vendor.dask.array.utils import validate_axis
 from cubed.vendor.dask.blockwise import broadcast_dimensions
 from cubed.vendor.dask.utils import has_keyword
@@ -246,26 +246,26 @@
                         "adjust_chunks values must be callable, int, or tuple"
                     )
     _chunks = tuple(chunks)
     shape = tuple(map(sum, _chunks))
 
     # replace arrays with zarr arrays
     zargs = list(args)
-    zargs[::2] = [a.zarray for a in arrays]
+    zargs[::2] = [a.zarray_maybe_lazy for a in arrays]
     in_names = [a.name for a in arrays]
 
     extra_source_arrays = kwargs.pop("extra_source_arrays", [])
     source_arrays = list(arrays) + list(extra_source_arrays)
 
     extra_projected_mem = kwargs.pop("extra_projected_mem", 0)
 
     name = gensym()
     spec = check_array_specs(arrays)
     if target_store is None:
-        target_store = new_temp_store(name=name, spec=spec)
+        target_store = new_temp_path(name=name, spec=spec)
     pipeline = primitive_blockwise(
         func,
         out_ind,
         *zargs,
         allowed_mem=spec.allowed_mem,
         reserved_mem=spec.reserved_mem,
         target_store=target_store,
@@ -277,14 +277,15 @@
         out_name=name,
         **kwargs,
     )
     plan = Plan._new(
         name,
         "blockwise",
         pipeline.target_array,
+        None,
         pipeline,
         pipeline.projected_mem + extra_projected_mem,
         spec.reserved_mem,
         pipeline.num_tasks,
         *source_arrays,
     )
     from cubed.array_api import Array
@@ -334,15 +335,17 @@
         dim_sel.tolist() if isinstance(dim_sel, np.ndarray) else dim_sel
         for dim_sel in selection
     )
     # Replace ellipsis with slices
     selection = replace_ellipsis(selection, x.shape)
 
     # Use a Zarr indexer just to find the resulting array shape and chunks
-    indexer = OrthogonalIndexer(selection, x.zarray)
+    # Need to use an in-memory representation since the Zarr file has not been written yet
+    inmem = zarr.empty_like(x.zarray_maybe_lazy, store=zarr.storage.MemoryStore())
+    indexer = OrthogonalIndexer(selection, inmem)
 
     shape = indexer.shape
     dtype = x.dtype
     chunks = tuple(
         s.dim_chunk_len
         for s in indexer.dim_indexers
         if not isinstance(s, IntDimIndexer)
@@ -588,28 +591,29 @@
 
 def rechunk(x, chunks, target_store=None):
     if x.chunks == normalize_chunks(chunks, x.shape, dtype=x.dtype):
         return x
     name = gensym()
     spec = x.spec
     if target_store is None:
-        target_store = new_temp_store(name=name, spec=spec)
-    temp_store = new_temp_store(name=f"{name}-intermediate", spec=spec)
+        target_store = new_temp_path(name=name, spec=spec)
+    temp_store = new_temp_path(name=f"{name}-intermediate", spec=spec)
     pipeline = primitive_rechunk(
-        x.zarray,
+        x.zarray_maybe_lazy,
         target_chunks=chunks,
         allowed_mem=spec.allowed_mem,
         reserved_mem=spec.reserved_mem,
         target_store=target_store,
         temp_store=temp_store,
     )
     plan = Plan._new(
         name,
         "rechunk",
         pipeline.target_array,
+        pipeline.intermediate_array,
         pipeline,
         pipeline.projected_mem,
         spec.reserved_mem,
         pipeline.num_tasks,
         x,
     )
```

### Comparing `cubed-0.7.0/cubed/extensions/history.py` & `cubed-0.8.0/cubed/extensions/history.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import pandas as pd
 
 from cubed.core.array import Callback
 from cubed.core.plan import visit_nodes
 
 
 class HistoryCallback(Callback):
-    def on_compute_start(self, dag):
+    def on_compute_start(self, dag, resume):
         plan = []
-        for name, node in visit_nodes(dag):
+        for name, node in visit_nodes(dag, resume):
             pipeline = node["pipeline"]
             plan.append(
                 dict(
                     array_name=name,
                     op_name=node["op_name"],
                     projected_mem=pipeline.projected_mem,
                     reserved_mem=node["reserved_mem"],
```

### Comparing `cubed-0.7.0/cubed/extensions/timeline.py` & `cubed-0.8.0/cubed/extensions/timeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cubed.core.array import Callback
 
 sns.set_style("whitegrid")
 pylab.switch_backend("Agg")
 
 
 class TimelineVisualizationCallback(Callback):
-    def on_compute_start(self, dag):
+    def on_compute_start(self, dag, resume):
         self.start_tstamp = time.time()
         self.stats = []
 
     def on_task_end(self, event):
         self.stats.append(asdict(event))
 
     def on_compute_end(self, dag):
```

### Comparing `cubed-0.7.0/cubed/extensions/tqdm.py` & `cubed-0.8.0/cubed/extensions/tqdm.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 class TqdmProgressBar(Callback):
     """Progress bar for a computation."""
 
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
 
-    def on_compute_start(self, dag):
+    def on_compute_start(self, dag, resume):
         from tqdm.auto import tqdm
 
         self.pbars = {}
         i = 0
-        for name, node in visit_nodes(dag):
+        for name, node in visit_nodes(dag, resume):
             num_tasks = node["pipeline"].num_tasks
             self.pbars[name] = tqdm(
                 *self.args, desc=name, total=num_tasks, position=i, **self.kwargs
             )
             i = i + 1
 
     def on_compute_end(self, dag):
```

### Comparing `cubed-0.7.0/cubed/primitive/blockwise.py` & `cubed-0.8.0/cubed/primitive/blockwise.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from functools import partial
 from typing import Callable, Dict
 
 import toolz
 import zarr
 from toolz import map
 
+from cubed.storage.zarr import lazy_empty
 from cubed.utils import chunk_memory, get_item, to_chunksize
 from cubed.vendor.dask.array.core import normalize_chunks
 from cubed.vendor.dask.blockwise import _get_coord_mapping, _make_dims, lol_product
 from cubed.vendor.dask.core import flatten
-from cubed.vendor.rechunker.types import ArrayProxy, Stage
+from cubed.vendor.rechunker.types import Stage
 
-from .types import CubedPipeline
+from .types import CubedArrayProxy, CubedPipeline
 
 sym_counter = 0
 
 
 def gensym(name):
     global sym_counter
     sym_counter += 1
@@ -32,47 +33,47 @@
 
     Attributes
     ----------
     block_function : Callable
         A function that maps input chunk indexes to an output chunk index.
     function : Callable
         A function that maps input chunks to an output chunk.
-    reads_map : Dict[str, ArrayProxy]
+    reads_map : Dict[str, CubedArrayProxy]
         Read proxy dictionary keyed by array name.
-    write : ArrayProxy
+    write : CubedArrayProxy
         Write proxy with an ``array`` attribute that supports ``__setitem__``.
     """
 
     block_function: Callable
     function: Callable
-    reads_map: Dict[str, ArrayProxy]
-    write: ArrayProxy
+    reads_map: Dict[str, CubedArrayProxy]
+    write: CubedArrayProxy
 
 
 def apply_blockwise(out_key, *, config=BlockwiseSpec):
     """Stage function for blockwise."""
     # lithops needs params to be lists not tuples, so convert back
     out_key = tuple(out_key)
     out_chunk_key = key_to_slices(out_key, config.write.array, config.write.chunks)
     args = []
     name_chunk_inds = config.block_function(("out",) + out_key)
     for name_chunk_ind in name_chunk_inds:
         name = name_chunk_ind[0]
         chunk_ind = name_chunk_ind[1:]
-        arr = config.reads_map[name].array
+        arr = config.reads_map[name].open()
         chunk_key = key_to_slices(chunk_ind, arr)
         arg = arr[chunk_key]
         args.append(arg)
 
     result = config.function(*args)
     if isinstance(result, dict):  # structured array with named fields
         for k, v in result.items():
-            config.write.array.set_basic_selection(out_chunk_key, v, fields=k)
+            config.write.open().set_basic_selection(out_chunk_key, v, fields=k)
     else:
-        config.write.array[out_chunk_key] = result
+        config.write.open()[out_chunk_key] = result
 
 
 def key_to_slices(key, arr, chunks=None):
     """Convert a chunk index key to a tuple of slices"""
     chunks = normalize_chunks(chunks or arr.chunks, shape=arr.shape, dtype=arr.dtype)
     return get_item(chunks, key)
 
@@ -167,23 +168,23 @@
 
     # end block func
 
     chunksize = to_chunksize(chunks)
     if isinstance(target_store, zarr.Array):
         target_array = target_store
     else:
-        target_array = zarr.empty(
-            shape, store=target_store, chunks=chunksize, dtype=dtype
+        target_array = lazy_empty(
+            shape, dtype=dtype, chunks=chunksize, store=target_store
         )
 
     func_with_kwargs = partial(func, **kwargs)
     read_proxies = {
-        name: ArrayProxy(array, array.chunks) for name, array in array_map.items()
+        name: CubedArrayProxy(array, array.chunks) for name, array in array_map.items()
     }
-    write_proxy = ArrayProxy(target_array, chunksize)
+    write_proxy = CubedArrayProxy(target_array, chunksize)
     spec = BlockwiseSpec(block_function, func_with_kwargs, read_proxies, write_proxy)
 
     stages = [
         Stage(
             apply_blockwise,
             gensym("apply_blockwise"),
             mappable=output_blocks,
@@ -208,15 +209,15 @@
     if projected_mem > allowed_mem:
         raise ValueError(
             f"Projected blockwise memory ({projected_mem}) exceeds allowed_mem ({allowed_mem}), including reserved_mem ({reserved_mem})"
         )
 
     num_tasks = len(output_blocks)
 
-    return CubedPipeline(stages, spec, target_array, projected_mem, num_tasks)
+    return CubedPipeline(stages, spec, target_array, None, projected_mem, num_tasks)
 
 
 # Code for fusing pipelines
 
 
 def is_fuse_candidate(pipeline):
     """
@@ -261,15 +262,15 @@
     write_proxy = pipeline2.config.write
     spec = BlockwiseSpec(fused_blockwise_func, fused_func, read_proxies, write_proxy)
 
     target_array = pipeline2.target_array
     projected_mem = max(pipeline1.projected_mem, pipeline2.projected_mem)
     num_tasks = pipeline2.num_tasks
 
-    return CubedPipeline(stages, spec, target_array, projected_mem, num_tasks)
+    return CubedPipeline(stages, spec, target_array, None, projected_mem, num_tasks)
 
 
 # blockwise functions
 
 
 def make_blockwise_function(
     func, output, out_indices, *arrind_pairs, numblocks=None, new_axes=None
```

### Comparing `cubed-0.7.0/cubed/random.py` & `cubed-0.8.0/cubed/random.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/runtime/backup.py` & `cubed-0.8.0/cubed/runtime/backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/runtime/executors/beam.py` & `cubed-0.8.0/cubed/runtime/executors/beam.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,19 +131,19 @@
             # for metric in counters:
             #     print(metric)
 
 
 class BeamDagExecutor(DagExecutor):
     """An execution engine that uses Apache Beam."""
 
-    def execute_dag(self, dag, callbacks=None, array_names=None, **kwargs):
+    def execute_dag(self, dag, callbacks=None, array_names=None, resume=None, **kwargs):
         dag = dag.copy()
         pipeline = beam.Pipeline(**kwargs)
 
-        for name, node in visit_nodes(dag):
+        for name, node in visit_nodes(dag, resume=resume):
             rechunker_pipeline = node["pipeline"]
 
             dep_nodes = list(dag.predecessors(name))
 
             pcolls = [
                 p
                 for (n, p) in nx.get_node_attributes(dag, "pcoll").items()
```

### Comparing `cubed-0.7.0/cubed/runtime/executors/lithops.py` & `cubed-0.8.0/cubed/runtime/executors/lithops.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from functools import partial
 from typing import Callable, Iterable
 
 from lithops.executors import FunctionExecutor
 from lithops.wait import ALWAYS, ANY_COMPLETED
 from six import reraise
 
-from cubed.core.array import TaskEndEvent
 from cubed.core.plan import visit_nodes
 from cubed.runtime.backup import should_launch_backup
 from cubed.runtime.types import DagExecutor
+from cubed.runtime.utils import handle_callbacks
 from cubed.vendor.rechunker.types import ParallelPipelines, PipelineExecutor
 
 logger = logging.getLogger(__name__)
 
 # Lithops represents delayed execution tasks as functions that require
 # a FunctionExecutor.
 Task = Callable[[FunctionExecutor], None]
@@ -56,150 +56,164 @@
 
 
 def map_unordered(
     lithops_function_executor,
     map_function,
     map_iterdata,
     include_modules=[],
-    max_failures=3,
+    timeout=None,
+    retries=2,
     use_backups=False,
     return_stats=False,
     **kwargs,
 ):
     """
     Apply a function to items of an input list, yielding results as they are completed
     (which may be different to the input order).
 
     A generalisation of Lithops `map`, with retries, and relaxed return ordering.
 
     :param lithops_function_executor: The Lithops function executor to use.
     :param map_function: The function to map over the data.
     :param map_iterdata: An iterable of input data.
     :param include_modules: Modules to include.
-    :param max_failures: The number of task failures to allow before raising an exception.
+    :param retries: The number of times to retry a failed task before raising an exception.
     :param use_backups: Whether to launch backup tasks to mitigate against slow-running tasks.
     :param return_stats: Whether to return lithops stats.
 
     :return: Function values (and optionally stats) as they are completed, not necessarily in the input order.
     """
-    failures = 0
     return_when = ALWAYS if use_backups else ANY_COMPLETED
 
-    inputs = map_iterdata
+    inputs = list(map_iterdata)
     tasks = {}
     start_times = {}
     end_times = {}
     backups = {}
     pending = []
 
     # can't use functools.partial here as we get an error in lithops
     # also, lithops extra_args doesn't work for this case
     partial_map_function = lambda x: map_function(x, **kwargs)
 
     futures = lithops_function_executor.map(
-        partial_map_function, inputs, include_modules=include_modules
+        partial_map_function, inputs, timeout=timeout, include_modules=include_modules
     )
     tasks.update({k: v for (k, v) in zip(futures, inputs)})
     start_times.update({k: time.monotonic() for k in futures})
     pending.extend(futures)
 
+    future_to_index = {f: i for i, f in enumerate(futures)}
+    failure_counts = [0] * len(inputs)
+
     while pending:
         finished, pending = lithops_function_executor.wait(
             pending, throw_except=False, return_when=return_when, show_progressbar=False
         )
-
         failed = []
         for future in finished:
             if future.error:
-                failures += 1
-                if failures > max_failures:
+                index = future_to_index[future]
+                failure_counts[index] = failure_counts[index] + 1
+                failure_count = failure_counts[index]
+
+                if failure_count > retries:
                     # re-raise exception
                     # TODO: why does calling status not raise the exception?
                     future.status(throw_except=True)
                     reraise(*future._exception)
                 failed.append(future)
             else:
                 end_times[future] = time.monotonic()
                 if return_stats:
-                    yield future.result(), future.stats
+                    yield future.result(), standardise_lithops_stats(future.stats)
                 else:
                     yield future.result()
 
+            # remove any backup task
             if use_backups:
-                # remove backups
                 backup = backups.get(future, None)
                 if backup:
                     if backup in pending:
                         pending.remove(backup)
                     del backups[future]
                     del backups[backup]
 
         if failed:
             # rerun and add to pending
-            inputs = [v for (fut, v) in tasks.items() if fut in failed]
+            inputs_to_rerun = []
+            input_indexes_to_rerun = []
+            for fut in failed:
+                index = future_to_index[fut]
+                inputs_to_rerun.append(inputs[index])
+                input_indexes_to_rerun.append(index)
+                del future_to_index[fut]
             # TODO: de-duplicate code from above
             futures = lithops_function_executor.map(
                 partial_map_function,
-                inputs,
+                inputs_to_rerun,
+                timeout=timeout,
                 include_modules=include_modules,
             )
-            tasks.update({k: v for (k, v) in zip(futures, inputs)})
+            tasks.update({k: v for (k, v) in zip(futures, inputs_to_rerun)})
             start_times.update({k: time.monotonic() for k in futures})
             pending.extend(futures)
 
+            future_to_index.update(
+                {f: i for i, f in zip(input_indexes_to_rerun, futures)}
+            )
+
         if use_backups:
             now = time.monotonic()
             for future in copy.copy(pending):
                 if future not in backups and should_launch_backup(
                     future, now, start_times, end_times
                 ):
-                    inputs = [v for (fut, v) in tasks.items() if fut == future]
-                    logger.info("Running backup task for %s", inputs)
+                    input = tasks[future]
+                    logger.info("Running backup task for %s", input)
                     futures = lithops_function_executor.map(
                         partial_map_function,
-                        inputs,
+                        [input],
+                        timeout=timeout,
                         include_modules=include_modules,
                     )
-                    tasks.update({k: v for (k, v) in zip(futures, inputs)})
+                    tasks.update({k: v for (k, v) in zip(futures, [input])})
                     start_times.update({k: time.monotonic() for k in futures})
                     pending.extend(futures)
-                    pending.remove(future)  # throw away slow one
                     backup = futures[0]  # TODO: launch multiple backups at once
                     backups[future] = backup
                     backups[backup] = future
             time.sleep(1)
 
 
-def execute_dag(dag, callbacks=None, array_names=None, **kwargs):
+def execute_dag(dag, callbacks=None, array_names=None, resume=None, **kwargs):
     use_backups = kwargs.pop("use_backups", False)
     with FunctionExecutor(**kwargs) as executor:
-        for name, node in visit_nodes(dag):
+        for name, node in visit_nodes(dag, resume=resume):
             pipeline = node["pipeline"]
             for stage in pipeline.stages:
                 if stage.mappable is not None:
                     for _, stats in map_unordered(
                         executor,
                         run_func,
                         list(stage.mappable),
                         func=stage.function,
                         config=pipeline.config,
                         name=name,
                         use_backups=use_backups,
                         return_stats=True,
                     ):
-                        if callbacks is not None:
-                            event = lithops_stats_to_task_end_event(name, stats)
-                            [callback.on_task_end(event) for callback in callbacks]
+                        stats["array_name"] = name
+                        handle_callbacks(callbacks, stats)
                 else:
                     raise NotImplementedError()
 
 
-def lithops_stats_to_task_end_event(name, stats):
-    return TaskEndEvent(
-        array_name=name,
+def standardise_lithops_stats(stats):
+    return dict(
         task_create_tstamp=stats["host_job_create_tstamp"],
         function_start_tstamp=stats["worker_func_start_tstamp"],
         function_end_tstamp=stats["worker_func_end_tstamp"],
         task_result_tstamp=stats["host_status_done_tstamp"],
         peak_measured_mem_start=stats["worker_peak_memory_start"],
         peak_measured_mem_end=stats["worker_peak_memory_end"],
     )
@@ -215,17 +229,16 @@
         for _, stats in map_unordered(
             lithops_function_executor,
             sf,
             list(stage.mappable),
             use_backups=use_backups,
             return_stats=True,
         ):
-            if callbacks is not None:
-                event = lithops_stats_to_task_end_event(name, stats)
-                [callback.on_task_end(event) for callback in callbacks]
+            stats["array_name"] = name
+            handle_callbacks(callbacks, stats)
 
     return stage_func
 
 
 def build_stage_func(stage, config):
     def sf():
         return stage.function(config=config)
```

### Comparing `cubed-0.7.0/cubed/runtime/executors/modal_async.py` & `cubed-0.8.0/cubed/runtime/executors/modal_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 from asyncio.exceptions import TimeoutError
 
 import modal
 import modal.aio
 from modal.exception import ConnectionError
 from tenacity import retry, retry_if_exception_type, stop_after_attempt
 
-from cubed.core.array import TaskEndEvent
 from cubed.core.plan import visit_nodes
 from cubed.runtime.backup import should_launch_backup
 from cubed.runtime.types import DagExecutor
-from cubed.utils import peak_measured_mem
+from cubed.runtime.utils import execute_with_stats, handle_callbacks
 
-async_stub = modal.aio.AioStub()
+async_stub = modal.aio.AioStub("async-stub")
 
 requirements_file = os.getenv("CUBED_MODAL_REQUIREMENTS_FILE")
 
 if requirements_file:
     image = modal.Image.debian_slim().pip_install_from_requirements(requirements_file)
 else:
     image = modal.Image.debian_slim().pip_install(
@@ -41,47 +40,46 @@
     secret=modal.Secret.from_name("my-aws-secret"),
     memory=2000,
     retries=2,
     is_generator=True,
 )
 async def async_run_remotely(input, func=None, config=None):
     print(f"running remotely on {input}")
-    peak_measured_mem_start = peak_measured_mem()
-    function_start_tstamp = time.time()
-    result = func(input, config=config)
-    function_end_tstamp = time.time()
-    peak_measured_mem_end = peak_measured_mem()
-    yield (
-        result,
-        function_start_tstamp,
-        function_end_tstamp,
-        peak_measured_mem_start,
-        peak_measured_mem_end,
-    )
+    # note we can't use the execution_stat decorator since it doesn't work with modal decorators
+    result, stats = execute_with_stats(func, input, config=config)
+    yield result, stats
 
 
 # We need map_unordered for the use_backups implementation
 async def map_unordered(
-    app_function, input, max_failures=3, use_backups=False, **kwargs
+    app_function, input, use_backups=False, return_stats=False, name=None, **kwargs
 ):
     """
     Apply a function to items of an input list, yielding results as they are completed
     (which may be different to the input order).
 
     :param app_function: The Modal function to map over the data.
     :param input: An iterable of input data.
-    :param max_failures: The number of task failures to allow before raising an exception.
     :param use_backups: Whether to launch backup tasks to mitigate against slow-running tasks.
     :param kwargs: Keyword arguments to pass to the function.
 
     :return: Function values (and optionally stats) as they are completed, not necessarily in the input order.
     """
+    task_create_tstamp = time.time()
+
     if not use_backups:
         async for result in app_function.map(input, kwargs=kwargs):
-            yield result
+            if return_stats:
+                result, stats = result
+                if name is not None:
+                    stats["array_name"] = name
+                stats["task_create_tstamp"] = task_create_tstamp
+                yield result, stats
+            else:
+                yield result
         return
 
     tasks = {asyncio.ensure_future(app_function.call(i, **kwargs)): i for i in input}
     pending = set(tasks.keys())
     t = time.monotonic()
     start_times = {f: t for f in pending}
     end_times = {}
@@ -91,18 +89,26 @@
         finished, pending = await asyncio.wait(
             pending, return_when=asyncio.FIRST_COMPLETED, timeout=2
         )
         # print("finished", finished)
         # print("pending", pending)
 
         for task in finished:
+            # TODO: use exception groups in Python 3.11 to handle case of multiple task exceptions
             if task.exception():
                 raise task.exception()
             end_times[task] = time.monotonic()
-            yield task.result()
+            if return_stats:
+                result, stats = task.result()
+                if name is not None:
+                    stats["array_name"] = name
+                stats["task_create_tstamp"] = task_create_tstamp
+                yield result, stats
+            else:
+                yield task.result()
 
             # remove any backup task
             if use_backups:
                 backup = backups.get(task, None)
                 if backup:
                     pending.remove(backup)
                     del backups[task]
@@ -125,58 +131,43 @@
 
 
 # This just retries the initial connection attempt, not the function calls
 @retry(
     retry=retry_if_exception_type((TimeoutError, ConnectionError)),
     stop=stop_after_attempt(3),
 )
-async def async_execute_dag(dag, callbacks=None, array_names=None, **kwargs):
+async def async_execute_dag(
+    dag, callbacks=None, array_names=None, resume=None, **kwargs
+):
     async with async_stub.run():
-        for name, node in visit_nodes(dag):
+        for name, node in visit_nodes(dag, resume=resume):
             pipeline = node["pipeline"]
 
             for stage in pipeline.stages:
                 if stage.mappable is not None:
-                    task_create_tstamp = time.time()
-                    async for result in map_unordered(
+                    async for _, stats in map_unordered(
                         async_run_remotely,
                         list(stage.mappable),
+                        return_stats=True,
+                        name=name,
                         func=stage.function,
                         config=pipeline.config,
                         **kwargs,
                     ):
-                        handle_callbacks(callbacks, name, result, task_create_tstamp)
+                        handle_callbacks(callbacks, stats)
                 else:
                     raise NotImplementedError()
 
 
-def handle_callbacks(callbacks, array_name, result, task_create_tstamp):
-    if callbacks is not None:
-        task_result_tstamp = time.time()
-        (
-            res,
-            function_start_tstamp,
-            function_end_tstamp,
-            peak_measured_mem_start,
-            peak_measured_mem_end,
-        ) = result
-        task_stats = dict(
-            task_create_tstamp=task_create_tstamp,
-            function_start_tstamp=function_start_tstamp,
-            function_end_tstamp=function_end_tstamp,
-            task_result_tstamp=task_result_tstamp,
-            peak_measured_mem_start=peak_measured_mem_start,
-            peak_measured_mem_end=peak_measured_mem_end,
-        )
-        event = TaskEndEvent(array_name=array_name, **task_stats)
-        [callback.on_task_end(event) for callback in callbacks]
-
-
 class AsyncModalDagExecutor(DagExecutor):
     """An execution engine that uses Modal's async API."""
 
-    def execute_dag(self, dag, callbacks=None, array_names=None, **kwargs):
+    def execute_dag(self, dag, callbacks=None, array_names=None, resume=None, **kwargs):
         asyncio.run(
             async_execute_dag(
-                dag, callbacks=callbacks, array_names=array_names, **kwargs
+                dag,
+                callbacks=callbacks,
+                array_names=array_names,
+                resume=resume,
+                **kwargs,
             )
         )
```

### Comparing `cubed-0.7.0/cubed/runtime/executors/python.py` & `cubed-0.8.0/cubed/runtime/executors/python.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 def exec_stage_func(func, *args, **kwargs):
     return func(*args, **kwargs)
 
 
 class PythonDagExecutor(DagExecutor):
     """The default execution engine that runs tasks sequentially uses Python loops."""
 
-    def execute_dag(self, dag, callbacks=None, array_names=None, **kwargs):
-        for name, node in visit_nodes(dag):
+    def execute_dag(self, dag, callbacks=None, array_names=None, resume=None, **kwargs):
+        for name, node in visit_nodes(dag, resume=resume):
             pipeline = node["pipeline"]
             for stage in pipeline.stages:
                 if stage.mappable is not None:
                     for m in stage.mappable:
                         exec_stage_func(stage.function, m, config=pipeline.config)
                         if callbacks is not None:
                             event = TaskEndEvent(array_name=name)
```

### Comparing `cubed-0.7.0/cubed/runtime/executors/python_async.py` & `cubed-0.8.0/cubed/runtime/executors/python_async.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,120 @@
 import asyncio
 import time
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 
 from aiostream import stream
-from tenacity import retry, stop_after_attempt
+from tenacity import Retrying, stop_after_attempt
 
-from cubed.core.array import TaskEndEvent
 from cubed.core.plan import visit_node_generations
 from cubed.runtime.types import DagExecutor
-from cubed.utils import peak_measured_mem
+from cubed.runtime.utils import execution_stats, handle_callbacks
 
 
-def execution_stats(func):
-    """Measure timing information and peak memory usage of a function call."""
-
-    def wrapper(*args, **kwargs):
-        peak_measured_mem_start = peak_measured_mem()
-        function_start_tstamp = time.time()
-        result = func(*args, **kwargs)
-        function_end_tstamp = time.time()
-        peak_measured_mem_end = peak_measured_mem()
-        return result, dict(
-            function_start_tstamp=function_start_tstamp,
-            function_end_tstamp=function_end_tstamp,
-            peak_measured_mem_start=peak_measured_mem_start,
-            peak_measured_mem_end=peak_measured_mem_end,
-        )
-
-    return wrapper
-
-
-@retry(stop=stop_after_attempt(3))
 @execution_stats
 def run_func(input, func=None, config=None, name=None):
     print(f"{name}: running on {input}")
     result = func(input, config=config)
     return result
 
 
 async def map_unordered(
     concurrent_executor,
     function,
     input,
-    max_failures=3,
+    retries=2,
     use_backups=False,
+    return_stats=False,
+    name=None,
     **kwargs,
 ):
-    print(f"{kwargs['name']}: running map_unordered")
+    if name is not None:
+        print(f"{name}: running map_unordered")
+    if retries == 0:
+        retrying_function = function
+    else:
+        retryer = Retrying(reraise=True, stop=stop_after_attempt(retries + 1))
+        retrying_function = partial(retryer, function)
+
+    task_create_tstamp = time.time()
     tasks = {
-        asyncio.wrap_future(concurrent_executor.submit(function, i, **kwargs)): i
+        asyncio.wrap_future(
+            concurrent_executor.submit(retrying_function, i, **kwargs)
+        ): i
         for i in input
     }
     pending = set(tasks.keys())
 
     while pending:
         finished, pending = await asyncio.wait(
             pending, return_when=asyncio.FIRST_COMPLETED, timeout=2
         )
         for task in finished:
+            # TODO: use exception groups in Python 3.11 to handle case of multiple task exceptions
             if task.exception():
                 raise task.exception()
-            yield task.result()
-
-
-async def produce(*args, **kwargs):
-    task_create_tstamp = time.time()
-    name = kwargs.get("name", None)
-    async for result, stats in map_unordered(*args, **kwargs):
-        stats["array_name"] = name
-        stats["task_create_tstamp"] = task_create_tstamp
-        yield result, stats
+            if return_stats:
+                result, stats = task.result()
+                if name is not None:
+                    stats["array_name"] = name
+                stats["task_create_tstamp"] = task_create_tstamp
+                yield result, stats
+            else:
+                yield task.result()
 
 
 def pipeline_to_stream(concurrent_executor, name, pipeline, **kwargs):
     if any([stage for stage in pipeline.stages if stage.mappable is None]):
         raise NotImplementedError("All stages must be mappable in pipelines")
     it = stream.iterate(
         [
             partial(
-                produce,
+                map_unordered,
                 concurrent_executor,
                 run_func,
                 list(stage.mappable),
+                return_stats=True,
+                name=name,
                 func=stage.function,
                 config=pipeline.config,
-                name=name,
                 **kwargs,
             )
             for stage in pipeline.stages
             if stage.mappable is not None
         ]
     )
     # concat stages, running only one stage at a time
     return stream.concatmap(it, lambda f: f(), task_limit=1)
 
 
-async def async_execute_dag(dag, callbacks=None, array_names=None, **kwargs):
+async def async_execute_dag(
+    dag, callbacks=None, array_names=None, resume=None, **kwargs
+):
     with ThreadPoolExecutor() as concurrent_executor:
-        for gen in visit_node_generations(dag):
+        for gen in visit_node_generations(dag, resume=resume):
             # run pipelines in the same topological generation in parallel by merging their streams
             streams = [
                 pipeline_to_stream(
                     concurrent_executor, name, node["pipeline"], **kwargs
                 )
                 for name, node in gen
             ]
             merged_stream = stream.merge(*streams)
             async with merged_stream.stream() as streamer:
                 async for _, stats in streamer:
                     handle_callbacks(callbacks, stats)
 
 
-def handle_callbacks(callbacks, stats):
-    if callbacks is not None:
-        task_result_tstamp = time.time()
-        event = TaskEndEvent(
-            task_result_tstamp=task_result_tstamp,
-            **stats,
-        )
-        [callback.on_task_end(event) for callback in callbacks]
-
-
 class AsyncPythonDagExecutor(DagExecutor):
     """An execution engine that uses Python asyncio."""
 
-    def execute_dag(self, dag, callbacks=None, array_names=None, **kwargs):
+    def execute_dag(self, dag, callbacks=None, array_names=None, resume=None, **kwargs):
         asyncio.run(
             async_execute_dag(
-                dag, callbacks=callbacks, array_names=array_names, **kwargs
+                dag,
+                callbacks=callbacks,
+                array_names=array_names,
+                resume=resume,
+                **kwargs,
             )
         )
```

### Comparing `cubed-0.7.0/cubed/runtime/pipeline.py` & `cubed-0.8.0/cubed/runtime/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import itertools
 import math
 from typing import Any, Iterable, Iterator, List, Tuple
 
 import numpy as np
 
 from cubed.primitive.types import CubedPipeline
+from cubed.storage.zarr import open_if_lazy_zarr_array
 from cubed.vendor.rechunker.types import CopySpec, Stage
 
 from .utils import gensym
 
 
 # differs from rechunker's chunk_keys to return a list rather than a tuple, to keep lithops happy
 def chunk_keys(
@@ -38,32 +39,32 @@
         return chunk_keys(self.shape, self.chunks)
 
 
 def copy_read_to_write(chunk_key, *, config=CopySpec):
     # workaround limitation of lithops.utils.verify_args
     if isinstance(chunk_key, list):
         chunk_key = tuple(chunk_key)
-    data = np.asarray(config.read.array[chunk_key])
-    config.write.array[chunk_key] = data
+    data = np.asarray(config.read.open()[chunk_key])
+    config.write.open()[chunk_key] = data
 
 
 def copy_read_to_intermediate(chunk_key, *, config=CopySpec):
     # workaround limitation of lithops.utils.verify_args
     if isinstance(chunk_key, list):
         chunk_key = tuple(chunk_key)
-    data = np.asarray(config.read.array[chunk_key])
-    config.intermediate.array[chunk_key] = data
+    data = np.asarray(config.read.open()[chunk_key])
+    config.intermediate.open()[chunk_key] = data
 
 
 def copy_intermediate_to_write(chunk_key, *, config=CopySpec):
     # workaround limitation of lithops.utils.verify_args
     if isinstance(chunk_key, list):
         chunk_key = tuple(chunk_key)
-    data = np.asarray(config.intermediate.array[chunk_key])
-    config.write.array[chunk_key] = data
+    data = np.asarray(config.intermediate.open()[chunk_key])
+    config.write.open()[chunk_key] = data
 
 
 def spec_to_pipeline(
     spec: CopySpec, target_array: Any, projected_mem: int, num_tasks: int
 ) -> CubedPipeline:
     # typing won't work until we start using numpy types
     shape = spec.read.array.shape  # type: ignore
@@ -84,22 +85,29 @@
             ),
             Stage(
                 copy_intermediate_to_write,
                 gensym("copy_intermediate_to_write"),
                 mappable=ChunkKeys(shape, spec.write.chunks),
             ),
         ]
-    return CubedPipeline(stages, spec, target_array, projected_mem, num_tasks)
+    return CubedPipeline(
+        stages, spec, target_array, spec.intermediate.array, projected_mem, num_tasks
+    )
 
 
-def already_computed(node_dict):
+def already_computed(node_dict, resume=None):
     """
     Return True if the array for a node doesn't have a pipeline to compute it,
     or it has already been computed (all chunks are present).
     """
     pipeline = node_dict.get("pipeline", None)
     if pipeline is None:
         return True
+
     target = node_dict.get("target", None)
-    if target.ndim > 0 and target.nchunks_initialized == target.nchunks:
-        return True
+    if resume and target is not None:
+        target = open_if_lazy_zarr_array(target)
+        # this check can be expensive since it has to list the directory to find nchunks
+        if target.ndim > 0 and target.nchunks_initialized == target.nchunks:
+            return True
+
     return False
```

### Comparing `cubed-0.7.0/cubed/tests/primitive/test_blockwise.py` & `cubed-0.8.0/cubed/tests/primitive/test_blockwise.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         + (itemsize * 2)  # source2 uncompressed chunk
         + (itemsize * 2 * 2)  # output compressed chunk
         + (itemsize * 2 * 2)  # output uncompressed chunk
     )
 
     assert pipeline.num_tasks == 4
 
+    pipeline.target_array.create()  # create lazy zarr array
+
     execute_pipeline(pipeline, executor=executor)
 
     res = zarr.open(target_store)
     assert_array_equal(res[:], np.outer([0, 1, 2], [10, 50, 100]))
 
 
 def _permute_dims(x, /, axes, allowed_mem, reserved_mem, target_store):
@@ -114,14 +116,16 @@
         + (itemsize * 2 * 2)  # source uncompressed chunk
         + (itemsize * 2 * 2)  # output compressed chunk
         + (itemsize * 2 * 2)  # output uncompressed chunk
     )
 
     assert pipeline.num_tasks == 4
 
+    pipeline.target_array.create()  # create lazy zarr array
+
     execute_pipeline(pipeline, executor=executor)
 
     res = zarr.open(target_store)
     assert_array_equal(
         res[:], np.transpose(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]), axes=(1, 0))
     )
```

### Comparing `cubed-0.7.0/cubed/tests/primitive/test_rechunk.py` & `cubed-0.8.0/cubed/tests/primitive/test_rechunk.py`

 * *Files 16% similar despite different names*

```diff
@@ -76,14 +76,19 @@
     assert pipeline.target_array.dtype == source.dtype
     assert pipeline.target_array.chunks == target_chunks
 
     assert pipeline.projected_mem == expected_projected_mem
 
     assert pipeline.num_tasks == expected_num_tasks
 
+    # create lazy zarr arrays
+    pipeline.target_array.create()
+    if pipeline.intermediate_array is not None:
+        pipeline.intermediate_array.create()
+
     execute_pipeline(pipeline, executor=executor)
 
     res = zarr.open(target_store)
     assert_array_equal(res[:], np.ones(shape))
     assert res.chunks == target_chunks
```

### Comparing `cubed-0.7.0/cubed/tests/runtime/test_backup.py` & `cubed-0.8.0/cubed/tests/runtime/test_backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/tests/test_array_api.py` & `cubed-0.8.0/cubed/tests/test_array_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
 
 def test_index_slice_unsupported_step(spec):
     with pytest.raises(NotImplementedError):
         a = xp.arange(12, chunks=(4,), spec=spec)
         a[3:10:2]
 
 
+@pytest.mark.xfail(reason="not currently compatible with lazy zarr arrays")
 def test_setitem(spec):
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
     b = xp.ones(())
     a[1, 2] = b
     assert_array_equal(a.compute(), np.array([[1, 2, 3], [4, 5, 1], [7, 8, 9]]))
```

### Comparing `cubed-0.7.0/cubed/tests/test_core.py` & `cubed-0.8.0/cubed/tests/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import numpy as np
 import pytest
 import zarr
 from numpy.testing import assert_array_equal
 
 import cubed
 import cubed.array_api as xp
+from cubed.extensions.history import HistoryCallback
+from cubed.extensions.timeline import TimelineVisualizationCallback
 from cubed.extensions.tqdm import TqdmProgressBar
 from cubed.primitive.blockwise import apply_blockwise
 from cubed.runtime.types import DagExecutor
 from cubed.tests.utils import MAIN_EXECUTORS, MODAL_EXECUTORS, TaskCounter, create_zarr
 
 
 @pytest.fixture()
@@ -205,16 +207,17 @@
 
 
 def test_rechunk_same_chunks(spec):
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 1), spec=spec)
     b = a.rechunk((2, 1))
     task_counter = TaskCounter()
     res = b.compute(callbacks=[task_counter])
-    # no tasks should have run since chunks are same
-    assert task_counter.value == 0
+    # no tasks except array creation task should have run since chunks are same
+    num_created_arrays = 1
+    assert task_counter.value == num_created_arrays
 
     assert_array_equal(res, np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]))
 
 
 def test_compute_is_idempotent(spec, executor):
     a = xp.ones((3, 3), chunks=(2, 2), spec=spec)
     b = xp.negative(a)
@@ -244,14 +247,55 @@
     spec2 = cubed.Spec(tmp_path, allowed_mem=200000)
     a = xp.ones((3, 3), chunks=(2, 2), spec=spec1)
     b = xp.ones((3, 3), chunks=(2, 2), spec=spec2)
     with pytest.raises(ValueError):
         xp.add(a, b)
 
 
+class TestSpecMemArgTypes:
+    def test_max_mem_deprecation_warning(self):
+        # Remove once max_mem fully deprecated in favour of allowed_mem
+        with pytest.warns(
+            DeprecationWarning,
+            match="`max_mem` is deprecated, please use `allowed_mem` instead",
+        ):
+            cubed.Spec(max_mem=100_000)
+
+    @pytest.mark.parametrize(
+        "input_value, expected_value",
+        [
+            (500, 500),
+            (100_000, 100_000),
+            ("500B", 500),
+            ("1kB", 1000),
+            ("1MB", 1000**2),
+            ("1GB", 1000**3),
+            ("1TB", 1000**4),
+            ("1PB", 1000**5),
+        ],
+    )
+    def test_convert_to_bytes(self, input_value, expected_value):
+        spec = cubed.Spec(allowed_mem=input_value)
+        assert spec.allowed_mem == expected_value
+
+    @pytest.mark.parametrize(
+        "input_value",
+        [
+            "1EB",  # EB is not a valid unit in this function
+            "1kb",  # lower-case k is not valid
+            "invalid",  # completely invalid input
+            -512,  # negative integer
+            1000.0,  # invalid type
+        ],
+    )
+    def test_convert_to_bytes_error(self, input_value):
+        with pytest.raises(ValueError):
+            cubed.Spec(allowed_mem=input_value)
+
+
 def test_reduction_multiple_rounds(tmp_path, executor):
     spec = cubed.Spec(tmp_path, allowed_mem=1000)
     a = xp.ones((100, 10), dtype=np.uint8, chunks=(1, 10), spec=spec)
     b = xp.sum(a, axis=0, dtype=np.uint8)
     # check that there is > 1 rechunk step
     rechunks = [
         n for (n, d) in b.plan.dag.nodes(data=True) if d["op_name"] == "rechunk"
@@ -382,30 +426,39 @@
 
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
     b = xp.asarray([[1, 1, 1], [1, 1, 1], [1, 1, 1]], chunks=(2, 2), spec=spec)
     c = xp.add(a, b)
     assert_array_equal(c.compute(), np.array([[2, 3, 4], [5, 6, 7], [8, 9, 10]]))
 
 
+@pytest.mark.skipif(
+    platform.system() == "Windows", reason="measuring memory does not run on windows"
+)
 def test_callbacks(spec, executor):
     if not isinstance(executor, DagExecutor):
         pytest.skip(f"{type(executor)} does not support callbacks")
 
     task_counter = TaskCounter()
-    progress = TqdmProgressBar()  # test indirectly (doesn't fail)
+    # test following indirectly by checking they don't cause a failure
+    progress = TqdmProgressBar()
+    hist = HistoryCallback()
+    timeline_viz = TimelineVisualizationCallback()
 
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
     b = xp.asarray([[1, 1, 1], [1, 1, 1], [1, 1, 1]], chunks=(2, 2), spec=spec)
     c = xp.add(a, b)
     assert_array_equal(
-        c.compute(executor=executor, callbacks=[task_counter, progress]),
+        c.compute(
+            executor=executor, callbacks=[task_counter, progress, hist, timeline_viz]
+        ),
         np.array([[2, 3, 4], [5, 6, 7], [8, 9, 10]]),
     )
 
-    assert task_counter.value == 4
+    num_created_arrays = 3
+    assert task_counter.value == num_created_arrays + 4
 
 
 @pytest.mark.cloud
 def test_callbacks_modal(spec, modal_executor):
     task_counter = TaskCounter(check_timestamps=False)
     tmp_path = "s3://cubed-unittest/callbacks"
     spec = cubed.Spec(tmp_path, allowed_mem=100000)
@@ -414,42 +467,47 @@
         b = xp.asarray([[1, 1, 1], [1, 1, 1], [1, 1, 1]], chunks=(2, 2), spec=spec)
         c = xp.add(a, b)
         assert_array_equal(
             c.compute(executor=modal_executor, callbacks=[task_counter]),
             np.array([[2, 3, 4], [5, 6, 7], [8, 9, 10]]),
         )
 
-        assert task_counter.value == 4
+        num_created_arrays = 3
+        assert task_counter.value == num_created_arrays + 4
     finally:
         fs = fsspec.open(tmp_path).fs
         fs.rm(tmp_path, recursive=True)
 
 
 def test_already_computed(spec):
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
     b = xp.asarray([[1, 1, 1], [1, 1, 1], [1, 1, 1]], chunks=(2, 2), spec=spec)
     c = xp.add(a, b)
     d = xp.negative(c)
 
-    assert d.plan.num_tasks(optimize_graph=False) == 8
+    num_created_arrays = 4  # a, b, c, d
+    assert d.plan.num_tasks(optimize_graph=False) == num_created_arrays + 8
 
     task_counter = TaskCounter()
     c.compute(callbacks=[task_counter], optimize_graph=False)
-    assert task_counter.value == 4
+    num_created_arrays = 3  # a, b, c
+    assert task_counter.value == num_created_arrays + 4
 
     # since c has already been computed, when computing d only 4 tasks are run, instead of 8
     task_counter = TaskCounter()
-    d.compute(callbacks=[task_counter], optimize_graph=False)
-    assert task_counter.value == 4
+    d.compute(callbacks=[task_counter], optimize_graph=False, resume=True)
+    # the create arrays tasks are run again, even though they exist
+    num_created_arrays = 4  # a, b, c, d
+    assert task_counter.value == num_created_arrays + 4
 
 
 @pytest.mark.skipif(platform.system() == "Windows", reason="does not run on windows")
-def test_measure_reserved_memory(executor):
+def test_measure_reserved_mem(executor):
     pytest.importorskip("lithops")
 
     from cubed.runtime.executors.lithops import LithopsDagExecutor
 
     if not isinstance(executor, LithopsDagExecutor):
-        pytest.skip(f"{type(executor)} does not support measure_reserved_memory")
+        pytest.skip(f"{type(executor)} does not support measure_reserved_mem")
 
-    reserved_memory = cubed.measure_reserved_memory(executor=executor)
+    reserved_memory = cubed.measure_reserved_mem(executor=executor)
     assert reserved_memory > 1_000_000  # over 1MB
```

### Comparing `cubed-0.7.0/cubed/tests/test_gufunc.py` & `cubed-0.8.0/cubed/tests/test_gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/tests/test_indexing.py` & `cubed-0.8.0/cubed/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/tests/test_mem_utilization.py` & `cubed-0.8.0/cubed/tests/test_mem_utilization.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def spec(tmp_path, reserved_mem):
     return cubed.Spec(tmp_path, allowed_mem=2_000_000_000, reserved_mem=reserved_mem)
 
 
 @pytest.fixture(scope="module")
 def reserved_mem():
     executor = LithopsDagExecutor(config=LITHOPS_LOCAL_CONFIG)
-    res = cubed.measure_reserved_memory(executor) * 1.05  # add some wiggle room
+    res = cubed.measure_reserved_mem(executor) * 1.05  # add some wiggle room
     return round_up_to_multiple(res, 10_000_000)  # round up to nearest multiple of 10MB
 
 
 def round_up_to_multiple(x, multiple=10):
     """Round up to the nearest multiple"""
     return math.ceil(x / multiple) * multiple
```

### Comparing `cubed-0.7.0/cubed/tests/test_optimization.py` & `cubed-0.8.0/cubed/tests/test_optimization.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,73 +14,79 @@
 
 def test_fusion(spec):
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
     b = xp.negative(a)
     c = xp.astype(b, np.float32)
     d = xp.negative(c)
 
-    assert d.plan.num_tasks(optimize_graph=False) == 12
-    assert d.plan.num_tasks(optimize_graph=True) == 4
+    num_created_arrays = 4  # a, b, c, d
+    assert d.plan.num_tasks(optimize_graph=False) == num_created_arrays + 12
+    num_created_arrays = 2  # a, d
+    assert d.plan.num_tasks(optimize_graph=True) == num_created_arrays + 4
 
     task_counter = TaskCounter()
     result = d.compute(callbacks=[task_counter])
-    assert task_counter.value == 4
+    assert task_counter.value == num_created_arrays + 4
 
     assert_array_equal(
         result,
         np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]).astype(np.float32),
     )
 
 
 def test_fusion_transpose(spec):
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
     b = xp.negative(a)
     c = xp.astype(b, np.float32)
     d = c.T
 
-    assert d.plan.num_tasks(optimize_graph=False) == 12
-    assert d.plan.num_tasks(optimize_graph=True) == 4
+    num_created_arrays = 4  # a, b, c, d
+    assert d.plan.num_tasks(optimize_graph=False) == num_created_arrays + 12
+    num_created_arrays = 2  # a, d
+    assert d.plan.num_tasks(optimize_graph=True) == num_created_arrays + 4
 
     task_counter = TaskCounter()
     result = d.compute(callbacks=[task_counter])
-    assert task_counter.value == 4
+    assert task_counter.value == num_created_arrays + 4
 
     assert_array_equal(
         result,
         np.array([[-1, -4, -7], [-2, -5, -8], [-3, -6, -9]]).astype(np.float32),
     )
 
 
 def test_no_fusion(spec):
     # b can't be fused with c because d also depends on b
     a = xp.ones((2, 2), chunks=(2, 2), spec=spec)
     b = xp.positive(a)
     c = xp.positive(b)
     d = xp.equal(b, c)
 
-    assert d.plan.num_tasks(optimize_graph=False) == 3
-    assert d.plan.num_tasks(optimize_graph=True) == 3
+    num_created_arrays = 4  # a, b, c, d
+    assert d.plan.num_tasks(optimize_graph=False) == num_created_arrays + 3
+    assert d.plan.num_tasks(optimize_graph=True) == num_created_arrays + 3
 
     task_counter = TaskCounter()
     result = d.compute(callbacks=[task_counter])
-    assert task_counter.value == 3
+    assert task_counter.value == num_created_arrays + 3
 
     assert_array_equal(result, np.ones((2, 2)))
 
 
 def test_no_fusion_multiple_edges(spec):
     a = xp.ones((2, 2), chunks=(2, 2), spec=spec)
     b = xp.positive(a)
     c = xp.asarray(b)
     # b and c are the same array, so d has a single dependency
     # with multiple edges
     # this should not be fused under the current logic
     d = xp.equal(b, c)
 
-    assert d.plan.num_tasks(optimize_graph=False) == 2
-    assert d.plan.num_tasks(optimize_graph=True) == 2
+    num_created_arrays = 3  # a, c, d
+    assert d.plan.num_tasks(optimize_graph=False) == num_created_arrays + 2
+    assert d.plan.num_tasks(optimize_graph=True) == num_created_arrays + 2
 
     task_counter = TaskCounter()
     result = d.compute(callbacks=[task_counter])
-    assert task_counter.value == 2
+    assert task_counter.value == num_created_arrays + 2
 
     assert_array_equal(result, np.full((2, 2), True))
```

### Comparing `cubed-0.7.0/cubed/tests/test_random.py` & `cubed-0.8.0/cubed/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/tests/test_utils.py` & `cubed-0.8.0/cubed/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/tests/utils.py` & `cubed-0.8.0/cubed/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     pass
 
 
 class TaskCounter(Callback):
     def __init__(self, check_timestamps=True) -> None:
         self.check_timestamps = check_timestamps
 
-    def on_compute_start(self, dag):
+    def on_compute_start(self, dag, resume):
         self.value = 0
 
     def on_task_end(self, event):
         if self.check_timestamps and event.task_create_tstamp is not None:
             assert (
                 event.task_result_tstamp
                 >= event.function_end_tstamp
```

### Comparing `cubed-0.7.0/cubed/vendor/dask/array/core.py` & `cubed-0.8.0/cubed/vendor/dask/array/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/dask/array/gufunc.py` & `cubed-0.8.0/cubed/vendor/dask/array/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/dask/array/reshape.py` & `cubed-0.8.0/cubed/vendor/dask/array/reshape.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/dask/array/utils.py` & `cubed-0.8.0/cubed/vendor/dask/array/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/dask/blockwise.py` & `cubed-0.8.0/cubed/vendor/dask/blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/dask/core.py` & `cubed-0.8.0/cubed/vendor/dask/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/dask/utils.py` & `cubed-0.8.0/cubed/vendor/dask/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/rechunker/algorithm.py` & `cubed-0.8.0/cubed/vendor/rechunker/algorithm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/rechunker/api.py` & `cubed-0.8.0/cubed/vendor/rechunker/api.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/rechunker/executors/python.py` & `cubed-0.8.0/cubed/vendor/rechunker/executors/python.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed/vendor/rechunker/types.py` & `cubed-0.8.0/cubed/vendor/rechunker/types.py`

 * *Files identical despite different names*

### Comparing `cubed-0.7.0/cubed.egg-info/PKG-INFO` & `cubed-0.8.0/cubed.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed
-Version: 0.7.0
+Version: 0.8.0
 Summary: Bounded-memory serverless distributed N-dimensional array processing
 Author-email: Tom White <tom.e.white@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/tomwhite/cubed
 Project-URL: documentation, https://tomwhite.github.io/cubed
 Project-URL: repository, https://github.com/tomwhite/cubed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cubed-0.7.0/cubed.egg-info/SOURCES.txt` & `cubed-0.8.0/cubed.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 cubed/runtime/executors/__init__.py
 cubed/runtime/executors/beam.py
 cubed/runtime/executors/lithops.py
 cubed/runtime/executors/modal.py
 cubed/runtime/executors/modal_async.py
 cubed/runtime/executors/python.py
 cubed/runtime/executors/python_async.py
+cubed/storage/__init__.py
+cubed/storage/zarr.py
 cubed/tests/__init__.py
 cubed/tests/test_array_api.py
 cubed/tests/test_core.py
 cubed/tests/test_gufunc.py
 cubed/tests/test_indexing.py
 cubed/tests/test_mem_utilization.py
 cubed/tests/test_optimization.py
@@ -62,14 +64,18 @@
 cubed/tests/primitive/__init__.py
 cubed/tests/primitive/test_blockwise.py
 cubed/tests/primitive/test_rechunk.py
 cubed/tests/runtime/__init__.py
 cubed/tests/runtime/test_backup.py
 cubed/tests/runtime/test_lithops.py
 cubed/tests/runtime/test_modal_async.py
+cubed/tests/runtime/test_python_async.py
+cubed/tests/runtime/utils.py
+cubed/tests/storage/__init__.py
+cubed/tests/storage/test_zarr.py
 cubed/vendor/__init__.py
 cubed/vendor/dask/__init__.py
 cubed/vendor/dask/blockwise.py
 cubed/vendor/dask/core.py
 cubed/vendor/dask/utils.py
 cubed/vendor/dask/array/__init__.py
 cubed/vendor/dask/array/core.py
```

### Comparing `cubed-0.7.0/pyproject.toml` & `cubed-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cubed"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
     {name = "Tom White", email = "tom.e.white@gmail.com"},
 ]
 license = {text = "Apache License 2.0"}
 description = "Bounded-memory serverless distributed N-dimensional array processing"
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
@@ -32,15 +32,17 @@
 ]
 
 [project.optional-dependencies]
 diagnostics = [
     "tqdm",
     "graphviz",
     "pydot",
-    "pandas"
+    "pandas",
+    "matplotlib",
+    "seaborn",
 ]
 beam = ["apache-beam", "gcsfs"]
 lithops = ["lithops[aws] >= 2.7.0"]
 modal = [
     "cubed[diagnostics]",
     "modal-client",
     "s3fs",
```

### Comparing `cubed-0.7.0/setup.cfg` & `cubed-0.8.0/setup.cfg`

 * *Files identical despite different names*

