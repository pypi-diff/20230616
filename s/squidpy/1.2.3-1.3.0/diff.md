# Comparing `tmp/squidpy-1.2.3.tar.gz` & `tmp/squidpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squidpy-1.2.3.tar", last modified: Tue Oct 18 14:13:29 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `squidpy-1.2.3.tar` & `squidpy-1.3.0.tar`

### file list

```diff
@@ -1,114 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.110927 squidpy-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-10-18 14:13:14.000000 squidpy-1.2.3/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-10-18 14:13:14.000000 squidpy-1.2.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-10-18 14:13:14.000000 squidpy-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-10-18 14:13:14.000000 squidpy-1.2.3/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)     4104 2022-10-18 14:13:14.000000 squidpy-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-18 14:13:14.000000 squidpy-1.2.3/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-18 14:13:14.000000 squidpy-1.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9265 2022-10-18 14:13:14.000000 squidpy-1.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-10-18 14:13:14.000000 squidpy-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-18 14:13:14.000000 squidpy-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2022-10-18 14:13:29.110927 squidpy-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-10-18 14:13:14.000000 squidpy-1.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-10-18 14:13:14.000000 squidpy-1.2.3/README_pypi.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.102927 squidpy-1.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-18 14:13:14.000000 squidpy-1.2.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-10-18 14:13:14.000000 squidpy-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-10-18 14:13:14.000000 squidpy-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 14:13:29.110927 squidpy-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-10-18 14:13:14.000000 squidpy-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.102927 squidpy-1.2.3/squidpy/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.102927 squidpy-1.2.3/squidpy/_constants/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/_constants/_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6708 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/_constants/_pkg_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/_constants/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14069 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7401 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.102927 squidpy-1.2.3/squidpy/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     4485 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/datasets/_10x_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3485 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/datasets/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/datasets/_dataset.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/datasets/_image.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/datasets/_image.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5549 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/datasets/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.106927 squidpy-1.2.3/squidpy/gr/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/gr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12010 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/gr/_build.py
--rw-r--r--   0 runner    (1001) docker     (121)    31607 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/gr/_ligrec.py
--rw-r--r--   0 runner    (1001) docker     (121)    12508 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/gr/_nhood.py
--rw-r--r--   0 runner    (1001) docker     (121)    17146 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/gr/_ppatterns.py
--rw-r--r--   0 runner    (1001) docker     (121)     8850 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/gr/_ripley.py
--rw-r--r--   0 runner    (1001) docker     (121)    10651 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/gr/_sepal.py
--rw-r--r--   0 runner    (1001) docker     (121)     9929 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/gr/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.106927 squidpy-1.2.3/squidpy/im/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/im/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    59995 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/im/_container.py
--rw-r--r--   0 runner    (1001) docker     (121)     5776 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/im/_coords.py
--rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/im/_feature.py
--rw-r--r--   0 runner    (1001) docker     (121)    18629 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/im/_feature_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9689 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/im/_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     4993 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/im/_process.py
--rw-r--r--   0 runner    (1001) docker     (121)    12631 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/im/_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.106927 squidpy-1.2.3/squidpy/pl/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_color_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11558 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.106927 squidpy-1.2.3/squidpy/pl/_interactive/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11989 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_interactive/_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     5010 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_interactive/_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_interactive/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6828 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_interactive/_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_interactive/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_interactive/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)    15745 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_ligrec.py
--rw-r--r--   0 runner    (1001) docker     (121)    15944 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (121)    35914 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    21463 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/pl/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.106927 squidpy-1.2.3/squidpy/read/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10457 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/read/_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-10-18 14:13:14.000000 squidpy-1.2.3/squidpy/read/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.102927 squidpy-1.2.3/squidpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2022-10-18 14:13:29.000000 squidpy-1.2.3/squidpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-10-18 14:13:29.000000 squidpy-1.2.3/squidpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 14:13:29.000000 squidpy-1.2.3/squidpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 14:13:29.000000 squidpy-1.2.3/squidpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-10-18 14:13:29.000000 squidpy-1.2.3/squidpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-18 14:13:29.000000 squidpy-1.2.3/squidpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.106927 squidpy-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11147 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.106927 squidpy-1.2.3/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/datasets/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/datasets/test_download_visium_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.110927 squidpy-1.2.3/tests/graph/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18968 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/graph/test_ligrec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/graph/test_nhood.py
--rw-r--r--   0 runner    (1001) docker     (121)     5879 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/graph/test_ppatterns.py
--rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/graph/test_ripley.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/graph/test_sepal.py
--rw-r--r--   0 runner    (1001) docker     (121)     8369 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/graph/test_spatial_neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.110927 squidpy-1.2.3/tests/image/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    54805 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/image/test_container.py
--rw-r--r--   0 runner    (1001) docker     (121)    10536 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/image/test_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     5469 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/image/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     6674 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/image/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    10718 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/image/test_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.110927 squidpy-1.2.3/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8778 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/plotting/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/plotting/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/plotting/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     9459 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/plotting/test_spatial_static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:29.110927 squidpy-1.2.3/tests/read/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-10-18 14:13:14.000000 squidpy-1.2.3/tests/read/test_visium.py
--rw-r--r--   0 runner    (1001) docker     (121)     6545 2022-10-18 14:13:14.000000 squidpy-1.2.3/tox.ini
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 squidpy-1.3.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 squidpy-1.3.0/.editorconfig
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 squidpy-1.3.0/.gitmodules
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 squidpy-1.3.0/.mypy.ini
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 squidpy-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 squidpy-1.3.0/.prettierignore
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 squidpy-1.3.0/.readthedocs.yml
+-rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 squidpy-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 squidpy-1.3.0/MANIFEST.in
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 squidpy-1.3.0/README_pypi.rst
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 squidpy-1.3.0/tox.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/.codecov.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/workflows/deployment.yml
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 squidpy-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 squidpy-1.3.0/.scripts/ci/download_data.py
+-rwxr-xr-x   0        0        0      527 2020-02-02 00:00:00.000000 squidpy-1.3.0/.scripts/ci/install_dependencies.sh
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/Makefile
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/api.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/classes.rst
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/conf.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/index.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/installation.rst
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/make.bat
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/references.bib
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/references.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release_notes.rst
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/utils.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_ext/typed_returns.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_static/css/dataframe.css
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_static/css/nbsphinx.css
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_static/css/sphinx_gallery.css
+-rw-r--r--   0        0        0   911945 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_static/img/figure1.png
+-rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_static/img/squidpy_horizontal.png
+-rw-r--r--   0        0        0    20146 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_static/img/squidpy_vertical.png
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.0.0.rst
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.0.1.rst
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.1.0.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.1.1.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.1.2.rst
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.2.0.rst
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.2.1.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.2.2.rst
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.2.3.rst
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-1.3.0.rst
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 squidpy-1.3.0/docs/release/notes-dev.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/__init__.py
+-rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/_docs.py
+-rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/_constants/__init__.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/_constants/_constants.py
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/_constants/_pkg_constants.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/_constants/_utils.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/datasets/_10x_datasets.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/datasets/__init__.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/datasets/_dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/datasets/_dataset.pyi
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/datasets/_image.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/datasets/_image.pyi
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/datasets/_utils.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/gr/__init__.py
+-rw-r--r--   0        0        0    12577 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/gr/_build.py
+-rw-r--r--   0        0        0    31742 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/gr/_ligrec.py
+-rw-r--r--   0        0        0    12832 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/gr/_nhood.py
+-rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/gr/_ppatterns.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/gr/_ripley.py
+-rw-r--r--   0        0        0    10860 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/gr/_sepal.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/gr/_utils.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/im/__init__.py
+-rw-r--r--   0        0        0    60101 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/im/_container.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/im/_coords.py
+-rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/im/_feature.py
+-rw-r--r--   0        0        0    18628 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/im/_feature_mixin.py
+-rw-r--r--   0        0        0     9682 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/im/_io.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/im/_process.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/im/_segment.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/__init__.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_color_utils.py
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_graph.py
+-rw-r--r--   0        0        0    15942 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_ligrec.py
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_spatial.py
+-rw-r--r--   0        0        0    36090 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_spatial_utils.py
+-rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_utils.py
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_var_by_distance.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_interactive/__init__.py
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_interactive/_controller.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_interactive/_model.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_interactive/_utils.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_interactive/_view.py
+-rw-r--r--   0        0        0    12146 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_interactive/_widgets.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/pl/_interactive/interactive.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/read/__init__.py
+-rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/read/_read.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/read/_utils.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/tl/__init__.py
+-rw-r--r--   0        0        0    10864 2020-02-02 00:00:00.000000 squidpy-1.3.0/src/squidpy/tl/_var_by_distance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0    35962 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/filtered_feature_bc_matrix.h5
+-rw-r--r--   0        0        0    11678 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/ligrec_no_numba.pickle
+-rw-r--r--   0        0        0   106788 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/paul15_means.pickle
+-rw-r--r--   0        0        0   602117 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/test_data.h5ad
+-rw-r--r--   0        0        0   229870 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/test_img.jpg
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/spatial/scalefactors_json.json
+-rw-r--r--   0        0        0    20014 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/spatial/tissue_hires_image.png
+-rw-r--r--   0        0        0   518124 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/spatial/tissue_lowres_image.png
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_data/spatial/tissue_positions_list.csv
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_axis.png
+-rw-r--r--   0        0        0    95400 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_channel.png
+-rw-r--r--   0        0        0    91924 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_channelwise.png
+-rw-r--r--   0        0        0   129565 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_channelwise_segmentation.png
+-rw-r--r--   0        0        0   122974 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_imshow_kwargs.png
+-rw-r--r--   0        0        0   119898 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_library_id.png
+-rw-r--r--   0        0        0    51525 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_scale_mask_circle_crop.png
+-rw-r--r--   0        0        0   140839 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_segmentation.png
+-rw-r--r--   0        0        0    67164 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_transpose_channelwise_False_False.png
+-rw-r--r--   0        0        0   180591 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_transpose_channelwise_False_True.png
+-rw-r--r--   0        0        0   236892 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_transpose_channelwise_True_False.png
+-rw-r--r--   0        0        0    76745 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/ContainerShow_transpose_channelwise_True_True.png
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_centrality_scores.png
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_centrality_scores_single.png
+-rw-r--r--   0        0        0    31775 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_co_occurrence.png
+-rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_co_occurrence_palette.png
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_interaction.png
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_interaction_dendro.png
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_nhood_enrichment.png
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_nhood_enrichment_ax.png
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_nhood_enrichment_dendro.png
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_ripley_f.png
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_ripley_f_nopalette.png
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_ripley_g.png
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Graph_ripley_l.png
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Heatmap_cbar_kwargs.png
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Heatmap_cbar_vmin_vmax.png
+-rw-r--r--   0        0        0    19521 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_alpha.png
+-rw-r--r--   0        0        0    18044 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_alpha_none.png
+-rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_cmap.png
+-rw-r--r--   0        0        0    19252 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_dendrogram_both.png
+-rw-r--r--   0        0        0    20981 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_dendrogram_clusters.png
+-rw-r--r--   0        0        0    20530 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_dendrogram_pairs.png
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_kwargs.png
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_means_range.png
+-rw-r--r--   0        0        0    29501 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_no_remove_empty_interactions.png
+-rw-r--r--   0        0        0    14454 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_pvalue_threshold.png
+-rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_remove_empty_interactions.png
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_remove_nonsig_interactions.png
+-rw-r--r--   0        0        0    10701 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_source_clusters.png
+-rw-r--r--   0        0        0    20234 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_swap_axes.png
+-rw-r--r--   0        0        0    21101 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_swap_axes_dedrogram.png
+-rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Ligrec_target_clusters.png
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_add_image.png
+-rw-r--r--   0        0        0    21995 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_blending.png
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_cat_cmap.png
+-rw-r--r--   0        0        0    21738 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_cont_cmap.png
+-rw-r--r--   0        0        0     9231 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_-200_-200_600_800.png
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_-200_-200_800_600.png
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_-200_-200_800_800.png
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_-200_200_600_800.png
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_-200_200_800_600.png
+-rw-r--r--   0        0        0    15960 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_-200_200_800_800.png
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_200_-200_600_800.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_200_-200_800_600.png
+-rw-r--r--   0        0        0    16043 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_200_-200_800_800.png
+-rw-r--r--   0        0        0    17445 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_200_200_600_800.png
+-rw-r--r--   0        0        0    16287 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_200_200_800_600.png
+-rw-r--r--   0        0        0    21234 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_corner_case_200_200_800_800.png
+-rw-r--r--   0        0        0    28180 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_crop_center.png
+-rw-r--r--   0        0        0    17228 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_crop_corner.png
+-rw-r--r--   0        0        0    21848 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_gene_X.png
+-rw-r--r--   0        0        0    22045 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_obs_categorical.png
+-rw-r--r--   0        0        0    21794 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_obs_continuous.png
+-rw-r--r--   0        0        0    25425 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_scalefactor.png
+-rw-r--r--   0        0        0    20173 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_simple_canvas.png
+-rw-r--r--   0        0        0    18340 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_symbol.png
+-rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/Napari_viewer_canvas.png
+-rw-r--r--   0        0        0    51439 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_palette_listed_cmap.png
+-rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_axfig.png
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_categorical_alpha.png
+-rw-r--r--   0        0        0    93592 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_crop.png
+-rw-r--r--   0        0        0    41672 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_crop_graph.png
+-rw-r--r--   0        0        0   118281 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_crop_noorigin.png
+-rw-r--r--   0        0        0   142407 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_group.png
+-rw-r--r--   0        0        0    51931 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_group_multi.png
+-rw-r--r--   0        0        0    25974 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_group_outline.png
+-rw-r--r--   0        0        0    57879 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_image.png
+-rw-r--r--   0        0        0    22237 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_noimage.png
+-rw-r--r--   0        0        0    51647 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_non_unique_colors.png
+-rw-r--r--   0        0        0    35072 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_nospatial.png
+-rw-r--r--   0        0        0    64688 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_novisium.png
+-rw-r--r--   0        0        0    48845 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_scatter_title_single.png
+-rw-r--r--   0        0        0   114278 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_segment.png
+-rw-r--r--   0        0        0   247009 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_segment_crop.png
+-rw-r--r--   0        0        0    82158 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/SpatialStatic_spatial_segment_group.png
+-rw-r--r--   0        0        0    31379 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/var_by_distance_single_anchor_and_gene.png
+-rw-r--r--   0        0        0    20962 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/var_by_distance_single_anchor_and_gene_two_categories.png
+-rw-r--r--   0        0        0   104786 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/var_by_distance_single_anchor_four_genes_two_categories_two_palettes.png
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/_images/var_by_distance_single_anchor_one_gene_two_categories_without_scatter.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/datasets/test_dataset.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/datasets/test_download_visium_dataset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/graph/__init__.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/graph/test_ligrec.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/graph/test_nhood.py
+-rw-r--r--   0        0        0     6969 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/graph/test_ppatterns.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/graph/test_ripley.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/graph/test_sepal.py
+-rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/graph/test_spatial_neighbors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/image/__init__.py
+-rw-r--r--   0        0        0    55061 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/image/test_container.py
+-rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/image/test_features.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/image/test_io.py
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/image/test_processing.py
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/image/test_segmentation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/plotting/__init__.py
+-rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/plotting/test_graph.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/plotting/test_image.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/plotting/test_interactive.py
+-rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/plotting/test_spatial_static.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/plotting/test_var_by_distance_plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/read/__init__.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/read/test_visium.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/tools/__init__.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 squidpy-1.3.0/tests/tools/test_var_by_distance.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 squidpy-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 squidpy-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 squidpy-1.3.0/README.rst
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 squidpy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 squidpy-1.3.0/PKG-INFO
```

### Comparing `squidpy-1.2.3/.gitignore` & `squidpy-1.3.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -71,18 +71,17 @@
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
-docs/_build/
-docs/source/auto_examples
-docs/source/auto_tutorials
-docs/source/gen_modules
+docs/build/
+docs/api
+docs/classes
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `squidpy-1.2.3/.mypy.ini` & `squidpy-1.3.0/.mypy.ini`

 * *Files 12% similar despite different names*

```diff
@@ -24,12 +24,11 @@
 no_implicit_reexport = True
 no_warn_no_return = True
 
 show_error_codes = True
 show_column_numbers = True
 error_summary = True
 
-[mypy-tests.*]
-ignore_errors = True
+no_namespace_packages = True
 
-[mypy-docs.*]
+[mypy-tests.*]
 ignore_errors = True
```

### Comparing `squidpy-1.2.3/CONTRIBUTING.rst` & `squidpy-1.3.0/CONTRIBUTING.rst`

 * *Files 14% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
 - create the new release notes
 - bump the version and create a new tag
 - run tests on the ``release/vX.X.X`` branch
 - publish on PyPI after all the tests have passed
 - merge ``release/vX.X.X`` into ``main``
 
-Alternatively, it's possible to create a new release using ``bump2version``, which can be installed as::
+It is possible to create a new release using ``bump2version``, which can be installed as::
 
     pip install bump2version
 
 Depending on what part of the version you want to update, you can run on ``main``::
 
     bump2version {major,minor,patch}
 
@@ -173,49 +173,15 @@
     git push --atomic <branch> <tag>
 
 or set ``push.followtags=true`` in your git config and do a regular ``git push``. In this case, CI will not
 create any release notes, run tests or do any merges.
 
 Creating release notes
 ----------------------
-By default, news fragments are automatically generated from successfully merged PRs using. Everything under
-``## Description`` section will be rendered as ``.rst`` files and automatically committed in the target branch in
-`docs/source/release/changelog <docs/source/release/changelog>`_.
-When a new release happens, ``towncrier`` gathers all news fragments and creates the release notes under
-`docs/source/release <docs/source/release>`_.
-
-When submitting a PR, it should be tagged with one of the following tags, in order for ``towncrier`` to know under
-which section to render the news:
-
-- bugfix: the PR fixes some bug
-- feature: the PR introduces a new feature
-- deprecation: the PR deprecates something (e.g. a function)
-- doc: the PR is related to documentation
-- misc: the PR is not applicable to the above
-
-If no label (or ``ignore-towncrier`` label) is specified, no news will be generated for the PR.
-If more than 1 is specified, the first one is used.
-
-To manually create news fragment, make sure that the PR doesn't generate it from the description as described above.
-The command to run is ``towncrier <PR_NUMBER>.<LABEL>``, where ``<LABEL>`` is one of the labels described above.
-This will create a new file in the appropriate location that needs to me modified and subsequently committed.
-
-To locally create the news fragment from an already existing PR, just run::
-
-    tox -e news -- <PR_NUMBER> --add-author
-
-You can modify the created fragment, then commit and run::
-
-    tox -e update-dev-notes
-
-In order to inject the fragment in the release note.
-
-Lastly, in order to see how the current news fragments would look like in the release notes, run::
-
-    towncrier build --draft
+Please take a look at the other release notes for formatting style. We are exploring other options for automatic release notes generation.
 
 Troubleshooting
 ---------------
 - **The enchant C library was not found**
   This can happen during the documentation build and because of a missing dependency for spell checker.
   The installation instructions for the dependency can be found
   `here <https://pyenchant.github.io/pyenchant/install.html#installing-the-enchant-c-library>`_.
```

### Comparing `squidpy-1.2.3/LICENSE` & `squidpy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squidpy-1.2.3/README.rst` & `squidpy-1.3.0/README_pypi.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,234 +1,184 @@
 00000000: 7c50 7950 497c 207c 446f 776e 6c6f 6164  |PyPI| |Download
