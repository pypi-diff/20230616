# Comparing `tmp/python-kraken-sdk-1.3.0.tar.gz` & `tmp/python-kraken-sdk-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kraken-sdk-1.3.0.tar", last modified: Wed May 24 05:26:32 2023, max compression
+gzip compressed data, was "python-kraken-sdk-1.4.0.tar", last modified: Fri Jun 16 18:19:00 2023, max compression
```

## Comparing `python-kraken-sdk-1.3.0.tar` & `python-kraken-sdk-1.4.0.tar`

### file list

```diff
@@ -1,147 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.899058 python-kraken-sdk-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.879058 python-kraken-sdk-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.879058 python-kraken-sdk-1.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/self-review.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.879058 python-kraken-sdk-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_build_doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_test_futures_private.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_test_futures_public.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_test_spot_private.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/_test_spot_public.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/cicd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/manual_build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/manual_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/manual_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/manual_test_futures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/manual_test_spot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    54399 2023-05-24 05:26:32.899058 python-kraken-sdk-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/links.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/src/about/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/about/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/src/base_api/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/base_api/base_api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/src/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/examples/futures_bot_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/examples/spot_bot_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/examples/spot_orderbook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/examples/trading_bot_templates.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/src/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/futures/futures_rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/futures/futures_websocket.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/src/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/issues.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/src/krakenexceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/krakenexceptions/krakenexceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.883058 python-kraken-sdk-1.3.0/docs/src/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/spot/spot_rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/docs/src/spot/spot_websocket.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/examples/futures_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/examples/futures_trading_bot_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/examples/futures_ws_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)   364081 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/examples/market_client_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/examples/spot_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/examples/spot_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/examples/spot_trading_bot_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/examples/spot_ws_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 05:26:32.000000 python-kraken-sdk-1.3.0/kraken/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/base_api/
--rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/base_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/futures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/futures/funding/
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/futures/funding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/futures/market/
--rw-r--r--   0 runner    (1001) docker     (123)    39219 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/futures/market/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/futures/trade/
--rw-r--r--   0 runner    (1001) docker     (123)    26318 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/futures/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/futures/user/
--rw-r--r--   0 runner    (1001) docker     (123)    34937 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/futures/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/futures/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/futures/websocket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/futures/ws_client/
--rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/futures/ws_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/spot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/spot/funding/
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/spot/funding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.887058 python-kraken-sdk-1.3.0/kraken/spot/market/
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/spot/market/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.891058 python-kraken-sdk-1.3.0/kraken/spot/staking/
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/spot/staking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.891058 python-kraken-sdk-1.3.0/kraken/spot/trade/
--rw-r--r--   0 runner    (1001) docker     (123)    27479 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/spot/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.891058 python-kraken-sdk-1.3.0/kraken/spot/user/
--rw-r--r--   0 runner    (1001) docker     (123)    39347 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/spot/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.891058 python-kraken-sdk-1.3.0/kraken/spot/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)    23026 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/spot/websocket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.891058 python-kraken-sdk-1.3.0/kraken/spot/ws_client/
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/kraken/spot/ws_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.891058 python-kraken-sdk-1.3.0/python_kraken_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54399 2023-05-24 05:26:32.000000 python-kraken-sdk-1.3.0/python_kraken_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-24 05:26:32.000000 python-kraken-sdk-1.3.0/python_kraken_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 05:26:32.000000 python-kraken-sdk-1.3.0/python_kraken_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 05:26:32.000000 python-kraken-sdk-1.3.0/python_kraken_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 05:26:32.000000 python-kraken-sdk-1.3.0/python_kraken_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 05:26:32.899058 python-kraken-sdk-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.891058 python-kraken-sdk-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.895058 python-kraken-sdk-1.3.0/tests/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/test_futures_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/test_futures_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/test_futures_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/test_futures_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/test_futures_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/futures/test_futures_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:26:32.899058 python-kraken-sdk-1.3.0/tests/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/test_spot_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/test_spot_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/test_spot_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/test_spot_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/test_spot_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/test_spot_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    15971 2023-05-24 05:26:16.000000 python-kraken-sdk-1.3.0/tests/spot/test_spot_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.503831 python-kraken-sdk-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.487831 python-kraken-sdk-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.487831 python-kraken-sdk-1.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/self-review.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_build_doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_test_futures_private.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_test_futures_public.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_test_spot_private.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/_test_spot_public.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/cicd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/manual_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/manual_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/manual_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/manual_test_futures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/manual_test_spot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    54494 2023-06-16 18:19:00.499831 python-kraken-sdk-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/links.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/src/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/about/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/src/base_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/base_api/base_api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/examples/futures_bot_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/examples/spot_bot_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/examples/spot_orderbook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/examples/trading_bot_templates.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/src/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/futures/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/futures/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/src/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/issues.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/src/krakenexceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/krakenexceptions/krakenexceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.491831 python-kraken-sdk-1.4.0/docs/src/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/spot/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/docs/src/spot/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.495831 python-kraken-sdk-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/examples/futures_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/examples/futures_trading_bot_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/examples/futures_ws_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)   364081 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/examples/market_client_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/examples/spot_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/examples/spot_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/examples/spot_trading_bot_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/examples/spot_ws_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.495831 python-kraken-sdk-1.4.0/kraken/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 18:19:00.000000 python-kraken-sdk-1.4.0/kraken/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.495831 python-kraken-sdk-1.4.0/kraken/base_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/base_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.495831 python-kraken-sdk-1.4.0/kraken/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.495831 python-kraken-sdk-1.4.0/kraken/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/futures/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39217 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26338 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/futures/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34957 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/futures/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.495831 python-kraken-sdk-1.4.0/kraken/futures/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/futures/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/futures/ws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.495831 python-kraken-sdk-1.4.0/kraken/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39336 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.495831 python-kraken-sdk-1.4.0/kraken/spot/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26546 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/kraken/spot/ws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.499831 python-kraken-sdk-1.4.0/python_kraken_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54494 2023-06-16 18:19:00.000000 python-kraken-sdk-1.4.0/python_kraken_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-16 18:19:00.000000 python-kraken-sdk-1.4.0/python_kraken_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:19:00.000000 python-kraken-sdk-1.4.0/python_kraken_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-16 18:19:00.000000 python-kraken-sdk-1.4.0/python_kraken_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 18:19:00.000000 python-kraken-sdk-1.4.0/python_kraken_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:19:00.503831 python-kraken-sdk-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.499831 python-kraken-sdk-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.499831 python-kraken-sdk-1.4.0/tests/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/test_futures_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/test_futures_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/test_futures_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/test_futures_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/test_futures_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/futures/test_futures_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.499831 python-kraken-sdk-1.4.0/tests/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:19:00.499831 python-kraken-sdk-1.4.0/tests/spot/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/fixture/orderbook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/test_spot_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/test_spot_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/test_spot_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/test_spot_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/test_spot_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/test_spot_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/test_spot_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-16 18:18:48.000000 python-kraken-sdk-1.4.0/tests/spot/test_spot_websocket.py
```

### Comparing `python-kraken-sdk-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `python-kraken-sdk-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `python-kraken-sdk-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/codecov.yml` & `python-kraken-sdk-1.4.0/.github/codecov.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,10 +14,10 @@
     patch:
       default:
         informational: true
 
 comment:
   layout: "reach, diff, flags, files"
   behavior: default
