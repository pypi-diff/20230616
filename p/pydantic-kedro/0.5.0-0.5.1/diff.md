# Comparing `tmp/pydantic-kedro-0.5.0.tar.gz` & `tmp/pydantic-kedro-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-kedro-0.5.0.tar", last modified: Thu Jun  1 20:15:27 2023, max compression
+gzip compressed data, was "pydantic-kedro-0.5.1.tar", last modified: Fri Jun 16 11:22:54 2023, max compression
```

## Comparing `pydantic-kedro-0.5.0.tar` & `pydantic-kedro-0.5.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/arbitrary_types.md
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/standalone_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.915988 pydantic-kedro-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/src/pydantic_kedro/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/_dict_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/_internals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:14:38.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/src/test/catalogs/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/catalogs/conf/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/conf/base/catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/catalogs/conf/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/conf/local/credentials.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/catalogs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/data/tst1.json
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/test_basic_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_docs_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_ds_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_ds_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_ds_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_nested_subtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.251469 pydantic-kedro-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.243468 pydantic-kedro-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.243468 pydantic-kedro-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-16 11:22:54.251469 pydantic-kedro-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.243468 pydantic-kedro-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/docs/arbitrary_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/docs/standalone_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:22:54.251469 pydantic-kedro-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.239468 pydantic-kedro-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.247469 pydantic-kedro-0.5.1/src/pydantic_kedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/_dict_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/_internals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.247469 pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/pydantic_kedro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.247469 pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-16 11:22:54.000000 pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-16 11:22:54.000000 pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:22:54.000000 pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:21:59.000000 pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-16 11:22:54.000000 pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 11:22:54.000000 pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.247469 pydantic-kedro-0.5.1/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.247469 pydantic-kedro-0.5.1/src/test/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.243468 pydantic-kedro-0.5.1/src/test/catalogs/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.247469 pydantic-kedro-0.5.1/src/test/catalogs/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/catalogs/conf/base/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.247469 pydantic-kedro-0.5.1/src/test/catalogs/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/catalogs/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/catalogs/conf/local/credentials.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:22:54.247469 pydantic-kedro-0.5.1/src/test/catalogs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/catalogs/data/tst1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/catalogs/test_basic_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_docs_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_ds_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_ds_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_ds_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_nested_subtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_strict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-16 11:21:46.000000 pydantic-kedro-0.5.1/src/test/test_utils.py
```

### Comparing `pydantic-kedro-0.5.0/.github/dependabot.yml` & `pydantic-kedro-0.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/.github/workflows/python-publish.yml` & `pydantic-kedro-0.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/.github/workflows/python-testing.yml` & `pydantic-kedro-0.5.1/.github/workflows/python-testing.yml`

 * *Files 0% similar despite different names*

```diff
@@ -38,9 +38,9 @@
       - name: Test with pytest
         run: |
           pytest
       - name: Test with mypy
         run: |
           mypy
       - name: Check Markdown (Optional)
-        uses: DavidAnson/markdownlint-cli2-action@v10
+        uses: DavidAnson/markdownlint-cli2-action@v11
         continue-on-error: true
```

### Comparing `pydantic-kedro-0.5.0/.pre-commit-config.yaml` & `pydantic-kedro-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/LICENSE` & `pydantic-kedro-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/PKG-INFO` & `pydantic-kedro-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.5.0
+Version: 0.5.1
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.5.0/README.md` & `pydantic-kedro-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/docs/arbitrary_types.md` & `pydantic-kedro-0.5.1/docs/arbitrary_types.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/docs/implementation_details.md` & `pydantic-kedro-0.5.1/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/docs/index.md` & `pydantic-kedro-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/docs/standalone_usage.md` & `pydantic-kedro-0.5.1/docs/standalone_usage.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/mkdocs.yml` & `pydantic-kedro-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/pyproject.toml` & `pydantic-kedro-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 ]
 urls = { github = "https://github.com/NowanIlfideme/pydantic-kedro" }
 
 [project.optional-dependencies]
 dev = [
     "setuptools>=61.0.0",
     "setuptools-scm[toml]>=6.2",
-    "pre-commit==3.3.2",
+    "pre-commit==3.3.3",
     "black==23.3.0",
     "isort==5.12.0",
-    "ruff==0.0.270",
+    "ruff==0.0.272",
     "mypy==1.3.0",
-    "pytest==7.3.1",
+    "pytest==7.3.2",
     # required for testing
     "kedro[pandas]",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]",
```

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/__init__.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/_dict_io.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/_dict_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,16 @@
         if _classlike(value):
             raw[key] = dict_to_model(value)
         elif isinstance(value, list):
             raw[key] = _list_manip(value)
         elif isinstance(value, dict):
             raw[key] = _dict_manip(value)
         # otherwise ignore
-    return pyd_kls(**raw)  # Consider parse_obj_as(pyd_kls, raw) ?
+    keywords = dict(raw)
+    del keywords[KLS_MARK_STR]
+    return pyd_kls(**keywords)  # Consider parse_obj_as(pyd_kls, keywords) ?
 
 
 def model_to_dict(model: BaseModel) -> Dict[str, Any]:
     """Conver model to dictionary."""
     with PatchPydanticIter():
         return model.dict()
```

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/_internals.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/_internals.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/auto.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/auto.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/folder.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/json.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/yaml.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/yaml.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/zip.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/datasets/zip.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/models.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/models.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro/utils.py` & `pydantic-kedro-0.5.1/src/pydantic_kedro/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/PKG-INFO` & `pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.5.0
+Version: 0.5.1
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/SOURCES.txt` & `pydantic-kedro-0.5.1/src/pydantic_kedro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,13 +39,14 @@
 src/test/test_docs_standalone.py
 src/test/test_ds_extended.py
 src/test/test_ds_pandas.py
 src/test/test_ds_simple.py
 src/test/test_import.py
 src/test/test_inheritance.py
 src/test/test_nested_subtypes.py
+src/test/test_strict.py
 src/test/test_utils.py
 src/test/catalogs/test_basic_catalog.py
 src/test/catalogs/conf/base/catalog.yml
 src/test/catalogs/conf/local/.gitkeep
 src/test/catalogs/conf/local/credentials.yml
 src/test/catalogs/data/tst1.json
```

### Comparing `pydantic-kedro-0.5.0/src/test/catalogs/test_basic_catalog.py` & `pydantic-kedro-0.5.1/src/test/catalogs/test_basic_catalog.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/test/test_auto.py` & `pydantic-kedro-0.5.1/src/test/test_auto.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/test/test_docs_standalone.py` & `pydantic-kedro-0.5.1/src/test/test_docs_standalone.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/test/test_ds_extended.py` & `pydantic-kedro-0.5.1/src/test/test_ds_extended.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/test/test_ds_pandas.py` & `pydantic-kedro-0.5.1/src/test/test_ds_pandas.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/test/test_ds_simple.py` & `pydantic-kedro-0.5.1/src/test/test_ds_simple.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/test/test_inheritance.py` & `pydantic-kedro-0.5.1/src/test/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.5.0/src/test/test_nested_subtypes.py` & `pydantic-kedro-0.5.1/src/test/test_nested_subtypes.py`

 * *Files identical despite different names*