-00000010: 737c 207c 4349 7c20 7c4e 6f74 6562 6f6f  s| |CI| |Noteboo
-00000020: 6b73 7c20 7c44 6f63 737c 207c 436f 7665  ks| |Docs| |Cove
-00000030: 7261 6765 7c20 7c44 6973 636f 7572 7365  rage| |Discourse
-00000040: 7c20 7c5a 756c 6970 7c0a 0a53 7175 6964  | |Zulip|..Squid
-00000050: 7079 202d 2053 7061 7469 616c 2053 696e  py - Spatial Sin
-00000060: 676c 6520 4365 6c6c 2041 6e61 6c79 7369  gle Cell Analysi
-00000070: 7320 696e 2050 7974 686f 6e0a 3d3d 3d3d  s in Python.====
+00000010: 737c 207c 4349 7c20 7c44 6f63 737c 207c  s| |CI| |Docs| |
+00000020: 436f 7665 7261 6765 7c20 7c44 6973 636f  Coverage| |Disco
+00000030: 7572 7365 7c20 7c5a 756c 6970 7c0a 0a53  urse| |Zulip|..S
+00000040: 7175 6964 7079 202d 2053 7061 7469 616c  quidpy - Spatial
+00000050: 2053 696e 676c 6520 4365 6c6c 2041 6e61   Single Cell Ana
+00000060: 6c79 7369 7320 696e 2050 7974 686f 6e0a  lysis in Python.
+00000070: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000000a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2e2e  ============....
-000000b0: 2072 6177 3a3a 2068 746d 6c0a 0a20 2020   raw:: html..   
-000000c0: 203c 7020 616c 6967 6e3d 2263 656e 7465   <p align="cente
-000000d0: 7222 3e0a 2020 2020 2020 2020 3c61 2068  r">.        <a h
-000000e0: 7265 663d 2268 7474 7073 3a2f 2f73 7175  ref="https://squ
-000000f0: 6964 7079 2e72 6561 6474 6865 646f 6373  idpy.readthedocs
-00000100: 2e69 6f2f 656e 2f73 7461 626c 652f 223e  .io/en/stable/">
-00000110: 0a20 2020 2020 2020 2020 2020 203c 696d  .            <im
-00000120: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00000130: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000140: 7465 6e74 2e63 6f6d 2f73 6376 6572 7365  tent.com/scverse
-00000150: 2f73 7175 6964 7079 2f6d 6169 6e2f 646f  /squidpy/main/do
-00000160: 6373 2f73 6f75 7263 652f 5f73 7461 7469  cs/source/_stati
-00000170: 632f 696d 672f 7371 7569 6470 795f 686f  c/img/squidpy_ho
-00000180: 7269 7a6f 6e74 616c 2e70 6e67 220a 2020  rizontal.png".  
-00000190: 2020 2020 2020 2020 2020 2077 6964 7468             width
-000001a0: 3d22 3430 3070 7822 2061 6c74 3d22 5371  ="400px" alt="Sq
-000001b0: 7569 6470 7920 6c6f 676f 223e 0a20 2020  uidpy logo">.   
-000001c0: 2020 2020 203c 2f61 3e0a 2020 2020 3c2f       </a>.    </
-000001d0: 703e 0a0a 0a2a 2a53 7175 6964 7079 2a2a  p>...**Squidpy**
-000001e0: 2069 7320 6120 746f 6f6c 2066 6f72 2074   is a tool for t
-000001f0: 6865 2061 6e61 6c79 7369 7320 616e 6420  he analysis and 
-00000200: 7669 7375 616c 697a 6174 696f 6e20 6f66  visualization of
-00000210: 2073 7061 7469 616c 206d 6f6c 6563 756c   spatial molecul
-00000220: 6172 2064 6174 612e 0a49 7420 6275 696c  ar data..It buil
-00000230: 6473 206f 6e20 746f 7020 6f66 2060 7363  ds on top of `sc
-00000240: 616e 7079 605f 2061 6e64 2060 616e 6e64  anpy`_ and `annd
-00000250: 6174 6160 5f2c 2066 726f 6d20 7768 6963  ata`_, from whic
-00000260: 6820 6974 2069 6e68 6572 6974 7320 6d6f  h it inherits mo
-00000270: 6475 6c61 7269 7479 2061 6e64 2073 6361  dularity and sca
-00000280: 6c61 6269 6c69 7479 2e0a 4974 2070 726f  lability..It pro
-00000290: 7669 6465 7320 616e 616c 7973 6973 2074  vides analysis t
-000002a0: 6f6f 6c73 2074 6861 7420 6c65 7665 7261  ools that levera
-000002b0: 6765 7320 7468 6520 7370 6174 6961 6c20  ges the spatial 
-000002c0: 636f 6f72 6469 6e61 7465 7320 6f66 2074  coordinates of t
-000002d0: 6865 2064 6174 612c 2061 7320 7765 6c6c  he data, as well
-000002e0: 2061 730a 7469 7373 7565 2069 6d61 6765   as.tissue image
-000002f0: 7320 6966 2061 7661 696c 6162 6c65 2e0a  s if available..
-00000300: 0a2e 2e20 7261 773a 3a20 6874 6d6c 0a0a  ... raw:: html..
-00000310: 2020 2020 3c70 2061 6c69 676e 3d22 6365      <p align="ce
-00000320: 6e74 6572 223e 0a20 2020 2020 2020 203c  nter">.        <
-00000330: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000340: 646f 692e 6f72 672f 3130 2e31 3033 382f  doi.org/10.1038/
-00000350: 7334 3135 3932 2d30 3231 2d30 3133 3538  s41592-021-01358
-00000360: 2d32 223e 0a20 2020 2020 2020 2020 2020  -2">.           
-00000370: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000380: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00000390: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6376  rcontent.com/scv
-000003a0: 6572 7365 2f73 7175 6964 7079 2f6d 6169  erse/squidpy/mai
-000003b0: 6e2f 646f 6373 2f73 6f75 7263 652f 5f73  n/docs/source/_s
-000003c0: 7461 7469 632f 696d 672f 6669 6775 7265  tatic/img/figure
-000003d0: 312e 706e 6722 0a20 2020 2020 2020 2020  1.png".         
-000003e0: 2020 2020 7769 6474 683d 2234 3030 7078      width="400px
-000003f0: 2220 616c 743d 2253 7175 6964 7079 2074  " alt="Squidpy t
-00000400: 6974 6c65 2066 6967 7572 6522 3e0a 2020  itle figure">.  
-00000410: 2020 2020 2020 3c2f 613e 0a20 2020 203c        </a>.    <
-00000420: 2f70 3e0a 0a56 6973 6974 206f 7572 2060  /p>..Visit our `
-00000430: 646f 6375 6d65 6e74 6174 696f 6e60 5f20  documentation`_ 
-00000440: 666f 7220 696e 7374 616c 6c61 7469 6f6e  for installation
-00000450: 2c20 7475 746f 7269 616c 732c 2065 7861  , tutorials, exa
-00000460: 6d70 6c65 7320 616e 6420 6d6f 7265 2e0a  mples and more..
-00000470: 0a4d 616e 7573 6372 6970 740a 2d2d 2d2d  .Manuscript.----
-00000480: 2d2d 2d2d 2d2d 0a50 6c65 6173 6520 7365  ------.Please se
-00000490: 6520 6f75 7220 6d61 6e75 7363 7269 7074  e our manuscript
-000004a0: 2060 5061 6c6c 612c 2053 7069 747a 6572   `Palla, Spitzer
-000004b0: 2065 7420 616c 2e20 2832 3032 3229 605f   et al. (2022)`_
-000004c0: 2069 6e20 2a2a 4e61 7475 7265 204d 6574   in **Nature Met
-000004d0: 686f 6473 2a2a 2074 6f20 6c65 6172 6e20  hods** to learn 
-000004e0: 6d6f 7265 2e0a 0a53 7175 6964 7079 2773  more...Squidpy's
-000004f0: 206b 6579 2061 7070 6c69 6361 7469 6f6e   key application
-00000500: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s.--------------
-00000510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a2d 2042  ------------.- B
-00000520: 7569 6c64 2061 6e64 2061 6e61 6c79 7a65  uild and analyze
-00000530: 2074 6865 206e 6569 6768 626f 7268 6f6f   the neighborhoo
-00000540: 6420 6772 6170 6820 6672 6f6d 2073 7061  d graph from spa
-00000550: 7469 616c 2063 6f6f 7264 696e 6174 6573  tial coordinates
-00000560: 2e0a 2d20 436f 6d70 7574 6520 7370 6174  ..- Compute spat
-00000570: 6961 6c20 7374 6174 6973 7469 6373 2066  ial statistics f
-00000580: 6f72 2063 656c 6c2d 7479 7065 7320 616e  or cell-types an
-00000590: 6420 6765 6e65 732e 0a2d 2045 6666 6963  d genes..- Effic
-000005a0: 6965 6e74 6c79 2073 746f 7265 2c20 616e  iently store, an
-000005b0: 616c 797a 6520 616e 6420 7669 7375 616c  alyze and visual
-000005c0: 697a 6520 6c61 7267 6520 7469 7373 7565  ize large tissue
-000005d0: 2069 6d61 6765 732c 206c 6576 6572 6167   images, leverag
-000005e0: 696e 6720 6073 6b69 6d61 6765 605f 2e0a  ing `skimage`_..
-000005f0: 2d20 496e 7465 7261 6374 6976 656c 7920  - Interactively 
-00000600: 6578 706c 6f72 6520 6061 6e6e 6461 7461  explore `anndata
-00000610: 605f 2061 6e64 206c 6172 6765 2074 6973  `_ and large tis
-00000620: 7375 6520 696d 6167 6573 2069 6e20 606e  sue images in `n
-00000630: 6170 6172 6960 5f2e 0a0a 496e 7374 616c  apari`_...Instal
-00000640: 6c61 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d  lation.---------
-00000650: 2d2d 2d0a 496e 7374 616c 6c20 5371 7569  ---.Install Squi
-00000660: 6470 7920 7669 6120 5079 5049 2062 7920  dpy via PyPI by 
-00000670: 7275 6e6e 696e 673a 3a0a 0a20 2020 2070  running::..    p
-00000680: 6970 2069 6e73 7461 6c6c 2073 7175 6964  ip install squid
-00000690: 7079 0a20 2020 2023 206f 7220 7769 7468  py.    # or with
-000006a0: 206e 6170 6172 6920 696e 636c 7564 6564   napari included
-000006b0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
-000006c0: 2027 7371 7569 6470 795b 696e 7465 7261   'squidpy[intera
-000006d0: 6374 6976 655d 270a 0a6f 7220 7669 6120  ctive]'..or via 
-000006e0: 436f 6e64 6120 6173 3a3a 0a0a 2020 2020  Conda as::..    
-000006f0: 636f 6e64 6120 696e 7374 616c 6c20 2d63  conda install -c
-00000700: 2063 6f6e 6461 2d66 6f72 6765 2073 7175   conda-forge squ
-00000710: 6964 7079 0a0a 436f 6e74 7269 6275 7469  idpy..Contributi
-00000720: 6e67 2074 6f20 5371 7569 6470 790a 2d2d  ng to Squidpy.--
-00000730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000740: 2d2d 2d2d 2d0a 5765 2061 7265 2068 6170  -----.We are hap
-00000750: 7079 2061 626f 7574 2061 6e79 2063 6f6e  py about any con
-00000760: 7472 6962 7574 696f 6e73 2120 4265 666f  tributions! Befo
-00000770: 7265 2079 6f75 2073 7461 7274 2c20 6368  re you start, ch
-00000780: 6563 6b20 6f75 7420 6f75 7220 6063 6f6e  eck out our `con
-00000790: 7472 6962 7574 696e 6720 6775 6964 6520  tributing guide 
-000007a0: 3c43 4f4e 5452 4942 5554 494e 472e 7273  <CONTRIBUTING.rs
-000007b0: 743e 605f 2e0a 0a2e 2e20 7c50 7950 497c  t>`_..... |PyPI|
-000007c0: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
-000007d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000007e0: 7079 7069 2f76 2f73 7175 6964 7079 2e73  pypi/v/squidpy.s
-000007f0: 7667 0a20 2020 203a 7461 7267 6574 3a20  vg.    :target: 
-00000800: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000810: 2f70 726f 6a65 6374 2f73 7175 6964 7079  /project/squidpy
-00000820: 2f0a 2020 2020 3a61 6c74 3a20 5079 5049  /.    :alt: PyPI
-00000830: 0a0a 2e2e 207c 4349 7c20 696d 6167 653a  .... |CI| image:
-00000840: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00000850: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000860: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
-00000870: 7363 7665 7273 652f 7371 7569 6470 792f  scverse/squidpy/
-00000880: 5465 7374 2f6d 6169 6e0a 2020 2020 3a74  Test/main.    :t
-00000890: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
-000008a0: 6974 6875 622e 636f 6d2f 7363 7665 7273  ithub.com/scvers
-000008b0: 652f 7371 7569 6470 792f 6163 7469 6f6e  e/squidpy/action
-000008c0: 730a 2020 2020 3a61 6c74 3a20 4349 0a0a  s.    :alt: CI..
-000008d0: 2e2e 207c 5072 652d 636f 6d6d 6974 7c20  .. |Pre-commit| 
-000008e0: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-000008f0: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
-00000900: 6974 2e63 692f 6261 6467 652f 6769 7468  it.ci/badge/gith
-00000910: 7562 2f73 6376 6572 7365 2f73 7175 6964  ub/scverse/squid
-00000920: 7079 2f6d 6169 6e2e 7376 670a 2020 203a  py/main.svg.   :
-00000930: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-00000940: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
-00000950: 6974 2e63 692f 6c61 7465 7374 2f67 6974  it.ci/latest/git
-00000960: 6875 622f 7363 7665 7273 652f 7371 7569  hub/scverse/squi
-00000970: 6470 792f 6d61 696e 0a20 2020 3a61 6c74  dpy/main.   :alt
-00000980: 3a20 7072 652d 636f 6d6d 6974 2e63 6920  : pre-commit.ci 
-00000990: 7374 6174 7573 0a0a 2e2e 207c 4e6f 7465  status.... |Note
-000009a0: 626f 6f6b 737c 2069 6d61 6765 3a3a 2068  books| image:: h
-000009b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000009c0: 6473 2e69 6f2f 6769 7468 7562 2f77 6f72  ds.io/github/wor
-000009d0: 6b66 6c6f 772f 7374 6174 7573 2f73 6376  kflow/status/scv
-000009e0: 6572 7365 2f73 7175 6964 7079 5f6e 6f74  erse/squidpy_not
-000009f0: 6562 6f6f 6b73 2f43 492f 6d61 696e 3f6c  ebooks/CI/main?l
-00000a00: 6162 656c 3d6e 6f74 6562 6f6f 6b73 0a20  abel=notebooks. 
-00000a10: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
-00000a20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000a30: 6376 6572 7365 2f73 7175 6964 7079 5f6e  cverse/squidpy_n
-00000a40: 6f74 6562 6f6f 6b73 2f61 6374 696f 6e73  otebooks/actions
-00000a50: 0a20 2020 203a 616c 743a 204e 6f74 6562  .    :alt: Noteb
-00000a60: 6f6f 6b73 2043 490a 0a2e 2e20 7c44 6f63  ooks CI.... |Doc
-00000a70: 737c 2069 6d61 6765 3a3a 2068 7474 7073  s| image:: https
-00000a80: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000a90: 6f2f 7265 6164 7468 6564 6f63 732f 7371  o/readthedocs/sq
-00000aa0: 7569 6470 790a 2020 2020 3a74 6172 6765  uidpy.    :targe
-00000ab0: 743a 2068 7474 7073 3a2f 2f73 7175 6964  t: https://squid
-00000ac0: 7079 2e72 6561 6474 6865 646f 6373 2e69  py.readthedocs.i
-00000ad0: 6f2f 656e 2f73 7461 626c 652f 0a20 2020  o/en/stable/.   
-00000ae0: 203a 616c 743a 2044 6f63 756d 656e 7461   :alt: Documenta
-00000af0: 7469 6f6e 0a0a 2e2e 207c 436f 7665 7261  tion.... |Covera
-00000b00: 6765 7c20 696d 6167 653a 3a20 6874 7470  ge| image:: http
-00000b10: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-00000b20: 682f 7363 7665 7273 652f 7371 7569 6470  h/scverse/squidp
-00000b30: 792f 6272 616e 6368 2f6d 6169 6e2f 6772  y/branch/main/gr
-00000b40: 6170 682f 6261 6467 652e 7376 670a 2020  aph/badge.svg.  
-00000b50: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
-00000b60: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000b70: 2f73 6376 6572 7365 2f73 7175 6964 7079  /scverse/squidpy
-00000b80: 0a20 2020 203a 616c 743a 2043 6f76 6572  .    :alt: Cover
-00000b90: 6167 650a 0a2e 2e20 7c44 6f77 6e6c 6f61  age.... |Downloa
-00000ba0: 6473 7c20 696d 6167 653a 3a20 6874 7470  ds| image:: http
-00000bb0: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
-00000bc0: 6467 652f 7371 7569 6470 790a 2020 2020  dge/squidpy.    
-00000bd0: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
-00000be0: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
-00000bf0: 6374 2f73 7175 6964 7079 0a20 2020 203a  ct/squidpy.    :
-00000c00: 616c 743a 2044 6f77 6e6c 6f61 6473 0a0a  alt: Downloads..
-00000c10: 2e2e 207c 4469 7363 6f75 7273 657c 2069  .. |Discourse| i
-00000c20: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
-00000c30: 6d67 2e73 6869 656c 6473 2e69 6f2f 6469  mg.shields.io/di
-00000c40: 7363 6f75 7273 652f 706f 7374 733f 636f  scourse/posts?co
-00000c50: 6c6f 723d 7965 6c6c 6f77 266c 6f67 6f3d  lor=yellow&logo=
-00000c60: 6469 7363 6f75 7273 6526 7365 7276 6572  discourse&server
-00000c70: 3d68 7474 7073 2533 4125 3246 2532 4664  =https%3A%2F%2Fd
-00000c80: 6973 636f 7572 7365 2e73 6376 6572 7365  iscourse.scverse
-00000c90: 2e6f 7267 0a20 2020 203a 7461 7267 6574  .org.    :target
-00000ca0: 3a20 6874 7470 733a 2f2f 6469 7363 6f75  : https://discou
-00000cb0: 7273 652e 7363 7665 7273 652e 6f72 672f  rse.scverse.org/
-00000cc0: 0a20 2020 203a 616c 743a 2044 6973 636f  .    :alt: Disco
-00000cd0: 7572 7365 0a0a 2e2e 207c 5a75 6c69 707c  urse.... |Zulip|
-00000ce0: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
-00000cf0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000d00: 6261 6467 652f 7a75 6c69 702d 6a6f 696e  badge/zulip-join
-00000d10: 5f63 6861 742d 2532 3336 3762 3038 662e  _chat-%2367b08f.
-00000d20: 7376 670a 2020 2020 3a74 6172 6765 743a  svg.    :target:
-00000d30: 2068 7474 7073 3a2f 2f73 6376 6572 7365   https://scverse
-00000d40: 2e7a 756c 6970 6368 6174 2e63 6f6d 0a20  .zulipchat.com. 
-00000d50: 2020 203a 616c 743a 205a 756c 6970 0a0a     :alt: Zulip..
-00000d60: 2e2e 205f 5061 6c6c 612c 2053 7069 747a  .. _Palla, Spitz
-00000d70: 6572 2065 7420 616c 2e20 2832 3032 3229  er et al. (2022)
-00000d80: 3a20 6874 7470 733a 2f2f 646f 692e 6f72  : https://doi.or
-00000d90: 672f 3130 2e31 3033 382f 7334 3135 3932  g/10.1038/s41592
-00000da0: 2d30 3231 2d30 3133 3538 2d32 0a2e 2e20  -021-01358-2... 
-00000db0: 5f73 6361 6e70 793a 2068 7474 7073 3a2f  _scanpy: https:/
-00000dc0: 2f73 6361 6e70 792e 7265 6164 7468 6564  /scanpy.readthed
-00000dd0: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-00000de0: 2f0a 2e2e 205f 616e 6e64 6174 613a 2068  /... _anndata: h
-00000df0: 7474 7073 3a2f 2f61 6e6e 6461 7461 2e72  ttps://anndata.r
-00000e00: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000e10: 2f73 7461 626c 652f 0a2e 2e20 5f6e 6170  /stable/... _nap
-00000e20: 6172 693a 2068 7474 7073 3a2f 2f6e 6170  ari: https://nap
-00000e30: 6172 692e 6f72 672f 0a2e 2e20 5f73 6b69  ari.org/... _ski
-00000e40: 6d61 6765 3a20 6874 7470 733a 2f2f 7363  mage: https://sc
-00000e50: 696b 6974 2d69 6d61 6765 2e6f 7267 2f0a  ikit-image.org/.
-00000e60: 2e2e 205f 646f 6375 6d65 6e74 6174 696f  .. _documentatio
-00000e70: 6e3a 2068 7474 7073 3a2f 2f73 7175 6964  n: https://squid
-00000e80: 7079 2e72 6561 6474 6865 646f 6373 2e69  py.readthedocs.i
-00000e90: 6f2f 656e 2f73 7461 626c 652f 0a         o/en/stable/.
+000000a0: 0a0a 2a2a 5371 7569 6470 792a 2a20 6973  ..**Squidpy** is
+000000b0: 2061 2074 6f6f 6c20 666f 7220 7468 6520   a tool for the 
+000000c0: 616e 616c 7973 6973 2061 6e64 2076 6973  analysis and vis
+000000d0: 7561 6c69 7a61 7469 6f6e 206f 6620 7370  ualization of sp
+000000e0: 6174 6961 6c20 6d6f 6c65 6375 6c61 7220  atial molecular 
+000000f0: 6461 7461 2e0a 4974 2062 7569 6c64 7320  data..It builds 
+00000100: 6f6e 2074 6f70 206f 6620 6073 6361 6e70  on top of `scanp
+00000110: 7960 5f20 616e 6420 6061 6e6e 6461 7461  y`_ and `anndata
+00000120: 605f 2c20 6672 6f6d 2077 6869 6368 2069  `_, from which i
+00000130: 7420 696e 6865 7269 7473 206d 6f64 756c  t inherits modul
+00000140: 6172 6974 7920 616e 6420 7363 616c 6162  arity and scalab
+00000150: 696c 6974 792e 0a49 7420 7072 6f76 6964  ility..It provid
+00000160: 6573 2061 6e61 6c79 7369 7320 746f 6f6c  es analysis tool
+00000170: 7320 7468 6174 206c 6576 6572 6167 6573  s that leverages
+00000180: 2074 6865 2073 7061 7469 616c 2063 6f6f   the spatial coo
+00000190: 7264 696e 6174 6573 206f 6620 7468 6520  rdinates of the 
+000001a0: 6461 7461 2c20 6173 2077 656c 6c20 6173  data, as well as
+000001b0: 0a74 6973 7375 6520 696d 6167 6573 2069  .tissue images i
+000001c0: 6620 6176 6169 6c61 626c 652e 0a0a 5669  f available...Vi
+000001d0: 7369 7420 6f75 7220 6064 6f63 756d 656e  sit our `documen
+000001e0: 7461 7469 6f6e 605f 2066 6f72 2069 6e73  tation`_ for ins
+000001f0: 7461 6c6c 6174 696f 6e2c 2074 7574 6f72  tallation, tutor
+00000200: 6961 6c73 2c20 6578 616d 706c 6573 2061  ials, examples a
+00000210: 6e64 206d 6f72 652e 0a0a 4d61 6e75 7363  nd more...Manusc
+00000220: 7269 7074 0a2d 2d2d 2d2d 2d2d 2d2d 2d0a  ript.----------.
+00000230: 506c 6561 7365 2073 6565 206f 7572 206d  Please see our m
+00000240: 616e 7573 6372 6970 7420 6050 616c 6c61  anuscript `Palla
+00000250: 2c20 5370 6974 7a65 7220 6574 2061 6c2e  , Spitzer et al.
+00000260: 2028 3230 3232 2960 5f20 696e 202a 2a4e   (2022)`_ in **N
+00000270: 6174 7572 6520 4d65 7468 6f64 732a 2a20  ature Methods** 
+00000280: 746f 206c 6561 726e 206d 6f72 652e 0a0a  to learn more...
+00000290: 5371 7569 6470 7927 7320 6b65 7920 6170  Squidpy's key ap
+000002a0: 706c 6963 6174 696f 6e73 0a2d 2d2d 2d2d  plications.-----
+000002b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000002c0: 2d2d 2d2d 2d0a 2d20 4275 696c 6420 616e  -----.- Build an
+000002d0: 6420 616e 616c 797a 6520 7468 6520 6e65  d analyze the ne
+000002e0: 6967 6862 6f72 686f 6f64 2067 7261 7068  ighborhood graph
+000002f0: 2066 726f 6d20 7370 6174 6961 6c20 636f   from spatial co
+00000300: 6f72 6469 6e61 7465 732e 0a2d 2043 6f6d  ordinates..- Com
+00000310: 7075 7465 2073 7061 7469 616c 2073 7461  pute spatial sta
+00000320: 7469 7374 6963 7320 666f 7220 6365 6c6c  tistics for cell
+00000330: 2d74 7970 6573 2061 6e64 2067 656e 6573  -types and genes
+00000340: 2e0a 2d20 4566 6669 6369 656e 746c 7920  ..- Efficiently 
+00000350: 7374 6f72 652c 2061 6e61 6c79 7a65 2061  store, analyze a
+00000360: 6e64 2076 6973 7561 6c69 7a65 206c 6172  nd visualize lar
+00000370: 6765 2074 6973 7375 6520 696d 6167 6573  ge tissue images
+00000380: 2c20 6c65 7665 7261 6769 6e67 2060 736b  , leveraging `sk
+00000390: 696d 6167 6560 5f2e 0a2d 2049 6e74 6572  image`_..- Inter
+000003a0: 6163 7469 7665 6c79 2065 7870 6c6f 7265  actively explore
+000003b0: 2060 616e 6e64 6174 6160 5f20 616e 6420   `anndata`_ and 
+000003c0: 6c61 7267 6520 7469 7373 7565 2069 6d61  large tissue ima
+000003d0: 6765 7320 696e 2060 6e61 7061 7269 605f  ges in `napari`_
+000003e0: 2e0a 0a49 6e73 7461 6c6c 6174 696f 6e0a  ...Installation.
+000003f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a49 6e73  ------------.Ins
+00000400: 7461 6c6c 2053 7175 6964 7079 2076 6961  tall Squidpy via
+00000410: 2050 7950 4920 6279 2072 756e 6e69 6e67   PyPI by running
+00000420: 3a3a 0a0a 2020 2020 7069 7020 696e 7374  ::..    pip inst
+00000430: 616c 6c20 7371 7569 6470 790a 2020 2020  all squidpy.    
+00000440: 2320 6f72 2077 6974 6820 6e61 7061 7269  # or with napari
+00000450: 2069 6e63 6c75 6465 640a 2020 2020 7069   included.    pi
+00000460: 7020 696e 7374 616c 6c20 2773 7175 6964  p install 'squid
+00000470: 7079 5b69 6e74 6572 6163 7469 7665 5d27  py[interactive]'
+00000480: 0a0a 6f72 2076 6961 2043 6f6e 6461 2061  ..or via Conda a
+00000490: 733a 3a0a 0a20 2020 2063 6f6e 6461 2069  s::..    conda i
+000004a0: 6e73 7461 6c6c 202d 6320 636f 6e64 612d  nstall -c conda-
+000004b0: 666f 7267 6520 7371 7569 6470 790a 0a43  forge squidpy..C
+000004c0: 6f6e 7472 6962 7574 696e 6720 746f 2053  ontributing to S
+000004d0: 7175 6964 7079 0a2d 2d2d 2d2d 2d2d 2d2d  quidpy.---------
+000004e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a57  --------------.W
+000004f0: 6520 6172 6520 6861 7070 7920 6162 6f75  e are happy abou
+00000500: 7420 616e 7920 636f 6e74 7269 6275 7469  t any contributi
+00000510: 6f6e 7321 2042 6566 6f72 6520 796f 7520  ons! Before you 
+00000520: 7374 6172 742c 2063 6865 636b 206f 7574  start, check out
+00000530: 206f 7572 2060 636f 6e74 7269 6275 7469   our `contributi
+00000540: 6e67 2067 7569 6465 203c 434f 4e54 5249  ng guide <CONTRI
+00000550: 4255 5449 4e47 2e72 7374 3e60 5f2e 0a0a  BUTING.rst>`_...
+00000560: 2e2e 207c 5079 5049 7c20 696d 6167 653a  .. |PyPI| image:
+00000570: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
+00000580: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000590: 7371 7569 6470 792e 7376 670a 2020 2020  squidpy.svg.    
+000005a0: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
+000005b0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000005c0: 742f 7371 7569 6470 792f 0a20 2020 203a  t/squidpy/.    :
+000005d0: 616c 743a 2050 7950 490a 0a2e 2e20 7c43  alt: PyPI.... |C
+000005e0: 497c 2069 6d61 6765 3a3a 2068 7474 7073  I| image:: https
+000005f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000600: 6f2f 6769 7468 7562 2f77 6f72 6b66 6c6f  o/github/workflo
+00000610: 772f 7374 6174 7573 2f73 6376 6572 7365  w/status/scverse
+00000620: 2f73 7175 6964 7079 2f54 6573 742f 6d61  /squidpy/Test/ma
+00000630: 696e 0a20 2020 203a 7461 7267 6574 3a20  in.    :target: 
+00000640: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000650: 6f6d 2f73 6376 6572 7365 2f73 7175 6964  om/scverse/squid
+00000660: 7079 2f61 6374 696f 6e73 0a20 2020 203a  py/actions.    :
+00000670: 616c 743a 2043 490a 0a2e 2e20 7c50 7265  alt: CI.... |Pre
+00000680: 2d63 6f6d 6d69 747c 2069 6d61 6765 3a3a  -commit| image::
+00000690: 2068 7474 7073 3a2f 2f72 6573 756c 7473   https://results
+000006a0: 2e70 7265 2d63 6f6d 6d69 742e 6369 2f62  .pre-commit.ci/b
+000006b0: 6164 6765 2f67 6974 6875 622f 7363 7665  adge/github/scve
+000006c0: 7273 652f 7371 7569 6470 792f 6d61 696e  rse/squidpy/main
+000006d0: 2e73 7667 0a20 2020 3a74 6172 6765 743a  .svg.   :target:
+000006e0: 2068 7474 7073 3a2f 2f72 6573 756c 7473   https://results
+000006f0: 2e70 7265 2d63 6f6d 6d69 742e 6369 2f6c  .pre-commit.ci/l
+00000700: 6174 6573 742f 6769 7468 7562 2f73 6376  atest/github/scv
+00000710: 6572 7365 2f73 7175 6964 7079 2f6d 6169  erse/squidpy/mai
+00000720: 6e0a 2020 203a 616c 743a 2070 7265 2d63  n.   :alt: pre-c
+00000730: 6f6d 6d69 742e 6369 2073 7461 7475 730a  ommit.ci status.
+00000740: 0a2e 2e20 7c44 6f63 737c 2069 6d61 6765  ... |Docs| image
+00000750: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
+00000760: 6869 656c 6473 2e69 6f2f 7265 6164 7468  hields.io/readth
+00000770: 6564 6f63 732f 7371 7569 6470 790a 2020  edocs/squidpy.  
+00000780: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+00000790: 3a2f 2f73 7175 6964 7079 2e72 6561 6474  ://squidpy.readt
+000007a0: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+000007b0: 626c 652f 0a20 2020 203a 616c 743a 2044  ble/.    :alt: D
+000007c0: 6f63 756d 656e 7461 7469 6f6e 0a0a 2e2e  ocumentation....
+000007d0: 207c 436f 7665 7261 6765 7c20 696d 6167   |Coverage| imag
+000007e0: 653a 3a20 6874 7470 733a 2f2f 636f 6465  e:: https://code
+000007f0: 636f 762e 696f 2f67 682f 7363 7665 7273  cov.io/gh/scvers
+00000800: 652f 7371 7569 6470 792f 6272 616e 6368  e/squidpy/branch
+00000810: 2f6d 6169 6e2f 6772 6170 682f 6261 6467  /main/graph/badg
+00000820: 652e 7376 670a 2020 2020 3a74 6172 6765  e.svg.    :targe
+00000830: 743a 2068 7474 7073 3a2f 2f63 6f64 6563  t: https://codec
+00000840: 6f76 2e69 6f2f 6768 2f73 6376 6572 7365  ov.io/gh/scverse
+00000850: 2f73 7175 6964 7079 0a20 2020 203a 616c  /squidpy.    :al
+00000860: 743a 2043 6f76 6572 6167 650a 0a2e 2e20  t: Coverage.... 
+00000870: 7c44 6f77 6e6c 6f61 6473 7c20 696d 6167  |Downloads| imag
+00000880: 653a 3a20 6874 7470 733a 2f2f 7065 7079  e:: https://pepy
+00000890: 2e74 6563 682f 6261 6467 652f 7371 7569  .tech/badge/squi
+000008a0: 6470 790a 2020 2020 3a74 6172 6765 743a  dpy.    :target:
+000008b0: 2068 7474 7073 3a2f 2f70 6570 792e 7465   https://pepy.te
+000008c0: 6368 2f70 726f 6a65 6374 2f73 7175 6964  ch/project/squid
+000008d0: 7079 0a20 2020 203a 616c 743a 2044 6f77  py.    :alt: Dow
+000008e0: 6e6c 6f61 6473 0a0a 2e2e 207c 4469 7363  nloads.... |Disc
+000008f0: 6f75 7273 657c 2069 6d61 6765 3a3a 2068  ourse| image:: h
+00000900: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000910: 6473 2e69 6f2f 6469 7363 6f75 7273 652f  ds.io/discourse/
+00000920: 706f 7374 733f 636f 6c6f 723d 7965 6c6c  posts?color=yell
+00000930: 6f77 266c 6f67 6f3d 6469 7363 6f75 7273  ow&logo=discours
+00000940: 6526 7365 7276 6572 3d68 7474 7073 2533  e&server=https%3
+00000950: 4125 3246 2532 4664 6973 636f 7572 7365  A%2F%2Fdiscourse
+00000960: 2e73 6376 6572 7365 2e6f 7267 0a20 2020  .scverse.org.   
+00000970: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
+00000980: 2f2f 6469 7363 6f75 7273 652e 7363 7665  //discourse.scve
+00000990: 7273 652e 6f72 672f 0a20 2020 203a 616c  rse.org/.    :al
+000009a0: 743a 2044 6973 636f 7572 7365 0a0a 2e2e  t: Discourse....
+000009b0: 207c 5a75 6c69 707c 2069 6d61 6765 3a3a   |Zulip| image::
+000009c0: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+000009d0: 656c 6473 2e69 6f2f 6261 6467 652f 7a75  elds.io/badge/zu
+000009e0: 6c69 702d 6a6f 696e 5f63 6861 742d 2532  lip-join_chat-%2
+000009f0: 3336 3762 3038 662e 7376 670a 2020 2020  367b08f.svg.    
+00000a00: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
+00000a10: 2f73 6376 6572 7365 2e7a 756c 6970 6368  /scverse.zulipch
+00000a20: 6174 2e63 6f6d 0a20 2020 203a 616c 743a  at.com.    :alt:
+00000a30: 205a 756c 6970 0a0a 2e2e 205f 5061 6c6c   Zulip.... _Pall
+00000a40: 612c 2053 7069 747a 6572 2065 7420 616c  a, Spitzer et al
+00000a50: 2e20 2832 3032 3229 3a20 6874 7470 733a  . (2022): https:
+00000a60: 2f2f 646f 692e 6f72 672f 3130 2e31 3033  //doi.org/10.103
+00000a70: 382f 7334 3135 3932 2d30 3231 2d30 3133  8/s41592-021-013
+00000a80: 3538 2d32 0a2e 2e20 5f73 6361 6e70 793a  58-2... _scanpy:
+00000a90: 2068 7474 7073 3a2f 2f73 6361 6e70 792e   https://scanpy.
+00000aa0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000ab0: 6e2f 7374 6162 6c65 2f0a 2e2e 205f 616e  n/stable/... _an
+00000ac0: 6e64 6174 613a 2068 7474 7073 3a2f 2f61  ndata: https://a
+00000ad0: 6e6e 6461 7461 2e72 6561 6474 6865 646f  nndata.readthedo
+00000ae0: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+00000af0: 0a2e 2e20 5f6e 6170 6172 693a 2068 7474  ... _napari: htt
+00000b00: 7073 3a2f 2f6e 6170 6172 692e 6f72 672f  ps://napari.org/
+00000b10: 0a2e 2e20 5f73 6b69 6d61 6765 3a20 6874  ... _skimage: ht
+00000b20: 7470 733a 2f2f 7363 696b 6974 2d69 6d61  tps://scikit-ima
+00000b30: 6765 2e6f 7267 2f0a 2e2e 205f 646f 6375  ge.org/... _docu
+00000b40: 6d65 6e74 6174 696f 6e3a 2068 7474 7073  mentation: https
+00000b50: 3a2f 2f73 7175 6964 7079 2e72 6561 6474  ://squidpy.readt
+00000b60: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+00000b70: 626c 652f 0a                             ble/.
```

### Comparing `squidpy-1.2.3/README_pypi.rst` & `squidpy-1.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-|PyPI| |Downloads| |CI| |Notebooks| |Docs| |Coverage| |Discourse| |Zulip|
+|PyPI| |Downloads| |CI| |Docs| |Coverage| |Discourse| |Zulip|
 
 Squidpy - Spatial Single Cell Analysis in Python
 ================================================
 
-.. image:: https://raw.githubusercontent.com/scverse/squidpy/main/docs/source/_static/img/squidpy_horizontal.png
-    :alt: Squidpy logo
-    :width: 400px
-    :align: center
-    :target: https://squidpy.readthedocs.io/en/stable/
-
 **Squidpy** is a tool for the analysis and visualization of spatial molecular data.
 It builds on top of `scanpy`_ and `anndata`_, from which it inherits modularity and scalability.
 It provides analysis tools that leverages the spatial coordinates of the data, as well as
 tissue images if available.
 
-.. image:: https://raw.githubusercontent.com/scverse/squidpy/main/docs/source/_static/img/figure1.png
-    :alt: Squidpy title figure
-    :width: 400px
-    :align: center
-    :target: https://doi.org/10.1038/s41592-021-01358-2
-
 Visit our `documentation`_ for installation, tutorials, examples and more.
 
 Manuscript
 ----------
 Please see our manuscript `Palla, Spitzer et al. (2022)`_ in **Nature Methods** to learn more.
 
 Squidpy's key applications
@@ -49,26 +37,22 @@
 -----------------------
 We are happy about any contributions! Before you start, check out our `contributing guide <CONTRIBUTING.rst>`_.
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/squidpy.svg
     :target: https://pypi.org/project/squidpy/
     :alt: PyPI
 
-.. |CI| image:: https://img.shields.io/github/workflow/status/scverse/squidpy/Test/main
+.. |CI| image:: https://img.shields.io/github/actions/workflow/status/scverse/squidpy/test.yml?branch=main
     :target: https://github.com/scverse/squidpy/actions
     :alt: CI
 
 .. |Pre-commit| image:: https://results.pre-commit.ci/badge/github/scverse/squidpy/main.svg
    :target: https://results.pre-commit.ci/latest/github/scverse/squidpy/main
    :alt: pre-commit.ci status
 
-.. |Notebooks| image:: https://img.shields.io/github/workflow/status/scverse/squidpy_notebooks/CI/main?label=notebooks
-    :target: https://github.com/scverse/squidpy_notebooks/actions
-    :alt: Notebooks CI
-
 .. |Docs| image:: https://img.shields.io/readthedocs/squidpy
     :target: https://squidpy.readthedocs.io/en/stable/
     :alt: Documentation
 
 .. |Coverage| image:: https://codecov.io/gh/scverse/squidpy/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/scverse/squidpy
     :alt: Coverage
