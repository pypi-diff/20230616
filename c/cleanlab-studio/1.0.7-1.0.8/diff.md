# Comparing `tmp/cleanlab-studio-1.0.7.tar.gz` & `tmp/cleanlab-studio-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.0.7.tar", last modified: Mon Jun 12 18:54:34 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.0.8.tar", last modified: Fri Jun 16 08:44:38 2023, max compression
```

## Comparing `cleanlab-studio-1.0.7.tar` & `cleanlab-studio-1.0.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/studio/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.648363 cleanlab-studio-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-06-16 08:44:38.644363 cleanlab-studio-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.628363 cleanlab-studio-1.0.8/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.632363 cleanlab-studio-1.0.8/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.632363 cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.632363 cleanlab-studio-1.0.8/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.636363 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.636363 cleanlab-studio-1.0.8/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.636363 cleanlab-studio-1.0.8/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.640363 cleanlab-studio-1.0.8/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.640363 cleanlab-studio-1.0.8/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.640363 cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.644363 cleanlab-studio-1.0.8/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/studio/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.628363 cleanlab-studio-1.0.8/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-06-16 08:44:38.000000 cleanlab-studio-1.0.8/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-16 08:44:38.000000 cleanlab-studio-1.0.8/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:44:38.000000 cleanlab-studio-1.0.8/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-16 08:44:38.000000 cleanlab-studio-1.0.8/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 08:44:38.000000 cleanlab-studio-1.0.8/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 08:44:38.000000 cleanlab-studio-1.0.8/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:44:38.648363 cleanlab-studio-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.644363 cleanlab-studio-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:38.644363 cleanlab-studio-1.0.8/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-16 08:44:22.000000 cleanlab-studio-1.0.8/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.7/LICENSE` & `cleanlab-studio-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/PKG-INFO` & `cleanlab-studio-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.7
+Version: 1.0.8
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
```

### Comparing `cleanlab-studio-1.0.7/README.md` & `cleanlab-studio-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/api_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,16 @@
     res = requests.get(
         cli_base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     cleanset_json: str = res.json()["cleanset_json"]
     cleanset_df: pd.DataFrame = pd.read_json(cleanset_json, orient="table")
+    id_col = get_id_column(api_key, cleanset_id)
+    cleanset_df.rename(columns={"id": id_col}, inplace=True)
     return cleanset_df
 
 
 def get_completion_status(api_key: str, dataset_id: str) -> bool:
     res = requests.get(
         cli_base_url + f"/datasets/{dataset_id}/complete",
         headers=_construct_headers(api_key),
```

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.0.8/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/errors.py` & `cleanlab-studio-1.0.8/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.0.8/cleanlab_studio/internal/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,16 @@
     res = requests.get(
         cli_base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     cleanset_json: str = res.json()["cleanset_json"]
     cleanset_df: pd.DataFrame = pd.read_json(cleanset_json, orient="table")
+    id_col = get_id_column(api_key, cleanset_id)
+    cleanset_df.rename(columns={"id": id_col}, inplace=True)
     return cleanset_df
 
 
 def get_id_column(api_key: str, cleanset_id: str) -> str:
     res = requests.get(
         cli_base_url + f"/cleansets/{cleanset_id}/id_column",
         headers=_construct_headers(api_key),
```

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.0.8/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.0.8/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.0.8/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.0.8/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/studio/clean.py` & `cleanlab-studio-1.0.8/cleanlab_studio/studio/clean.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.0.8/cleanlab_studio/studio/studio.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio/studio/upload.py` & `cleanlab-studio-1.0.8/cleanlab_studio/studio/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.0.8/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.7
+Version: 1.0.8
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
```

### Comparing `cleanlab-studio-1.0.7/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.0.8/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/setup.py` & `cleanlab-studio-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.0.8/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.0.8/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.0.8/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.7/tests/datasets/utils.py` & `cleanlab-studio-1.0.8/tests/datasets/utils.py`

 * *Files identical despite different names*