-  require_changes: true # if false: post the comment even if coverage don't change
+  require_changes: true # if false: post the comment even if coverage doesn't change
   require_base: no # [yes :: must have a base report to post]
   require_head: yes # [yes :: must have a head report to post]
```

### Comparing `python-kraken-sdk-1.3.0/.github/pull_request_template.md` & `python-kraken-sdk-1.4.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/self-review.md` & `python-kraken-sdk-1.4.0/.github/self-review.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_build.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_build.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_build_doc.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_build_doc.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_codecov.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_codecov.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_codeql.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_codeql.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_pypi_publish.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_test_futures_private.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_test_futures_private.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_test_futures_public.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_test_futures_public.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_test_spot_private.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_test_spot_private.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/_test_spot_public.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/_test_spot_public.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/cicd.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/manual_build.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/manual_build.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/manual_test_futures.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/manual_test_futures.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/manual_test_spot.yaml` & `python-kraken-sdk-1.4.0/.github/workflows/manual_test_spot.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.github/workflows/release.yml` & `python-kraken-sdk-1.4.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.gitignore` & `python-kraken-sdk-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.pre-commit-config.yaml` & `python-kraken-sdk-1.4.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,14 @@
       - id: check-executables-have-shebangs
       - id: trailing-whitespace
       - id: fix-byte-order-marker
       - id: fix-encoding-pragma
       - id: mixed-line-ending
       - id: requirements-txt-fixer
       - id: end-of-file-fixer
-      - id: pretty-format-json
       - id: detect-private-key
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: python-use-type-annotations
       - id: rst-backticks
       # - id: rst-inline-touching-normal
```

### Comparing `python-kraken-sdk-1.3.0/.pylintrc` & `python-kraken-sdk-1.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/.readthedocs.yaml` & `python-kraken-sdk-1.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/CHANGELOG.md` & `python-kraken-sdk-1.4.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 # Changelog
 
 ## [Unreleased](https://github.com/btschwertfeger/python-kraken-sdk/tree/HEAD)
 