```

### Comparing `squidpy-1.2.3/squidpy/_constants/_constants.py` & `squidpy-1.3.0/src/squidpy/_constants/_constants.py`

 * *Files identical despite different names*

### Comparing `squidpy-1.2.3/squidpy/_constants/_pkg_constants.py` & `squidpy-1.3.0/src/squidpy/_constants/_pkg_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Internal constants not exposed to the user."""
 from __future__ import annotations
 
-from typing import Any, Union, Mapping, Callable, Optional, Sequence
+from typing import Any, Callable, Mapping, Optional, Sequence, Union
 
 from anndata import AnnData
 
 from squidpy._constants._constants import Processing, SegmentationBackend
 
 _SEP = "_"
 
@@ -17,20 +17,20 @@
     def __get__(self, obj: Any, owner: Any) -> str:
         return self.f(owner)
 
 
 class Key:
     class img:
         @classmethod
-        def segment(cls, backend: Union[str, SegmentationBackend], layer_added: Optional[str] = None) -> str:
+        def segment(cls, backend: str | SegmentationBackend, layer_added: str | None = None) -> str:
             return f"segmented_{SegmentationBackend(backend).s}" if layer_added is None else layer_added
 
         @classmethod
         def process(
-            cls, method: Union[str, Processing, Callable[[Any], Any]], img_id: str, layer_added: Optional[str] = None
+            cls, method: str | Processing | Callable[[Any], Any], img_id: str, layer_added: str | None = None
         ) -> str:
             if layer_added is not None:
                 return layer_added
             if isinstance(method, Processing):
                 method = method.s
             elif callable(method):
                 method = getattr(method, "__name__", "custom")
@@ -87,19 +87,19 @@
             return "scalefactors"
 
         @cprop
         def size_key(cls) -> str:
             return "spot_diameter_fullres"
 
         @classmethod
-        def spatial_neighs(cls, value: Optional[str] = None) -> str:
+        def spatial_neighs(cls, value: str | None = None) -> str:
             return f"{Key.obsm.spatial}_neighbors" if value is None else f"{value}_neighbors"
 
         @classmethod
-        def ligrec(cls, cluster: str, value: Optional[str] = None) -> str:
+        def ligrec(cls, cluster: str, value: str | None = None) -> str:
             return f"{cluster}_ligrec" if value is None else value
 
         @classmethod
         def nhood_enrichment(cls, cluster: str) -> str:
             return f"{cluster}_nhood_enrichment"
 
         @classmethod
@@ -123,15 +123,15 @@
             return f"{cluster}_colors"
 
         @classmethod
         def spot_diameter(
             cls,
             adata: AnnData,
             spatial_key: str,
-            library_id: Optional[str] = None,
+            library_id: str | None = None,
             spot_diameter_key: str = "spot_diameter_fullres",
         ) -> float:
             try:
                 return float(adata.uns[spatial_key][library_id]["scalefactors"][spot_diameter_key])
             except KeyError:
                 raise KeyError(
                     f"Unable to get the spot diameter from "
@@ -170,15 +170,15 @@
 
         @classmethod
         def _sort_haystack(
             cls,
             adata: AnnData,
             spatial_key: str,
             library_id: Sequence[str] | str | None = None,
-            sub_key: Optional[str] = None,
+            sub_key: str | None = None,
         ) -> Sequence[str] | None:
             if spatial_key not in adata.uns:
                 raise KeyError(f"Spatial key {spatial_key!r} not found in `adata.uns`.")
             haystack = list(adata.uns[spatial_key])
             if library_id is not None:
                 if isinstance(library_id, str):
                     library_id = [library_id]
@@ -191,13 +191,13 @@
                             f"with following `library_id`: {library_id}."
                         )
                 return library_id
             return haystack
 
     class obsp:
         @classmethod
-        def spatial_dist(cls, value: Optional[str] = None) -> str:
+        def spatial_dist(cls, value: str | None = None) -> str:
             return f"{Key.obsm.spatial}_distances" if value is None else f"{value}_distances"
 
         @classmethod
-        def spatial_conn(cls, value: Optional[str] = None) -> str:
+        def spatial_conn(cls, value: str | None = None) -> str:
             return f"{Key.obsm.spatial}_connectivities" if value is None else f"{value}_connectivities"
```

### Comparing `squidpy-1.2.3/squidpy/_constants/_utils.py` & `squidpy-1.3.0/src/squidpy/_constants/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import annotations
+
 from abc import ABC, ABCMeta
 from enum import Enum, EnumMeta
-from typing import Any, Type, Tuple, Mapping, Callable
 from functools import wraps
+from typing import Any, Callable, Mapping, Tuple
 
 
-def _pretty_raise_enum(cls: Type["ModeEnum"], fun: Callable[..., Any]) -> Callable[..., Any]:
+def _pretty_raise_enum(cls: type[ModeEnum], fun: Callable[..., Any]) -> Callable[..., Any]:
     @wraps(fun)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         try:
             return fun(*args, **kwargs)
         except ValueError as e:
             _cls, value, *_ = args
             e.args = (cls._format(value),)
@@ -45,18 +47,18 @@
         return str(self.value)
 
 
 class ABCEnumMeta(EnumMeta, ABCMeta):
     """Metaclass which injects."""
 
     def __new__(  # noqa: D102
-        cls, clsname: str, bases: Tuple[EnumMeta, ...], namespace: Mapping[str, Any]
-    ) -> "ABCEnumMeta":
+        cls, clsname: str, bases: tuple[EnumMeta, ...], namespace: Mapping[str, Any]
+    ) -> ABCEnumMeta:
         res = super().__new__(cls, clsname, bases, namespace)  # type: ignore[arg-type]
-        res.__new__ = _pretty_raise_enum(res, res.__new__)  # type: ignore[assignment,arg-type]
+        res.__new__ = _pretty_raise_enum(res, res.__new__)  # type: ignore[method-assign,arg-type]
         return res
 
 
 # TODO(michalk8): subclass string; remove .s?
 class ModeEnum(ErrorFormatterABC, PrettyEnum, metaclass=ABCEnumMeta):
     """Enum which prints available values when invalid value has been passed."""
```

### Comparing `squidpy-1.2.3/squidpy/_docs.py` & `squidpy-1.3.0/src/squidpy/_docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
-from docrep import DocstringProcessor
-from typing import Any, Callable
 from textwrap import dedent
+from typing import Any, Callable
+
+from docrep import DocstringProcessor
 
 from squidpy._constants._pkg_constants import Key
 
 
 def inject_docs(**kwargs: Any) -> Callable[..., Any]:  # noqa: D103
     # taken from scanpy
     def decorator(obj: Any) -> Any:
```

### Comparing `squidpy-1.2.3/squidpy/_utils.py` & `squidpy-1.3.0/src/squidpy/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """Spatial tools general utility functions."""
 from __future__ import annotations
 
-import joblib as jl
-
+from contextlib import contextmanager
 from enum import Enum
+from multiprocessing import Manager, cpu_count
 from queue import Queue
-from typing import Union  # noqa: F401
-from typing import Any, Callable, Hashable, Iterable, Sequence, Generator, TYPE_CHECKING
 from threading import Thread
-from contextlib import contextmanager
-from multiprocessing import Manager, cpu_count
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generator,
+    Hashable,
+    Iterable,
+    Sequence,
+    Union,  # noqa: F401
+)
 
+import joblib as jl
 import numpy as np
 
 __all__ = ["singledispatchmethod", "Signal", "SigQueue", "NDArray", "NDArrayA"]
 
 
 try:
     from functools import singledispatchmethod
@@ -107,16 +114,16 @@
 
     Returns
     -------
     The result depending on ``callable``, ``extractor``.
     """
     if show_progress_bar:
         try:
-            from tqdm.auto import tqdm
             import ipywidgets  # noqa: F401
+            from tqdm.auto import tqdm
         except ImportError:
             try:
                 from tqdm.std import tqdm
             except ImportError:
                 tqdm = None
     else:
         tqdm = None
```

### Comparing `squidpy-1.2.3/squidpy/datasets/_10x_datasets.py` & `squidpy-1.3.0/src/squidpy/datasets/_10x_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Literal, NamedTuple
-from pathlib import Path
 import tarfile
+from pathlib import Path
+from typing import (
+    Literal,
+    NamedTuple,
+    Union,  # noqa: F401
+)
 
-from scanpy import _utils
 from anndata import AnnData
+from scanpy import _utils
 from scanpy._settings import settings
 
-from squidpy.datasets._utils import PathLike
 from squidpy._constants._constants import TenxVersions
+from squidpy.datasets._utils import PathLike
 
 __all__ = ["visium"]
 
 
 class VisiumFiles(NamedTuple):
     feature_matrix: str
     spatial_attrs: str
```

### Comparing `squidpy-1.2.3/squidpy/datasets/_dataset.py` & `squidpy-1.3.0/src/squidpy/datasets/_dataset.py`

 * *Files identical despite different names*

### Comparing `squidpy-1.2.3/squidpy/datasets/_image.py` & `squidpy-1.3.0/src/squidpy/datasets/_image.py`

 * *Files identical despite different names*

### Comparing `squidpy-1.2.3/squidpy/datasets/_utils.py` & `squidpy-1.3.0/src/squidpy/datasets/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
+import os
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Tuple, Union, Callable, Optional, Sequence
-from inspect import Parameter, signature, Signature
+from dataclasses import dataclass, field
+from inspect import Parameter, Signature, signature
 from pathlib import Path
-from dataclasses import field, dataclass
-import os
+from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union
 
-from scanpy import read, logging as logg
+import anndata
 from anndata import AnnData
+from scanpy import logging as logg
+from scanpy import read
 from scanpy._utils import check_presence_download
-import anndata
 
 PathLike = Union[os.PathLike, str]
 Function_t = Callable[..., Union[AnnData, Any]]
 
 
 @dataclass(frozen=True)
 class Metadata(ABC):
     """Base class handling metadata."""
 
     name: str
     url: str
 
     doc_header: Optional[str] = field(default=None, repr=False)
     path: Optional[PathLike] = field(default=None, repr=False)
-    shape: Optional[Tuple[int, int]] = field(default=None, repr=False)
+    shape: Optional[tuple[int, int]] = field(default=None, repr=False)
     library_id: Optional[Union[str, Sequence[str]]] = field(default=None, repr=False)
 
     _DOC_FMT = ""
 
     def __post_init__(self) -> None:
         if self.doc_header is None:
             object.__setattr__(self, "doc_header", f"Download `{self.name.title().replace('_', ' ')}` data.")
@@ -43,15 +44,15 @@
     def _download(self, fpath: PathLike, backup_url: str, **kwargs: Any) -> Any:
         pass
 
     @abstractmethod
     def _create_signature(self) -> Signature:
         pass
 
-    def _create_function(self, name: str, glob_ns: Dict[str, Any]) -> None:
+    def _create_function(self, name: str, glob_ns: dict[str, Any]) -> None:
         if name in globals():
             raise KeyError(f"Function name `{name}` is already present in `{sorted(globals().keys())}`.")
 
         sig = self._create_signature()
         globals()["NoneType"] = type(None)  # __post_init__ return annotation
         globals()[name] = self
 
@@ -144,16 +145,15 @@
     path
         Path where to save the .tiff image.
     kwargs
         Keyword arguments for :meth:`squidpy.im.ImageContainer.add_img`.
 
     Returns
     -------
-    :class:`squidpy.im.ImageContainer`
-        The image data."""
+    :class:`squidpy.im.ImageContainer` The image data."""
     # not the perfect annotation, but better than nothing
     _EXT = ".tiff"
 
     def _create_signature(self) -> Signature:
         return signature(lambda _: _).replace(
             parameters=[
                 Parameter("path", kind=Parameter.POSITIONAL_OR_KEYWORD, annotation=PathLike, default=None),
```

### Comparing `squidpy-1.2.3/squidpy/gr/_build.py` & `squidpy-1.3.0/src/squidpy/gr/_build.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 """Functions for building graphs from spatial coordinates."""
 from __future__ import annotations
 
-from typing import List, Tuple, Union, Iterable  # noqa: F401
+import warnings
 from functools import partial
 from itertools import chain
-import warnings
+from typing import Iterable, List, Tuple, Union  # noqa: F401
 
-from scanpy import logging as logg
+import numpy as np
 from anndata import AnnData
 from anndata.utils import make_index_unique
-
 from numba import njit
+from scanpy import logging as logg
 from scipy.sparse import (
-    spmatrix,
+    SparseEfficiencyWarning,
     block_diag,
     csr_matrix,
     isspmatrix_csr,
-    SparseEfficiencyWarning,
+    spmatrix,
 )
 from scipy.spatial import Delaunay
-from sklearn.neighbors import NearestNeighbors
 from sklearn.metrics.pairwise import cosine_similarity, euclidean_distances
-import numpy as np
+from sklearn.neighbors import NearestNeighbors
+from spatialdata import SpatialData
 
+from squidpy._constants._constants import CoordType, Transform
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d, inject_docs
 from squidpy._utils import NDArrayA
 from squidpy.gr._utils import (
-    _save_data,
+    _assert_categorical_obs,
     _assert_positive,
     _assert_spatial_basis,
-    _assert_categorical_obs,
+    _save_data,
 )
-from squidpy._constants._constants import CoordType, Transform
-from squidpy._constants._pkg_constants import Key
 
 __all__ = ["spatial_neighbors"]
 
 
 @d.dedent
 @inject_docs(t=Transform, c=CoordType)
 def spatial_neighbors(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     spatial_key: str = Key.obsm.spatial,
     library_key: str | None = None,
     coord_type: str | CoordType | None = None,
     n_neighs: int = 6,
     radius: float | tuple[float, float] | None = None,
     delaunay: bool = False,
     n_rings: int = 1,
+    percentile: float | None = None,
     transform: str | Transform | None = None,
     set_diag: bool = False,
     key_added: str = "spatial",
     copy: bool = False,
 ) -> tuple[csr_matrix, csr_matrix] | None:
     """
     Create a graph from spatial coordinates.
@@ -78,14 +79,16 @@
 
             - :class:`float` - compute the graph based on neighborhood radius.
             - :class:`tuple` - prune the final graph to only contain edges in interval `[min(radius), max(radius)]`.
     delaunay
         Whether to compute the graph from Delaunay triangulation. Only used when ``coord_type = {c.GENERIC.s!r}``.
     n_rings
         Number of rings of neighbors for grid data. Only used when ``coord_type = {c.GRID.s!r}``.
+    percentile
+        Percentile of the distances to use as threshold. Only used when ``coord_type = {c.GENERIC.s!r}``.
     transform
         Type of adjacency matrix transform. Valid options are:
 
             - `{t.SPECTRAL.s!r}` - spectral transformation of the adjacency matrix.
             - `{t.COSINE.s!r}` - cosine transformation of the adjacency matrix.
             - `{t.NONE.v}` - no transformation of the adjacency matrix.
     set_diag
@@ -100,14 +103,16 @@
 
     Otherwise, modifies the ``adata`` with the following keys:
 
         - :attr:`anndata.AnnData.obsp` ``['{{key_added}}_connectivities']`` - the spatial connectivities.
         - :attr:`anndata.AnnData.obsp` ``['{{key_added}}_distances']`` - the spatial distances.
         - :attr:`anndata.AnnData.uns`  ``['{{key_added}}']`` - :class:`dict` containing parameters.
     """
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     _assert_positive(n_rings, name="n_rings")
     _assert_positive(n_neighs, name="n_neighs")
     _assert_spatial_basis(adata, spatial_key)
 
     transform = Transform.NONE if transform is None else Transform(transform)
     if coord_type is None:
         if radius is not None:
@@ -135,19 +140,20 @@
         coord_type=coord_type,
         n_neighs=n_neighs,
         radius=radius,
         delaunay=delaunay,
         n_rings=n_rings,
         transform=transform,
         set_diag=set_diag,
+        percentile=percentile,
     )
 
     if library_key is not None:
-        mats: List[Tuple[spmatrix, spmatrix]] = []
-        ixs = []
+        mats: list[tuple[spmatrix, spmatrix]] = []
+        ixs = []  # type: ignore[var-annotated]
         for lib in libs:
             ixs.extend(np.where(adata.obs[library_key] == lib)[0])
             mats.append(_build_fun(adata[adata.obs[library_key] == lib]))
         ixs = np.argsort(ixs)  # type: ignore[assignment] # invert
         Adj = block_diag([m[0] for m in mats], format="csr")[ixs, :][:, ixs]
         Dst = block_diag([m[1] for m in mats], format="csr")[ixs, :][:, ixs]
     else:
@@ -177,14 +183,15 @@
     coord_type: str | CoordType | None = None,
     n_neighs: int = 6,
     radius: float | tuple[float, float] | None = None,
     delaunay: bool = False,
     n_rings: int = 1,
     transform: str | Transform | None = None,
     set_diag: bool = False,
+    percentile: float | None = None,
 ) -> tuple[csr_matrix, csr_matrix]:
     coords = adata.obsm[spatial_key]
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", SparseEfficiencyWarning)
         if coord_type == CoordType.GRID:
             Adj, Dst = _build_grid(coords, n_neighs=n_neighs, n_rings=n_rings, delaunay=delaunay, set_diag=set_diag)
         elif coord_type == CoordType.GENERIC:
@@ -199,14 +206,19 @@
         mask = (Dst.data < minn) | (Dst.data > maxx)
         a_diag = Adj.diagonal()
 
         Dst.data[mask] = 0.0
         Adj.data[mask] = 0.0
         Adj.setdiag(a_diag)
 
+    if percentile is not None and coord_type == CoordType.GENERIC:
+        threshold = np.percentile(Dst.data, percentile)
+        Adj[Dst > threshold] = 0.0
+        Dst[Dst > threshold] = 0.0
+
     Adj.eliminate_zeros()
     Dst.eliminate_zeros()
 
     # check transform
     if transform == Transform.SPECTRAL:
         Adj = _transform_a_spectral(Adj)
     elif transform == Transform.COSINE:
```

### Comparing `squidpy-1.2.3/squidpy/gr/_ligrec.py` & `squidpy-1.3.0/src/squidpy/gr/_ligrec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 """Permutation test function as described in CellPhoneDB 2.0."""
 from __future__ import annotations
 
 from abc import ABC
-from types import MappingProxyType
-from typing import (
-    Any,
-    Tuple,
-    Union,
-    Literal,
-    Mapping,
-    Iterable,
-    Sequence,
-    TYPE_CHECKING,
-)
+from collections import namedtuple
 from functools import partial
 from itertools import product
-from collections import namedtuple
+from types import MappingProxyType
+from typing import TYPE_CHECKING, Any, Iterable, Literal, Mapping, Sequence, Union
 
-from scanpy import logging as logg
+import numpy as np
+import pandas as pd
 from anndata import AnnData
-
 from numba import njit, prange  # noqa: F401
+from scanpy import logging as logg
 from scipy.sparse import csc_matrix
-import numpy as np
-import pandas as pd
+from spatialdata import SpatialData
 
+from squidpy._constants._constants import ComplexPolicy, CorrAxis
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d, inject_docs
-from squidpy._utils import Signal, NDArrayA, SigQueue, parallelize, _get_n_cores
+from squidpy._utils import NDArrayA, Signal, SigQueue, _get_n_cores, parallelize
 from squidpy.gr._utils import (
-    _save_data,
-    _genesymbols,
+    _assert_categorical_obs,
     _assert_positive,
-    _create_sparse_df,
     _check_tuple_needles,
-    _assert_categorical_obs,
+    _create_sparse_df,
+    _genesymbols,
+    _save_data,
 )
-from squidpy._constants._constants import CorrAxis, ComplexPolicy
-from squidpy._constants._pkg_constants import Key
 
 __all__ = ["ligrec", "PermutationTest"]
 
 StrSeq = Sequence[str]
-SeqTuple = Sequence[Tuple[str, str]]
-Interaction_t = Union[pd.DataFrame, Mapping[str, StrSeq], StrSeq, Tuple[StrSeq, StrSeq], SeqTuple]
-Cluster_t = Union[StrSeq, Tuple[StrSeq, StrSeq], SeqTuple]
+SeqTuple = Sequence[tuple[str, str]]
+Interaction_t = Union[pd.DataFrame, Mapping[str, StrSeq], StrSeq, tuple[StrSeq, StrSeq], SeqTuple]
+Cluster_t = Union[StrSeq, tuple[StrSeq, StrSeq], SeqTuple]
 
 SOURCE = "source"
 TARGET = "target"
 
 TempResult = namedtuple("TempResult", ["means", "pvalues"])
 
 _template = """
@@ -625,15 +616,15 @@
 
         _ = super().prepare(interactions, complex_policy=complex_policy)
         return self
 
 
 @d.dedent
 def ligrec(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     cluster_key: str,
     interactions: Interaction_t | None = None,
     complex_policy: Literal["min", "all"] = ComplexPolicy.MIN.v,
     threshold: float = 0.01,
     corr_method: str | None = None,
     corr_axis: Literal["interactions", "clusters"] = CorrAxis.CLUSTERS.v,
     use_raw: bool = True,
@@ -653,14 +644,16 @@
     gene_symbols
         Key in :attr:`anndata.AnnData.var` to use instead of :attr:`anndata.AnnData.var_names`.
 
     Returns
     -------
     %(ligrec_test_returns)s
     """  # noqa: D400
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     with _genesymbols(adata, key=gene_symbols, use_raw=use_raw, make_unique=False):
         return (  # type: ignore[no-any-return]
             PermutationTest(adata, use_raw=use_raw)
             .prepare(interactions, complex_policy=complex_policy, **kwargs)
             .test(
                 cluster_key=cluster_key,
                 threshold=threshold,
@@ -738,15 +731,15 @@
     mask = groups.apply(lambda c: ((c > 0).sum() / len(c)) >= threshold).values.T  # (n_genes, n_clusters)
     # (n_cells, n_genes)
     data = np.array(data[data.columns.difference(["clusters"])].values, dtype=np.float64, order="C")
     # all 3 should be C contiguous
 
     return parallelize(  # type: ignore[no-any-return]
         _analysis_helper,
-        np.arange(n_perms, dtype=np.int32),
+        np.arange(n_perms, dtype=np.int32).tolist(),
         n_jobs=n_jobs,
         unit="permutation",
         extractor=extractor,
         **kwargs,
     )(
         data,
         mean,
@@ -813,21 +806,21 @@
     n_cls = mean.shape[1]
     return_means = np.min(perms) == 0
 
     # ideally, these would be both sparse array, but there is no numba impl. (sparse.COO is read-only and very limited)
     # keep it f64, because we're setting NaN
     res = np.zeros((len(interactions), len(interaction_clusters)), dtype=np.float64)
     numba_parallel = (
-        (np.prod(res.shape) >= 2**20 or clustering.shape[0] >= 2**15) if numba_parallel is None else numba_parallel
+        (np.prod(res.shape) >= 2**20 or clustering.shape[0] >= 2**15) if numba_parallel is None else numba_parallel  # type: ignore[assignment]
     )
 
     fn_key = f"_test_{n_cls}_{int(return_means)}_{bool(numba_parallel)}"
     if fn_key not in globals():
         exec(
-            compile(_create_template(n_cls, return_means=return_means, parallel=numba_parallel), "", "exec"), globals()
+            compile(_create_template(n_cls, return_means=return_means, parallel=numba_parallel), "", "exec"), globals()  # type: ignore[arg-type]
         )
     _test = globals()[fn_key]
 
     if return_means:
         res_means: NDArrayA | None = np.zeros((len(interactions), len(interaction_clusters)), dtype=np.float64)
         test = partial(_test, res_means=res_means)
     else:
```

### Comparing `squidpy-1.2.3/squidpy/gr/_nhood.py` & `squidpy-1.3.0/src/squidpy/gr/_nhood.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """Functions for neighborhood enrichment analysis (permutation test, centralities measures etc.)."""
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Any, Callable, Iterable, Sequence
 from functools import partial
+from typing import (
+    Any,
+    Callable,
+    Iterable,
+    Sequence,
+    Union,  # noqa: F401
+)
 
-from scanpy import logging as logg
-from anndata import AnnData
-
-from numba import njit, prange  # noqa: F401
+import networkx as nx
+import numba.types as nt
 import numpy as np
 import pandas as pd
-import numba.types as nt
-
-import networkx as nx
+from anndata import AnnData
+from numba import njit, prange  # noqa: F401
+from scanpy import logging as logg
+from spatialdata import SpatialData
 
+from squidpy._constants._constants import Centrality
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d, inject_docs
-from squidpy._utils import Signal, NDArrayA, SigQueue, parallelize, _get_n_cores
+from squidpy._utils import NDArrayA, Signal, SigQueue, _get_n_cores, parallelize
 from squidpy.gr._utils import (
-    _save_data,
-    _assert_positive,
     _assert_categorical_obs,
     _assert_connectivity_key,
+    _assert_positive,
+    _save_data,
 )
-from squidpy._constants._constants import Centrality
-from squidpy._constants._pkg_constants import Key
 
 __all__ = ["nhood_enrichment", "centrality_scores", "interaction_matrix"]
 
 dt = nt.uint32  # data type aliases (both for numpy and numba should match)
 ndt = np.uint32
 _template = """
 @njit(dt[:, :](dt[:], dt[:], dt[:]), parallel={parallel}, fastmath=True)
@@ -114,15 +118,15 @@
 
     return globals()[fn_key]  # type: ignore[no-any-return]
 
 
 @d.get_sections(base="nhood_ench", sections=["Parameters"])
 @d.dedent
 def nhood_enrichment(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     cluster_key: str,
     connectivity_key: str | None = None,
     n_perms: int = 1000,
     numba_parallel: bool = False,
     seed: int | None = None,
     copy: bool = False,
     n_jobs: int | None = None,
@@ -148,14 +152,16 @@
     If ``copy = True``, returns a :class:`tuple` with the z-score and the enrichment count.
 
     Otherwise, modifies the ``adata`` with the following keys:
 
         - :attr:`anndata.AnnData.uns` ``['{cluster_key}_nhood_enrichment']['zscore']`` - the enrichment z-score.
         - :attr:`anndata.AnnData.uns` ``['{cluster_key}_nhood_enrichment']['count']`` - the enrichment count.
     """
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     connectivity_key = Key.obsp.spatial_conn(connectivity_key)
     _assert_categorical_obs(adata, cluster_key)
     _assert_connectivity_key(adata, connectivity_key)
     _assert_positive(n_perms, name="n_perms")
 
     adj = adata.obsp[connectivity_key]
     original_clust = adata.obs[cluster_key]
@@ -169,15 +175,15 @@
     count = _test(indices, indptr, int_clust)
 
     n_jobs = _get_n_cores(n_jobs)
     start = logg.info(f"Calculating neighborhood enrichment using `{n_jobs}` core(s)")
 
     perms = parallelize(
         _nhood_enrichment_helper,
-        collection=np.arange(n_perms),
+        collection=np.arange(n_perms).tolist(),
         extractor=np.vstack,
         n_jobs=n_jobs,
         backend=backend,
         show_progress_bar=show_progress_bar,
     )(callback=_test, indices=indices, indptr=indptr, int_clust=int_clust, n_cls=n_cls, seed=seed)
     zscore = (count - perms.mean(axis=0)) / perms.std(axis=0)
 
@@ -192,15 +198,15 @@
         time=start,
     )
 
 
 @d.dedent
 @inject_docs(c=Centrality)
 def centrality_scores(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     cluster_key: str,
     score: str | Iterable[str] | None = None,
     connectivity_key: str | None = None,
     copy: bool = False,
     n_jobs: int | None = None,
     backend: str = "loky",
     show_progress_bar: bool = False,
@@ -229,14 +235,16 @@
     Returns
     -------
     If ``copy = True``, returns a :class:`pandas.DataFrame`. Otherwise, modifies the ``adata`` with the following key:
 
         - :attr:`anndata.AnnData.uns` ``['{{cluster_key}}_centrality_scores']`` - the centrality scores,
           as mentioned above.
     """
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     connectivity_key = Key.obsp.spatial_conn(connectivity_key)
     _assert_categorical_obs(adata, cluster_key)
     _assert_connectivity_key(adata, connectivity_key)
 
     if isinstance(score, (str, Centrality)):
         centrality = [score]
     elif score is None:
@@ -280,15 +288,15 @@
     if copy:
         return df
     _save_data(adata, attr="uns", key=Key.uns.centrality_scores(cluster_key), data=df, time=start)
 
 
 @d.dedent
 def interaction_matrix(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     cluster_key: str,
     connectivity_key: str | None = None,
     normalized: bool = False,
     copy: bool = False,
     weights: bool = False,
 ) -> NDArrayA | None:
     """
@@ -309,14 +317,16 @@
     -------
     If ``copy = True``, returns the interaction matrix.
 
     Otherwise, modifies the ``adata`` with the following key:
 
         - :attr:`anndata.AnnData.uns` ``['{cluster_key}_interactions']`` - the interaction matrix.
     """
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     connectivity_key = Key.obsp.spatial_conn(connectivity_key)
     _assert_categorical_obs(adata, cluster_key)
     _assert_connectivity_key(adata, connectivity_key)
 
     cats = adata.obs[cluster_key]
     mask = ~pd.isnull(cats).values
     cats = cats.loc[mask]
@@ -325,15 +335,15 @@
 
     g = adata.obsp[connectivity_key]
     g = g[mask, :][:, mask]
     n_cats = len(cats.cat.categories)
 
     g_data = g.data if weights else np.broadcast_to(1, shape=len(g.data))
     dtype = int if pd.api.types.is_bool_dtype(g.dtype) or pd.api.types.is_integer_dtype(g.dtype) else float
-    output = np.zeros((n_cats, n_cats), dtype=dtype)
+    output = np.zeros((n_cats, n_cats), dtype=dtype)  # type: ignore[var-annotated]
 
     _interaction_matrix(g_data, g.indices, g.indptr, cats.cat.codes.to_numpy(), output)
 
     if normalized:
         output = output / output.sum(axis=1).reshape((-1, 1))
 
     if copy:
```

### Comparing `squidpy-1.2.3/squidpy/gr/_ppatterns.py` & `squidpy-1.3.0/src/squidpy/gr/_ppatterns.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,73 @@
 """Functions for point patterns spatial statistics."""
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Literal  # < 3.8
-from typing import Any, Dict, Iterable, Sequence, TYPE_CHECKING
 from itertools import chain
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Iterable,
+    Literal,  # < 3.8
+    Sequence,
+    Union,  # noqa: F401
+)
 
-from scanpy import logging as logg
+import numba.types as nt
+import numpy as np
+import pandas as pd
 from anndata import AnnData
+from numba import njit
+from numpy.random import default_rng
+from scanpy import logging as logg
 from scanpy.get import _get_obs_rep
 from scanpy.metrics._gearys_c import _gearys_c
 from scanpy.metrics._morans_i import _morans_i
-
-from numba import njit
 from scipy import stats
-from numpy.random import default_rng
 from scipy.sparse import spmatrix
 from sklearn.metrics import pairwise_distances
 from sklearn.preprocessing import normalize
+from spatialdata import SpatialData
 from statsmodels.stats.multitest import multipletests
-import numpy as np
-import pandas as pd
-import numba.types as nt
 
+from squidpy._constants._constants import SpatialAutocorr
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d, inject_docs
-from squidpy._utils import Signal, NDArrayA, SigQueue, parallelize, _get_n_cores
+from squidpy._utils import NDArrayA, Signal, SigQueue, _get_n_cores, parallelize
 from squidpy.gr._utils import (
-    _save_data,
-    _assert_positive,
-    _assert_spatial_basis,
     _assert_categorical_obs,
     _assert_connectivity_key,
     _assert_non_empty_sequence,
+    _assert_positive,
+    _assert_spatial_basis,
+    _save_data,
 )
-from squidpy._constants._constants import SpatialAutocorr
-from squidpy._constants._pkg_constants import Key
 
 __all__ = ["spatial_autocorr", "co_occurrence"]
 
 
 it = nt.int32
 ft = nt.float32
 tt = nt.UniTuple
 ip = np.int32
 fp = np.float32
 
 
 @d.dedent
 @inject_docs(key=Key.obsp.spatial_conn(), sp=SpatialAutocorr)
 def spatial_autocorr(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     connectivity_key: str = Key.obsp.spatial_conn(),
-    genes: str | Sequence[str] | None = None,
+    genes: str | int | Sequence[str] | Sequence[int] | None = None,
     mode: Literal["moran", "geary"] = SpatialAutocorr.MORAN.s,  # type: ignore[assignment]
     transformation: bool = True,
     n_perms: int | None = None,
     two_tailed: bool = False,
     corr_method: str | None = "fdr_bh",
+    attr: Literal["obs", "X", "obsm"] = "X",
     layer: str | None = None,
     seed: int | None = None,
     use_raw: bool = False,
     copy: bool = False,
     n_jobs: int | None = None,
     backend: str = "loky",
     show_progress_bar: bool = True,
@@ -71,35 +78,45 @@
     See :cite:`pysal` for reference.
 
     Parameters
     ----------
     %(adata)s
     %(conn_key)s
     genes
-        List of gene names, as stored in :attr:`anndata.AnnData.var_names`, used to compute global
-        spatial autocorrelation statistic.
+        Depending on the ``attr``:
+
+            - if ``attr = 'X'``, it corresponds to genes stored in :attr:`anndata.AnnData.var_names`.
+              If `None`, it's computed :attr:`anndata.AnnData.var` ``['highly_variable']``,
+              if present. Otherwise, it's computed for all genes.
+            - if ``attr = 'obs'``, it corresponds to a list of columns in :attr:`anndata.AnnData.obs`.
+              If `None`, use all numerical columns.
+            - if ``attr = 'obsm'``, it corresponds to indices in :attr:`anndata.AnnData.obsm` ``['{{layer}}']``.
+              If `None`, all indices are used.
 
-        If `None`, it's computed :attr:`anndata.AnnData.var` ``['highly_variable']``, if present. Otherwise,
-        it's computed for all genes.
     mode
         Mode of score calculation:
 
             - `{sp.MORAN.s!r}` - `Moran's I autocorrelation <https://en.wikipedia.org/wiki/Moran%27s_I>`_.
             - `{sp.GEARY.s!r}` - `Geary's C autocorrelation <https://en.wikipedia.org/wiki/Geary%27s_C>`_.
 
     transformation
         If `True`, weights in :attr:`anndata.AnnData.obsp` ``['{key}']`` are row-normalized,
         advised for analytic p-value calculation.
     %(n_perms)s
         If `None`, only p-values under normality assumption are computed.
     two_tailed
         If `True`, p-values are two-tailed, otherwise they are one-tailed.
     %(corr_method)s
+    use_raw
+        Whether to access :attr:`anndata.AnnData.raw`. Only used when ``attr = 'X'``.
     layer
+        Depending on ``attr``:
         Layer in :attr:`anndata.AnnData.layers` to use. If `None`, use :attr:`anndata.AnnData.X`.
+    attr
+        Which attribute of :class:`~anndata.AnnData` to access. See ``genes`` parameter for more information.
     %(seed)s
     %(copy)s
     %(parallelize)s
 
     Returns
     -------
     If ``copy = True``, returns a :class:`pandas.DataFrame` with the following keys:
@@ -116,30 +133,58 @@
         - `'var_sim'` - variance of `'score'` from permutations.
 
     Otherwise, modifies the ``adata`` with the following key:
 
         - :attr:`anndata.AnnData.uns` ``['moranI']`` - the above mentioned dataframe, if ``mode = {sp.MORAN.s!r}``.
         - :attr:`anndata.AnnData.uns` ``['gearyC']`` - the above mentioned dataframe, if ``mode = {sp.GEARY.s!r}``.
     """
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     _assert_connectivity_key(adata, connectivity_key)
 
-    if genes is None:
-        if "highly_variable" in adata.var:
-            genes = adata[:, adata.var["highly_variable"]].var_names.values
-        else:
-            genes = adata.var_names.values
-    if use_raw:
+    def extract_X(adata: AnnData, genes: str | Sequence[str] | None) -> tuple[NDArrayA | spmatrix, Sequence[Any]]:
+        if genes is None:
+            if "highly_variable" in adata.var:
+                genes = adata[:, adata.var["highly_variable"]].var_names.values
+            else:
+                genes = adata.var_names.values
+        elif isinstance(genes, str):
+            genes = [genes]
+
+        if not use_raw:
+            return _get_obs_rep(adata[:, genes], use_raw=False, layer=layer).T, genes
         if adata.raw is None:
             raise AttributeError("No `.raw` attribute found. Try specifying `use_raw=False`.")
         genes = list(set(genes) & set(adata.raw.var_names))
-        vals = adata.raw[:, genes].X.T
-    else:
-        vals = _get_obs_rep(adata[:, genes], use_raw=False, layer=layer).T
+        return adata.raw[:, genes].X.T, genes
 
-    genes = _assert_non_empty_sequence(genes, name="genes")
+    def extract_obs(adata: AnnData, cols: str | Sequence[str] | None) -> tuple[NDArrayA | spmatrix, Sequence[Any]]:
+        if cols is None:
+            df = adata.obs.select_dtypes(include=np.number)
+            return df.T.to_numpy(), df.columns
+        if isinstance(cols, str):
+            cols = [cols]
+        return adata.obs[cols].T.to_numpy(), cols
+
+    def extract_obsm(adata: AnnData, ixs: int | Sequence[int] | None) -> tuple[NDArrayA | spmatrix, Sequence[Any]]:
+        if layer not in adata.obsm:
+            raise KeyError(f"Key `{layer!r}` not found in `adata.obsm`.")
+        if ixs is None:
+            ixs = np.arange(adata.obsm[layer].shape[1])  # type: ignore[assignment]
+        ixs = list(np.ravel([ixs]))
+        return adata.obsm[layer][:, ixs].T, ixs
+
+    if attr == "X":
+        vals, index = extract_X(adata, genes)  # type: ignore[arg-type]
+    elif attr == "obs":
+        vals, index = extract_obs(adata, genes)  # type: ignore[arg-type]
+    elif attr == "obsm":
+        vals, index = extract_obsm(adata, genes)  # type: ignore[arg-type]
+    else:
+        raise NotImplementedError(f"Extracting from `adata.{attr}` is not yet implemented.")
 
     mode = SpatialAutocorr(mode)  # type: ignore[assignment]
     if TYPE_CHECKING:
         assert isinstance(mode, SpatialAutocorr)
     params = {"mode": mode.s, "transformation": transformation, "two_tailed": two_tailed}
 
     if mode == SpatialAutocorr.MORAN:
@@ -178,15 +223,15 @@
         )(mode=mode, g=g, vals=vals, seed=seed)
     else:
         score_perms = None
 
     with np.errstate(divide="ignore"):
         pval_results = _p_value_calc(score, score_perms, g, params)
 
-    df = pd.DataFrame({params["stat"]: score, **pval_results}, index=genes)
+    df = pd.DataFrame({params["stat"]: score, **pval_results}, index=index)
 
     if corr_method is not None:
         for pv in filter(lambda x: "pval" in x, df.columns):
             _, pvals_adj, _, _ = multipletests(df[pv].values, alpha=0.05, method=corr_method)
             df[f"{pv}_{corr_method}"] = pvals_adj
 
     df.sort_values(by=params["stat"], ascending=params["ascending"], inplace=True)
@@ -268,15 +313,14 @@
     idx_splits: Iterable[tuple[int, int]],
     spatial_splits: Sequence[NDArrayA],
     labs_splits: Sequence[NDArrayA],
     labs_unique: NDArrayA,
     interval: NDArrayA,
     queue: SigQueue | None = None,
 ) -> pd.DataFrame:
-
     out_lst = []
     for t in idx_splits:
         idx_x, idx_y = t
         labs_x = labs_splits[idx_x]
         labs_y = labs_splits[idx_y]
         dist = pairwise_distances(spatial_splits[idx_x], spatial_splits[idx_y])
 
@@ -290,15 +334,15 @@
         queue.put(Signal.FINISH)
 
     return out_lst
 
 
 @d.dedent
 def co_occurrence(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     cluster_key: str,
     spatial_key: str = Key.obsm.spatial,
     interval: int | NDArrayA = 50,
     copy: bool = False,
     n_splits: int | None = None,
     n_jobs: int | None = None,
     backend: str = "loky",
@@ -328,14 +372,16 @@
     Otherwise, modifies the ``adata`` with the following keys:
 
         - :attr:`anndata.AnnData.uns` ``['{cluster_key}_co_occurrence']['occ']`` - the co-occurrence probabilities
           across interval thresholds.
         - :attr:`anndata.AnnData.uns` ``['{cluster_key}_co_occurrence']['interval']`` - the distance thresholds
           computed at ``interval``.
     """
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     _assert_categorical_obs(adata, key=cluster_key)
     _assert_spatial_basis(adata, key=spatial_key)
 
     spatial = adata.obsm[spatial_key].astype(fp)
     original_clust = adata.obs[cluster_key]
 
     # annotate cluster idx
@@ -364,18 +410,18 @@
                 f"prevent `{n_obs}x{n_obs}` distance matrix from being created"
             )
         else:
             n_splits = 1
     n_splits = max(min(n_splits, n_obs), 1)
 
     # split array and labels
-    spatial_splits = tuple(s for s in np.array_split(spatial, n_splits, axis=0) if len(s))
-    labs_splits = tuple(s for s in np.array_split(labs, n_splits, axis=0) if len(s))
+    spatial_splits = tuple(s for s in np.array_split(spatial, n_splits, axis=0) if len(s))  # type: ignore[arg-type]
+    labs_splits = tuple(s for s in np.array_split(labs, n_splits, axis=0) if len(s))  # type: ignore[arg-type]
     # create idx array including unique combinations and self-comparison
-    x, y = np.triu_indices_from(np.empty((n_splits, n_splits)))
+    x, y = np.triu_indices_from(np.empty((n_splits, n_splits)))  # type: ignore[arg-type]
     idx_splits = [(i, j) for i, j in zip(x, y)]
 
     n_jobs = _get_n_cores(n_jobs)
     start = logg.info(
         f"Calculating co-occurrence probabilities for `{len(interval)}` intervals "
         f"`{len(idx_splits)}` split combinations using `{n_jobs}` core(s)"
     )
@@ -416,16 +462,16 @@
     return thres_min.astype(fp), thres_max.astype(fp)
 
 
 def _p_value_calc(
     score: NDArrayA,
     sims: NDArrayA | None,
     weights: spmatrix | NDArrayA,
-    params: Dict[str, Any],
-) -> Dict[str, Any]:
+    params: dict[str, Any],
+) -> dict[str, Any]:
     """
     Handle p-value calculation for spatial autocorrelation function.
 
     Parameters
     ----------
     score
         (n_features,).
@@ -446,15 +492,15 @@
     p_norm, var_norm = _analytic_pval(score, weights, params)
     results = {"pval_norm": p_norm, "var_norm": var_norm}
 
     if sims is None:
         return results
 
     n_perms = sims.shape[0]
-    large_perm = (sims >= score).sum(axis=0)  # type: ignore[attr-defined]
+    large_perm = (sims >= score).sum(axis=0)
     # subtract total perm for negative values
     large_perm[(n_perms - large_perm) < large_perm] = n_perms - large_perm[(n_perms - large_perm) < large_perm]
     # get p-value based on permutation
     p_sim: NDArrayA = (large_perm + 1) / (n_perms + 1)
 
     # get p-value based on standard normal approximation from permutations
     e_score_sim = sims.sum(axis=0) / n_perms
@@ -470,15 +516,15 @@
     results["pval_z_sim"] = p_z_sim
     results["pval_sim"] = p_sim
     results["var_sim"] = var_sim
 
     return results
 
 
-def _analytic_pval(score: NDArrayA, g: spmatrix | NDArrayA, params: Dict[str, Any]) -> tuple[NDArrayA, float]:
+def _analytic_pval(score: NDArrayA, g: spmatrix | NDArrayA, params: dict[str, Any]) -> tuple[NDArrayA, float]:
     """
     Analytic p-value computation.
 
     See `Moran's I <https://pysal.org/esda/_modules/esda/moran.html#Moran>`_ and
     `Geary's C <https://pysal.org/esda/_modules/esda/geary.html#Geary>`_ implementation.
     """
     s0, s1, s2 = _g_moments(g)
@@ -509,15 +555,15 @@
     See `pysal <https://pysal.org/libpysal/_modules/libpysal/weights/weights.html#W>`_ implementation.
     """
     # s0
     s0 = w.sum()
 
     # s1
     t = w.transpose() + w
-    t2 = t.multiply(t)
+    t2 = t.multiply(t)  # type: ignore[union-attr]
     s1 = t2.sum() / 2.0
 
     # s2
     s2array: NDArrayA = np.array(w.sum(1) + w.sum(0).transpose()) ** 2
     s2 = s2array.sum()
 
     return s0, s1, s2
```

### Comparing `squidpy-1.2.3/squidpy/gr/_ripley.py` & `squidpy-1.3.0/src/squidpy/gr/_ripley.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """Functions for point patterns spatial statistics."""
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Literal, TYPE_CHECKING
+from typing import (
+    TYPE_CHECKING,
+    Literal,
+    Union,  # noqa: F401
+)
 
-from scanpy import logging as logg
+import numpy as np
+import pandas as pd
 from anndata import AnnData
-
 from numpy.random import default_rng
-from scipy.spatial import Delaunay, ConvexHull
+from scanpy import logging as logg
+from scipy.spatial import ConvexHull, Delaunay
+from scipy.spatial.distance import pdist
 from sklearn.neighbors import NearestNeighbors
 from sklearn.preprocessing import LabelEncoder
-from scipy.spatial.distance import pdist
-import numpy as np
-import pandas as pd
+from spatialdata import SpatialData
 
-from squidpy._docs import d, inject_docs
-from squidpy._utils import NDArrayA
-from squidpy.gr._utils import _save_data, _assert_spatial_basis, _assert_categorical_obs
 from squidpy._constants._constants import RipleyStat
 from squidpy._constants._pkg_constants import Key
+from squidpy._docs import d, inject_docs
+from squidpy._utils import NDArrayA
+from squidpy.gr._utils import _assert_categorical_obs, _assert_spatial_basis, _save_data
 
 __all__ = ["ripley"]
 
 
 @d.dedent
 @inject_docs(key=Key.obsm.spatial, rp=RipleyStat)
 def ripley(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     cluster_key: str,
     mode: Literal["F", "G", "L"] = "F",
     spatial_key: str = Key.obsm.spatial,
     metric: str = "euclidean",
     n_neigh: int = 2,
     n_simulations: int = 100,
     n_observations: int = 1000,
@@ -59,20 +62,22 @@
 
     `{rp.L.s!r}` we first need to compute :math:`K(t)`, which is defined as:
 
     .. math::
 
         K(t) = \frac{{1}}{{\lambda}} \sum_{{i \ne j}} \frac{{I(d_{{i,j}}<t)}}{{n}}
 
+
     and then we apply a variance-stabilizing transformation:
 
     .. math::
 
         L(t) = (\frac{{K(t)}}{{\pi}})^{{1/2}}
 
+
     Parameters
     ----------
     %(adata)s
     %(cluster_key)s
     mode
         Which Ripley's statistic to compute.
     %(spatial_key)s
@@ -98,14 +103,16 @@
 
     References
     ----------
     For reference, check out
     `Wikipedia <https://en.wikipedia.org/wiki/Spatial_descriptive_statistics#Ripley's_K_and_L_functions>`_
     or :cite:`Baddeley2015-lm`.
     """
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     _assert_categorical_obs(adata, key=cluster_key)
     _assert_spatial_basis(adata, key=spatial_key)
     coordinates = adata.obsm[spatial_key]
     clusters = adata.obs[cluster_key].values
 
     mode = RipleyStat(mode)  # type: ignore[assignment]
     if TYPE_CHECKING:
@@ -199,15 +206,15 @@
 def _f_g_function(distances: NDArrayA, support: NDArrayA) -> tuple[NDArrayA, NDArrayA]:
     counts, bins = np.histogram(distances, bins=support)
     fracs = np.cumsum(counts) / counts.sum()
     return bins, np.concatenate((np.zeros((1,), dtype=float), fracs))
 
 
 def _l_function(distances: NDArrayA, support: NDArrayA, n: int, area: float) -> tuple[NDArrayA, NDArrayA]:
-    n_pairs_less_than_d = (distances < support.reshape(-1, 1)).sum(axis=1)  # type: ignore[attr-defined]
+    n_pairs_less_than_d = (distances < support.reshape(-1, 1)).sum(axis=1)
     intensity = n / area
     k_estimate = ((n_pairs_less_than_d * 2) / n) / intensity
     l_estimate = np.sqrt(k_estimate / np.pi)
     return support, l_estimate
 
 
 def _ppp(hull: ConvexHull, n_simulations: int, n_observations: int, seed: int | None = None) -> NDArrayA:
```

### Comparing `squidpy-1.2.3/squidpy/gr/_sepal.py` & `squidpy-1.3.0/src/squidpy/gr/_sepal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Literal  # < 3.8
-from typing import Callable, Sequence
+from typing import (
+    Callable,
+    Literal,  # < 3.8
+    Sequence,
+    Union,  # noqa: F401
+)
 
-from scanpy import logging as logg
+import numpy as np
+import pandas as pd
 from anndata import AnnData
-
 from numba import njit
-from scipy.sparse import issparse, spmatrix, csr_matrix, isspmatrix_csr
+from scanpy import logging as logg
+from scipy.sparse import csr_matrix, issparse, isspmatrix_csr, spmatrix
 from sklearn.metrics import pairwise_distances
-import numpy as np
-import pandas as pd
+from spatialdata import SpatialData
 
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d, inject_docs
-from squidpy._utils import Signal, NDArrayA, SigQueue, parallelize, _get_n_cores
+from squidpy._utils import NDArrayA, Signal, SigQueue, _get_n_cores, parallelize
 from squidpy.gr._utils import (
-    _save_data,
-    _extract_expression,
-    _assert_spatial_basis,
     _assert_connectivity_key,
     _assert_non_empty_sequence,
+    _assert_spatial_basis,
+    _extract_expression,
+    _save_data,
 )
-from squidpy._constants._pkg_constants import Key
 
 __all__ = ["sepal"]
 
 
 @d.dedent
 @inject_docs(key=Key.obsp.spatial_conn())
 def sepal(
-    adata: AnnData,
+    adata: AnnData | SpatialData,
     max_neighs: Literal[4, 6],
     genes: str | Sequence[str] | None = None,
     n_iter: int | None = 30000,
     dt: float = 0.001,
     thresh: float = 1e-8,
     connectivity_key: str = Key.obsp.spatial_conn(),
     spatial_key: str = Key.obsm.spatial,
@@ -90,14 +93,16 @@
         - :attr:`anndata.AnnData.uns` ``['sepal_score']`` - the sepal scores.
 
     Notes
     -----
     If some genes in :attr:`anndata.AnnData.uns` ``['sepal_score']`` are `NaN`,
     consider re-running the function with increased ``n_iter``.
     """
+    if isinstance(adata, SpatialData):
+        adata = adata.table
     _assert_connectivity_key(adata, connectivity_key)
     _assert_spatial_basis(adata, key=spatial_key)
     if max_neighs not in (4, 6):
         raise ValueError(f"Expected `max_neighs` to be either `4` or `6`, found `{max_neighs}`.")
 
     spatial = adata.obsm[spatial_key].astype(np.float_)
 
@@ -123,15 +128,15 @@
 
     # get counts
     vals, genes = _extract_expression(adata, genes=genes, use_raw=use_raw, layer=layer)
     start = logg.info(f"Calculating sepal score for `{len(genes)}` genes using `{n_jobs}` core(s)")
 
     score = parallelize(
         _score_helper,
-        collection=np.arange(len(genes)),
+        collection=np.arange(len(genes)).tolist(),
         extractor=np.hstack,
         use_ixs=False,
         n_jobs=n_jobs,
         backend=backend,
         show_progress_bar=show_progress_bar,
     )(
         vals=vals,
@@ -177,15 +182,16 @@
     elif max_neighs == 6:
         fun = _laplacian_hex
     else:
         raise NotImplementedError(f"Laplacian for `{max_neighs}` neighbors is not yet implemented.")
 
     score, sparse = [], issparse(vals)
     for i in ixs:
-        conc = vals[:, i].A.flatten() if sparse else vals[:, i].copy()
+        conc = vals[:, i].A.flatten() if sparse else vals[:, i].copy()  # type: ignore[union-attr]
+        conc = vals[:, i].A.flatten() if sparse else vals[:, i].copy()  # type: ignore[union-attr]
         time_iter = _diffusion(conc, fun, n_iter, sat, sat_idx, unsat, unsat_idx, dt=dt, thresh=thresh)
         score.append(dt * time_iter)
 
         if queue is not None:
             queue.put(Signal.UPDATE)
 
     if queue is not None:
@@ -268,15 +274,15 @@
     ----------
     Approximate Methods of Higher Analysis,
     Curtis D. Benster, L.V. Kantorovich, V.I. Krylov,
     ISBN-13: 978-0486821603.
     """
     d2f: NDArrayA = nbrs - 6 * centers
     d2f = d2f / h**2
-    d2f = (d2f * 2) / 3  # type: ignore[assignment]
+    d2f = (d2f * 2) / 3
 
     return d2f
 
 
 # taken from https://github.com/almaan/sepal/blob/master/sepal/models.py
 @njit(fastmath=True)
 def _entropy(
```

### Comparing `squidpy-1.2.3/squidpy/gr/_utils.py` & `squidpy-1.3.0/src/squidpy/gr/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Graph utilities."""
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Any, Hashable, Iterable, Sequence, TYPE_CHECKING
 from contextlib import contextmanager
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Hashable,
+    Iterable,
+    Sequence,
+    Union,  # noqa: F401
+)
 
-from scanpy import logging as logg
+import numpy as np
+import pandas as pd
 from anndata import AnnData
-from anndata.utils import make_index_unique
 from anndata._core.views import ArrayView, SparseCSCView, SparseCSRView
-
-from scipy.sparse import issparse, spmatrix, csc_matrix, csr_matrix
+from anndata.utils import make_index_unique
 from pandas.api.types import infer_dtype, is_categorical_dtype
-import numpy as np
-import pandas as pd
+from scanpy import logging as logg
+from scipy.sparse import csc_matrix, csr_matrix, issparse, spmatrix
 
 from squidpy._docs import d
 from squidpy._utils import NDArrayA, _unique_order_preserving
 
 
 def _check_tuple_needles(
     needles: Sequence[tuple[Any, Any]],
```

### Comparing `squidpy-1.2.3/squidpy/im/_container.py` & `squidpy-1.3.0/src/squidpy/im/_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,67 +1,64 @@
 from __future__ import annotations
 
+import re
 from copy import copy, deepcopy
+from functools import partial
+from itertools import chain
+from pathlib import Path
 from types import MappingProxyType
 from typing import (
+    TYPE_CHECKING,
     Any,
-    Union,
-    Literal,
-    Mapping,
-    TypeVar,
     Callable,
     Iterable,
     Iterator,
+    Literal,
+    Mapping,
     Sequence,
-    TYPE_CHECKING,
+    TypeVar,
+    Union,
 )
-from pathlib import Path
-from functools import partial
-from itertools import chain
-import re
-import validators
-
-from scanpy import logging as logg
-from anndata import AnnData
-from scanpy.plotting.palettes import default_102 as default_palette
 
-from dask import delayed
-import numpy as np
-import xarray as xr
 import dask.array as da
-
-from matplotlib.colors import ListedColormap
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-
-from skimage.util import img_as_float
+import numpy as np
+import validators
+import xarray as xr
+from anndata import AnnData
+from dask import delayed
+from matplotlib.colors import ListedColormap
+from scanpy import logging as logg
+from scanpy.plotting.palettes import default_102 as default_palette
 from skimage.transform import rescale
+from skimage.util import img_as_float
 
+from squidpy._constants._constants import InferDimensions
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d, inject_docs
 from squidpy._utils import NDArrayA, singledispatchmethod
-from squidpy.im._io import _lazy_load_image, _infer_dimensions, _assert_dims_present
 from squidpy.gr._utils import (
     _assert_in_range,
-    _assert_positive,
+    _assert_non_empty_sequence,
     _assert_non_negative,
+    _assert_positive,
     _assert_spatial_basis,
-    _assert_non_empty_sequence,
 )
 from squidpy.im._coords import (
-    CropCoords,
-    CropPadding,
     _NULL_COORDS,
     _NULL_PADDING,
+    CropCoords,
+    CropPadding,
     TupleSerializer,
-    _update_attrs_scale,
     _update_attrs_coords,
+    _update_attrs_scale,
 )
 from squidpy.im._feature_mixin import FeatureMixin
-from squidpy._constants._constants import InferDimensions
-from squidpy._constants._pkg_constants import Key
+from squidpy.im._io import _assert_dims_present, _infer_dimensions, _lazy_load_image
 
 FoI_t = Union[int, float]
 Pathlike_t = Union[str, Path]
 Arraylike_t = Union[NDArrayA, xr.DataArray]
 InferDims_t = Union[Literal["default", "prefer_channels", "prefer_z"], Sequence[str]]
 Input_t = Union[Pathlike_t, Arraylike_t, "ImageContainer"]
 Interactive = TypeVar("Interactive")  # cannot import because of cyclic dependencies
@@ -577,15 +574,20 @@
         cval: FoI_t = 0,
         mask_circle: bool = False,
         preserve_dtypes: bool = True,
         **_: Any,
     ) -> xr.Dataset:
         def _rescale(arr: xr.DataArray) -> xr.DataArray:
             scaling_fn = partial(
-                rescale, scale=[scale, scale, 1], preserve_range=True, order=1, channel_axis=-1, cval=cval
+                rescale,
+                preserve_range=True,
+                scale=[scale, scale, 1],
+                order=1,
+                channel_axis=-1,
+                cval=cval,
             )
             dtype = arr.dtype
 
             if isinstance(arr.data, da.Array):
                 shape = np.maximum(np.round(scale * np.asarray(arr.shape)), 1)
                 shape[-1] = arr.shape[-1]
                 shape[-2] = arr.shape[-2]
@@ -720,17 +722,15 @@
         spot_diameter_key: str = "spot_diameter_fullres",
         spot_scale: float = 1.0,
         obs_names: Iterable[Any] | None = None,
         as_array: str | bool = False,
         squeeze: bool = True,
         return_obs: bool = False,
         **kwargs: Any,
-    ) -> (
-        Iterator[ImageContainer] | Iterator[NDArrayA] | Iterator[tuple[NDArrayA, ...]] | Iterator[dict[str, NDArrayA]]
-    ):
+    ) -> Iterator[ImageContainer] | Iterator[NDArrayA] | Iterator[tuple[NDArrayA, ...]] | Iterator[dict[str, NDArrayA]]:
         """
         Iterate over :attr:`anndata.AnnData.obs_names` and extract crops.
 
         Implemented for 10X spatial datasets.
         For Z-stacks, the specified ``library_id`` or list of ``library_id`` need to match the name of the Z-dimension.
         Always extracts 2D crops from the specified Z-dimension.
 
@@ -780,28 +780,28 @@
                     raise NotImplementedError(_ERROR_NOTIMPLEMENTED_LIBID)
                 obs_library_ids = [library_id] * adata.n_obs
             except ValueError as e:
                 if "Unable to determine which library id to use" in str(e):
                     raise ValueError(
                         str(e)
                         + " Or specify a key in `adata.obs` containing a mapping from observations to library ids."
-                    )
+                    ) from e
                 else:
                     raise e
         else:
             try:
                 obs_library_ids = adata.obs[library_id]
             except KeyError:
                 logg.debug(
                     f"Unable to find library ids in `adata.obs[{library_id!r}]`. "
                     f"Trying in `adata.uns[{spatial_key!r}]`"
                 )
                 library_id = Key.uns.library_id(adata, spatial_key=spatial_key, library_id=library_id)
                 if not isinstance(library_id, str):
-                    raise NotImplementedError(_ERROR_NOTIMPLEMENTED_LIBID)
+                    raise NotImplementedError(_ERROR_NOTIMPLEMENTED_LIBID) from None
                 obs_library_ids = [library_id] * adata.n_obs
 
         lids = set(obs_library_ids)
         if len(self.data.z) > 1 and len(lids) == 1:
             logg.warning(
                 f"ImageContainer has `{len(self.data.z)}` Z-dimensions, using library id `{next(iter(lids))}` for all"
             )
@@ -973,15 +973,15 @@
 
         if channel is not None:
             channel = np.asarray([channel]).ravel()  # type: ignore[assignment]
             if not len(channel):  # type: ignore[arg-type]
                 raise ValueError("No channels have been selected.")
             arr = arr[{arr.dims[-1]: channel}]
         else:
-            channel = np.arange(arr.shape[-1])
+            channel = np.arange(arr.shape[-1])  # type: ignore[assignment]
         if TYPE_CHECKING:
             assert isinstance(channel, Sequence)
 
         n_channels = arr.shape[-1]
         if n_channels not in (1, 3, 4) and not channelwise:
             logg.warning(f"Unable to plot image with `{n_channels}`. Setting `channelwise=True`")
             channelwise = True
@@ -1110,15 +1110,15 @@
         Returns
         -------
         Interactive view of this container. Screenshot of the canvas can be taken by
         :meth:`squidpy.pl.Interactive.screenshot`.
         """
         from squidpy.pl import Interactive  # type: ignore[attr-defined]
 
-        return Interactive(  # type: ignore[no-any-return]
+        return Interactive(  # type: ignore[return-value]
             img=self,
             adata=adata,
             spatial_key=spatial_key,
             library_key=library_key,
             library_id=library_id,
             cmap=cmap,
             palette=palette,
```

### Comparing `squidpy-1.2.3/squidpy/im/_coords.py` & `squidpy-1.3.0/src/squidpy/im/_coords.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Union  # noqa: F401
-from typing import Any, Hashable
 from dataclasses import dataclass
+from typing import (
+    Any,
+    Hashable,
+    Union,  # noqa: F401
+)
 
 import numpy as np
 
+from squidpy._constants._pkg_constants import Key
 from squidpy._utils import NDArrayA
 from squidpy.gr._utils import _assert_non_negative
-from squidpy._constants._pkg_constants import Key
 
 
 def _circular_mask(arr: NDArrayA, y: int, x: int, radius: float) -> NDArrayA:
     Y, X = np.ogrid[: arr.shape[0], : arr.shape[1]]
     return np.asarray(((Y - y) ** 2 + (X - x) ** 2) <= radius**2)
```

### Comparing `squidpy-1.2.3/squidpy/im/_feature.py` & `squidpy-1.3.0/src/squidpy/im/_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from __future__ import annotations
 
 from types import MappingProxyType
-from typing import Union  # noqa: F401
-from typing import Any, Mapping, Sequence, TYPE_CHECKING
-
-from scanpy import logging as logg
-from anndata import AnnData
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Mapping,
+    Sequence,
+    Union,  # noqa: F401
+)
 
 import pandas as pd
+from anndata import AnnData
+from scanpy import logging as logg
 
+from squidpy._constants._constants import ImageFeature
 from squidpy._docs import d, inject_docs
-from squidpy._utils import Signal, SigQueue, parallelize, _get_n_cores
+from squidpy._utils import Signal, SigQueue, _get_n_cores, parallelize
 from squidpy.gr._utils import _save_data
 from squidpy.im._container import ImageContainer
-from squidpy._constants._constants import ImageFeature
 
 __all__ = ["calculate_image_features"]
 
 
 @d.dedent
 @inject_docs(f=ImageFeature)
 def calculate_image_features(
```

### Comparing `squidpy-1.2.3/squidpy/im/_feature_mixin.py` & `squidpy-1.3.0/src/squidpy/im/_feature_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from __future__ import annotations
 
 from typing import (
+    TYPE_CHECKING,
     Any,
-    Dict,
-    Union,
     Callable,
+    Dict,
     Iterable,
     Protocol,
     Sequence,
-    TYPE_CHECKING,
+    Union,
 )
 
 import numpy as np
+import skimage.measure
 import xarray as xr
-
+from skimage.feature import graycomatrix, graycoprops
 from skimage.util import img_as_ubyte
-from skimage.feature import graycoprops, graycomatrix
-import skimage.measure
 
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d
 from squidpy._utils import NDArrayA
 from squidpy.gr._utils import _assert_non_empty_sequence
-from squidpy.im._coords import CropCoords, _NULL_PADDING
-from squidpy._constants._pkg_constants import Key
+from squidpy.im._coords import _NULL_PADDING, CropCoords
 
-Feature_t = Dict[str, Any]
+Feature_t = dict[str, Any]
 Channel_t = Union[int, Sequence[int]]
 
 
 def _get_channels(xr_img: NDArrayA | xr.DataArray, channels: Channel_t | None) -> list[int]:
     """Get correct channel ranges for feature calculation."""
     # if channels is None, compute features for all channels
     all_channels = list(range(xr_img.shape[-1]))
@@ -375,15 +374,15 @@
             if intensity_layer is None:
                 raise ValueError("Please specify `intensity_layer` if using intensity properties.")
             channels = _get_channels(self[intensity_layer], channels)
             channels = _assert_non_empty_sequence(channels, name="channels")
         else:
             channels = ()
 
-        features: Dict[str, Any] = {}
+        features: dict[str, Any] = {}
         label_arr = self[label_layer].sel(z=library_id)
         label_arr_0 = label_arr[..., 0].values
         # calculate features that do not depend on the intensity image
         tmp_features = skimage.measure.regionprops_table(label_arr_0, properties=no_intensity_props)
         for p in no_intensity_props:
             if p == "label":
                 features[f"{feature_name}_{p}"] = len(tmp_features["label"])
```

### Comparing `squidpy-1.2.3/squidpy/im/_io.py` & `squidpy-1.3.0/src/squidpy/im/_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
-from PIL import Image
-from typing import Union  # noqa: F401
-from typing import Mapping
 from pathlib import Path
+from typing import (
+    Mapping,
+    Union,  # noqa: F401
+)
 
-from scanpy import logging as logg
-
-from dask import delayed
+import dask.array as da
 import numpy as np
 import xarray as xr
-import dask.array as da
-
-from tifffile import TiffFile
+from dask import delayed
+from PIL import Image
+from scanpy import logging as logg
 from skimage.io import imread
+from tifffile import TiffFile
 
+from squidpy._constants._constants import InferDimensions
 from squidpy._docs import inject_docs
 from squidpy._utils import NDArrayA
-from squidpy._constants._constants import InferDimensions
 
 
 def _assert_dims_present(dims: tuple[str, ...], include_z: bool = True) -> None:
     missing_dims = ({"y", "x", "z"} if include_z else {"y", "x"}) - set(dims)
     if missing_dims:
         raise ValueError(f"Expected to find `{sorted(missing_dims)}` dimension(s) in `{dims}`.")
```

### Comparing `squidpy-1.2.3/squidpy/im/_process.py` & `squidpy-1.3.0/src/squidpy/im/_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 from types import MappingProxyType
-from typing import Union  # noqa: F401
-from typing import Any, Mapping, Callable, Sequence
+from typing import (
+    Any,
+    Callable,
+    Mapping,
+    Sequence,
+    Union,  # noqa: F401
+)
 
-from scanpy import logging as logg
-
-from scipy.ndimage import gaussian_filter as scipy_gf
 import dask.array as da
-
 from dask_image.ndfilters import gaussian_filter as dask_gf
+from scanpy import logging as logg
+from scipy.ndimage import gaussian_filter as scipy_gf
 
+from squidpy._constants._constants import Processing
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d, inject_docs
 from squidpy._utils import NDArrayA
 from squidpy.im._container import ImageContainer
-from squidpy._constants._constants import Processing
-from squidpy._constants._pkg_constants import Key
 
 __all__ = ["process"]
 
 
 @d.dedent
 @inject_docs(p=Processing)
 def process(
```

### Comparing `squidpy-1.2.3/squidpy/im/_segment.py` & `squidpy-1.3.0/src/squidpy/im/_segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from types import MappingProxyType
-from typing import Union  # noqa: F401
-from typing import Any, Mapping, Callable, Sequence, TYPE_CHECKING
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Mapping,
+    Sequence,
+    Union,  # noqa: F401
+)
 
+import dask.array as da
+import numpy as np
 from scanpy import logging as logg
-
 from scipy import ndimage as ndi
-import numpy as np
-import dask.array as da
-
 from skimage.feature import peak_local_max
 from skimage.filters import threshold_otsu
 from skimage.segmentation import watershed
 
+from squidpy._constants._constants import SegmentationBackend
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d, inject_docs
 from squidpy._utils import NDArrayA, singledispatchmethod
 from squidpy.im._container import ImageContainer
-from squidpy._constants._constants import SegmentationBackend
-from squidpy._constants._pkg_constants import Key
 
 __all__ = ["SegmentationModel", "SegmentationWatershed", "SegmentationCustom"]
 _SEG_DTYPE = np.uint32
 _SEG_DTYPE_N_BITS = _SEG_DTYPE(0).nbytes * 8
 
 
 class SegmentationModel(ABC):
@@ -120,17 +124,17 @@
             dtype=_SEG_DTYPE,
             num_blocks=img.numblocks,
             shift=shift,
             drop_axis=img.ndim - 1,  # y, x, z, c; -1 seems to be bugged
             **kwargs,
         )
         from dask_image.ndmeasure._utils._label import (
-            relabel_blocks,
-            label_adjacency_graph,
             connected_components_delayed,
+            label_adjacency_graph,
+            relabel_blocks,
         )
 
         # max because labels are not continuous (and won't be continuous)
         label_groups = label_adjacency_graph(img, None, img.max())
         new_labeling = connected_components_delayed(label_groups)
         relabeled = relabel_blocks(img, new_labeling)
```

### Comparing `squidpy-1.2.3/squidpy/pl/_color_utils.py` & `squidpy-1.3.0/src/squidpy/pl/_color_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Utils for plotting functions."""
 from __future__ import annotations
 
-from cycler import cycler, Cycler
-from typing import Any, Union, Mapping, Optional, Sequence
+from typing import Any, Mapping, Optional, Sequence, Union
 
-from scanpy import logging as logg
+import matplotlib.pyplot as plt
+import numpy as np
 from anndata import AnnData
+from cycler import Cycler, cycler
+from matplotlib.colors import ListedColormap, to_hex, to_rgba
+from scanpy import logging as logg
 from scanpy.plotting._utils import add_colors_for_categorical_sample_annotation
 
-import numpy as np
-
-from matplotlib.colors import to_hex, to_rgba, ListedColormap
-import matplotlib.pyplot as plt
-
 from squidpy._constants._pkg_constants import Key
 
 Palette_t = Union[str, ListedColormap, None]
 
 
 def _maybe_set_colors(
     source: AnnData, target: AnnData, key: str, palette: str | ListedColormap | Cycler | Sequence[Any] | None = None
@@ -30,15 +28,15 @@
         if isinstance(palette, ListedColormap):  # `scanpy` requires it
             palette = cycler(color=palette.colors)
         add_colors_for_categorical_sample_annotation(target, key=key, force_update_colors=True, palette=palette)
 
 
 def _get_palette(
     adata: AnnData,
-    cluster_key: Optional[str],
+    cluster_key: str | None,
     categories: Sequence[Any],
     palette: Palette_t = None,
     alpha: float = 1.0,
 ) -> Mapping[str, str] | None:
     if palette is None:
         try:
             palette = adata.uns[Key.uns.colors(cluster_key)]  # type: ignore[arg-type]
```

### Comparing `squidpy-1.2.3/squidpy/pl/_graph.py` & `squidpy-1.3.0/src/squidpy/pl/_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 """Plotting for graph functions."""
 from __future__ import annotations
 
-from types import MappingProxyType
-from typing import Union  # noqa: F401
-from typing import Any, Literal, Mapping, Sequence, TYPE_CHECKING
 from pathlib import Path
+from types import MappingProxyType
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Literal,
+    Mapping,
+    Sequence,
+    Union,  # noqa: F401
+)
 
-from anndata import AnnData
-
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
-from matplotlib.axes import Axes
 import seaborn as sns
-import matplotlib.pyplot as plt
+from anndata import AnnData
+from matplotlib.axes import Axes
 
+from squidpy._constants._constants import RipleyStat
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d
 from squidpy.gr._utils import (
-    _get_valid_values,
     _assert_categorical_obs,
     _assert_non_empty_sequence,
+    _get_valid_values,
 )
-from squidpy.pl._utils import _heatmap, save_fig
 from squidpy.pl._color_utils import Palette_t, _get_palette, _maybe_set_colors
-from squidpy._constants._constants import RipleyStat
-from squidpy._constants._pkg_constants import Key
+from squidpy.pl._utils import _heatmap, save_fig
 
 __all__ = ["centrality_scores", "interaction_matrix", "nhood_enrichment", "ripley", "co_occurrence"]
 
 
-def _get_data(adata: AnnData, cluster_key: str, func_name: str, **kwargs: Any) -> Any:
+def _get_data(adata: AnnData, cluster_key: str, func_name: str, attr: str = "uns", **kwargs: Any) -> Any:
     key = getattr(Key.uns, func_name)(cluster_key, **kwargs)
+
     try:
-        return adata.uns[key]
+        if attr == "uns":
+            return adata.uns[key]
+        elif attr == "obsm":
+            return adata.obsm[key]
+        else:
+            raise ValueError(f"attr must be either 'uns' or 'obsm', got {attr}")
     except KeyError:
         raise KeyError(
             f"Unable to get the data from `adata.uns[{key!r}]`. "
             f"Please run `squidpy.gr.{func_name}(..., cluster_key={cluster_key!r})` first."
         ) from None
 
 
@@ -79,15 +89,15 @@
         legend_kwargs["loc"] = "center left"
         legend_kwargs.setdefault("bbox_to_anchor", (1, 0.5))
 
     scores = df.columns.values
     df[cluster_key] = df.index.values
 
     clusters = adata.obs[cluster_key].cat.categories
-    palette = _get_palette(adata, cluster_key=cluster_key, categories=clusters)
+    palette = _get_palette(adata, cluster_key=cluster_key, categories=clusters, palette=palette)
 
     score = scores if score is None else score
     score = _assert_non_empty_sequence(score, name="centrality scores")
     score = sorted(_get_valid_values(score, scores))
 
     fig, axs = plt.subplots(1, len(score), figsize=figsize, dpi=dpi, constrained_layout=True)
     axs = np.ravel(axs)  # make into iterable
@@ -284,15 +294,15 @@
 
     legend_kwargs = dict(legend_kwargs)
     if "loc" not in legend_kwargs:
         legend_kwargs["loc"] = "center left"
         legend_kwargs.setdefault("bbox_to_anchor", (1, 0.5))
 
     categories = adata.obs[cluster_key].cat.categories
-    palette = _get_palette(adata, cluster_key=cluster_key, categories=categories) if palette is None else palette
+    palette = _get_palette(adata, cluster_key=cluster_key, categories=categories, palette=palette)
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
     else:
         fig = ax.figure
     sns.lineplot(
         y="stats",
         x="bins",
```

### Comparing `squidpy-1.2.3/squidpy/pl/_interactive/_controller.py` & `squidpy-1.3.0/src/squidpy/pl/_interactive/_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 from __future__ import annotations
 
-from typing import Any, TYPE_CHECKING
 from pathlib import Path
+from typing import TYPE_CHECKING, Any
 
-from scanpy import logging as logg
-from anndata import AnnData
-
-from pandas.core.dtypes.common import is_categorical_dtype
 import numpy as np
 import pandas as pd
 import xarray as xr
-
-from PyQt5.QtWidgets import QLabel, QWidget, QGridLayout
-
+from anndata import AnnData
 from napari import Viewer
 from napari.layers import Points, Shapes
+from pandas.core.dtypes.common import is_categorical_dtype
+from PyQt5.QtWidgets import QGridLayout, QLabel, QWidget
+from scanpy import logging as logg
 
-from squidpy.im import ImageContainer  # type: ignore[attr-defined]
 from squidpy._docs import d
 from squidpy._utils import NDArrayA, singledispatchmethod
-from squidpy.pl._utils import _points_inside_triangles
-from squidpy.pl._interactive._view import ImageView
+from squidpy.im import ImageContainer  # type: ignore[attr-defined]
 from squidpy.pl._interactive._model import ImageModel
 from squidpy.pl._interactive._utils import (
-    _get_categorical,
     _display_channelwise,
+    _get_categorical,
     _position_cluster_labels,
 )
+from squidpy.pl._interactive._view import ImageView
 from squidpy.pl._interactive._widgets import RangeSlider  # type: ignore[attr-defined]
+from squidpy.pl._utils import _points_inside_triangles
 
 __all__ = ["ImageController"]
 
 # label string: attribute name
 _WIDGETS_TO_HIDE = {
     "symbol:": "symbolComboBox",
     "point size:": "sizeSlider",
```

### Comparing `squidpy-1.2.3/squidpy/pl/_interactive/_model.py` & `squidpy-1.3.0/src/squidpy/pl/_interactive/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
-from typing import Sequence, TYPE_CHECKING
-from dataclasses import field, dataclass
-
-from anndata import AnnData
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Sequence
 
 import numpy as np
+from anndata import AnnData
 
-from squidpy.im import ImageContainer  # type: ignore[attr-defined]
-from squidpy._utils import NDArrayA, _unique_order_preserving
-from squidpy.gr._utils import _assert_spatial_basis, _assert_categorical_obs
-from squidpy.pl._utils import ALayer
-from squidpy.im._coords import CropCoords, CropPadding, _NULL_COORDS, _NULL_PADDING
 from squidpy._constants._constants import Symbol
 from squidpy._constants._pkg_constants import Key
+from squidpy._utils import NDArrayA, _unique_order_preserving
+from squidpy.gr._utils import _assert_categorical_obs, _assert_spatial_basis
+from squidpy.im import ImageContainer  # type: ignore[attr-defined]
+from squidpy.im._coords import _NULL_COORDS, _NULL_PADDING, CropCoords, CropPadding
+from squidpy.pl._utils import ALayer
 
 __all__ = ["ImageModel"]
 
 
 @dataclass
 class ImageModel:
     """Model which holds the data for interactive visualization."""
```

### Comparing `squidpy-1.2.3/squidpy/pl/_interactive/_utils.py` & `squidpy-1.3.0/src/squidpy/pl/_interactive/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
-from scanpy import logging as logg
+import dask.array as da
+import numpy as np
+import pandas as pd
 from anndata import AnnData
-from scanpy.plotting._utils import add_colors_for_categorical_sample_annotation
-
+from matplotlib.colors import to_hex, to_rgb
 from numba import njit
-from scipy.spatial import KDTree
 from pandas._libs.lib import infer_dtype
 from pandas.core.dtypes.common import is_categorical_dtype
-import numpy as np
-import pandas as pd
-import dask.array as da
-
-from matplotlib.colors import to_hex, to_rgb
+from scanpy import logging as logg
+from scanpy.plotting._utils import add_colors_for_categorical_sample_annotation
+from scipy.spatial import KDTree
 
-from squidpy._utils import NDArrayA
 from squidpy._constants._pkg_constants import Key
+from squidpy._utils import NDArrayA
 
 
 def _get_categorical(
     adata: AnnData,
     key: str,
     palette: str | None = None,
     vec: pd.Series | None = None,
```

### Comparing `squidpy-1.2.3/squidpy/pl/_interactive/_view.py` & `squidpy-1.3.0/src/squidpy/pl/_interactive/_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from __future__ import annotations
 
 from typing import Any
 
-from scanpy import logging as logg
-
+import napari
 import numpy as np
-
-from PyQt5.QtWidgets import QLabel, QWidget, QComboBox, QHBoxLayout
-
 from napari.layers import Points
-import napari
+from PyQt5.QtWidgets import QComboBox, QHBoxLayout, QLabel, QWidget
+from scanpy import logging as logg
 
 from squidpy.pl._interactive._model import ImageModel
 from squidpy.pl._interactive._widgets import (  # type: ignore[attr-defined]
-    CBarWidget,
     AListWidget,
+    CBarWidget,
+    LibraryListWidget,
     ObsmIndexWidget,
     TwoStateCheckBox,
-    LibraryListWidget,
 )
 
 __all__ = ["ImageView"]
 
 
 class ImageView:
     """
```

### Comparing `squidpy-1.2.3/squidpy/pl/_interactive/_widgets.py` & `squidpy-1.3.0/src/squidpy/pl/_interactive/_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # type: ignore
 from __future__ import annotations
 
 from abc import abstractmethod
-from vispy import scene
-from typing import Any, Tuple, Iterable
-from vispy.scene.widgets import ColorBarWidget
-from vispy.color.colormap import Colormap, MatplotlibColormap
-
-from scanpy import logging as logg
+from typing import Any, Iterable, Tuple
 
 import numpy as np
 import pandas as pd
-
+from napari.layers import Points
 from PyQt5 import QtCore, QtWidgets
-from superqt import QRangeSlider
 from PyQt5.QtCore import Qt
-
-from napari.layers import Points
+from scanpy import logging as logg
+from superqt import QRangeSlider
+from vispy import scene
+from vispy.color.colormap import Colormap, MatplotlibColormap
+from vispy.scene.widgets import ColorBarWidget
 
 from squidpy.pl._utils import ALayer
 
 __all__ = ["TwoStateCheckBox", "AListWidget", "CBarWidget", "RangeSlider", "ObsmIndexWidget", "LibraryListWidget"]
 
 
 class ListWidget(QtWidgets.QListWidget):
@@ -136,15 +133,15 @@
         self.clear()
         self.addItems(self._alayer.get_items(self._attr))
 
     def _onAction(self, items: Iterable[str]) -> None:
         for item in sorted(set(items)):
             try:
                 vec, name = self._getter(item, index=self.getIndex())
-            except Exception as e:  # noqa: B902
+            except Exception as e:  # noqa: BLE001
                 logg.error(e)
                 continue
             self._controller.add_points(vec, key=item, layer_name=name)
 
     def setRaw(self, is_raw: bool) -> None:
         if is_raw == self.getRaw():
             return
@@ -300,28 +297,28 @@
         return self._cmap
 
     def onCmapChanged(self, value: str) -> None:
         # this does not trigger update for some reason...
         self._colorbar.cmap = self._create_colormap(value)
         self._colorbar._colorbar._update()
 
-    def setClim(self, value: Tuple[float, float]) -> None:
+    def setClim(self, value: tuple[float, float]) -> None:
         if value == self._clim:
             return
 
         self._clim = value
         self.climChanged.emit(*value)
 
-    def getClim(self) -> Tuple[float, float]:
+    def getClim(self) -> tuple[float, float]:
         return self._clim
 
-    def getOclim(self) -> Tuple[float, float]:
+    def getOclim(self) -> tuple[float, float]:
         return self._oclim
 
-    def setOclim(self, value: Tuple[float, float]) -> None:
+    def setOclim(self, value: tuple[float, float]) -> None:
         # original color limit used for 0-1 normalization
         self._oclim = value
 
     def onClimChanged(self, minn: float, maxx: float) -> None:
         # ticks are not working with vispy's colorbar
         self._colorbar.cmap = self._create_colormap(self.getCmap())
         self._colorbar.clim = (self.FORMAT.format(minn), self.FORMAT.format(maxx))
@@ -353,15 +350,15 @@
         self.setValue((0, 100))
         self.setSliderPosition((0, 100))
         self.setSingleStep(0.01)
         self.setOrientation(Qt.Horizontal)
 
         self.valueChanged.connect(self._onValueChange)
 
-    def _onValueChange(self, percentile: Tuple[float, float]) -> None:
+    def _onValueChange(self, percentile: tuple[float, float]) -> None:
         # TODO(michalk8): use constants
         v = self._layer.metadata["data"]
         clipped = np.clip(v, *np.percentile(v, percentile))
 
         self._layer.metadata = {**self._layer.metadata, "perc": percentile}
         self._layer.face_color = "value"
         self._layer.properties = {"value": clipped}
```

### Comparing `squidpy-1.2.3/squidpy/pl/_interactive/interactive.py` & `squidpy-1.3.0/src/squidpy/pl/_interactive/interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Any
-
-from scanpy import logging as logg
-from anndata import AnnData
+from typing import (
+    Any,
+    Union,  # noqa: F401
+)
 
 import matplotlib.pyplot as plt
+from anndata import AnnData
+from scanpy import logging as logg
 
-from squidpy.im import ImageContainer  # type: ignore[attr-defined]
 from squidpy._docs import d
 from squidpy._utils import NDArrayA
+from squidpy.im import ImageContainer  # type: ignore[attr-defined]
 from squidpy.pl._utils import save_fig
 
 try:
     from squidpy.pl._interactive._controller import ImageController
 except ImportError as e:
     _error: str | None = str(e)
 else:
```

### Comparing `squidpy-1.2.3/squidpy/pl/_ligrec.py` & `squidpy-1.3.0/src/squidpy/pl/_ligrec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Any, Mapping, Sequence, TYPE_CHECKING
 from pathlib import Path
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Mapping,
+    Sequence,
+    Union,  # noqa: F401
+)
 
-from scanpy import logging as logg
-from anndata import AnnData
-import scanpy as sc
-
-from scipy.cluster import hierarchy as sch
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
+import scanpy as sc
+from anndata import AnnData
 from matplotlib.axes import Axes
 from matplotlib.colorbar import ColorbarBase
-import matplotlib.pyplot as plt
+from scanpy import logging as logg
+from scipy.cluster import hierarchy as sch
 
-from squidpy._docs import d
-from squidpy._utils import verbosity, _unique_order_preserving
-from squidpy.pl._utils import save_fig, _dendrogram, _filter_kwargs
 from squidpy._constants._constants import DendrogramAxis
 from squidpy._constants._pkg_constants import Key
+from squidpy._docs import d
+from squidpy._utils import _unique_order_preserving, verbosity
+from squidpy.pl._utils import _dendrogram, _filter_kwargs, save_fig
 
 __all__ = ["ligrec"]
 
 _SEP = " | "  # cluster separator
 
 
 class CustomDotplot(sc.pl.DotPlot):
-
     BASE = 10
 
     DEFAULT_LARGEST_DOT = 50.0
     DEFAULT_NUM_COLORBAR_TICKS = 5
     DEFAULT_NUM_LEGEND_DOTS = 5
 
     def __init__(self, minn: float, delta: float, alpha: float | None, *args: Any, **kwargs: Any):
@@ -261,14 +263,23 @@
     elif isinstance(source_groups, str):
         source_groups = (source_groups,)
 
     if target_groups is None:
         target_groups = adata["pvalues"].columns.get_level_values(1)
     if isinstance(target_groups, str):
         target_groups = (target_groups,)
+
+    if not isinstance(adata, AnnData):
+        for s in source_groups:
+            if s not in adata["means"].columns.get_level_values(0):
+                raise ValueError(f"Invalid cluster in source group: {s}.")
+        for t in target_groups:
+            if t not in adata["means"].columns.get_level_values(1):
+                raise ValueError(f"Invalid cluster in target group: {t}.")
+
     if title is None:
         title = "Receptor-ligand test"
 
     source_groups, _ = _unique_order_preserving(source_groups)  # type: ignore[assignment]
     target_groups, _ = _unique_order_preserving(target_groups)  # type: ignore[assignment]
 
     pvals: pd.DataFrame = adata["pvalues"].loc[:, (source_groups, target_groups)]
@@ -289,18 +300,14 @@
 
     if dendrogram == DendrogramAxis.INTERACTING_CLUSTERS:
         # rows are now cluster combinations, not interacting pairs
         pvals = pvals.T
         means = means.T
 
     for cls, size in (pvals.groupby(level=0, axis=1)).size().to_dict().items():
-        size = np.unique(list(size.values()))
-        if len(size) != 1:
-            raise ValueError(f"Expected all groups to have the same number of interacting clusters, found `{size}`.")
-        size = size[0]
         label_ranges[cls] = (start, start + size - 1)
         start += size
     label_ranges = {k: label_ranges[k] for k in sorted(label_ranges.keys())}
 
     pvals = pvals[label_ranges.keys()]
     pvals = -np.log10(pvals + min(1e-3, alpha if alpha is not None else 1e-3)).fillna(0)
 
@@ -330,15 +337,15 @@
             pvals = pvals.iloc[row_order, :].iloc[:, col_order]
             means = means.iloc[row_order, :].iloc[:, col_order]
         elif dendrogram is not None:
             adata.uns["dendrogram"] = get_dendrogram(adata)
     except IndexError:
         # just in case pandas indexing fails
         raise
-    except Exception as e:
+    except Exception as e:  # noqa: BLE001
         logg.warning(f"Unable to create a dendrogram. Reason: `{e}`")
         dendrogram = None
 
     kwargs["dot_edge_lw"] = 0
     kwargs.setdefault("cmap", "viridis")
     kwargs.setdefault("grid", True)
     kwargs.pop("color_on", None)  # interferes with tori
```

### Comparing `squidpy-1.2.3/squidpy/pl/_spatial.py` & `squidpy-1.3.0/src/squidpy/pl/_spatial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,123 +1,124 @@
-from types import MappingProxyType
-from typing import Any, List, Tuple, Union, Mapping, Callable, Optional, Sequence
-from pathlib import Path
+from __future__ import annotations
+
 import itertools
+from pathlib import Path
+from types import MappingProxyType
+from typing import Any, Callable, List, Mapping, Optional, Sequence, Tuple, Union
 
 from anndata import AnnData
-
 from matplotlib.axes import Axes
 from matplotlib.colors import Colormap
 from matplotlib.figure import Figure
 
+from squidpy._constants._constants import ScatterShape
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d
 from squidpy.gr._utils import _assert_spatial_basis
-from squidpy.pl._utils import save_fig, sanitize_anndata
 from squidpy.pl._spatial_utils import (
-    _subs,
-    _SeqStr,
-    _FontSize,
-    _SeqArray,
-    _SeqFloat,
     Palette_t,
-    _Normalize,
+    _AvailShapes,
     _CoordTuple,
+    _decorate_axs,
+    _FontSize,
     _FontWeight,
+    _image_spatial_attrs,
+    _Normalize,
     _plot_edges,
-    _AvailShapes,
-    _set_outline,
-    _decorate_axs,
     _plot_scatter,
     _plot_segment,
-    _set_ax_title,
-    _set_coords_crops,
     _prepare_args_plot,
-    _image_spatial_attrs,
     _prepare_params_plot,
+    _SeqArray,
+    _SeqFloat,
+    _SeqStr,
+    _set_ax_title,
     _set_color_source_vec,
+    _set_coords_crops,
+    _set_outline,
+    _subs,
 )
-from squidpy._constants._constants import ScatterShape
-from squidpy._constants._pkg_constants import Key
+from squidpy.pl._utils import sanitize_anndata, save_fig
 
 
 @d.get_sections(base="spatial_plot", sections=["Returns"])
 @d.get_extended_summary(base="spatial_plot")
 @d.dedent
 def _spatial_plot(
     adata: AnnData,
-    shape: Optional[_AvailShapes] = None,
-    color: Optional[Union[str, Sequence[Optional[str]]]] = None,
-    groups: Optional[_SeqStr] = None,
-    library_id: Optional[_SeqStr] = None,
-    library_key: Optional[str] = None,
+    shape: _AvailShapes | None = None,
+    color: str | Sequence[str | None] | None = None,
+    groups: _SeqStr | None = None,
+    library_id: _SeqStr | None = None,
+    library_key: str | None = None,
     spatial_key: str = Key.obsm.spatial,
     # image
-    img: Optional[Union[bool, _SeqArray]] = True,
-    img_res_key: Optional[str] = Key.uns.image_res_key,
-    img_alpha: Optional[float] = None,
-    img_cmap: Union[Colormap, Optional[str]] = None,
-    img_channel: Optional[Union[int, List[int]]] = None,
+    img: bool | _SeqArray | None = True,
+    img_res_key: str | None = Key.uns.image_res_key,
+    img_alpha: float | None = None,
+    img_cmap: Colormap | str | None = None,
+    img_channel: int | list[int] | None = None,
     # segment
-    seg: Optional[Union[bool, _SeqArray]] = None,
-    seg_key: Optional[str] = Key.uns.image_seg_key,
-    seg_cell_id: Optional[str] = None,
-    seg_contourpx: Optional[int] = None,
+    seg: bool | _SeqArray | None = None,
+    seg_key: str | None = Key.uns.image_seg_key,
+    seg_cell_id: str | None = None,
+    seg_contourpx: int | None = None,
     seg_outline: bool = False,
     # features
-    use_raw: Optional[bool] = None,
-    layer: Optional[str] = None,
-    alt_var: Optional[str] = None,
+    use_raw: bool | None = None,
+    layer: str | None = None,
+    alt_var: str | None = None,
     # size, coords, cmap, palette
-    size: Optional[_SeqFloat] = None,
-    size_key: Optional[str] = Key.uns.size_key,
-    scale_factor: Optional[_SeqFloat] = None,
-    crop_coord: Optional[Union[_CoordTuple, Sequence[_CoordTuple]]] = None,
-    cmap: Optional[Union[str, Colormap]] = None,
+    size: _SeqFloat | None = None,
+    size_key: str | None = Key.uns.size_key,
+    scale_factor: _SeqFloat | None = None,
+    crop_coord: _CoordTuple | Sequence[_CoordTuple] | None = None,
+    cmap: str | Colormap | None = None,
     palette: Palette_t = None,
     alpha: float = 1.0,
-    norm: Optional[_Normalize] = None,
-    na_color: Union[str, Tuple[float, ...]] = (0, 0, 0, 0),
+    norm: _Normalize | None = None,
+    na_color: str | tuple[float, ...] = (0, 0, 0, 0),
     # edges
-    connectivity_key: Optional[str] = None,
+    connectivity_key: str | None = None,
     edges_width: float = 1.0,
-    edges_color: Union[str, Sequence[str], Sequence[float]] = "grey",
+    edges_color: str | Sequence[str] | Sequence[float] = "grey",
     # panels
     library_first: bool = True,
-    frameon: Optional[bool] = None,
-    wspace: Optional[float] = None,
+    frameon: bool | None = None,
+    wspace: float | None = None,
     hspace: float = 0.25,
     ncols: int = 4,
     # outline
     outline: bool = False,
-    outline_color: Tuple[str, str] = ("black", "white"),
-    outline_width: Tuple[float, float] = (0.3, 0.05),
+    outline_color: tuple[str, str] = ("black", "white"),
+    outline_width: tuple[float, float] = (0.3, 0.05),
     # legend
-    legend_loc: Optional[str] = "right margin",
-    legend_fontsize: Optional[Union[int, float, _FontSize]] = None,
-    legend_fontweight: Union[int, _FontWeight] = "bold",
-    legend_fontoutline: Optional[int] = None,
+    legend_loc: str | None = "right margin",
+    legend_fontsize: int | float | _FontSize | None = None,
+    legend_fontweight: int | _FontWeight = "bold",
+    legend_fontoutline: int | None = None,
     legend_na: bool = True,
     colorbar: bool = True,
     # scalebar
-    scalebar_dx: Optional[_SeqFloat] = None,
-    scalebar_units: Optional[_SeqStr] = None,
+    scalebar_dx: _SeqFloat | None = None,
+    scalebar_units: _SeqStr | None = None,
     # title and axis
-    title: Optional[_SeqStr] = None,
-    axis_label: Optional[_SeqStr] = None,
-    fig: Optional[Figure] = None,
-    ax: Optional[Union[Axes, Sequence[Axes]]] = None,
+    title: _SeqStr | None = None,
+    axis_label: _SeqStr | None = None,
+    fig: Figure | None = None,
+    ax: Axes | Sequence[Axes] | None = None,
     return_ax: bool = False,
-    figsize: Optional[Tuple[float, float]] = None,
-    dpi: Optional[int] = None,
-    save: Optional[Union[str, Path]] = None,
+    figsize: tuple[float, float] | None = None,
+    dpi: int | None = None,
+    save: str | Path | None = None,
     # kwargs
     scalebar_kwargs: Mapping[str, Any] = MappingProxyType({}),
     edges_kwargs: Mapping[str, Any] = MappingProxyType({}),
     **kwargs: Any,
-) -> Optional[Union[Axes, Sequence[Axes]]]:
+) -> Axes | Sequence[Axes] | None:
     """
     Plot spatial omics data.
 
     Use ``library_id`` to select the image. If multiple ``library_id`` are available, use ``library_key`` in
     :attr:`anndata.AnnData.obs` to plot the subsets.
     Use ``crop_coord`` to crop the spatial plot based on coordinate boundaries.
 
@@ -374,17 +375,17 @@
     return wrapper
 
 
 @d.dedent
 @_wrap_signature
 def spatial_scatter(
     adata: AnnData,
-    shape: Optional[_AvailShapes] = ScatterShape.CIRCLE.v,
+    shape: _AvailShapes | None = ScatterShape.CIRCLE.v,
     **kwargs: Any,
-) -> Optional[Union[Axes, Sequence[Axes]]]:
+) -> Axes | Sequence[Axes] | None:
     """
     Plot spatial omics data with data overlayed on top.
 
     The plotted shapes (circles, squares or hexagons) have a real "size" with respect to their
     coordinate space, which can be specified via the ``size`` or ``size_key`` argument.
 
         - Use ``img_key`` to display the image in the background.
@@ -419,20 +420,20 @@
 
 
 @d.dedent  # type: ignore[arg-type]
 @_wrap_signature
 def spatial_segment(
     adata: AnnData,
     seg_cell_id: str,
-    seg: Optional[Union[bool, _SeqArray]] = True,
+    seg: bool | _SeqArray | None = True,
     seg_key: str = Key.uns.image_seg_key,
-    seg_contourpx: Optional[int] = None,
+    seg_contourpx: int | None = None,
     seg_outline: bool = False,
     **kwargs: Any,
-) -> Optional[Union[Axes, Sequence[Axes]]]:
+) -> Axes | Sequence[Axes] | None:
     """
     Plot spatial omics data with segmentation masks on top.
 
     Argument ``seg_cell_id`` in :attr:`anndata.AnnData.obs` controls unique segmentation mask's ids to be plotted.
     By default, ``'segmentation'``, ``seg_key`` for the segmentation and ``'hires'`` for the image is attempted.
 
         - Use ``seg_key`` to display the image in the background.
```

### Comparing `squidpy-1.2.3/squidpy/pl/_spatial_utils.py` & `squidpy-1.3.0/src/squidpy/pl/_spatial_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 from __future__ import annotations
 
+import itertools
 from copy import copy
+from functools import partial
+from numbers import Number
 from types import MappingProxyType
 from typing import (
+    TYPE_CHECKING,
     Any,
     List,
-    Type,
-    Tuple,
-    Union,
     Literal,
     Mapping,
+    NamedTuple,
     Optional,
     Sequence,
-    NamedTuple,
-    TYPE_CHECKING,
+    Tuple,
+    Type,
+    Union,
 )
-from numbers import Number
-from functools import partial
-from matplotlib_scalebar.scalebar import ScaleBar
-import itertools
-
-from scanpy import logging as logg
-from anndata import AnnData
-from scanpy._settings import settings as sc_settings
-from scanpy.plotting._tools.scatterplots import _add_categorical_legend
 
-from pandas.api.types import CategoricalDtype
-from pandas.core.dtypes.common import is_categorical_dtype
+import dask.array as da
 import numpy as np
 import pandas as pd
-import dask.array as da
-
-from matplotlib import colors, pyplot as plt, rcParams, patheffects
-from matplotlib.cm import get_cmap
+from anndata import AnnData
+from matplotlib import colors, patheffects, rcParams
+from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
+from matplotlib.cm import get_cmap
+from matplotlib.collections import Collection, PatchCollection
 from matplotlib.colors import (
+    ColorConverter,
     Colormap,
+    ListedColormap,
     Normalize,
     TwoSlopeNorm,
-    ColorConverter,
-    ListedColormap,
 )
 from matplotlib.figure import Figure
-from matplotlib.patches import Circle, Polygon, Rectangle
 from matplotlib.gridspec import GridSpec
-from matplotlib.collections import Collection, PatchCollection
-
-from skimage.util import map_array
+from matplotlib.patches import Circle, Polygon, Rectangle
+from matplotlib_scalebar.scalebar import ScaleBar
+from pandas.api.types import CategoricalDtype
+from pandas.core.dtypes.common import is_categorical_dtype
+from scanpy import logging as logg
+from scanpy._settings import settings as sc_settings
+from scanpy.plotting._tools.scatterplots import _add_categorical_legend
 from skimage.color import label2rgb
-from skimage.morphology import square, erosion
+from skimage.morphology import erosion, square
 from skimage.segmentation import find_boundaries
+from skimage.util import map_array
 
+from squidpy._constants._constants import ScatterShape
+from squidpy._constants._pkg_constants import Key
 from squidpy._utils import NDArrayA
-from squidpy.pl._utils import _assert_value_in_obs
 from squidpy.im._coords import CropCoords
 from squidpy.pl._color_utils import _get_palette, _maybe_set_colors
-from squidpy._constants._constants import ScatterShape
-from squidpy._constants._pkg_constants import Key
+from squidpy.pl._utils import _assert_value_in_obs
 
 _AvailShapes = Literal["circle", "square", "hex"]
 Palette_t = Optional[Union[str, ListedColormap]]
 _Normalize = Union[Normalize, Sequence[Normalize]]
 _SeqStr = Union[str, Sequence[str]]
 _SeqFloat = Union[float, Sequence[float]]
 _SeqArray = Union[NDArrayA, Sequence[NDArrayA]]
@@ -72,15 +70,15 @@
 # named tuples
 class FigParams(NamedTuple):
     """Figure params."""
 
     fig: Figure
     ax: Axes
     axs: Sequence[Axes] | None
-    iter_panels: Tuple[Sequence[Any], Sequence[Any]]
+    iter_panels: tuple[Sequence[Any], Sequence[Any]]
     title: _SeqStr | None
     ax_labels: Sequence[str]
     frameon: bool | None
 
 
 class CmapParams(NamedTuple):
     """Cmap params."""
@@ -120,17 +118,17 @@
 
 class SpatialParams(NamedTuple):
     """Color params."""
 
     library_id: Sequence[str]
     scale_factor: Sequence[float]
     size: Sequence[float]
-    img: Sequence[NDArrayA] | Tuple[None, ...]
-    segment: Sequence[NDArrayA] | Tuple[None, ...]
-    cell_id: Sequence[NDArrayA] | Tuple[None, ...]
+    img: Sequence[NDArrayA] | tuple[None, ...]
+    segment: Sequence[NDArrayA] | tuple[None, ...]
+    cell_id: Sequence[NDArrayA] | tuple[None, ...]
 
 
 to_hex = partial(colors.to_hex, keep_alpha=True)
 
 
 def _get_library_id(
     adata: AnnData,
@@ -167,17 +165,17 @@
 
 def _get_image(
     adata: AnnData,
     library_id: Sequence[str],
     spatial_key: str = Key.obsm.spatial,
     img: bool | _SeqArray | None = None,
     img_res_key: str | None = None,
-    img_channel: int | List[int] | None = None,
+    img_channel: int | list[int] | None = None,
     img_cmap: Colormap | str | None = None,
-) -> Union[Sequence[NDArrayA], Tuple[None, ...]]:
+) -> Sequence[NDArrayA] | tuple[None, ...]:
     from squidpy.pl._utils import _to_grayscale
 
     if isinstance(img, (list, np.ndarray, da.Array)):
         img = _get_list(img, _type=(np.ndarray, da.Array), ref_len=len(library_id), name="img")
     else:
         image_mapping = Key.uns.library_mapping(adata, spatial_key, Key.uns.image_key, library_id)
         if img_res_key is None:
@@ -205,15 +203,15 @@
 def _get_segment(
     adata: AnnData,
     library_id: Sequence[str],
     seg_cell_id: str | None = None,
     library_key: str | None = None,
     seg: _SeqArray | bool | None = None,
     seg_key: str | None = None,
-) -> Tuple[Sequence[NDArrayA], Sequence[NDArrayA]] | Tuple[Tuple[None, ...], Tuple[None, ...]]:
+) -> tuple[Sequence[NDArrayA], Sequence[NDArrayA]] | tuple[tuple[None, ...], tuple[None, ...]]:
     if seg_cell_id not in adata.obs:
         raise ValueError(f"Cell id `{seg_cell_id!r}` not found in `adata.obs`.")
     cell_id_vec = adata.obs[seg_cell_id].values
 
     if library_key not in adata.obs:
         raise ValueError(f"Library key `{library_key}` not found in `adata.obs`.")
     if not np.issubdtype(cell_id_vec.dtype, np.integer):
@@ -231,15 +229,15 @@
     adata: AnnData,
     library_id: Sequence[str],
     spatial_key: str = Key.obsm.spatial,
     img_res_key: str | None = None,
     scale_factor: _SeqFloat | None = None,
     size: _SeqFloat | None = None,
     size_key: str | None = Key.uns.size_key,
-) -> Tuple[Sequence[float], Sequence[float]]:
+) -> tuple[Sequence[float], Sequence[float]]:
     try:
         scalefactor_mapping = Key.uns.library_mapping(adata, spatial_key, Key.uns.scalefactor_key, library_id)
         scalefactors = _get_unique_map(scalefactor_mapping)
     except KeyError as e:
         scalefactors = None
         logg.debug(f"Setting `scalefactors={scalefactors}`, reason: `{e}`")
 
@@ -283,15 +281,15 @@
     adata: AnnData,
     shape: _AvailShapes | None = None,
     spatial_key: str = Key.obsm.spatial,
     library_id: Sequence[str] | None = None,
     library_key: str | None = None,
     img: bool | _SeqArray | None = None,
     img_res_key: str | None = Key.uns.image_res_key,
-    img_channel: int | List[int] | None = None,
+    img_channel: int | list[int] | None = None,
     seg: _SeqArray | bool | None = None,
     seg_key: str | None = None,
     cell_id_key: str | None = None,
     scale_factor: _SeqFloat | None = None,
     size: _SeqFloat | None = None,
     size_key: str | None = Key.uns.size_key,
     img_cmap: Colormap | str | None = None,
@@ -349,15 +347,15 @@
 
 
 def _set_coords_crops(
     adata: AnnData,
     spatial_params: SpatialParams,
     spatial_key: str,
     crop_coord: Sequence[_CoordTuple] | _CoordTuple | None = None,
-) -> Tuple[List[NDArrayA], List[CropCoords] | List[None]]:
+) -> tuple[list[NDArrayA], list[CropCoords] | list[None]]:
     if crop_coord is None:
         crops = [None] * len(spatial_params.library_id)
     else:
         crop_coord = _get_list(crop_coord, _type=tuple, ref_len=len(spatial_params.library_id), name="crop_coord")
         crops = [CropCoords(*cr) * sf for cr, sf in zip(crop_coord, spatial_params.scale_factor)]  # type: ignore[misc]
 
     coords = adata.obsm[spatial_key]
@@ -380,29 +378,29 @@
         return adata
 
     def subset_by_key(
         adata: AnnData,
         coords: NDArrayA,
         key: str | None,
         values: Sequence[Any] | None,
-    ) -> Tuple[AnnData, NDArrayA]:
+    ) -> tuple[AnnData, NDArrayA]:
         if key is None or values is None:
             return adata, coords
         if key not in adata.obs or not is_categorical_dtype(adata.obs[key]):
             return adata, coords
         try:
             mask = adata.obs[key].isin(values).values
             msg = f"None of `adata.obs[{key}]` are in `{values}`"
             return assert_notempty(adata[mask], msg=msg), coords[mask]
         except KeyError:
             raise KeyError(f"Unable to find `{key!r}` in `adata.obs`.") from None
 
     def subset_by_coords(
         adata: AnnData, coords: NDArrayA, img: NDArrayA | None, crop_coords: CropCoords | None
-    ) -> Tuple[AnnData, NDArrayA, NDArrayA | None]:
+    ) -> tuple[AnnData, NDArrayA, NDArrayA | None]:
         if crop_coords is None:
             return adata, coords, img
 
         mask = (
             (coords[:, 0] >= crop_coords.x0)
             & (coords[:, 0] <= crop_coords.x1)
             & (coords[:, 1] >= crop_coords.y0)
@@ -425,18 +423,18 @@
 def _get_unique_map(dic: Mapping[str, Any]) -> Sequence[Any]:
     """Get intersection of dict values."""
     return sorted(set.intersection(*map(set, dic.values())))
 
 
 def _get_list(
     var: Any,
-    _type: Type[Any] | Tuple[Type[Any], ...],
+    _type: type[Any] | tuple[type[Any], ...],
     ref_len: int | None = None,
     name: str | None = None,
-) -> List[Any]:
+) -> list[Any]:
     if isinstance(var, _type):
         return [var] if ref_len is None else ([var] * ref_len)
     if isinstance(var, list):
         if ref_len is not None and ref_len != len(var):
             raise ValueError(
                 f"Variable: `{name}` has length: {len(var)}, which is not equal to reference length: {ref_len}."
             )