-[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.2.0...HEAD)
+[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.3.0...HEAD)
+
+**Implemented enhancements:**
+
+- Add the `truncate` parameter to `create_order` of the Spot websocket client [\#111](https://github.com/btschwertfeger/python-kraken-sdk/issues/111)
+- Add the `truncate` parameter to create_order of the Spot websocket clients' `create_order` and `cancel_order`+ `kraken.spot.Trade.edit_order` [\#113](https://github.com/btschwertfeger/python-kraken-sdk/pull/113) ([btschwertfeger](https://github.com/btschwertfeger))
+
+Uncategorized merged pull requests:
+
+- Update `/examples/spot_orderbook.py` [\#110](https://github.com/btschwertfeger/python-kraken-sdk/pull/110) ([btschwertfeger](https://github.com/btschwertfeger))
+
+## [v1.3.0](https://github.com/btschwertfeger/python-kraken-sdk/tree/v1.3.0) (2023-05-24)
+
+[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.2.0...v1.3.0)
 
 **Breaking changes:**
 
+- Rename `kraken.futures.User.get_unwindqueue` to `kraken.futures.User.get_unwind_queue` [\#107](https://github.com/btschwertfeger/python-kraken-sdk/issues/107)
+- Prepare release v1.3.0 [\#99](https://github.com/btschwertfeger/python-kraken-sdk/pull/99) ([btschwertfeger](https://github.com/btschwertfeger))
 - Change `kraken.spot.User.get_balances` and add `kraken.spot.User.get_balance` [\#98](https://github.com/btschwertfeger/python-kraken-sdk/pull/98) ([btschwertfeger](https://github.com/btschwertfeger))
 - Rename `get_tradeable_asset_pair` to `get_asset_pairs` and make the `pair` parameter optional [\#93](https://github.com/btschwertfeger/python-kraken-sdk/pull/93) ([btschwertfeger](https://github.com/btschwertfeger))
 - Extend typing + add `KrakenUnknownMethodError` and `KrakenBadRequestError` + Fix \#65 [\#87](https://github.com/btschwertfeger/python-kraken-sdk/pull/87) ([btschwertfeger](https://github.com/btschwertfeger))
 
 **Implemented enhancements:**
 
 - `kraken.spot.Trade.create_order`: Ability to use floats as trade amounts or prices [\#94](https://github.com/btschwertfeger/python-kraken-sdk/issues/94)
@@ -20,14 +35,15 @@
 **Fixed bugs:**
 
 - `kraken.spot.User(...).get_balances('ZUSD')` silently does the wrong thing. [\#88](https://github.com/btschwertfeger/python-kraken-sdk/issues/88)
 - `kraken.spot.Trade.cancel_order_batch` endpoint in Spot trading does not work. `{'error': ['EAPI:Bad request']}` [\#65](https://github.com/btschwertfeger/python-kraken-sdk/issues/65)
 
 **Closed issues:**
 
+- Add a realtime Spot order book example [\#103](https://github.com/btschwertfeger/python-kraken-sdk/issues/103)
 - `kraken.spot.Trade.create_order`: documentatoin for txid outdated. [\#96](https://github.com/btschwertfeger/python-kraken-sdk/issues/96)
 - Create `CONTRIBUTING.md` [\#91](https://github.com/btschwertfeger/python-kraken-sdk/issues/91)
 - Extend the typing - using mypy [\#84](https://github.com/btschwertfeger/python-kraken-sdk/issues/84)
 
 Uncategorized merged pull requests:
 
 - Create a contribution guideline [\#92](https://github.com/btschwertfeger/python-kraken-sdk/pull/92) ([btschwertfeger](https://github.com/btschwertfeger))
```

### Comparing `python-kraken-sdk-1.3.0/CODE_OF_CONDUCT.md` & `python-kraken-sdk-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/CONTRIBUTING.md` & `python-kraken-sdk-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/LICENSE` & `python-kraken-sdk-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/Makefile` & `python-kraken-sdk-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/PKG-INFO` & `python-kraken-sdk-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kraken-sdk
-Version: 1.3.0
+Version: 1.4.0
 Summary: Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,15 @@
 
 ## Features
 
 Clients:
 
 - Spot REST Clients
 - Spot Websocket Client
+- Spot Orderbook Client
 - Futures REST Clients
 - Futures Websocket Client
 
 General:
 
 - access both public and private endpoints
 - responsive error handling and custom exceptions
@@ -756,15 +757,15 @@
 ```bash
 python3 -m pip install python-kraken-sdk
 ```
 
 ### 2. Register at Kraken and generate API Keys:
 
 - Spot Trading: https://www.kraken.com/u/security/api
-- Futures Trading: https://futures.kraken.com/trade/settings/api
+- Futures Trading: https://futures.kraken.com/trade/settings/api (see _[help](https://docs.futures.kraken.com/#introduction-generate-api-keys)_)
 - Futures Sandbox: https://demo-futures.kraken.com/settings/api
 
 ### 3. Start using the provided example scripts
 
 ### 4. Error handling
 
 If any unexpected behavior occurs, please check <b style="color: yellow">your API permissions</b>, <b style="color: yellow">rate limits</b>, update the python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error persists please open an issue.
@@ -845,15 +846,15 @@
 ... can be found in `/examples/spot_ws_examples.py`
 
 ```python
 import time
 import asyncio
 from kraken.spot import KrakenSpotWSClient
 
-async def main() -> None:
+async def main()
 
     key = "kraken-public-key"
     secret = "kraken-secret-key"
 
     class Bot(KrakenSpotWSClient):
         async def on_message(self, msg):
             if isinstance(msg, dict) and "event" in msg:
```

### Comparing `python-kraken-sdk-1.3.0/README.md` & `python-kraken-sdk-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 ## Features
 
 Clients:
 
 - Spot REST Clients
 - Spot Websocket Client
+- Spot Orderbook Client
 - Futures REST Clients
 - Futures Websocket Client
 
 General:
 
 - access both public and private endpoints
 - responsive error handling and custom exceptions
@@ -84,15 +85,15 @@
 ```bash
 python3 -m pip install python-kraken-sdk
 ```
 
 ### 2. Register at Kraken and generate API Keys:
 
 - Spot Trading: https://www.kraken.com/u/security/api
-- Futures Trading: https://futures.kraken.com/trade/settings/api
+- Futures Trading: https://futures.kraken.com/trade/settings/api (see _[help](https://docs.futures.kraken.com/#introduction-generate-api-keys)_)
 - Futures Sandbox: https://demo-futures.kraken.com/settings/api
 
 ### 3. Start using the provided example scripts
 
 ### 4. Error handling
 
 If any unexpected behavior occurs, please check <b style="color: yellow">your API permissions</b>, <b style="color: yellow">rate limits</b>, update the python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error persists please open an issue.
@@ -173,15 +174,15 @@
 ... can be found in `/examples/spot_ws_examples.py`
 
 ```python
 import time
 import asyncio
 from kraken.spot import KrakenSpotWSClient
 
-async def main() -> None:
+async def main()
 
     key = "kraken-public-key"
     secret = "kraken-secret-key"
 
     class Bot(KrakenSpotWSClient):
         async def on_message(self, msg):
             if isinstance(msg, dict) and "event" in msg:
```

### Comparing `python-kraken-sdk-1.3.0/docs/Makefile` & `python-kraken-sdk-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/conf.py` & `python-kraken-sdk-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/index.rst` & `python-kraken-sdk-1.4.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 =============================================
 
 |GitHub badge| |License badge| |PyVersions badge| |Downloads badge|
 |CodeQL badge| |CI/CD badge| |codecov badge| |Typing badge|
 |Release date badge| |Release version badge| |DOI badge|
 
 .. toctree::
-   :maxdepth: 2
    :caption: Contents:
+   :maxdepth: 2
 
    src/introduction.rst
    src/getting_started/getting_started.rst
    src/examples/trading_bot_templates.rst
    src/issues.rst
-   src/spot/spot_rest.rst
-   src/spot/spot_websocket.rst
-   src/futures/futures_rest.rst
-   src/futures/futures_websocket.rst
+   src/spot/rest.rst
+   src/spot/websockets.rst
+   src/futures/rest.rst
+   src/futures/websockets.rst
    src/base_api/base_api.rst
    src/krakenexceptions/krakenexceptions.rst
    src/about/license.rst
 
 Indices and tables
 ==================
```

### Comparing `python-kraken-sdk-1.3.0/docs/links.rst` & `python-kraken-sdk-1.4.0/docs/links.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/make.bat` & `python-kraken-sdk-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/src/examples/futures_bot_template.rst` & `python-kraken-sdk-1.4.0/docs/src/examples/futures_bot_template.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/src/examples/spot_bot_template.rst` & `python-kraken-sdk-1.4.0/docs/src/examples/spot_bot_template.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/src/examples/trading_bot_templates.rst` & `python-kraken-sdk-1.4.0/docs/src/examples/trading_bot_templates.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/src/getting_started/getting_started.rst` & `python-kraken-sdk-1.4.0/docs/src/getting_started/getting_started.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/src/introduction.rst` & `python-kraken-sdk-1.4.0/docs/src/introduction.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/docs/src/issues.rst` & `python-kraken-sdk-1.4.0/docs/src/issues.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Known Issues
 ============
 
+Issues listed here: `python-kraken-sdk/issues`_
+
 Futures Trading
 ---------------
 
 - Kraken's API doesn't seem to know the ``trailing_stop`` order type and raises an error if this type
   is part of an order. This order type is documented here https://docs.futures.kraken.com/#http-api-trading-v3-api-order-management-send-order
 
   .. code-block:: python
```

### Comparing `python-kraken-sdk-1.3.0/examples/futures_examples.py` & `python-kraken-sdk-1.4.0/examples/futures_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/examples/futures_trading_bot_template.py` & `python-kraken-sdk-1.4.0/examples/futures_trading_bot_template.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/examples/futures_ws_examples.py` & `python-kraken-sdk-1.4.0/examples/futures_ws_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/examples/market_client_example.ipynb` & `python-kraken-sdk-1.4.0/examples/market_client_example.ipynb`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/examples/spot_examples.py` & `python-kraken-sdk-1.4.0/examples/spot_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/examples/spot_trading_bot_template.py` & `python-kraken-sdk-1.4.0/examples/spot_trading_bot_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 
 import requests
 import urllib3
 
 from kraken.exceptions import KrakenException
 from kraken.spot import Funding, KrakenSpotWSClient, Market, Staking, Trade, User
 
-logging.basicConfig(
-    format="%(asctime)s %(module)s,line: %(lineno)d %(levelname)8s | %(message)s",
-    datefmt="%Y/%m/%d %H:%M:%S",
-    level=logging.INFO,
-)
-logging.getLogger().setLevel(logging.INFO)
-logging.getLogger("requests").setLevel(logging.WARNING)
-logging.getLogger("urllib3").setLevel(logging.WARNING)
-
 
 class TradingBot(KrakenSpotWSClient):
     """
     Class that implements the trading strategy
 
     * The on_message function gets all events from the websocket feed
     * Decisions can be made based on these events
```

### Comparing `python-kraken-sdk-1.3.0/examples/spot_ws_examples.py` & `python-kraken-sdk-1.4.0/examples/spot_ws_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 logging.getLogger("requests").setLevel(logging.WARNING)
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 
 async def main() -> None:
     """Create bot and subscribe to topics/feeds"""
 
-    key: str = os.getenv("API_KEY")
-    secret: str = os.getenv("SECRET_KEY")
+    key: str = os.getenv("SPOT_API_KEY")
+    secret: str = os.getenv("SPOT_SECRET_KEY")
 
     # ___Custom_Trading_Bot______________
     class Bot(KrakenSpotWSClient):
         """Can be used to create a custom trading strategy/bot"""
 
         async def on_message(self: "Bot", msg: Union[list, dict]) -> None:
             """Receives the websocket messages"""
@@ -43,17 +43,17 @@
                 topic = msg["event"]
                 if topic in ("heartbeat", "pong"):
                     return
 
             print(msg)
             # if condition:
             #     await self.create_order(
-            #         ordertype='limit',
-            #         side='buy',
-            #         pair='BTC/EUR',
+            #         ordertype="limit",
+            #         side="buy",
+            #         pair="BTC/EUR",
             #         price=20000,
             #         volume=200
             #     )
             # ... it is also possible to call regular REST endpoints
             # but using the websocket messages is more efficient
             # you can also un/subscribe here using self.subscribe/self-unsubscribe
```

### Comparing `python-kraken-sdk-1.3.0/kraken/base_api/__init__.py` & `python-kraken-sdk-1.4.0/kraken/base_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import base64
 import hashlib
 import hmac
 import json
 import time
 import urllib.parse
+from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 from urllib.parse import urljoin
 from uuid import uuid1
 
 import requests
 
 from kraken.exceptions import KrakenException
@@ -50,14 +51,15 @@
     :param parameter_name: The parameter name to transform into string
     :type parameter_name: str
     :return: The called function
     :rtype: Callable
     """
 
     def decorator(func: Callable) -> Callable:
+        @wraps(func)  # required for sphinx to discover the func
         def wrapper(*args: Any, **kwargs: Any) -> Any:
             if parameter_name in kwargs:
                 value: Any = kwargs[parameter_name]
                 if isinstance(value, str) or value is None:
                     pass
                 elif isinstance(value, list):
                     kwargs[parameter_name] = ",".join(value)
@@ -182,15 +184,14 @@
         if sandbox:
             raise ValueError("Sandbox not available for Kraken Spot trading.")
         if url != "":
             self.url = url
         else:
             self.url = urljoin(self.URL, self.API_V)
 
-        self.__nonce: int = 0
         self.__key: str = key
         self.__secret: str = secret
         self.__use_custom_exceptions: bool = use_custom_exceptions
 
         self.__err_handler: KrakenErrorHandler = KrakenErrorHandler()
         self.__session: requests.Session = requests.Session()
         self.__session.headers.update({"User-Agent": "python-kraken-sdk"})
@@ -243,17 +244,16 @@
             if (
                 not self.__key
                 or self.__key == ""
                 or not self.__secret
                 or self.__secret == ""
             ):
                 raise ValueError("Missing credentials.")
-            self.__nonce = (self.__nonce + 1) % 1
-            params["nonce"] = str(int(time.time() * 1000)) + str(self.__nonce).zfill(4)
 
+            params["nonce"] = str(int(time.time() * 100_000_000))
             content_type: str
             sign_data: str
 
             if do_json:
                 content_type = "application/json; charset=utf-8"
                 sign_data = json.dumps(params)
             else:
@@ -410,15 +410,14 @@
         elif self.sandbox:
             self.url = self.SANDBOX_URL
         else:
             self.url = self.URL
 
         self.__key: str = key
         self.__secret: str = secret
-        self.__nonce: int = 0
         self.__use_custom_exceptions: bool = use_custom_exceptions
 
         self.__err_handler: KrakenErrorHandler = KrakenErrorHandler()
         self.__session: requests.Session = requests.Session()
         self.__session.headers.update({"User-Agent": "python-kraken-sdk"})
 
     def _request(
@@ -478,16 +477,15 @@
             if (
                 not self.__key
                 or self.__key == ""
                 or not self.__secret
                 or self.__secret == ""
             ):
                 raise ValueError("Missing credentials")
-            self.__nonce = (self.__nonce + 1) % 1
-            nonce: str = str(int(time.time() * 1000)) + str(self.__nonce).zfill(4)
+            nonce: str = str(int(time.time() * 100_000_000))
             headers.update(
                 {
                     "Content-Type": "application/x-www-form-urlencoded; charset=utf-8",
                     "Nonce": nonce,
                     "APIKey": self.__key,
                     "Authent": self._get_kraken_futures_signature(
                         uri, query_string + post_string, nonce
```

### Comparing `python-kraken-sdk-1.3.0/kraken/exceptions/__init__.py` & `python-kraken-sdk-1.4.0/kraken/exceptions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         self.EXCEPTION_ASSIGNMENT: Dict[str, Any] = {
             ##      Spot, Margin, and Futures trading Errors
             ##
             "EGeneral:Invalid arguments": self.KrakenInvalidArgumentsError,
             "EGeneral:Invalid arguments:Index unavailable": self.KrakenInvalidArgumentsIndexUnavailableError,
             "EGeneral:Permission denied": self.KrakenPermissionDeniedError,
             "EGeneral:Unknown method": self.KrakenUnknownMethodError,
+            "EGeneral:Temporary lockout": self.KrakenTemporaryLockoutError,
             "EService:Unavailable": self.KrakenServiceUnavailableError,
             "EService:Market in cancel_only mode": self.KrakenMarketInOnlyCancelModeError,
             "EService:Market in post_only mode": self.KrakenMarketInOnlyPostModeError,
             "EService:Deadline elapsed": self.KrakenDeadlineElapsedError,
             "EAPI:Invalid key": self.KrakenInvalidAPIKeyError,
             "EAPI:Invalid signature": self.KrakenInvalidSignatureError,
             "EAPI:Invalid nonce": self.KrakenInvalidNonceError,
@@ -295,11 +296,15 @@
     class KrakenToManyAddressesError(Exception):
         """To many addresses specified."""
 
     @docstring_message
     class KrakenUnknownMethodError(Exception):
         """The endpoint or method is not known."""
 
+    @docstring_message
+    class KrakenTemporaryLockoutError(Exception):
+        """The account was temporary locked out."""
+
     # ? ____CUSTOM_EXCEPTIONS_________
     @docstring_message
     class MaxReconnectError(Exception):
         """To many reconnect tries."""
```

### Comparing `python-kraken-sdk-1.3.0/kraken/futures/funding/__init__.py` & `python-kraken-sdk-1.4.0/kraken/futures/funding.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 
 """Module that implements the Kraken Futures Funding client"""
 
 from typing import Optional, Union
 
-from ...base_api import KrakenBaseFuturesAPI
+from ..base_api import KrakenBaseFuturesAPI
 
 
 class Funding(KrakenBaseFuturesAPI):
     """
     Class that implements the Kraken Futures Funding client
 
     If the sandbox environment is chosen, the keys must be generated from here:
```

### Comparing `python-kraken-sdk-1.3.0/kraken/futures/market/__init__.py` & `python-kraken-sdk-1.4.0/kraken/futures/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # GitHub: https://github.com/btschwertfeger
 
 """Module that implements the Kraken Futures market client"""
 
 from functools import lru_cache
 from typing import List, Optional, Union
 
-from ...base_api import KrakenBaseFuturesAPI, defined
+from ..base_api import KrakenBaseFuturesAPI, defined
 
 
 class Market(KrakenBaseFuturesAPI):
 
     """
     Class that implements the Kraken Futures market client
 
@@ -286,15 +286,15 @@
         :param symbol: The asset/symbol to get the orderbook from
         :type symbol: str, optional
         :return: The current orderbook for the futures contracts
         :rtype: dict
 
         .. code-block:: python
             :linenos:
-            :caption: Futures Market: Get the assets order book
+            :caption: Futures Market: Get the assets orderbook
 
             >>> from kraken.futures import Market
             >>> Market().get_orderbook(symbol="PI_XBTUSD")
             {
                 'result': 'success', 'orderBook': {
                     'bids': [
                         [27909, 3000], [27908.5, 1703], [27906, 1716],
```

### Comparing `python-kraken-sdk-1.3.0/kraken/futures/trade/__init__.py` & `python-kraken-sdk-1.4.0/kraken/futures/trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the Kraken Futures trade client"""
 
 from typing import List, Optional, Tuple, Union
 
-from ...base_api import KrakenBaseFuturesAPI, defined
+from ..base_api import KrakenBaseFuturesAPI, defined
 
 
 class Trade(KrakenBaseFuturesAPI):
     """
     Class that implements the Kraken Futures trade client
 
     If the sandbox environment is chosen, the keys must be generated from here:
@@ -20,15 +20,15 @@
 
     :param key: Futures API public key (default: ``""``)
     :type key: str, optional
     :param secret: Futures API secret key (default: ``""``)
     :type secret: str, optional
     :param url: Alternative URL to access the Futures Kraken API (default: https://futures.kraken.com)
     :type url: str, optional
-    :param sandbox: If set to ``True`` the URL will be https://demo-futures.kraken.com
+    :param sandbox: If set to ``True`` the URL will be https://demo-futures.kraken.com (default: ``False``)
     :type sandbox: bool, optional
 
     .. code-block:: python
         :linenos:
         :caption: Futures Trade: Create the trade client
 
         >>> from kraken.futures import Trade
```

### Comparing `python-kraken-sdk-1.3.0/kraken/futures/user/__init__.py` & `python-kraken-sdk-1.4.0/kraken/futures/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """Module that implements the Kraken Futures user client"""
 
 from typing import Optional, Union
 
 import requests
 
-from ...base_api import KrakenBaseFuturesAPI, defined
+from ..base_api import KrakenBaseFuturesAPI, defined
 
 
 class User(KrakenBaseFuturesAPI):
     """
     Class that implements the Kraken Futures user client
 
     If the sandbox environment is chosen, the keys must be generated from here:
@@ -22,15 +22,15 @@
 
     :param key: Futures API public key (default: ``""``)
     :type key: str, optional
     :param secret: Futures API secret key (default: ``""``)
     :type secret: str, optional
     :param url: Alternative URL to access the Futures Kraken API (default: https://futures.kraken.com)
     :type url: str, optional
-    :param sandbox: If set to ``True`` the URL will be https://demo-futures.kraken.com
+    :param sandbox: If set to ``True`` the URL will be https://demo-futures.kraken.com (default: ``False``)
     :type sandbox: bool, optional
 
     .. code-block:: python
         :linenos:
         :caption: Futures User: Create the user client
 
         >>> from kraken.futures import User
```

### Comparing `python-kraken-sdk-1.3.0/kraken/futures/websocket/__init__.py` & `python-kraken-sdk-1.4.0/kraken/futures/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/kraken/futures/ws_client/__init__.py` & `python-kraken-sdk-1.4.0/kraken/futures/ws_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
-"""Provides the KrakenWsClientCl class to use the Kraken Futures websockets."""
+"""Provides the websocket client for Kraken Futures"""
 
 import base64
 import hashlib
 import hmac
 import logging
 from copy import deepcopy
 from typing import Any, Dict, List, Optional
 
-from ...base_api import KrakenBaseFuturesAPI
-from ...exceptions import KrakenException
-from ...futures.websocket import ConnectFuturesWebsocket
+from ..base_api import KrakenBaseFuturesAPI
+from ..exceptions import KrakenException
+from .websocket import ConnectFuturesWebsocket
 
 
 class KrakenFuturesWSClient(KrakenBaseFuturesAPI):
     """
     Class to access public and (optional)
     private/authenticated websocket connection.
```

### Comparing `python-kraken-sdk-1.3.0/kraken/spot/funding/__init__.py` & `python-kraken-sdk-1.4.0/kraken/spot/funding.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the Spot Funding client"""
 
 from typing import List, Optional, Union
 
-from ...base_api import KrakenBaseSpotAPI, defined
+from ..base_api import KrakenBaseSpotAPI, defined
 
 
 class Funding(KrakenBaseSpotAPI):
     """
     Class that implements the Spot Funding client. Currently there
     are no funding endpoints that could be accesses without authentication.
```

### Comparing `python-kraken-sdk-1.3.0/kraken/spot/market/__init__.py` & `python-kraken-sdk-1.4.0/kraken/spot/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
-"""Module that implements the Kraken Spot market client"""
+"""Module that implements the Kraken Spot Market client"""
 
 from functools import lru_cache
 from typing import List, Optional, Union
 
-from ...base_api import KrakenBaseSpotAPI, defined, ensure_string
+from ..base_api import KrakenBaseSpotAPI, defined, ensure_string
 
 
 class Market(KrakenBaseSpotAPI):
     """
     Class that implements the Kraken Spot Market client. Can be used to access
     the Kraken Spot market data.
 
@@ -300,15 +300,15 @@
         :type count: int, optional
 
         :return:
         :rtype: dict
 
         .. code-block:: python
             :linenos:
-            :caption: Spot Market: Get the order book
+            :caption: Spot Market: Get the orderbook
 
             >>> from kraken.spot import Market
             >>> Market().get_order_book(pair="XBTUSD", count=2)
             {
                 'XXBTZUSD': {
                     'asks': [
                         ['28000.00000', '1.091', 1680714417],
```

### Comparing `python-kraken-sdk-1.3.0/kraken/spot/staking/__init__.py` & `python-kraken-sdk-1.4.0/kraken/spot/staking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
-"""Module that implements the Kraken Spot Stakung client"""
+"""Module that implements the Kraken Spot Staking client"""
 
 from typing import List, Optional, Union
 
-from ...base_api import KrakenBaseSpotAPI, defined
+from ..base_api import KrakenBaseSpotAPI, defined
 
 
 class Staking(KrakenBaseSpotAPI):
     """
     Class that implements the Kraken Spot Staking client. Currently there
     are no staking endpoints that could be accesses without authentication.
```

### Comparing `python-kraken-sdk-1.3.0/kraken/spot/trade/__init__.py` & `python-kraken-sdk-1.4.0/kraken/spot/trade.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 """Module that implements the Kraken Trade Spot client"""
 
 from decimal import Decimal
 from functools import lru_cache
 from math import floor
 from typing import List, Optional, Union
 
-from ...base_api import KrakenBaseSpotAPI, defined, ensure_string
-from ...spot import Market
+from ..base_api import KrakenBaseSpotAPI, defined, ensure_string
+from .market import Market
 
 
 class Trade(KrakenBaseSpotAPI):
     """
     Class that implements the Kraken Trade Spot client
 
     :param key: Spot API public key (default: ``""``)
@@ -129,15 +129,15 @@
         :type stptype: str, optional
         :param oflags: Order flags like ``post``, ``fcib``, ``fciq``, ``nomp``,
             ``viqc`` (see the referenced Kraken documentation for more information)
         :type oflags: str | List[str], optional
         :param timeinforce: how long the order remains in the orderbook, one of:
             ``GTC``, ``IOC``, ``GTD`` (see the referenced Kraken documentation for more information)
         :type timeinforce: str, optional
-        :param displayvol: Define how much of the volume is visible in the order book (iceberg)
+        :param displayvol: Define how much of the volume is visible in the orderbook (iceberg)
         :type displayvol: str | int | float, optional
         :param starttim: Unix timestamp or seconds defining the start time (default: ``"0"``)
         :type starttim: str, optional
         :param expiretm: Unix timestamp or time in seconds defining the expiration of the order,
             (default: ``"0"`` - i.e., no expiration)
         :type expiretm: str, optional
         :param close_ordertype: Conditional close order type, one of: ``limit``, ``stop-loss``,
@@ -311,38 +311,34 @@
             "take-profit-limit",
         )
 
         if defined(trigger):
             if ordertype not in trigger_ordertypes:
                 raise ValueError(f"Cannot use trigger on ordertype {ordertype}!")
             params["trigger"] = trigger
-
         if defined(timeinforce):
             params["timeinforce"] = timeinforce
         if defined(expiretm):
             params["expiretm"] = str(expiretm)
-
         if defined(price):
             params["price"] = (
                 price
                 if not truncate
                 else self.truncate(amount=price, amount_type="price", pair=pair)
             )
-
         if ordertype in ("stop-loss-limit", "take-profit-limit"):
             if not defined(price2):
                 raise ValueError(
                     f"Ordertype {ordertype} requires a secondary price (price2)!"
                 )
             params["price2"] = str(price2)
         elif price2 is not None:
             raise ValueError(
                 f"Ordertype {ordertype} dos not allow a second price (price2)!"
             )
-
         if defined(leverage):
             params["leverage"] = str(leverage)
         if defined(oflags):
             params["oflags"] = oflags
         if defined(close_ordertype):
             params["close[ordertype]"] = close_ordertype
         if defined(close_price):
@@ -439,14 +435,15 @@
     def edit_order(
         self: "Trade",
         txid: str,
         pair: str,
         volume: Optional[Union[str, int, float]] = None,
         price: Optional[Union[str, int, float]] = None,
         price2: Optional[Union[str, int, float]] = None,
+        truncate: bool = False,
         oflags: Optional[str] = None,
         deadline: Optional[str] = None,
         cancel_response: Optional[bool] = None,
         validate: bool = False,
         userref: Optional[int] = None,
     ) -> dict:
         """
@@ -463,14 +460,18 @@
         :type pair: str
         :param volume: Set a new volume
         :type volume: str | int | float, optional
         :param price: Set a new price
         :type price: str | int | float, optional
         :param price2: Set a new second price
         :type price2: str | int | float, optional
+        :param truncate: If enabled: round the ``price`` and ``volume`` to Kraken's
+            maximum allowed decimal places. See https://support.kraken.com/hc/en-us/articles/4521313131540
+            fore more information about decimals.
+        :type truncate: bool, optional
         :param oflags: Order flags like ``post``, ``fcib``, ``fciq``, ``nomp``, ``viqc`` (see the referenced Kraken documentation for more information)
         :type oflags: str | List[str], optional
         :param deadline: (see the referenced Kraken documentation for more information)
         :type deadline: string
         :param cancel_response: See the referenced Kraken documentation for more information
         :type cancel_response: bool, optional
         :param validate: Validate the order without placing on the market (default: ``False``)
@@ -503,17 +504,25 @@
                 }
             }
         """
         params: dict = {"txid": txid, "pair": pair, "validate": validate}
         if defined(userref):
             params["userref"] = userref
         if defined(volume):
-            params["volume"] = volume
+            params["volume"] = (
+                str(volume)
+                if not truncate
+                else self.truncate(amount=volume, amount_type="volume", pair=pair)
+            )
         if defined(price):
-            params["price"] = price
+            params["price"] = (
+                str(price)
+                if not truncate
+                else self.truncate(amount=price, amount_type="price", pair=pair)
+            )
         if defined(price2):
             params["price2"] = price2
         if defined(oflags):
             params["oflags"] = oflags
         if defined(cancel_response):
             params["cancel_response"] = cancel_response
         if defined(deadline):
@@ -669,14 +678,46 @@
         :raises ValueError: If the ``amount_type`` is ``price`` and the price is less
             than the costmin.
         :raises ValueError: If the ``amount_type`` is ``volume`` and the volume is
             less than the ordermin.
         :raises ValueError: If no valid ``amount_type`` was passed.
         :return: A string representation of the amount.
         :rtype: str
+
+        .. code-block:: python
+            :linenos:
+            :caption: Spot Trade: Truncate
+
+            >>> print(trade.truncate(
+            ...     amount=0.123456789,
+            ...     amount_type="volume",
+            ...     pair="XBTUSD"
+            ... ))
+            0.12345678
+
+            >>> print(trade.truncate(
+            ...     amount=21123.12849829993,
+            ...     amount_type="price",
+            ...     pair="XBTUSD")
+            ... ))
+            21123.1
+
+            >>> print(trade.truncate(
+            ...     amount=0.1,
+            ...     amount_type="volume",
+            ...     pair="XBTUSD"
+            ... ))
+            0.10000000
+
+            >>> print(trade.truncate(
+            ...     amount=21123,
+            ...     amount_type="price",
+            ...     pair="XBTUSD"
+            ... ))
+            21123.0
         """
         if amount_type not in ("price", "volume"):
             raise ValueError("Amount type must be 'volume' or 'price'!")
 
         pair_data: dict = self.__market.get_asset_pairs(pair=pair)
         data: dict = pair_data[list(pair_data)[0]]
```

### Comparing `python-kraken-sdk-1.3.0/kraken/spot/user/__init__.py` & `python-kraken-sdk-1.4.0/kraken/spot/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # GitHub: https://github.com/btschwertfeger
 #
 
 """ Module that implements the Kraken Spot User client"""
 from decimal import Decimal
 from typing import List, Optional, Union
 
-from ...base_api import KrakenBaseSpotAPI, defined, ensure_string
+from ..base_api import KrakenBaseSpotAPI, defined, ensure_string
 
 
 class User(KrakenBaseSpotAPI):
     """
     Class that implements the Kraken Spot User client
 
     Requires the ``Query funds`` permission in the API key settings.
@@ -763,15 +763,15 @@
             params={"trades": trades, "id": id_},
         )
 
     @ensure_string("pair")
     def get_trade_volume(
         self: "User",
         pair: Optional[Union[str, List[str]]] = None,
-        fee_info: Optional[bool] = True,
+        fee_info: bool = True,
     ) -> dict:
         """
         Get the 30-day user specific trading volume in USD.
 
         Requires the ``Query funds`` permission in the API key settings.
 
         - https://docs.kraken.com/rest/#operation/getTradeVolume
```

### Comparing `python-kraken-sdk-1.3.0/pyproject.toml` & `python-kraken-sdk-1.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-kraken-sdk"
 dynamic = ["version"]
 authors = [
-  { name="Benjamin Thomas Schwertfeger", email="contact@b-schwertfeger.de" },
+  {name = "Benjamin Thomas Schwertfeger", email = "contact@b-schwertfeger.de"},
 ]
 description = "Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 dependencies = [
     "asyncio>=3.4",
@@ -77,23 +77,24 @@
 #
 [tool.pytest]
 junit_family = "xunit2"
 testpaths = ["tests"]
 
 [tool.pytest.ini_options]
 markers = [
-    "selection: Used to run a specific test by hand.",
+    "select: Used to run a specific test by hand.",
     "spot: mark a test that tests a Spot endpoint.",
     "spot_auth: mark a test that tests a authenticaed Spot endpoint.",
     "spot_trade: mark a test that tests a Spot Trade endpoint.",
     "spot_user: mark a test that tests a Spot User endpoint.",
     "spot_market: mark a test that tests a Spot Market endpoint.",
     "spot_funding: mark a test that tests a Spot Funding endpoint.",
     "spot_staking: mark a test that tests a Spot Staking endpoint.",
-    "spot_websocket: mark a test that tests a Spot Websocket endpoint.",
+    "spot_websocket: mark a test that tests the Spot Websocket client.",
+    "spot_orderbook: mark a test that tests the Spot Orderbook client.",
     "futures: mark a test that tests a Futures endpoint.",
     "futures_auth: mark a test that tests a authenticated Futures endpoint.",
     "futures_market: mark a test that tests a Futures Market endpoint.",
     "futures_user: mark a test that tests a Futures User endpoint.",
     "futures_trade: mark a test that tests a Futures Trade endpoint.",
     "futures_funding: mark a test that tests a Futures Funding endpoint.",
     "futures_websocket: mark a test that tests a Futures Websocket endpoint.",
```

### Comparing `python-kraken-sdk-1.3.0/python_kraken_sdk.egg-info/PKG-INFO` & `python-kraken-sdk-1.4.0/python_kraken_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kraken-sdk
-Version: 1.3.0
+Version: 1.4.0
 Summary: Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,15 @@
 
 ## Features
 
 Clients:
 
 - Spot REST Clients
 - Spot Websocket Client
+- Spot Orderbook Client
 - Futures REST Clients
 - Futures Websocket Client
 
 General:
 
 - access both public and private endpoints
 - responsive error handling and custom exceptions
@@ -756,15 +757,15 @@
 ```bash
 python3 -m pip install python-kraken-sdk
 ```
 
 ### 2. Register at Kraken and generate API Keys:
 
 - Spot Trading: https://www.kraken.com/u/security/api
-- Futures Trading: https://futures.kraken.com/trade/settings/api
+- Futures Trading: https://futures.kraken.com/trade/settings/api (see _[help](https://docs.futures.kraken.com/#introduction-generate-api-keys)_)
 - Futures Sandbox: https://demo-futures.kraken.com/settings/api
 
 ### 3. Start using the provided example scripts
 
 ### 4. Error handling
 
 If any unexpected behavior occurs, please check <b style="color: yellow">your API permissions</b>, <b style="color: yellow">rate limits</b>, update the python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error persists please open an issue.
@@ -845,15 +846,15 @@
 ... can be found in `/examples/spot_ws_examples.py`
 
 ```python
 import time
 import asyncio
 from kraken.spot import KrakenSpotWSClient
 
-async def main() -> None:
+async def main()
 
     key = "kraken-public-key"
     secret = "kraken-secret-key"
 
     class Bot(KrakenSpotWSClient):
         async def on_message(self, msg):
             if isinstance(msg, dict) and "event" in msg:
```

### Comparing `python-kraken-sdk-1.3.0/python_kraken_sdk.egg-info/SOURCES.txt` & `python-kraken-sdk-1.4.0/python_kraken_sdk.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 .github/codecov.yml
 .github/pull_request_template.md
+.github/release.yaml
 .github/self-review.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/_build.yaml
 .github/workflows/_build_doc.yaml
 .github/workflows/_codecov.yaml
 .github/workflows/_codeql.yaml
@@ -30,62 +31,63 @@
 .github/workflows/cicd.yaml
 .github/workflows/codeql.yaml
 .github/workflows/manual_build.yaml
 .github/workflows/manual_codeql.yaml
 .github/workflows/manual_pre_commit.yaml
 .github/workflows/manual_test_futures.yaml
 .github/workflows/manual_test_spot.yaml
-.github/workflows/release.yml
+.github/workflows/release.yaml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/links.rst
 docs/make.bat
 docs/requirements.txt
 docs/src/introduction.rst
 docs/src/issues.rst
 docs/src/about/license.rst
 docs/src/base_api/base_api.rst
 docs/src/examples/futures_bot_template.rst
 docs/src/examples/spot_bot_template.rst
 docs/src/examples/spot_orderbook.rst
 docs/src/examples/trading_bot_templates.rst
-docs/src/futures/futures_rest.rst
-docs/src/futures/futures_websocket.rst
+docs/src/futures/rest.rst
+docs/src/futures/websockets.rst
 docs/src/getting_started/getting_started.rst
 docs/src/krakenexceptions/krakenexceptions.rst
-docs/src/spot/spot_rest.rst
-docs/src/spot/spot_websocket.rst
+docs/src/spot/rest.rst
+docs/src/spot/websockets.rst
 examples/futures_examples.py
 examples/futures_trading_bot_template.py
 examples/futures_ws_examples.py
 examples/market_client_example.ipynb
 examples/spot_examples.py
 examples/spot_orderbook.py
 examples/spot_trading_bot_template.py
 examples/spot_ws_examples.py
 kraken/__init__.py
 kraken/_version.py
 kraken/base_api/__init__.py
 kraken/exceptions/__init__.py
 kraken/futures/__init__.py
-kraken/futures/funding/__init__.py
-kraken/futures/market/__init__.py
-kraken/futures/trade/__init__.py
-kraken/futures/user/__init__.py
+kraken/futures/funding.py
+kraken/futures/market.py
+kraken/futures/trade.py
+kraken/futures/user.py
+kraken/futures/ws_client.py
 kraken/futures/websocket/__init__.py
-kraken/futures/ws_client/__init__.py
 kraken/spot/__init__.py
-kraken/spot/funding/__init__.py
-kraken/spot/market/__init__.py
-kraken/spot/staking/__init__.py
-kraken/spot/trade/__init__.py
-kraken/spot/user/__init__.py
+kraken/spot/funding.py
+kraken/spot/market.py
+kraken/spot/orderbook.py
+kraken/spot/staking.py
+kraken/spot/trade.py
+kraken/spot/user.py
+kraken/spot/ws_client.py
 kraken/spot/websocket/__init__.py
-kraken/spot/ws_client/__init__.py
 python_kraken_sdk.egg-info/PKG-INFO
 python_kraken_sdk.egg-info/SOURCES.txt
 python_kraken_sdk.egg-info/dependency_links.txt
 python_kraken_sdk.egg-info/requires.txt
 python_kraken_sdk.egg-info/top_level.txt
 tests/__init__.py
 tests/futures/__init__.py
@@ -99,11 +101,13 @@
 tests/futures/test_futures_websocket.py
 tests/spot/__init__.py
 tests/spot/conftest.py
 tests/spot/helper.py
 tests/spot/test_spot_base_api.py
 tests/spot/test_spot_funding.py
 tests/spot/test_spot_market.py
+tests/spot/test_spot_orderbook.py
 tests/spot/test_spot_staking.py
 tests/spot/test_spot_trade.py
 tests/spot/test_spot_user.py
-tests/spot/test_spot_websocket.py
+tests/spot/test_spot_websocket.py
+tests/spot/fixture/orderbook.json
```

### Comparing `python-kraken-sdk-1.3.0/tests/futures/conftest.py` & `python-kraken-sdk-1.4.0/tests/futures/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,27 @@
 # GitHub: https://github.com/btschwertfeger
 #
 
 import os
 
 import pytest
 
-from kraken.futures import Funding, Market, Trade, User
+from kraken.futures import Funding, KrakenFuturesWSClient, Market, Trade, User
+
+
+@pytest.fixture
+def futures_api_key() -> str:
+    """Returns the Futures API key"""
+    return os.getenv("FUTURES_API_KEY")
+
+
+@pytest.fixture
+def futures_secret_key() -> str:
+    """Returns the Futures API secret key"""
+    return os.getenv("FUTURES_SECRET_KEY")
 
 
 @pytest.fixture
 def futures_market() -> Market:
     """
     Fixture providing an unauthenticated Futures Market client
     """
```

### Comparing `python-kraken-sdk-1.3.0/tests/futures/test_futures_base_api.py` & `python-kraken-sdk-1.4.0/tests/futures/test_futures_base_api.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/tests/futures/test_futures_funding.py` & `python-kraken-sdk-1.4.0/tests/futures/test_futures_funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/tests/futures/test_futures_market.py` & `python-kraken-sdk-1.4.0/tests/futures/test_futures_market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/tests/futures/test_futures_trade.py` & `python-kraken-sdk-1.4.0/tests/futures/test_futures_trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/tests/futures/test_futures_user.py` & `python-kraken-sdk-1.4.0/tests/futures/test_futures_user.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/tests/spot/conftest.py` & `python-kraken-sdk-1.4.0/tests/spot/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,26 @@
 
 import pytest
 
 from kraken.spot import Funding, Market, Staking, Trade, User
 
 
 @pytest.fixture
+def spot_api_key() -> str:
+    """Returns the Kraken Spot API Key for testing."""
+    return os.getenv("SPOT_API_KEY")
+
+
+@pytest.fixture
+def spot_secret_key() -> str:
+    """Returns the Kraken Spot API secret for testing."""
+    return os.getenv("SPOT_SECRET_KEY")
+
+
+@pytest.fixture
 def spot_auth_user() -> User:
     """
     Fixture providing an authenticated Spot user client.
     """
     return User(key=os.getenv("SPOT_API_KEY"), secret=os.getenv("SPOT_SECRET_KEY"))
```

### Comparing `python-kraken-sdk-1.3.0/tests/spot/test_spot_base_api.py` & `python-kraken-sdk-1.4.0/tests/spot/test_spot_base_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 """Module that checks the general Spot Base API class."""
 
 import pytest
 
 from kraken.base_api import KrakenBaseSpotAPI
 from kraken.exceptions import KrakenException
+from kraken.spot import Funding, Market, Staking, Trade, User
 
 from .helper import is_not_error
 
 
 @pytest.mark.spot
 def test_KrakenBaseSpotAPI_without_exception() -> None:
     """
@@ -34,24 +35,29 @@
         "error": ["EAPI:Invalid key"]
     }
 
 
 @pytest.mark.spot
 @pytest.mark.spot_auth
 def test_spot_rest_contextmanager(
-    spot_market, spot_auth_funding, spot_auth_trade, spot_auth_user, spot_auth_staking
+    spot_market: Market,
+    spot_auth_funding: Funding,
+    spot_auth_trade: Trade,
+    spot_auth_user: User,
+    spot_auth_staking: Staking,
 ) -> None:
     """
     Checks if the clients can be used as context manager.
     """
     with spot_market as market:
-        assert is_not_error(market.get_assets())
+        result = market.get_assets()
+        assert is_not_error(result), result
 
     with spot_auth_funding as funding:
-        isinstance(funding.get_deposit_methods(asset="XBT"), list)
+        assert isinstance(funding.get_deposit_methods(asset="XBT"), list)
 
     with spot_auth_user as user:
         assert is_not_error(user.get_account_balance())
 
     with spot_auth_staking as staking:
         assert isinstance(staking.get_pending_staking_transactions(), list)
```

### Comparing `python-kraken-sdk-1.3.0/tests/spot/test_spot_funding.py` & `python-kraken-sdk-1.4.0/tests/spot/test_spot_funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/tests/spot/test_spot_market.py` & `python-kraken-sdk-1.4.0/tests/spot/test_spot_market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/tests/spot/test_spot_staking.py` & `python-kraken-sdk-1.4.0/tests/spot/test_spot_staking.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.3.0/tests/spot/test_spot_trade.py` & `python-kraken-sdk-1.4.0/tests/spot/test_spot_trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,25 +162,27 @@
 @pytest.mark.spot_auth
 @pytest.mark.spot_trade
 def test_edit_order(spot_auth_trade: Trade) -> None:
     """
     Test the ``edit_order`` function by editing an order.
 
     KrakenException.KrakenPermissionDeniedError: since CI does not have
-    trade permissions.
+    trade permissions. If the request would be malformed, another
+    exception could be observed.
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
         spot_auth_trade.edit_order(
             txid="OHYO67-6LP66-HMQ437",
             userref="12345678",
             volume=1.25,
             pair="XBTUSD",
             price=27500,
             price2=26500,
             cancel_response=False,
+            truncate=True,
             oflags=["post"],
             validate=True,
         )
 
 
 @pytest.mark.spot
 @pytest.mark.spot_auth
```

### Comparing `python-kraken-sdk-1.3.0/tests/spot/test_spot_user.py` & `python-kraken-sdk-1.4.0/tests/spot/test_spot_user.py`

 * *Files identical despite different names*