@@ -452,19 +450,20 @@
     adata: AnnData,
     value_to_plot: str | None,
     use_raw: bool | None = None,
     alt_var: str | None = None,
     layer: str | None = None,
     groups: _SeqStr | None = None,
     palette: Palette_t = None,
-    na_color: str | Tuple[float, ...] | None = None,
+    na_color: str | tuple[float, ...] | None = None,
     alpha: float = 1.0,
-) -> Tuple[NDArrayA | pd.Series | None, NDArrayA, bool]:
+) -> tuple[NDArrayA | pd.Series | None, NDArrayA, bool]:
     if value_to_plot is None:
-        return np.full(adata.n_obs, to_hex(na_color)), np.broadcast_to(np.nan, adata.n_obs), False
+        color = np.full(adata.n_obs, to_hex(na_color))
+        return color, color, False
 
     if alt_var is not None and value_to_plot not in adata.obs and value_to_plot not in adata.var_names:
         value_to_plot = adata.var_names[adata.var[alt_var] == value_to_plot][0]
     if use_raw and value_to_plot not in adata.obs:
         color_source_vector = adata.raw.obs_vector(value_to_plot)
     else:
         color_source_vector = adata.obs_vector(value_to_plot, layer=layer)
@@ -529,15 +528,15 @@
         alpha = ColorConverter().to_rgba_array(c)[..., -1]
         collection.set_facecolor(c)
         collection.set_alpha(alpha)
 
     return collection
 
 
-def _make_poly(x: NDArrayA, y: NDArrayA, r: float, n: int, i: int) -> Tuple[NDArrayA, NDArrayA]:
+def _make_poly(x: NDArrayA, y: NDArrayA, r: float, n: int, i: int) -> tuple[NDArrayA, NDArrayA]:
     x_i = x + r * np.sin((np.pi / n) * (1 + 2 * i))
     y_i = y + r * np.cos((np.pi / n) * (1 + 2 * i))
     return x_i, y_i
 
 
 def _plot_edges(
     adata: AnnData,
@@ -564,15 +563,15 @@
     )
     edge_collection.set_rasterized(sc_settings._vector_friendly)
     ax.add_collection(edge_collection)
 
 
 def _get_title_axlabels(
     title: _SeqStr | None, axis_label: _SeqStr | None, spatial_key: str, n_plots: int
-) -> Tuple[_SeqStr | None, Sequence[str]]:
+) -> tuple[_SeqStr | None, Sequence[str]]:
     if title is not None:
         if isinstance(title, (tuple, list)) and len(title) != n_plots:
             raise ValueError(f"Expected `{n_plots}` titles, found `{len(title)}`.")
         elif isinstance(title, str):
             title = [title] * n_plots
     else:
         title = None
@@ -590,15 +589,15 @@
     return title, axis_labels
 
 
 def _get_scalebar(
     scalebar_dx: _SeqFloat | None = None,
     scalebar_units: _SeqStr | None = None,
     len_lib: int | None = None,
-) -> Tuple[Sequence[float] | None, Sequence[str] | None]:
+) -> tuple[Sequence[float] | None, Sequence[str] | None]:
     if scalebar_dx is not None:
         _scalebar_dx = _get_list(scalebar_dx, _type=float, ref_len=len_lib, name="scalebar_dx")
         scalebar_units = "um" if scalebar_units is None else scalebar_units
         _scalebar_units = _get_list(scalebar_units, _type=str, ref_len=len_lib, name="scalebar_units")
     else:
         _scalebar_dx = None
         _scalebar_units = None
@@ -620,15 +619,15 @@
     img_alpha: float | None = None,
     palette: Palette_t = None,
     alpha: float = 1.0,
     legend_fontsize: int | float | _FontSize | None = None,
     legend_fontweight: int | _FontWeight = "bold",
     legend_loc: str | None = "right margin",
     legend_fontoutline: int | None = None,
-    na_color: str | Tuple[float, ...] = (0.0, 0.0, 0.0, 0.0),
+    na_color: str | tuple[float, ...] = (0.0, 0.0, 0.0, 0.0),
     na_in_legend: bool = True,
     colorbar: bool = True,
     scalebar_dx: Sequence[float] | None = None,
     scalebar_units: Sequence[str] | None = None,
     scalebar_kwargs: Mapping[str, Any] = MappingProxyType({}),
 ) -> Axes:
     ax.set_yticks([])
@@ -684,26 +683,30 @@
     seg: NDArrayA,
     cell_id: NDArrayA,
     color_vector: NDArrayA | pd.Series[CategoricalDtype],
     color_source_vector: pd.Series[CategoricalDtype],
     cmap_params: CmapParams,
     seg_erosionpx: int | None = None,
     seg_boundaries: bool = False,
-    na_color: str | Tuple[float, ...] = (0, 0, 0, 0),
+    na_color: str | tuple[float, ...] = (0, 0, 0, 0),
 ) -> NDArrayA:
     cell_id = np.array(cell_id)
 
     if is_categorical_dtype(color_vector):
         if isinstance(na_color, tuple) and len(na_color) == 4 and np.any(color_source_vector.isna()):
             cell_id[color_source_vector.isna()] = 0
         val_im: NDArrayA = map_array(seg, cell_id, color_vector.codes + 1)  # type: ignore
         cols = colors.to_rgba_array(color_vector.categories)  # type: ignore
     else:
         val_im = map_array(seg, cell_id, cell_id)  # replace with same seg id to remove missing segs
-        cols = cmap_params.cmap(cmap_params.norm(color_vector))
+        try:
+            cols = cmap_params.cmap(cmap_params.norm(color_vector))
+        except TypeError:
+            assert all(colors.is_color_like(c) for c in color_vector), "Not all values are color-like."
+            cols = colors.to_rgba_array(color_vector)
 
     if seg_erosionpx is not None:
         val_im[val_im == erosion(val_im, square(seg_erosionpx))] = 0
 
     seg_im: NDArrayA = label2rgb(
         label=val_im,
         colors=cols,
@@ -770,45 +773,45 @@
     hspace: float = 0.25,
     ncols: int = 4,
     cmap: Colormap | str | None = None,
     norm: _Normalize | None = None,
     library_first: bool = True,
     img_cmap: Colormap | str | None = None,
     frameon: bool | None = None,
-    na_color: str | Tuple[float, ...] | None = (0.0, 0.0, 0.0, 0.0),
+    na_color: str | tuple[float, ...] | None = (0.0, 0.0, 0.0, 0.0),
     vmin: float | None = None,
     vmax: float | None = None,
     vcenter: float | None = None,
     title: _SeqStr | None = None,
     axis_label: _SeqStr | None = None,
     scalebar_dx: _SeqFloat | None = None,
     scalebar_units: _SeqStr | None = None,
-    figsize: Tuple[float, float] | None = None,
+    figsize: tuple[float, float] | None = None,
     dpi: int | None = None,
     fig: Figure | None = None,
     ax: Axes | Sequence[Axes] | None = None,
     **kwargs: Any,
-) -> Tuple[FigParams, CmapParams, ScalebarParams, Any]:
+) -> tuple[FigParams, CmapParams, ScalebarParams, Any]:
     if library_first:
-        iter_panels: Tuple[range | Sequence[str | None], range | Sequence[str | None]] = (
+        iter_panels: tuple[range | Sequence[str | None], range | Sequence[str | None]] = (
             range(len(spatial_params.library_id)),
             color_params.color,
         )
     else:
         iter_panels = (color_params.color, range(len(spatial_params.library_id)))
     num_panels = len(list(itertools.product(*iter_panels)))
 
     wspace = 0.75 / rcParams["figure.figsize"][0] + 0.02 if wspace is None else wspace
     figsize = rcParams["figure.figsize"] if figsize is None else figsize
     dpi = rcParams["figure.dpi"] if dpi is None else dpi
     if num_panels > 1 and ax is None:
         fig, grid = _panel_grid(
             num_panels=num_panels, hspace=hspace, wspace=wspace, ncols=ncols, dpi=dpi, figsize=figsize
         )
-        axs: Union[Sequence[Axes], None] = [plt.subplot(grid[c]) for c in range(num_panels)]
+        axs: Sequence[Axes] | None = [plt.subplot(grid[c]) for c in range(num_panels)]
     elif num_panels > 1 and ax is not None:
         if len(ax) != num_panels:
             raise ValueError(f"Len of `ax`: {len(ax)} is not equal to number of panels: {num_panels}.")
         if fig is None:
             raise ValueError(
                 f"Invalid value of `fig`: {fig}. If a list of `Axes` is passed, a `Figure` must also be specified."
             )
@@ -844,17 +847,17 @@
 
 
 def _panel_grid(
     num_panels: int,
     hspace: float,
     wspace: float,
     ncols: int,
-    figsize: Tuple[float, float],
+    figsize: tuple[float, float],
     dpi: int | None = None,
-) -> Tuple[Figure, GridSpec]:
+) -> tuple[Figure, GridSpec]:
     n_panels_x = min(ncols, num_panels)
     n_panels_y = np.ceil(num_panels / n_panels_x).astype(int)
 
     fig = plt.figure(
         figsize=(figsize[0] * n_panels_x * (1 + wspace), figsize[1] * n_panels_y),
         dpi=dpi,
     )
@@ -887,19 +890,18 @@
         ax.set_title(fig_params.title[count])
     return ax
 
 
 def _set_outline(
     size: float,
     outline: bool = False,
-    outline_width: Tuple[float, float] = (0.3, 0.05),
-    outline_color: Tuple[str, str] = ("black", "white"),
+    outline_width: tuple[float, float] = (0.3, 0.05),
+    outline_color: tuple[str, str] = ("black", "white"),
     **kwargs: Any,
-) -> Tuple[OutlineParams, Any]:
-
+) -> tuple[OutlineParams, Any]:
     bg_width, gap_width = outline_width
     point = np.sqrt(size)
     gap_size = (point + (point * gap_width) * 2) ** 2
     bg_size = (np.sqrt(gap_size) + (point * bg_width) * 2) ** 2
     # the default black and white colors can be changes using the contour_config parameter
     bg_color, gap_color = outline_color
 
@@ -914,18 +916,17 @@
     coords: NDArrayA,
     ax: Axes,
     outline_params: OutlineParams,
     cmap_params: CmapParams,
     color_params: ColorParams,
     size: float,
     color_vector: NDArrayA,
-    na_color: str | Tuple[float, ...] = (0, 0, 0, 0),  # TODO(giovp): remove?
+    na_color: str | tuple[float, ...] = (0, 0, 0, 0),  # TODO(giovp): remove?
     **kwargs: Any,
-) -> Tuple[Axes, Collection | PatchCollection]:
-
+) -> tuple[Axes, Collection | PatchCollection]:
     if color_params.shape is not None:
         scatter = partial(_shaped_scatter, shape=color_params.shape, alpha=color_params.alpha)
     else:
         scatter = partial(ax.scatter, marker=".", alpha=color_params.alpha, plotnonfinite=True)
 
     # prevents reusing vmin/vmax when sharing a norm
     norm = copy(cmap_params.norm)
@@ -974,18 +975,17 @@
     color_source_vector: pd.Series[CategoricalDtype],
     ax: Axes,
     cmap_params: CmapParams,
     color_params: ColorParams,
     categorical: bool,
     seg_contourpx: int | None = None,
     seg_outline: bool = False,
-    na_color: str | Tuple[float, ...] = (0, 0, 0, 0),
+    na_color: str | tuple[float, ...] = (0, 0, 0, 0),
     **kwargs: Any,
-) -> Tuple[Axes, Collection]:
-
+) -> tuple[Axes, Collection]:
     img = _map_color_seg(
         seg=seg,
         cell_id=cell_id,
         color_vector=color_vector,
         color_source_vector=color_source_vector,
         cmap_params=cmap_params,
         seg_erosionpx=seg_contourpx,
@@ -999,10 +999,10 @@
         cmap=cmap_params.cmap if not categorical else None,
         norm=cmap_params.norm if not categorical else None,
         alpha=color_params.alpha,
         origin="lower",
         zorder=3,
         **kwargs,
     )
-    cax = ax.add_collection(_cax, autolim=False)
+    cax = ax.add_image(_cax)
 
     return ax, cax
```

### Comparing `squidpy-1.2.3/squidpy/pl/_utils.py` & `squidpy-1.3.0/src/squidpy/pl/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 from __future__ import annotations
 
+import os
 from copy import copy
+from functools import wraps
+from inspect import signature
+from pathlib import Path
 from types import MappingProxyType
 from typing import (
+    TYPE_CHECKING,
     Any,
+    Callable,
     List,
-    Tuple,
-    Union,
     Mapping,
-    Callable,
     Optional,
     Sequence,
-    TYPE_CHECKING,
+    Tuple,
+    Union,
 )
-from inspect import signature
-from pathlib import Path
-from functools import wraps
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-import os
 
-from scanpy import logging as logg, settings
+import matplotlib as mpl
+import numpy as np
+import pandas as pd
 from anndata import AnnData
-
-from dask import array as da, delayed
+from dask import array as da
+from dask import delayed
+from matplotlib import colors as mcolors
+from matplotlib import pyplot as plt
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
+from mpl_toolkits.axes_grid1 import make_axes_locatable
 from numba import njit, prange
-from scipy.sparse import issparse, spmatrix
-from scipy.cluster import hierarchy as sch
 from pandas._libs.lib import infer_dtype
 from pandas.core.dtypes.common import (
     is_bool_dtype,
-    is_object_dtype,
-    is_string_dtype,
+    is_categorical_dtype,
     is_integer_dtype,
     is_numeric_dtype,
-    is_categorical_dtype,
+    is_object_dtype,
+    is_string_dtype,
 )
-import numpy as np
-import pandas as pd
-
-from matplotlib import colors as mcolors, pyplot as plt
-from matplotlib.axes import Axes
-from matplotlib.figure import Figure
-import matplotlib as mpl
-
+from scanpy import logging as logg
+from scanpy import settings
+from scipy.cluster import hierarchy as sch
+from scipy.sparse import issparse, spmatrix
 from skimage import img_as_float32
 from skimage.color import rgb2gray
 
+from squidpy._constants._pkg_constants import Key
 from squidpy._docs import d
 from squidpy._utils import NDArrayA
 from squidpy.gr._utils import _assert_categorical_obs
-from squidpy._constants._pkg_constants import Key
 
-Vector_name_t = Tuple[Optional[Union[pd.Series, NDArrayA]], Optional[str]]
+Vector_name_t = tuple[Optional[Union[pd.Series, NDArrayA]], Optional[str]]
 
 
 @d.dedent
 def save_fig(fig: Figure, path: str | Path, make_dir: bool = True, ext: str = "png", **kwargs: Any) -> None:
     """
     Save a figure.
 
@@ -98,16 +98,16 @@
 
     fig.savefig(path, **kwargs)
 
 
 @d.dedent
 def extract(
     adata: AnnData,
-    obsm_key: List[str] | str = "img_features",
-    prefix: List[str] | str | None = None,
+    obsm_key: list[str] | str = "img_features",
+    prefix: list[str] | str | None = None,
 ) -> AnnData:
     """
     Create a temporary :class:`anndata.AnnData` object for plotting.
 
     Move columns from :attr:`anndata.AnnData.obsm` ``['{obsm_key}']`` to :attr:`anndata.AnnData.obs` to enable
     the use of :mod:`scanpy.plotting` functions.
 
@@ -163,21 +163,22 @@
     for i, cur_obsm_key in enumerate(obsm_key):
         obsm = adata.obsm[cur_obsm_key]
         if isinstance(obsm, pd.DataFrame):
             # names will be column_names
             for col in obsm.columns:
                 obs_key = f"{prefix[i]}{col}"
                 _warn_if_exists_obs(tmp_adata, obs_key)
-                tmp_adata.obs[obs_key] = obsm.loc[:, col]
+                tmp_adata.obs[obs_key] = obsm[col]
         else:
             # names will be integer indices
             for j in range(obsm.shape[1]):
                 obs_key = f"{prefix[i]}{j}"
                 _warn_if_exists_obs(tmp_adata, obs_key)
-                tmp_adata.obs[obs_key] = obsm[:, j]
+                # https://github.com/scverse/squidpy/issues/646
+                tmp_adata.obs[obs_key] = pd.Series(obsm[:, j], index=tmp_adata.obs_names)
 
     return tmp_adata
 
 
 @njit(cache=True, fastmath=True)
 def _point_inside_triangles(triangles: NDArrayA) -> np.bool_:
     # modified from napari
@@ -344,15 +345,15 @@
     @library_id.setter
     def library_id(self, library_id: str | int) -> None:
         if isinstance(library_id, int):
             library_id = self._ix_to_group[library_id]
         self._library_id = library_id
 
     @_ensure_dense_vector
-    def get_obs(self, name: str, **_: Any) -> Tuple[pd.Series | NDArrayA | None, str]:
+    def get_obs(self, name: str, **_: Any) -> tuple[pd.Series | NDArrayA | None, str]:
         """
         Return an observation.
 
         Parameters
         ----------
         name
             Key in :attr:`anndata.AnnData.obs` to access.
@@ -362,15 +363,15 @@
         The values and the formatted ``name``.
         """
         if name not in self.adata.obs.columns:
             raise KeyError(f"Key `{name}` not found in `adata.obs`.")
         return self.adata.obs[name], self._format_key(name, layer_modifier=False)
 
     @_ensure_dense_vector
-    def get_var(self, name: str | int, **_: Any) -> Tuple[NDArrayA | None, str]:
+    def get_var(self, name: str | int, **_: Any) -> tuple[NDArrayA | None, str]:
         """
         Return a gene.
 
         Parameters
         ----------
         name
             Gene name in :attr:`anndata.AnnData.var_names` or :attr:`anndata.AnnData.raw.var_names`,
@@ -384,15 +385,15 @@
         try:
             ix = adata._normalize_indices((slice(None), name))
         except KeyError:
             raise KeyError(f"Key `{name}` not found in `adata.{'raw.' if self.raw else ''}var_names`.") from None
 
         return self.adata._get_X(use_raw=self.raw, layer=self.layer)[ix], self._format_key(name, layer_modifier=True)
 
-    def get_items(self, attr: str) -> Tuple[str, ...]:
+    def get_items(self, attr: str) -> tuple[str, ...]:
         """
         Return valid keys for an attribute.
 
         Parameters
         ----------
         attr
             Attribute of :mod:`anndata.AnnData` to access.
@@ -403,15 +404,15 @@
         """
         adata = self.adata.raw if self.raw and attr in ("var",) else self.adata
         if attr in ("obs", "obsm"):
             return tuple(map(str, getattr(adata, attr).keys()))
         return tuple(map(str, getattr(adata, attr).index))
 
     @_ensure_dense_vector
-    def get_obsm(self, name: str, index: int | str = 0) -> Tuple[NDArrayA | None, str]:
+    def get_obsm(self, name: str, index: int | str = 0) -> tuple[NDArrayA | None, str]:
         """
         Return a vector from :attr:`anndata.AnnData.obsm`.
 
         Parameters
         ----------
         name
             Key in :attr:`anndata.AnnData.obsm`.
@@ -499,16 +500,16 @@
             kw.update(color=_get_black_or_white(val, cmap))
             im.axes.text(j, i, valfmt(data[i, j], None), **kw)
 
 
 def _get_cmap_norm(
     adata: AnnData,
     key: str,
-    order: Tuple[List[int], List[int]] | None | None = None,
-) -> Tuple[mcolors.ListedColormap, mcolors.ListedColormap, mcolors.BoundaryNorm, mcolors.BoundaryNorm, int]:
+    order: tuple[list[int], list[int]] | None | None = None,
+) -> tuple[mcolors.ListedColormap, mcolors.ListedColormap, mcolors.BoundaryNorm, mcolors.BoundaryNorm, int]:
     n_cls = adata.obs[key].nunique()
 
     colors = adata.uns[Key.uns.colors(key)]
 
     if order is not None:
         row_order, col_order = order
         row_colors = [colors[i] for i in row_order]
@@ -527,15 +528,15 @@
 def _heatmap(
     adata: AnnData,
     key: str,
     title: str = "",
     method: str | None = None,
     cont_cmap: str | mcolors.Colormap = "viridis",
     annotate: bool = True,
-    figsize: Tuple[float, float] | None = None,
+    figsize: tuple[float, float] | None = None,
     dpi: int | None = None,
     cbar_kwargs: Mapping[str, Any] = MappingProxyType({}),
     ax: Axes | None = None,
     **kwargs: Any,
 ) -> mpl.figure.Figure:
     _assert_categorical_obs(adata, key=key)
 
@@ -545,15 +546,15 @@
         fig, ax = plt.subplots(constrained_layout=True, dpi=dpi, figsize=figsize)
     else:
         fig = ax.figure
 
     if method is not None:
         row_order, col_order, _, col_link = _dendrogram(adata.X, method, optimal_ordering=adata.n_obs <= 1500)
     else:
-        row_order = col_order = np.arange(len(adata.uns[Key.uns.colors(key)]))
+        row_order = col_order = np.arange(len(adata.uns[Key.uns.colors(key)])).tolist()
 
     row_order = row_order[::-1]
     row_labels = adata.obs[key][row_order]
     data = adata[row_order, col_order].X
 
     row_cmap, col_cmap, row_norm, col_norm, n_cls = _get_cmap_norm(adata, key, order=(row_order, col_order))
 
@@ -607,15 +608,15 @@
 
 
 def _filter_kwargs(func: Callable[..., Any], kwargs: Mapping[str, Any]) -> dict[str, Any]:
     style_args = {k for k in signature(func).parameters.keys()}  # noqa: C416
     return {k: v for k, v in kwargs.items() if k in style_args}
 
 
-def _dendrogram(data: NDArrayA, method: str, **kwargs: Any) -> Tuple[List[int], List[int], List[int], List[int]]:
+def _dendrogram(data: NDArrayA, method: str, **kwargs: Any) -> tuple[list[int], list[int], list[int], list[int]]:
     link_kwargs = _filter_kwargs(sch.linkage, kwargs)
     dendro_kwargs = _filter_kwargs(sch.dendrogram, kwargs)
 
     # Row-cluster
     row_link = sch.linkage(data, method=method, **link_kwargs)
     row_dendro = sch.dendrogram(row_link, no_plot=True, **dendro_kwargs)
     row_order = row_dendro["leaves"]
```

### Comparing `squidpy-1.2.3/squidpy/read/_read.py` & `squidpy-1.3.0/src/squidpy/read/_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
-from typing import Union  # noqa: F401
-from typing import Any
-from pathlib import Path
+import json
 import os
 import re
-import json
-
-from scanpy import logging as logg
-from anndata import AnnData
+from pathlib import Path
+from typing import (
+    Any,
+    Union,  # noqa: F401
+)
 
-from scipy.sparse import csr_matrix
 import numpy as np
 import pandas as pd
+from anndata import AnnData
+from scanpy import logging as logg
+from scipy.sparse import csr_matrix
 
-from squidpy.read._utils import _load_image, _read_counts
-from squidpy.datasets._utils import PathLike
 from squidpy._constants._pkg_constants import Key
+from squidpy.datasets._utils import PathLike
+from squidpy.read._utils import _load_image, _read_counts
 
 __all__ = ["visium", "vizgen", "nanostring"]
 
 
 def visium(
     path: PathLike,
     *,
@@ -83,14 +84,16 @@
 
     coords = pd.read_csv(
         tissue_positions_file,
         header=1 if tissue_positions_file.name == "tissue_positions.csv" else None,
         index_col=0,
     )
     coords.columns = ["in_tissue", "array_row", "array_col", "pxl_col_in_fullres", "pxl_row_in_fullres"]
+    # https://github.com/scverse/squidpy/issues/657
+    coords.set_index(coords.index.astype(adata.obs.index.dtype), inplace=True)
 
     adata.obs = pd.merge(adata.obs, coords, how="left", left_index=True, right_index=True)
     adata.obsm[Key.obsm.spatial] = adata.obs[["pxl_row_in_fullres", "pxl_col_in_fullres"]].values
     adata.obs.drop(columns=["pxl_row_in_fullres", "pxl_col_in_fullres"], inplace=True)
 
     if source_image_path is not None:
         source_image_path = Path(source_image_path).absolute()
@@ -152,18 +155,17 @@
     adata.obsm["blank_genes"] = pd.DataFrame(
         adata[:, blank_genes].X.copy(), columns=adata.var_names[blank_genes], index=adata.obs_names
     )
     adata = adata[:, ~blank_genes].copy()
 
     adata.X = csr_matrix(adata.X)
 
-    # fmt: off
     coords = pd.read_csv(path / meta_file, header=0, index_col=0)
-    coords.columns = ["fov", "volume", "center_x", "center_y", "min_x", "max_x", "min_y", "max_y"]
-    # fmt: on
+    # https://github.com/scverse/squidpy/issues/657
+    coords.set_index(coords.index.astype("str"), inplace=True)
 
     adata.obs = pd.merge(adata.obs, coords, how="left", left_index=True, right_index=True)
     adata.obsm[Key.obsm.spatial] = adata.obs[["center_x", "center_y"]].values
     adata.obs.drop(columns=["center_x", "center_y"], inplace=True)
 
     if transformation_file is not None:
         matrix = pd.read_csv(path / f"images/{transformation_file}", sep=" ", header=None)
```

### Comparing `squidpy-1.2.3/squidpy/read/_utils.py` & `squidpy-1.3.0/src/squidpy/read/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
-from PIL import Image
-from h5py import File
-from typing import Any, Tuple, Optional
 from pathlib import Path
-
-from scanpy import read_10x_h5
-from anndata import AnnData, read_mtx, read_text
+from typing import Any, Optional, Tuple
 
 import numpy as np
+from anndata import AnnData, read_mtx, read_text
+from h5py import File
+from PIL import Image
+from scanpy import read_10x_h5
 
+from squidpy._constants._pkg_constants import Key
 from squidpy._utils import NDArrayA
 from squidpy.datasets._utils import PathLike
-from squidpy._constants._pkg_constants import Key
 
 
 def _read_counts(
     path: str | Path,
     count_file: str,
-    library_id: Optional[str] = None,
+    library_id: str | None = None,
     **kwargs: Any,
-) -> Tuple[AnnData, str]:
+) -> tuple[AnnData, str]:
     path = Path(path)
     if count_file.endswith(".h5"):
         adata: AnnData = read_10x_h5(path / count_file, **kwargs)
         with File(path / count_file, mode="r") as f:
             attrs = dict(f.attrs)
             if library_id is None:
                 try:
```

### Comparing `squidpy-1.2.3/tests/conftest.py` & `squidpy-1.3.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
+from __future__ import annotations
+
+import pickle
+import sys
+import warnings
 from abc import ABC, ABCMeta
-from typing import Tuple, Mapping, Callable, Optional, Sequence
-from pathlib import Path
 from functools import wraps
 from itertools import product
-import sys
-import pickle
-import pytest
-import warnings
+from pathlib import Path
+from typing import Callable, Mapping, Optional, Sequence, Tuple
 
-from anndata import AnnData, OldFormatWarning
-import scanpy as sc
 import anndata as ad
-
-from scipy.sparse import csr_matrix
+import matplotlib
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
+import pytest
+import scanpy as sc
+import squidpy as sq
+from anndata import AnnData, OldFormatWarning
 from matplotlib.testing.compare import compare_images
-import matplotlib
-import matplotlib.pyplot as plt
-
+from scipy.sparse import csr_matrix
+from squidpy._constants._pkg_constants import Key
 from squidpy.gr import spatial_neighbors
 from squidpy.im._container import ImageContainer
-from squidpy._constants._pkg_constants import Key
-import squidpy as sq
 
 HERE: Path = Path(__file__).parent
 
 EXPECTED = HERE / "_images"
 ACTUAL = HERE / "figures"
 TOL = 50
 DPI = 40
@@ -69,14 +68,19 @@
 
 
 @pytest.fixture(scope="session")
 def adata_mibitof() -> AnnData:
     return sq.datasets.mibitof().copy()
 
 
+@pytest.fixture(scope="session")
+def adata_seqfish() -> AnnData:
+    return sq.datasets.seqfish().copy()
+
+
 @pytest.fixture()
 def adata() -> AnnData:
     return _adata.copy()
 
 
 @pytest.fixture()
 def adata_palette() -> AnnData:
@@ -227,20 +231,20 @@
 
 @pytest.fixture()
 def napari_cont() -> ImageContainer:
     return ImageContainer("tests/_data/test_img.jpg", layer="V1_Adult_Mouse_Brain", library_id="V1_Adult_Mouse_Brain")
 
 
 @pytest.fixture()
-def interactions(adata: AnnData) -> Tuple[Sequence[str], Sequence[str]]:
+def interactions(adata: AnnData) -> tuple[Sequence[str], Sequence[str]]:
     return tuple(product(adata.raw.var_names[:5], adata.raw.var_names[:5]))  # type: ignore
 
 
 @pytest.fixture()
-def complexes(adata: AnnData) -> Sequence[Tuple[str, str]]:
+def complexes(adata: AnnData) -> Sequence[tuple[str, str]]:
     g = adata.raw.var_names
     return [
         (g[0], g[1]),
         (f"{g[2]}_{g[3]}", g[4]),
         (g[5], f"{g[6]}_{g[7]}"),
         (f"{g[8]}_{g[9]}", f"{g[10]}_{g[11]}"),
         (f"foo_{g[12]}_bar_baz", g[13]),
@@ -325,15 +329,15 @@
 def non_visium_adata():
     non_visium_coords = np.array([[1, 0], [3, 0], [5, 6], [0, 4]])
     adata = AnnData(X=non_visium_coords, dtype=int)
     adata.obsm[Key.obsm.spatial] = non_visium_coords
     return adata
 
 
-def _decorate(fn: Callable, clsname: str, name: Optional[str] = None) -> Callable:
+def _decorate(fn: Callable, clsname: str, name: str | None = None) -> Callable:
     @wraps(fn)
     def save_and_compare(self, *args, **kwargs):
         fn(self, *args, **kwargs)
         self.compare(fig_name)
 
     if not callable(fn):
         raise TypeError(f"Expected a `callable` for class `{clsname}`, found `{type(fn).__name__}`.")
@@ -356,15 +360,15 @@
         return super().__new__(cls, clsname, superclasses, attributedict)
 
 
 # ideally, we would you metaclass=PlotTesterMeta and all plotting tests just subclass this
 # but for some reason, pytest erases the metaclass info
 class PlotTester(ABC):
     @classmethod
-    def compare(cls, basename: str, tolerance: Optional[float] = None):
+    def compare(cls, basename: str, tolerance: float | None = None):
         ACTUAL.mkdir(parents=True, exist_ok=True)
         out_path = ACTUAL / f"{basename}.png"
 
         plt.savefig(out_path, dpi=DPI)
         plt.close()
 
         if tolerance is None:
```

### Comparing `squidpy-1.2.3/tests/datasets/test_dataset.py` & `squidpy-1.3.0/tests/datasets/test_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from types import FunctionType
-from pathlib import Path
-from http.client import RemoteDisconnected
-import pytest
 import warnings
+from http.client import RemoteDisconnected
+from pathlib import Path
+from types import FunctionType
 
-from anndata import AnnData, OldFormatWarning
-
+import pytest
 import squidpy as sq
+from anndata import AnnData, OldFormatWarning
 
 
 class TestDatasetsImports:
     @pytest.mark.parametrize("func", sq.datasets._dataset.__all__ + sq.datasets._image.__all__)
     def test_import(self, func):
         assert hasattr(sq.datasets, func), dir(sq.datasets)
         fn = getattr(sq.datasets, func)
```

### Comparing `squidpy-1.2.3/tests/datasets/test_download_visium_dataset.py` & `squidpy-1.3.0/tests/datasets/test_download_visium_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """"
 Tests to make sure the Visium example datasets load.
 """
 
-from pathlib import Path
-import pytest
 import subprocess
+from pathlib import Path
 
-from scanpy._settings import settings
+import pytest
 from anndata.tests.helpers import assert_adata_equal
-
+from scanpy._settings import settings
 from squidpy.datasets import visium
 
 
 @pytest.mark.timeout(120)
 @pytest.mark.internet()
 @pytest.mark.parametrize(
     "sample", ["V1_Mouse_Kidney", "Targeted_Visium_Human_SpinalCord_Neuroscience", "Visium_FFPE_Human_Breast_Cancer"]
```

### Comparing `squidpy-1.2.3/tests/graph/test_ligrec.py` & `squidpy-1.3.0/tests/graph/test_ligrec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from time import time
-from typing import Tuple, Mapping, Optional, Sequence, TYPE_CHECKING
-from itertools import product
 import sys
-import pytest
-
-from scanpy import settings as s
-from anndata import AnnData
-from scanpy.datasets import blobs
-import scanpy as sc
+from itertools import product
+from time import time
+from typing import TYPE_CHECKING, Mapping, Optional, Sequence, Tuple
 
-from pandas.testing import assert_frame_equal
 import numpy as np
 import pandas as pd
-
+import pytest
+import scanpy as sc
+from anndata import AnnData
+from pandas.testing import assert_frame_equal
+from scanpy import settings as s
+from scanpy.datasets import blobs
+from squidpy._constants._pkg_constants import Key
 from squidpy.gr import ligrec
 from squidpy.gr._ligrec import PermutationTest
-from squidpy._constants._pkg_constants import Key
 
 _CK = "leiden"
-Interactions_t = Tuple[Sequence[str], Sequence[str]]
-Complexes_t = Sequence[Tuple[str, str]]
+Interactions_t = tuple[Sequence[str], Sequence[str]]
+Complexes_t = Sequence[tuple[str, str]]
 
 
 class TestInvalidBehavior:
     def test_not_adata(self):
         with pytest.raises(TypeError, match=r"Expected `adata` to be of type `anndata.AnnData`"):
             ligrec(None, _CK)
 
     def test_adata_no_raw(self, adata: AnnData):
         del adata.raw
         with pytest.raises(AttributeError, match=r"No `.raw` attribute"):
             ligrec(adata, _CK, use_raw=True)
 
     def test_raw_has_different_n_obs(self, adata: AnnData):
         adata.raw = blobs(n_observations=adata.n_obs + 1)
-        with pytest.raises(ValueError, match=rf"Expected `{adata.n_obs}` cells in `.raw`"):
+        # raise below happend with anndata < 0.9
+        # with pytest.raises(ValueError, match=rf"Expected `{adata.n_obs}` cells in `.raw`"):
+        with pytest.raises(ValueError, match=rf"Index length mismatch: {adata.n_obs} vs. {adata.n_obs + 1}"):
             ligrec(adata, _CK)
 
     def test_invalid_cluster_key(self, adata: AnnData, interactions: Interactions_t):
         with pytest.raises(KeyError, match=r"Cluster key `foobar` not found"):
             ligrec(adata, cluster_key="foobar", interactions=interactions)
 
     def test_cluster_key_is_not_categorical(self, adata: AnnData, interactions: Interactions_t):
```

### Comparing `squidpy-1.2.3/tests/graph/test_nhood.py` & `squidpy-1.3.0/tests/graph/test_nhood.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-import pytest
-
-from anndata import AnnData
-
 import numpy as np
 import pandas as pd
-
+import pytest
+from anndata import AnnData
+from squidpy._constants._pkg_constants import Key
 from squidpy.gr import (
-    nhood_enrichment,
     centrality_scores,
-    spatial_neighbors,
     interaction_matrix,
+    nhood_enrichment,
+    spatial_neighbors,
 )
-from squidpy._constants._pkg_constants import Key
 
 _CK = "leiden"
 
 
 class TestNhoodEnrichment:
     def _assert_common(self, adata: AnnData):
         key = Key.uns.nhood_enrichment(_CK)
```

### Comparing `squidpy-1.2.3/tests/graph/test_ppatterns.py` & `squidpy-1.3.0/tests/graph/test_ppatterns.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import pytest
+from typing import Any, Literal
 
+import numpy as np
+import pytest
 from anndata import AnnData
-
 from pandas.testing import assert_frame_equal
-import numpy as np
-
+from squidpy._constants._pkg_constants import Key
 from squidpy.gr import co_occurrence, spatial_autocorr
 from squidpy.gr._ppatterns import _find_min_max
-from squidpy._constants._pkg_constants import Key
 
 MORAN_K = "moranI"
 GEARY_C = "gearyC"
 
 
 @pytest.mark.parametrize("mode", ["moran", "geary"])
 def test_spatial_autocorr_seq_par(dummy_adata: AnnData, mode: str):
@@ -54,15 +53,15 @@
     spatial_autocorr(dummy_adata, mode=mode)
     dummy_adata.var["highly_variable"] = rng.choice([True, False], size=dummy_adata.var_names.shape)
     # seed will work only when multiprocessing/loky
     df_1 = spatial_autocorr(dummy_adata, mode=mode, copy=True, n_jobs=n_jobs, seed=42, n_perms=50)
     df_2 = spatial_autocorr(dummy_adata, mode=mode, copy=True, n_jobs=n_jobs, seed=42, n_perms=50)
 
     idx_df = df_1.index.values
-    idx_adata = dummy_adata[:, dummy_adata.var.highly_variable.values].var_names.values
+    idx_adata = dummy_adata[:, dummy_adata.var["highly_variable"].values].var_names.values
 
     if mode == "moran":
         UNS_KEY = MORAN_K
     elif mode == "geary":
         UNS_KEY = GEARY_C
     assert UNS_KEY in dummy_adata.uns.keys()
     # assert fdr correction in adata.uns
@@ -78,14 +77,43 @@
     # assert idx are sorted and contain same elements
     assert not np.array_equal(idx_df, idx_adata)
     np.testing.assert_array_equal(sorted(idx_df), sorted(idx_adata))
     # check parallel gives same results
     assert_frame_equal(df_1, df_2)
 
 
+@pytest.mark.parametrize(
+    "attr,layer,genes",
+    [
+        ("X", None, None),
+        ("obs", None, None),
+        ("obs", None, "foo"),
+        ("obsm", "spatial", None),
+        ("obsm", "spatial", [1, 0]),
+    ],
+)
+def test_spatial_autocorr_attr(dummy_adata: AnnData, attr: Literal["X", "obs", "obsm"], layer: str, genes: Any):
+    if attr == "obs":
+        if isinstance(genes, str):
+            dummy_adata.obs[genes] = np.random.RandomState(42).normal(size=(dummy_adata.n_obs,))
+            index = [genes]
+        else:
+            index = dummy_adata.obs.select_dtypes(include=np.number).columns
+    elif attr == "X":
+        index = dummy_adata.var_names if genes is None else genes
+    elif attr == "obsm":
+        index = np.arange(dummy_adata.obsm[layer].shape[1]) if genes is None else genes
+
+    spatial_autocorr(dummy_adata, attr=attr, mode="moran", layer=layer, genes=genes)
+
+    df = dummy_adata.uns[MORAN_K]
+    np.testing.assert_array_equal(np.isfinite(df), True)
+    np.testing.assert_array_equal(sorted(df.index), sorted(index))
+
+
 def test_co_occurrence(adata: AnnData):
     """
     check co_occurrence score and shape
     """
     co_occurrence(adata, cluster_key="leiden")
 
     # assert occurrence in adata.uns
```

### Comparing `squidpy-1.2.3/tests/graph/test_ripley.py` & `squidpy-1.3.0/tests/graph/test_ripley.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
+import numpy as np
 import pytest
-
 from anndata import AnnData
-
-import numpy as np
-
-from squidpy.gr import ripley
 from squidpy._constants._constants import RipleyStat
+from squidpy.gr import ripley
 
 CLUSTER_KEY = "leiden"
 
 
 @pytest.mark.parametrize("mode", list(RipleyStat))
 def test_ripley_modes(adata_ripley: AnnData, mode: RipleyStat):
     adata = adata_ripley
```

### Comparing `squidpy-1.2.3/tests/graph/test_sepal.py` & `squidpy-1.3.0/tests/graph/test_sepal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
+import numpy as np
 from anndata import AnnData
-
 from pandas.testing import assert_frame_equal
-import numpy as np
-
 from squidpy.gr import sepal, spatial_neighbors
 
 UNS_KEY = "sepal_score"
 
 
 def test_sepal_seq_par(adata: AnnData):
     """Check whether sepal results are the same for seq. and parallel computation."""
```

### Comparing `squidpy-1.2.3/tests/graph/test_spatial_neighbors.py` & `squidpy-1.3.0/tests/graph/test_spatial_neighbors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Tuple
-import pytest
 
-from anndata import AnnData
 import anndata as ad
-
-from scipy.sparse import isspmatrix_csr
 import numpy as np
-
-from squidpy.gr import spatial_neighbors
+import pytest
+from anndata import AnnData
+from scipy.sparse import isspmatrix_csr
 from squidpy._constants._pkg_constants import Key
+from squidpy.gr import spatial_neighbors
+from squidpy.gr._build import _build_connectivity
 
 
 class TestSpatialNeighbors:
     # ground-truth Delaunay distances
     _gt_ddist = np.array(
         [
             [0.0, 2.0, 0.0, 4.12310563],
@@ -86,15 +85,15 @@
         np.testing.assert_array_equal(
             adata_concat[adata_concat.obs["library_id"] == batch2].obsp[Key.obsp.spatial_conn()].A,
             adata2.obsp[Key.obsp.spatial_conn()].A,
         )
 
     @pytest.mark.parametrize("type_rings", [("grid", 1), ("grid", 6), ("generic", 1)])
     @pytest.mark.parametrize("set_diag", [False, True])
-    def test_set_diag(self, adata_squaregrid: AnnData, set_diag: bool, type_rings: Tuple[str, int]):
+    def test_set_diag(self, adata_squaregrid: AnnData, set_diag: bool, type_rings: tuple[str, int]):
         typ, n_rings = type_rings
         spatial_neighbors(adata_squaregrid, coord_type=typ, set_diag=set_diag, n_rings=n_rings)
         G = adata_squaregrid.obsp[Key.obsp.spatial_conn()]
         D = adata_squaregrid.obsp[Key.obsp.spatial_dist()]
 
         np.testing.assert_array_equal(G.diagonal(), float(set_diag))
         np.testing.assert_array_equal(D.diagonal(), 0.0)
@@ -151,15 +150,15 @@
         np.testing.assert_array_equal(
             adata_concat[adata_concat.obs["library_id"] == batch2].obsp[Key.obsp.spatial_conn()].A,
             non_visium_adata2.obsp[Key.obsp.spatial_conn()].A,
         )
 
     @pytest.mark.parametrize("set_diag", [False, True])
     @pytest.mark.parametrize("radius", [(0, np.inf), (2.0, 4.0), (-42, -420), (100, 200)])
-    def test_radius_min_max(self, non_visium_adata: AnnData, radius: Tuple[float, float], set_diag: bool):
+    def test_radius_min_max(self, non_visium_adata: AnnData, radius: tuple[float, float], set_diag: bool):
         gt_ddist = self._gt_ddist.copy()
         gt_dgraph = self._gt_dgraph.copy()
 
         minn, maxx = sorted(radius)
         mask = (gt_ddist < minn) | (gt_ddist > maxx)
         gt_ddist[mask] = 0.0
         gt_dgraph[mask] = 0.0
@@ -179,7 +178,27 @@
 
         assert isspmatrix_csr(conn)
         assert isspmatrix_csr(dist)
         assert Key.obsp.spatial_conn() not in non_visium_adata.obsp
         assert Key.obsp.spatial_dist() not in non_visium_adata.obsp
         np.testing.assert_allclose(dist.A, self._gt_ddist)
         np.testing.assert_allclose(conn.A, self._gt_dgraph)
+
+    @pytest.mark.parametrize("percentile", [99.0, 95.0])
+    def test_percentile_filtering(self, adata_hne: AnnData, percentile: float, coord_type="generic"):
+        conn, dist = spatial_neighbors(adata_hne, coord_type=coord_type, copy=True)
+        conn_filtered, dist_filtered = spatial_neighbors(
+            adata_hne, coord_type=coord_type, percentile=percentile, copy=True
+        )
+
+        # check whether there are less connectivities in the filtered graph and whether the max distance is smaller
+        assert not ((conn != conn_filtered).nnz == 0)
+        assert dist.max() > dist_filtered.max()
+
+        Adj, Dst = _build_connectivity(adata_hne.obsm["spatial"], n_neighs=6, return_distance=True, set_diag=False)
+        threshold = np.percentile(Dst.data, percentile)
+        Adj[Dst > threshold] = 0.0
+        Dst[Dst > threshold] = 0.0
+        Adj.eliminate_zeros()
+        Dst.eliminate_zeros()
+
+        assert dist_filtered.max() == Dst.max()
```

### Comparing `squidpy-1.2.3/tests/image/test_container.py` & `squidpy-1.3.0/tests/image/test_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import Any, Set, List, Tuple, Union, Optional, Sequence
-from pathlib import Path
-from itertools import permutations
+import subprocess
 from collections import defaultdict
 from html.parser import HTMLParser
-from pytest_mock import MockerFixture
-import pytest
-import imageio
-import subprocess
+from itertools import permutations
+from pathlib import Path
+from typing import Any, List, Optional, Sequence, Set, Tuple, Union
 
-from anndata import AnnData
 import anndata as ad
-
-import numpy as np
-import xarray as xr
 import dask.array as da
-
+import imageio.v3 as iio
+import numpy as np
+import pytest
+import squidpy as sq
 import tifffile
-
-from squidpy.im import ImageContainer
-from squidpy.im._coords import CropCoords, CropPadding, _NULL_COORDS
+import xarray as xr
+from anndata import AnnData
+from PIL import Image
+from pytest_mock import MockerFixture
 from squidpy._constants._pkg_constants import Key
-import squidpy as sq
+from squidpy.im import ImageContainer
+from squidpy.im._coords import _NULL_COORDS, CropCoords, CropPadding
 
 
 class SimpleHTMLValidator(HTMLParser):  # modified from CellRank
     def __init__(self, n_expected_rows: int, expected_tags: Set[str], **kwargs: Any):
         super().__init__(**kwargs)
         self._cnt = defaultdict(int)
         self._n_rows = 0
@@ -78,14 +76,15 @@
 
         assert img.data is not dataset
         assert "foo" in img
         assert img.shape == (100, 100)
         np.testing.assert_array_equal(img.data.values(), dataset.values)
         assert img.data.attrs == dataset.attrs
 
+    @pytest.mark.skip(reason="Sometimes fails to load image")
     def test_save_load_zarr(self, tmpdir):
         img = ImageContainer(np.random.normal(size=(100, 100, 1)))
         img.data.attrs["scale"] = 42
         img.save(Path(tmpdir) / "foo.zarr")
 
         img2 = ImageContainer.load(Path(tmpdir) / "foo.zarr")
         proc = None
@@ -150,19 +149,24 @@
     def test_add_img_invalid_zdim(self, cont: ImageContainer):
         with pytest.raises(ValueError, match=r"Expected image to have `1` Z-dimension\(s\), found `10`."):
             cont.add_img(np.random.normal(size=(*cont.shape, 10, 3)), dims=["y", "x", "z", "channels"])
 
     @pytest.mark.parametrize("ext", ["jpg", "png"])
     @pytest.mark.parametrize("shape", [(100, 200, 3), (100, 200, 1)])
     def test_load_ext(self, shape: Tuple[int, ...], ext: str, tmpdir):
-        img_orig = np.random.randint(low=0, high=255, size=shape, dtype=np.uint8)
         fname = tmpdir / f"tmp.{ext}"
-        imageio.imsave(str(fname), img_orig)
 
-        gt = imageio.imread(str(fname))  # because of compression, we load again
+        if shape == (100, 200, 1):
+            img = np.random.randint(256, size=(100, 200), dtype=np.uint8)
+            img_orig = Image.fromarray(img)
+        else:
+            img_orig = np.random.randint(low=0, high=255, size=shape, dtype=np.uint8)
+        iio.imwrite(str(fname), img_orig)
+
+        gt = iio.imread(str(fname))  # because of compression, we load again
         cont = ImageContainer(str(fname))
 
         np.testing.assert_array_equal(cont["image"].values.squeeze(), gt.squeeze())
 
     @pytest.mark.parametrize("shape", [(100, 200, 3), (100, 200, 1), (10, 100, 200, 1)])
     def test_load_tiff(self, shape: Tuple[int, ...], tmpdir):
         img_orig = np.random.randint(low=0, high=255, size=shape, dtype=np.uint8)
@@ -927,15 +931,15 @@
             assert el.shape == (7, 7)
         res = ImageContainer.uncrop(els)
         assert (res.data["image"].sel(z="2").values == cont_comb.data["image"].sel(z="2").values).all()
 
     @pytest.mark.parametrize("channel", [None, 0])
     @pytest.mark.parametrize("copy", [False, True])
     @pytest.mark.parametrize("library_id", [["l1"], ["l2"], ["l1", "l2", "l3"], None])
-    def test_apply(self, copy: bool, channel: Optional[int], library_id: Optional[Union[List[str], str]]):
+    def test_apply(self, copy: bool, channel: Optional[int], library_id: Optional[Union[list[str], str]]):
         cont = ImageContainer(
             np.random.normal(size=(100, 100, 3, 2)), dims=("y", "x", "z", "channels"), library_id=["l1", "l2", "l3"]
         )
         orig = cont.copy()
 
         if library_id is None:
             library_ids = ["l1", "l2", "l3"]
```

### Comparing `squidpy-1.2.3/tests/image/test_features.py` & `squidpy-1.3.0/tests/image/test_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from typing import Tuple, Sequence
-from pytest_mock import MockerFixture
-import pytest
-
-from anndata import AnnData
+from typing import Sequence, Tuple
 
 import numpy as np
 import pandas as pd
-
-from squidpy.im._feature import calculate_image_features
-from squidpy.im._container import ImageContainer
+import pytest
+from anndata import AnnData
+from pytest_mock import MockerFixture
 from squidpy._constants._constants import ImageFeature
+from squidpy.im._container import ImageContainer
+from squidpy.im._feature import calculate_image_features
 
 
 class TestFeatureMixin:
     def test_container_empty(self):
         cont = ImageContainer()
         with pytest.raises(ValueError, match=r"The container is empty."):
             cont.features_summary("image")
@@ -23,15 +21,15 @@
             small_cont.features_summary("foobar")
 
     def test_invalid_channels(self, small_cont: ImageContainer):
         with pytest.raises(ValueError, match=r"Channel `-1` is not in"):
             small_cont.features_summary("image", channels=-1)
 
     @pytest.mark.parametrize("quantiles", [(), (0.5,), (0.1, 0.9)])
-    def test_summary_quantiles(self, small_cont: ImageContainer, quantiles: Tuple[float, ...]):
+    def test_summary_quantiles(self, small_cont: ImageContainer, quantiles: tuple[float, ...]):
         if not len(quantiles):
             with pytest.raises(ValueError, match=r"No quantiles have been selected."):
                 small_cont.features_summary("image", quantiles=quantiles, feature_name="foo", channels=(0, 1))
         else:
             features = small_cont.features_summary("image", quantiles=quantiles, feature_name="foo", channels=(0, 1))
             haystack = features.keys()
 
@@ -139,15 +137,15 @@
         summary_features = small_cont.features_summary("image", feature_name="summary", channels=[0])
 
         assert len(custom_features) == 1
         assert f"{np.mean.__name__}_0" in custom_features
         assert custom_features[f"{np.mean.__name__}_0"] == summary_features["summary_ch-0_mean"]
 
     def test_custom_returns_iterable(self, small_cont: ImageContainer):
-        def dummy(_: np.ndarray) -> Tuple[int, int]:
+        def dummy(_: np.ndarray) -> tuple[int, int]:
             return 0, 1
 
         features = small_cont.features_custom(dummy, layer="image", feature_name="foo")
 
         assert len(features) == 2
         assert features["foo_0"] == 0
         assert features["foo_1"] == 1
```

### Comparing `squidpy-1.2.3/tests/image/test_io.py` & `squidpy-1.3.0/tests/image/test_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import Dict, Tuple, Union, Optional
-from pytest_mock import MockerFixture
-import pytest
+from typing import Dict, Optional, Tuple, Union
 
+import dask.array as da
 import numpy as np
+import pytest
+import tifffile
 import xarray as xr
-import dask.array as da
-
+from pytest_mock import MockerFixture
 from skimage.io import imread
-import tifffile
-
-from squidpy.im._io import _lazy_load_image, _infer_dimensions, _get_image_shape_dtype
 from squidpy._constants._constants import InferDimensions
+from squidpy.im._io import _get_image_shape_dtype, _infer_dimensions, _lazy_load_image
 
 
 class TestIO:
     @staticmethod
-    def _create_image(path: str, shape: Tuple[int, ...]):
+    def _create_image(path: str, shape: tuple[int, ...]):
         dtype = np.uint8 if len(shape) <= 3 else np.float32
         img = np.random.randint(0, 255, size=shape).astype(dtype)
         # set `photometric` to remove warnings
         tifffile.imwrite(path, img, photometric=tifffile.TIFF.PHOTOMETRIC.MINISBLACK)
 
         return img
 
@@ -31,27 +29,27 @@
             (64, 101, 4),
             (1, 101, 64, 1),
             (1, 101, 64, 3),
             (3, 101, 64, 1),
             (3, 101, 64, 4),
         ],
     )
-    def test_get_shape(self, shape: Tuple[int, ...], tmpdir):
+    def test_get_shape(self, shape: tuple[int, ...], tmpdir):
         path = str(tmpdir / "img.tiff")
         img = self._create_image(path, shape)
 
         actual_shape, actual_dtype = _get_image_shape_dtype(path)
         np.testing.assert_array_equal(actual_shape, shape)
         assert actual_dtype == img.dtype, (actual_dtype, img.dtype)
 
     @pytest.mark.parametrize("infer_dim", list(InferDimensions))
     @pytest.mark.parametrize(
         "shape", [(101, 64), (101, 64, 3), (3, 64, 101), (1, 101, 64, 3), (1, 101, 64, 1), (3, 101, 64, 1)]
     )
-    def test_infer_dimensions(self, shape: Tuple[int, ...], infer_dim: str, mocker: MockerFixture):
+    def test_infer_dimensions(self, shape: tuple[int, ...], infer_dim: str, mocker: MockerFixture):
         mocker.patch("squidpy.im._io._get_image_shape_dtype", return_value=(shape, np.uint8))
         infer_dim = InferDimensions(infer_dim)
         actual_shape, actual_dims, _, _ = _infer_dimensions("non_existent", infer_dim)
 
         if len(shape) == 2:
             np.testing.assert_array_equal(actual_dims, ["y", "x", "z", "channels"])
             np.testing.assert_array_equal(actual_shape, shape + (1, 1))
@@ -79,15 +77,15 @@
             elif infer_dim == InferDimensions.Z_LAST:
                 np.testing.assert_array_equal(actual_dims, ["channels", "y", "x", "z"])
             else:
                 np.testing.assert_array_equal(actual_dims, ["z", "y", "x", "channels"])
             np.testing.assert_array_equal(actual_shape, shape)
 
     @pytest.mark.parametrize("chunks", [100, (1, 100, 100, 3), "auto", None, {"y": 100, "x": 100}])
-    def test_lazy_load_image(self, chunks: Optional[Union[int, Tuple[int, ...], str, Dict[str, int]]], tmpdir):
+    def test_lazy_load_image(self, chunks: Optional[Union[int, tuple[int, ...], str, dict[str, int]]], tmpdir):
         path = str(tmpdir / "img.tiff")
         img = self._create_image(path, (256, 256, 3))
 
         res = _lazy_load_image(path, chunks=chunks)
 
         assert isinstance(res, xr.DataArray)
         assert isinstance(res.data, da.Array)
```

### Comparing `squidpy-1.2.3/tests/image/test_processing.py` & `squidpy-1.3.0/tests/image/test_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Tuple, Union, Callable, Optional, Sequence
-from pytest_mock import MockerFixture
-import pytest
+from typing import Callable, Optional, Sequence, Tuple, Union
 
-import numpy as np
 import dask.array as da
-
-from squidpy.im import process, ImageContainer
+import numpy as np
+import pytest
+from pytest_mock import MockerFixture
 from squidpy._constants._pkg_constants import Key
+from squidpy.im import ImageContainer, process
 
 
 class TestProcess:
     def test_invalid_layer(self, small_cont: ImageContainer):
         with pytest.raises(KeyError, match=r"Image layer `foobar` not found in"):
             process(small_cont, layer="foobar")
 
@@ -84,15 +83,15 @@
         spy.assert_called_once()
         np.testing.assert_array_equal(small_cont["foo"].values, small_cont["image"].values)
 
     @pytest.mark.parametrize("dask_input", [False, True])
     @pytest.mark.parametrize("chunks", [25, (50, 50, 1, 3), "auto"])
     @pytest.mark.parametrize("lazy", [False, True])
     def test_dask_processing(
-        self, small_cont: ImageContainer, dask_input: bool, chunks: Union[int, Tuple[int, ...], str], lazy: bool
+        self, small_cont: ImageContainer, dask_input: bool, chunks: Union[int, tuple[int, ...], str], lazy: bool
     ):
         def func(chunk: np.ndarray):
             if isinstance(chunks, tuple):
                 np.testing.assert_array_equal(chunk.shape, chunks)
             elif isinstance(chunks, int):
                 np.testing.assert_array_equal(chunk.shape, [chunks, chunks, 1, 3])
```

### Comparing `squidpy-1.2.3/tests/image/test_segmentation.py` & `squidpy-1.3.0/tests/image/test_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from typing import Tuple, Union, Callable, Optional, Sequence
-from pytest_mock import MockerFixture
-import pytest
+from typing import Callable, Optional, Sequence, Tuple, Union
 
-import numpy as np
 import dask.array as da
-
+import numpy as np
+import pytest
+from pytest_mock import MockerFixture
+from squidpy._constants._constants import SegmentationBackend
+from squidpy._constants._pkg_constants import Key
 from squidpy.im import (
-    segment,
     ImageContainer,
     SegmentationCustom,
     SegmentationWatershed,
+    segment,
 )
 from squidpy.im._segment import _SEG_DTYPE
-from squidpy._constants._constants import SegmentationBackend
-from squidpy._constants._pkg_constants import Key
 
 
 def dummy_segment(arr: np.ndarray) -> np.ndarray:
     assert isinstance(arr, np.ndarray)
     assert arr.ndim == 3
     return arr[..., 0].astype(np.uint32)
 
@@ -145,15 +144,15 @@
         assert small_cont["bar"].values.dtype == _SEG_DTYPE
         np.testing.assert_array_equal(small_cont["bar"].values, 0)
 
     @pytest.mark.parametrize("dask_input", [False, True])
     @pytest.mark.parametrize("chunks", [25, (50, 50, 1), "auto"])
     @pytest.mark.parametrize("lazy", [False, True])
     def test_dask_segment(
-        self, small_cont: ImageContainer, dask_input: bool, chunks: Union[int, Tuple[int, ...], str], lazy: bool
+        self, small_cont: ImageContainer, dask_input: bool, chunks: Union[int, tuple[int, ...], str], lazy: bool
     ):
         def func(chunk: np.ndarray):
             if isinstance(chunks, tuple):
                 np.testing.assert_array_equal(chunk.shape, [chunks[0] + 2 * d, chunks[1] + 2 * d, 1])
             elif isinstance(chunks, int):
                 np.testing.assert_array_equal(chunk.shape, [chunks + 2 * d, chunks + 2 * d, 1])
```

### Comparing `squidpy-1.2.3/tests/plotting/test_graph.py` & `squidpy-1.3.0/tests/plotting/test_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from copy import deepcopy
 from typing import Mapping
-import pytest
-
-from anndata import AnnData
-import scanpy as sc
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
-import matplotlib.pyplot as plt
-
+import pytest
+import scanpy as sc
+from anndata import AnnData
 from squidpy import gr, pl
+
 from tests.conftest import DPI, PlotTester, PlotTesterMeta
 
 C_KEY = "leiden"
 
 
 sc.pl.set_rcParams_defaults()
 sc.set_figure_params(dpi=40, color_map="viridis")
@@ -141,16 +139,18 @@
             pl.ligrec(ligrec_result, alpha=1.2)
 
     def test_invalid_means_range_size(self, ligrec_result: Mapping[str, pd.DataFrame]):
         with pytest.raises(ValueError, match=r"Expected `means_range` to be a sequence of size `2`, found `3`."):
             pl.ligrec(ligrec_result, means_range=[0, 1, 2])
 
     def test_invalid_clusters(self, ligrec_result: Mapping[str, pd.DataFrame]):
-        with pytest.raises(ValueError, match=r"No valid clusters have been selected."):
-            pl.ligrec(ligrec_result, source_groups="foo", target_groups="bar")
+        source_groups = "foo"
+        target_groups = "bar"
+        with pytest.raises(ValueError, match=r"Invalid cluster in .*"):
+            pl.ligrec(ligrec_result, source_groups=source_groups, target_groups=target_groups)
 
     def test_all_interactions_empty(self, ligrec_result: Mapping[str, pd.DataFrame]):
         empty = pd.DataFrame(np.nan, index=ligrec_result["pvalues"].index, columns=ligrec_result["pvalues"].columns)
 
         with pytest.raises(ValueError, match=r"After removing rows with only NaN interactions, none remain."):
             pl.ligrec({"means": empty, "pvalues": empty, "metadata": empty}, remove_empty_interactions=True)
```

### Comparing `squidpy-1.2.3/tests/plotting/test_image.py` & `squidpy-1.3.0/tests/plotting/test_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
 import pytest
-
-from anndata import AnnData
 import scanpy as sc
-
-import numpy as np
-
+import squidpy as sq
+from anndata import AnnData
 from matplotlib.testing.compare import compare_images
-import matplotlib.pyplot as plt
-
 from squidpy.im import ImageContainer
-from tests.conftest import DPI, TOL, ACTUAL, EXPECTED, PlotTester, PlotTesterMeta
-import squidpy as sq
+
+from tests.conftest import ACTUAL, DPI, EXPECTED, TOL, PlotTester, PlotTesterMeta
 
 
 class TestContainerShow(PlotTester, metaclass=PlotTesterMeta):
     def test_channelwise_wrong_number_of_axes(self, cont: ImageContainer):
         fig, ax = plt.subplots(dpi=DPI, tight_layout=True)
         with pytest.raises(ValueError, match=r"Expected `ax` to be of shape `\(1, 3\)`"):
             cont.show(ax=ax, channelwise=True)
@@ -66,44 +64,41 @@
         plt.savefig(ACTUAL / basename, dpi=DPI)
         plt.close()
         res = compare_images(str(EXPECTED / basename), ACTUAL / basename, TOL)
 
         assert res is None, res
 
 
-def test_extract(adata: AnnData, cont: ImageContainer, caplog):
-    """
-    Calculate features and extract columns to obs
-    """
-    # get obsm
+@pytest.mark.parametrize("is_view", [False, True])
+def test_extract(adata: AnnData, cont: ImageContainer, caplog, is_view: bool):
     sq.im.calculate_image_features(adata, cont, features=["summary"])
 
     # extract columns (default values)
-    extr_adata = sq.pl.extract(adata)
+    extr_adata = sq.pl.extract(adata[:10] if is_view else adata)
     # Test that expected columns exist
     for col in [
         "summary_ch-0_quantile-0.9",
         "summary_ch-0_quantile-0.5",
         "summary_ch-0_quantile-0.1",
         "summary_ch-1_quantile-0.9",
         "summary_ch-1_quantile-0.5",
         "summary_ch-1_quantile-0.1",
         "summary_ch-2_quantile-0.9",
         "summary_ch-2_quantile-0.5",
         "summary_ch-2_quantile-0.1",
     ]:
-        assert col in extr_adata.obs.columns
+        np.testing.assert_array_equal(np.isfinite(extr_adata.obs[col]), True)
 
     # get obsm that is a numpy array
     adata.obsm["pca_features"] = sc.pp.pca(np.asarray(adata.obsm["img_features"]), n_comps=3)
     # extract columns
-    extr_adata = sq.pl.extract(adata, obsm_key="pca_features", prefix="pca_features")
+    extr_adata = sq.pl.extract(adata[3:10] if is_view else adata, obsm_key="pca_features", prefix="pca_features")
     # Test that expected columns exist
     for col in ["pca_features_0", "pca_features_1", "pca_features_2"]:
-        assert col in extr_adata.obs.columns
+        np.testing.assert_array_equal(np.isfinite(extr_adata.obs[col]), True)
 
     # extract multiple obsm at once (no prefix)
     extr_adata = sq.pl.extract(adata, obsm_key=["img_features", "pca_features"])
     # Test that expected columns exist
     for col in [
         "summary_ch-0_quantile-0.9",
         "summary_ch-0_quantile-0.5",
@@ -114,16 +109,8 @@
         "summary_ch-2_quantile-0.9",
         "summary_ch-2_quantile-0.5",
         "summary_ch-2_quantile-0.1",
         "0",
         "1",
         "2",
     ]:
-        assert col in extr_adata.obs.columns
-
-    # TODO: test similarly to ligrec
-    # currently logging to stderr, and not captured by caplog
-    # extract obsm twice and make sure that warnings are issued
-    # with caplog.at_level(logging.WARNING):
-    #    extr2_adata = sq.pl.extract(extr_adata, obsm_key=['pca_features'])
-    #    log = caplog.text
-    #    assert "will be overwritten by extract" in log
+        np.testing.assert_array_equal(np.isfinite(extr_adata.obs[col]), True)
```

### Comparing `squidpy-1.2.3/tests/plotting/test_interactive.py` & `squidpy-1.3.0/tests/plotting/test_interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from typing import Tuple
-import sys
-import pytest
 import platform
+import sys
+from typing import Tuple
 
-from scanpy import settings as s
-from anndata import AnnData
-
-from scipy.sparse import issparse
+import matplotlib.pyplot as plt
 import numpy as np
-
+import pytest
+from anndata import AnnData
 from matplotlib.testing.compare import compare_images
-import matplotlib.pyplot as plt
-
+from scanpy import settings as s
+from scipy.sparse import issparse
 from squidpy.im import ImageContainer
-from tests.conftest import DPI, TOL, ACTUAL, EXPECTED, PlotTester, PlotTesterMeta
+
+from tests.conftest import ACTUAL, DPI, EXPECTED, TOL, PlotTester, PlotTesterMeta
 
 
 @pytest.mark.skipif(platform.system() == "Linux", reason="Fails on ubuntu")
 @pytest.mark.qt()
 class TestNapari(PlotTester, metaclass=PlotTesterMeta):
     def test_add_same_layer(self, adata: AnnData, napari_cont: ImageContainer, capsys):
         from napari.layers import Points
@@ -142,15 +140,15 @@
         viewer.screenshot(dpi=DPI)
 
     @pytest.mark.skip(reason="Soon to be deprecated.")
     @pytest.mark.parametrize("size", [(800, 600), (600, 800), (800, 800)])
     @pytest.mark.parametrize("x", [-200, 200])
     @pytest.mark.parametrize("y", [-200, 200])
     def test_corner_corner_cases(
-        self, qtbot, adata: AnnData, napari_cont: ImageContainer, y: int, x: int, size: Tuple[int, int]
+        self, qtbot, adata: AnnData, napari_cont: ImageContainer, y: int, x: int, size: tuple[int, int]
     ):
         viewer = napari_cont.crop_corner(y, x, size=size).interactive(adata)
         bdata = viewer.adata
         cnt = viewer._controller
 
         cnt.add_points(bdata.obs_vector(bdata.var_names[42]), layer_name="foo")
```

### Comparing `squidpy-1.2.3/tests/plotting/test_spatial_static.py` & `squidpy-1.3.0/tests/plotting/test_spatial_static.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 from __future__ import annotations
 
-from typing import Sequence
-from functools import partial
-import pytest
 import platform
+from functools import partial
+from typing import Sequence
 
-from anndata import AnnData
-import scanpy as sc
-
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
+import pytest
+import scanpy as sc
+from anndata import AnnData
 from matplotlib.colors import ListedColormap
-import matplotlib.pyplot as plt
-
 from squidpy import pl
+from squidpy._constants._pkg_constants import Key
 from squidpy.gr import spatial_neighbors
-from tests.conftest import PlotTester, PlotTesterMeta
 from squidpy.pl._spatial_utils import _get_library_id
-from squidpy._constants._pkg_constants import Key
+
+from tests.conftest import PlotTester, PlotTesterMeta
 
 sc.set_figure_params(dpi=40, color_map="viridis")
 
 # WARNING:
 # 1. all classes must both subclass PlotTester and use metaclass=PlotTesterMeta
 # 2. tests which produce a plot must be prefixed with `test_plot_`
 # 3. if the tolerance needs to be change, don't prefix the function with `test_plot_`, but with something else
 #    the comp. function can be accessed as `self.compare(<your_filename>, tolerance=<your_tolerance>)`
 #    ".png" is appended to <your_filename>, no need to set it
 
 
 class TestSpatialStatic(PlotTester, metaclass=PlotTesterMeta):
     def test_tol_plot_spatial_scatter_image(self, adata_hne: AnnData):
         pl.spatial_scatter(adata_hne, na_color="lightgrey")
-        self.compare("SpatialStatic_spatial_scatter_image", tolerance=60)
+        self.compare("SpatialStatic_spatial_scatter_image", tolerance=70)
 
     def test_plot_spatial_scatter_noimage(self, adata_hne: AnnData):
         pl.spatial_scatter(adata_hne, shape=None, na_color="lightgrey")
 
     def test_plot_spatial_scatter_group_outline(self, adata_hne: AnnData):
         pl.spatial_scatter(adata_hne, shape="circle", color="cluster", groups="Cortex_1", outline=True)
 
@@ -187,24 +185,25 @@
             crop_coord=[(100, 100, 500, 500), (100, 100, 500, 500), (100, 100, 500, 500)],
             img_alpha=0.5,
         )
 
     def test_plot_spatial_scatter_categorical_alpha(self, adata_hne: AnnData):
         pl.spatial_scatter(adata_hne, shape="circle", color="cluster", alpha=0)
 
-    def test_plot_spatial_scatter_non_unique_colors(self, adata_hne: AnnData):
+    def test_tol_plot_spatial_scatter_non_unique_colors(self, adata_hne: AnnData):
         adata_hne.uns["cluster_colors"] = ["#000000"] * len(adata_hne.uns["cluster_colors"])
         pl.spatial_scatter(adata_hne, color="cluster", legend_loc=None)
+        self.compare("SpatialStatic_spatial_scatter_non_unique_colors", tolerance=70)
 
     def test_tol_plot_palette_listed_cmap(self, adata_hne: AnnData):
         del adata_hne.uns["cluster_colors"]
         palette = plt.get_cmap("Set3")
         assert isinstance(palette, ListedColormap)
         pl.spatial_scatter(adata_hne, color="cluster", palette=palette, legend_loc=None)
-        self.compare("SpatialStatic_palette_listed_cmap", tolerance=60)
+        self.compare("SpatialStatic_palette_listed_cmap", tolerance=70)
 
 
 class TestSpatialStaticUtils:
     @staticmethod
     def _create_anndata(shape: str | None, library_id: str | Sequence[str] | None, library_key: str | None):
         n_obs = len(library_id) * 2 if isinstance(library_id, list) else 2
         X = np.empty((n_obs, 3))
```

### Comparing `squidpy-1.2.3/tests/read/test_visium.py` & `squidpy-1.3.0/tests/read/test_visium.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from anndata.tests.helpers import assert_adata_equal
-
-from squidpy.read import visium
 from squidpy._constants._pkg_constants import Key
+from squidpy.read import visium
 
 
 def test_read_visium():
     # Test that reading .h5 file works and does not have any global effects.
     h5_file_path = "tests/_data"
     spec_genome_v3 = visium(h5_file_path, genome="GRCh38", load_images=True)
     nospec_genome_v3 = visium(h5_file_path)
```

