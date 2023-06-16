# Comparing `tmp/sphinx_argparse_cli-1.8.3.tar.gz` & `tmp/sphinx_argparse_cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_argparse_cli-1.8.3.tar", last modified: Tue Dec 28 23:27:10 2021, max compression
+gzip compressed data, was "sphinx_argparse_cli-1.9.0.tar", last modified: Fri Jun 24 17:55:50 2022, max compression
```

## Comparing `sphinx_argparse_cli-1.8.3.tar` & `sphinx_argparse_cli-1.9.0.tar`

### file list

```diff
@@ -1,109 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.011628 sphinx_argparse_cli-1.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.003628 sphinx_argparse_cli-1.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.003628 sphinx_argparse_cli-1.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6389 2021-12-28 23:27:10.011628 sphinx_argparse_cli-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4891 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.003628 sphinx_argparse_cli-1.8.3/roots/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.003628 sphinx_argparse_cli-1.8.3/roots/test-basic/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-basic/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-basic/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.003628 sphinx_argparse_cli-1.8.3/roots/test-complex/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-complex/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-complex/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-complex/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-group-title-empty-prefixes/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-empty-prefixes/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-empty-prefixes/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-empty-prefixes/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom-subcommands/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom-subcommands/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom-subcommands/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom-subcommands/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-default/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-default/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-default/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-default/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty-subcommands/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty-subcommands/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty-subcommands/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty-subcommands/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-prog-replacement/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-prog-replacement/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-prog-replacement/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-prog-replacement/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-subcommand-replacement/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-subcommand-replacement/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-subcommand-replacement/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-subcommand-replacement/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-lower-upper-refs/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-lower-upper-refs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-lower-upper-refs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-lower-upper-refs/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-prog/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-prog/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-prog/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-prog/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-ref/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-ref-duplicate-label/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref-duplicate-label/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref-duplicate-label/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref-duplicate-label/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref-duplicate-label/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-ref-prefix-doc/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref-prefix-doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref-prefix-doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-ref-prefix-doc/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-store-true-false/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-store-true-false/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-store-true-false/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-store-true-false/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.007628 sphinx_argparse_cli-1.8.3/roots/test-title-empty/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-title-empty/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-title-empty/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-title-empty/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.011628 sphinx_argparse_cli-1.8.3/roots/test-title-set/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-title-set/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-title-set/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/roots/test-title-set/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2021-12-28 23:27:10.011628 sphinx_argparse_cli-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.003628 sphinx_argparse_cli-1.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.011628 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13308 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli/_logic.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-12-28 23:27:09.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.011628 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6389 2021-12-28 23:27:09.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2955 2021-12-28 23:27:10.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 23:27:09.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-28 23:27:09.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-12-28 23:27:09.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 23:27:09.000000 sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:27:10.011628 sphinx_argparse_cli-1.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/tests/complex.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/tests/complex_pre_310.txt
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     9756 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/tests/test_logic.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/tests/test_sphinx_argparse_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/tox.ini
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-12-28 23:27:03.000000 sphinx_argparse_cli-1.8.3/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.187126 sphinx_argparse_cli-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7134 2022-06-24 17:55:50.187126 sphinx_argparse_cli-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5638 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-basic/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-basic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-basic/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-complex/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-complex/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-complex/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-complex/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-description-empty/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-description-empty/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-description-empty/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-description-empty/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-description-set/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-description-set/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-description-set/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-description-set/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-group-title-empty-prefixes/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-empty-prefixes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-empty-prefixes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-empty-prefixes/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom-subcommands/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom-subcommands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom-subcommands/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom-subcommands/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-default/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-default/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-default/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-default/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty-subcommands/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty-subcommands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty-subcommands/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty-subcommands/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-prog-replacement/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-prog-replacement/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-prog-replacement/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-prog-replacement/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-subcommand-replacement/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-subcommand-replacement/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-subcommand-replacement/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-subcommand-replacement/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-hook/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-hook/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-hook/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-hook/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-hook-fail/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-hook-fail/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-hook-fail/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-hook-fail/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-lower-upper-refs/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-lower-upper-refs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-lower-upper-refs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-lower-upper-refs/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-prog/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-prog/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-prog/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-prog/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-ref/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-ref-duplicate-label/
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref-duplicate-label/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref-duplicate-label/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref-duplicate-label/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref-duplicate-label/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-ref-prefix-doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref-prefix-doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref-prefix-doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-ref-prefix-doc/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-store-true-false/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-store-true-false/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-store-true-false/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-store-true-false/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-title-empty/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-title-empty/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-title-empty/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-title-empty/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/roots/test-title-set/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-title-set/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-title-set/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/roots/test-title-set/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-06-24 17:55:50.187126 sphinx_argparse_cli-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.179125 sphinx_argparse_cli-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14278 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli/_logic.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-24 17:55:49.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.183126 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7134 2022-06-24 17:55:49.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-06-24 17:55:50.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 17:55:49.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-24 17:55:49.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-24 17:55:50.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 17:55:48.000000 sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:55:50.187126 sphinx_argparse_cli-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/tests/complex.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/tests/complex_pre_310.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10503 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/tests/test_logic.py
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/tests/test_sphinx_argparse_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2022-06-24 17:55:40.000000 sphinx_argparse_cli-1.9.0/whitelist.txt
```

### Comparing `sphinx_argparse_cli-1.8.3/.github/workflows/check.yml` & `sphinx_argparse_cli-1.9.0/.github/workflows/check.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,22 @@
         py:
           - "3.10"
           - 3.9
           - 3.8
           - 3.7
     steps:
       - name: setup python for tox
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - name: install tox
         run: python -m pip install tox
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: setup python for test ${{ matrix.py }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.py }}
       - name: pick environment to run
         run: |
           import subprocess; import json; import os
           major, minor, impl = json.loads(subprocess.check_output(["python", "-c", "import json; import sys; import platform; print(json.dumps([sys.version_info[0], sys.version_info[1], platform.python_implementation()]));"], universal_newlines=True))
           with open(os.environ['GITHUB_ENV'], 'a') as file_handler:
@@ -56,17 +56,17 @@
       fail-fast: false
       matrix:
         tox_env:
           - type
           - dev
           - pkg_check
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: setup Python 3.10
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - name: install tox
         run: python -m pip install tox
       - name: run check for ${{ matrix.tox_env }}
         run: python -m tox -e ${{ matrix.tox_env }}
         env:
@@ -74,20 +74,20 @@
 
   publish:
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     needs: [check, test]
     runs-on: ubuntu-20.04
     steps:
       - name: setup python to build package
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - name: install build
         run: python -m pip install build
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: build package
         run: python -m build --sdist --wheel . -o dist
       - name: publish to PyPI
         uses: pypa/gh-action-pypi-publish@master
         with:
           skip_existing: true
           user: __token__
```

### Comparing `sphinx_argparse_cli-1.8.3/.pre-commit-config.yaml` & `sphinx_argparse_cli-1.9.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.3.0
     hooks:
       - id: check-ast
       - id: check-builtin-literals
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: check-yaml
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.30.0
+    rev: v2.34.0
     hooks:
       - id: pyupgrade
         args: [ "--py36-plus" ]
   - repo: https://github.com/PyCQA/isort
     rev: 5.10.1
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 21.12b0
+    rev: 22.3.0
     hooks:
       - id: black
         args: [ --safe ]
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.0
+    rev: v1.12.1
     hooks:
       - id: blacken-docs
-        additional_dependencies: [ black==21.12b0 ]
+        additional_dependencies: [ black==22.1 ]
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.9.0
     hooks:
       - id: rst-backticks
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: "0.5.1"
+    rev: "0.5.2"
     hooks:
       - id: tox-ini-fmt
         args: [ "-p", "fix" ]
   - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.20.0
+    rev: v1.20.1
     hooks:
       - id: setup-cfg-fmt
         args: [ --min-py3-version, "3.7", "--max-py-version", "3.10" ]
   - repo: https://github.com/PyCQA/flake8
     rev: 4.0.1
     hooks:
       - id: flake8
         additional_dependencies:
-          - flake8-bugbear==21.11.29
-          - flake8-comprehensions==3.7
+          - flake8-bugbear==22.1.11
+          - flake8-comprehensions==3.8
           - flake8-pytest-style==1.6
           - flake8-spellcheck==0.24
           - flake8-unused-arguments==0.0.9
           - flake8-noqa==1.2.1
           - pep8-naming==0.12.1
```

### Comparing `sphinx_argparse_cli-1.8.3/CHANGELOG.md` & `sphinx_argparse_cli-1.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## 1.9.0
+
+- Add the option to override the description using the `description` attribute of the directive
+- Add the option to retrieve the arguments by hooking argparse, in cases where `func` consumes the arguments
+  and does not return them
+
 ## 1.8.2
 
 - Don't raise label clashing warnings for options which only differ between upper and lower case
 
 ## 1.8.1
 
 - Fix reference clashing for options which only differ between upper and lower case
```

### Comparing `sphinx_argparse_cli-1.8.3/CODE_OF_CONDUCT.md` & `sphinx_argparse_cli-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/LICENSE.txt` & `sphinx_argparse_cli-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/PKG-INFO` & `sphinx_argparse_cli-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_argparse_cli
-Version: 1.8.3
+Version: 1.9.0
 Summary: render CLI arguments (sub-commands friendly) defined by argparse module
 Home-page: https://github.com/tox-dev/sphinx-argparse-cli
 Author: Bernat Gabor
 Author-email: gaborjbernat@gmail.com
 Maintainer: Bernat Gabor
 Maintainer-email: gaborjbernat@gmail.com
 License: MIT
@@ -65,29 +65,41 @@
 
 Within the reStructuredText files use the `sphinx_argparse_cli` directive that takes, at least, two arguments:
 
 | Name                   | Description                                                                                                                                                                      |
 | ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | module                 | the module path to where the parser is defined                                                                                                                                   |
 | func                   | the name of the function that once called with no arguments constructs the parser                                                                                                |
-| prog                   | (optional) the module path to where the parser is defined                                                                                                                        |
+| prog                   | (optional) when provided, overwrites the `<prog>` name.                                                                                                                          |                                                                                                                     |
+| hook                   | (optional) hook `argparse` to retrieve the parser if `func` uses a parser instead of returning it.                                                                               |
 | title                  | (optional) when provided, overwrites the `<prog> - CLI interface` title added by default and when empty, will not be included                                                    |
+| description            | (optional) when provided, overwrites the description and when empty, will not be included                                                                                        |
 | usage_width            | (optional) how large should usage examples be - defaults to 100 character                                                                                                        |
 | group_title_prefix     | (optional) groups subsections title prefixes, accepts the string `{prog}` as a replacement for the program name - defaults to `{prog}`                                           |
 | group_sub_title_prefix | (optional) subcommands groups subsections title prefixes, accepts replacement of `{prog}` and `{subcommand}` for program and subcommand name - defaults to `{prog} {subcommand}` |
 
 For example:
 
 ```rst
 .. sphinx_argparse_cli::
   :module: a_project.cli
   :func: build_parser
   :prog: my-cli-program
 ```
 
+If you have code that creates and uses a parser but does not return it, you can specify the `:hook:` flag:
+
+```rst
+.. sphinx_argparse_cli::
+  :module: a_project.cli
+  :func: main
+  :hook:
+  :prog: my-cli-program
+```
+
 ### Refer to generated content
 
 The tool will register reference links to all anchors. This means that you can use the sphinx `ref` role to refer to
 both the (sub)command title/groups and every flag/argument. The tool offers a configuration flag
 `sphinx_argparse_cli_prefix_document` (change by setting this variable in `conf.py` - by default `False`). This option
 influences the reference ids generated. If it's false the reference will be the anchor id (the text appearing after the
 `'#` in the URI once you click on it). If it's true the anchor id will be prefixed by the document name (this is useful
@@ -101,9 +113,7 @@
 
 For example in case of a `tox` command, and `sphinx_argparse_cli_prefix_document=True`, and the current document name
 being `cli`:
 
 - to refer to the optional arguments group use `` :ref:`cli:tox-optional-arguments`  ``,
 - to refer to the run subcommand use `` :ref:`cli:tox-run`  ``,
 - to refer to flag `--magic` of the `run` sub-command use `` :ref:`cli:tox-run---magic`  ``.
-
-
```

### Comparing `sphinx_argparse_cli-1.8.3/README.md` & `sphinx_argparse_cli-1.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -29,29 +29,41 @@
 
 Within the reStructuredText files use the `sphinx_argparse_cli` directive that takes, at least, two arguments:
 
 | Name                   | Description                                                                                                                                                                      |
 | ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | module                 | the module path to where the parser is defined                                                                                                                                   |
 | func                   | the name of the function that once called with no arguments constructs the parser                                                                                                |
-| prog                   | (optional) the module path to where the parser is defined                                                                                                                        |
+| prog                   | (optional) when provided, overwrites the `<prog>` name.                                                                                                                          |                                                                                                                     |
+| hook                   | (optional) hook `argparse` to retrieve the parser if `func` uses a parser instead of returning it.                                                                               |
 | title                  | (optional) when provided, overwrites the `<prog> - CLI interface` title added by default and when empty, will not be included                                                    |
+| description            | (optional) when provided, overwrites the description and when empty, will not be included                                                                                        |
 | usage_width            | (optional) how large should usage examples be - defaults to 100 character                                                                                                        |
 | group_title_prefix     | (optional) groups subsections title prefixes, accepts the string `{prog}` as a replacement for the program name - defaults to `{prog}`                                           |
 | group_sub_title_prefix | (optional) subcommands groups subsections title prefixes, accepts replacement of `{prog}` and `{subcommand}` for program and subcommand name - defaults to `{prog} {subcommand}` |
 
 For example:
 
 ```rst
 .. sphinx_argparse_cli::
   :module: a_project.cli
   :func: build_parser
   :prog: my-cli-program
 ```
 
+If you have code that creates and uses a parser but does not return it, you can specify the `:hook:` flag:
+
+```rst
+.. sphinx_argparse_cli::
+  :module: a_project.cli
+  :func: main
+  :hook:
+  :prog: my-cli-program
+```
+
 ### Refer to generated content
 
 The tool will register reference links to all anchors. This means that you can use the sphinx `ref` role to refer to
 both the (sub)command title/groups and every flag/argument. The tool offers a configuration flag
 `sphinx_argparse_cli_prefix_document` (change by setting this variable in `conf.py` - by default `False`). This option
 influences the reference ids generated. If it's false the reference will be the anchor id (the text appearing after the
 `'#` in the URI once you click on it). If it's true the anchor id will be prefixed by the document name (this is useful
```

### Comparing `sphinx_argparse_cli-1.8.3/pyproject.toml` & `sphinx_argparse_cli-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/roots/test-complex/parser.py` & `sphinx_argparse_cli-1.9.0/roots/test-complex/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/roots/test-group-title-empty-prefixes/parser.py` & `sphinx_argparse_cli-1.9.0/roots/test-group-title-empty-prefixes/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom/parser.py` & `sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-custom-subcommands/parser.py` & `sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-custom-subcommands/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-empty-subcommands/parser.py` & `sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-empty-subcommands/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-prog-replacement/parser.py` & `sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-prog-replacement/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/roots/test-group-title-prefix-subcommand-replacement/parser.py` & `sphinx_argparse_cli-1.9.0/roots/test-group-title-prefix-subcommand-replacement/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/setup.cfg` & `sphinx_argparse_cli-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli/_logic.py` & `sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli/_logic.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     HelpFormatter,
     _ArgumentGroup,
     _StoreFalseAction,
     _StoreTrueAction,
     _SubParsersAction,
 )
 from collections import defaultdict, namedtuple
-from typing import Iterator, cast
+from typing import Any, Iterator, cast
 
 from docutils.nodes import (
     Element,
     Node,
     Text,
     bullet_list,
     fully_normalize_name,
@@ -28,15 +28,16 @@
     paragraph,
     reference,
     section,
     strong,
     title,
     whitespace_normalize_name,
 )
-from docutils.parsers.rst.directives import (  # type: ignore # no stubs
+from docutils.parsers.rst.directives import (
+    flag,
     positive_int,
     unchanged,
     unchanged_required,
 )
 from docutils.parsers.rst.states import RSTState, RSTStateMachine
 from docutils.statemachine import StringList
 from sphinx.domains.std import StandardDomain
@@ -56,16 +57,18 @@
 
 class SphinxArgparseCli(SphinxDirective):
     name = "sphinx_argparse_cli"
     has_content = False
     option_spec = {
         "module": unchanged_required,
         "func": unchanged_required,
+        "hook": flag,
         "prog": unchanged,
         "title": unchanged,
+        "description": unchanged,
         "usage_width": positive_int,
         "group_title_prefix": unchanged,
         "group_sub_title_prefix": unchanged,
     }
 
     def __init__(
         self,
@@ -86,18 +89,32 @@
         self._std_domain: StandardDomain = cast(StandardDomain, self.env.get_domain("std"))
 
     @property
     def parser(self) -> ArgumentParser:
         if self._parser is None:
             module_name, attr_name = self.options["module"], self.options["func"]
             parser_creator = getattr(__import__(module_name, fromlist=[attr_name]), attr_name)
-            self._parser = parser_creator()
+            if "hook" in self.options:
+                original_parse_known_args = ArgumentParser.parse_known_args
+                ArgumentParser.parse_known_args = _argparse_parse_known_args_hook  # type: ignore
+                try:
+                    parser_creator()
+                except HookError as hooked:
+                    self._parser = hooked.parser
+                finally:
+                    ArgumentParser.parse_known_args = original_parse_known_args  # type: ignore
+            else:
+                self._parser = parser_creator()
+
+            del sys.modules[module_name]  # no longer needed cleanup
+            if self._parser is None:
+                raise self.error("Failed to hook argparse to get ArgumentParser")
+
             if "prog" in self.options:
                 self._parser.prog = self.options["prog"]
-            del sys.modules[module_name]  # no longer needed cleanup
         return self._parser
 
     def load_sub_parsers(self) -> Iterator[tuple[list[str], str, ArgumentParser]]:
         top_sub_parser = self.parser._subparsers
         if not top_sub_parser:
             return
         parser_to_args: dict[int, list[str]] = defaultdict(list)
@@ -123,16 +140,17 @@
         self.env.note_reread()  # this document needs to be always updated
         title_text = self.options.get("title", f"{self.parser.prog} - CLI interface").strip()
         if title_text.strip() == "":
             home_section: Element = paragraph()
         else:
             home_section = section("", title("", Text(title_text)), ids=[make_id(title_text)], names=[title_text])
 
-        if self.parser.description:
-            desc_paragraph = paragraph("", Text(self.parser.description))
+        description = self.options.get("description", self.parser.description)
+        if description:
+            desc_paragraph = paragraph("", Text(description))
             home_section += desc_paragraph
         # construct groups excluding sub-parsers
         home_section += self._mk_usage(self.parser)
         for group in self.parser._action_groups:
             if not group._group_actions or group is self.parser._subparsers:
                 continue
             home_section += self._mk_option_group(group, prefix=self.parser.prog.split("/")[-1])
@@ -319,8 +337,17 @@
 def load_help_text(help_text: str) -> str:
     single_quote = SINGLE_QUOTE.sub("``'\\1'``", help_text)
     double_quote = DOUBLE_QUOTE.sub('``"\\1"``', single_quote)
     literal_curly_braces = CURLY_BRACES.sub("``{\\1}``", double_quote)
     return literal_curly_braces
 
 
+class HookError(Exception):
+    def __init__(self, parser: ArgumentParser):
+        self.parser = parser
+
+
+def _argparse_parse_known_args_hook(self: ArgumentParser, *args: Any, **kwargs: Any) -> None:  # noqa: U100
+    raise HookError(self)
+
+
 __all__ = ("SphinxArgparseCli",)
```

### Comparing `sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/PKG-INFO` & `sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-argparse-cli
-Version: 1.8.3
+Version: 1.9.0
 Summary: render CLI arguments (sub-commands friendly) defined by argparse module
 Home-page: https://github.com/tox-dev/sphinx-argparse-cli
 Author: Bernat Gabor
 Author-email: gaborjbernat@gmail.com
 Maintainer: Bernat Gabor
 Maintainer-email: gaborjbernat@gmail.com
 License: MIT
@@ -65,29 +65,41 @@
 
 Within the reStructuredText files use the `sphinx_argparse_cli` directive that takes, at least, two arguments:
 
 | Name                   | Description                                                                                                                                                                      |
 | ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | module                 | the module path to where the parser is defined                                                                                                                                   |
 | func                   | the name of the function that once called with no arguments constructs the parser                                                                                                |
-| prog                   | (optional) the module path to where the parser is defined                                                                                                                        |
+| prog                   | (optional) when provided, overwrites the `<prog>` name.                                                                                                                          |                                                                                                                     |
+| hook                   | (optional) hook `argparse` to retrieve the parser if `func` uses a parser instead of returning it.                                                                               |
 | title                  | (optional) when provided, overwrites the `<prog> - CLI interface` title added by default and when empty, will not be included                                                    |
+| description            | (optional) when provided, overwrites the description and when empty, will not be included                                                                                        |
 | usage_width            | (optional) how large should usage examples be - defaults to 100 character                                                                                                        |
 | group_title_prefix     | (optional) groups subsections title prefixes, accepts the string `{prog}` as a replacement for the program name - defaults to `{prog}`                                           |
 | group_sub_title_prefix | (optional) subcommands groups subsections title prefixes, accepts replacement of `{prog}` and `{subcommand}` for program and subcommand name - defaults to `{prog} {subcommand}` |
 
 For example:
 
 ```rst
 .. sphinx_argparse_cli::
   :module: a_project.cli
   :func: build_parser
   :prog: my-cli-program
 ```
 
+If you have code that creates and uses a parser but does not return it, you can specify the `:hook:` flag:
+
+```rst
+.. sphinx_argparse_cli::
+  :module: a_project.cli
+  :func: main
+  :hook:
+  :prog: my-cli-program
+```
+
 ### Refer to generated content
 
 The tool will register reference links to all anchors. This means that you can use the sphinx `ref` role to refer to
 both the (sub)command title/groups and every flag/argument. The tool offers a configuration flag
 `sphinx_argparse_cli_prefix_document` (change by setting this variable in `conf.py` - by default `False`). This option
 influences the reference ids generated. If it's false the reference will be the anchor id (the text appearing after the
 `'#` in the URI once you click on it). If it's true the anchor id will be prefixed by the document name (this is useful
@@ -101,9 +113,7 @@
 
 For example in case of a `tox` command, and `sphinx_argparse_cli_prefix_document=True`, and the current document name
 being `cli`:
 
 - to refer to the optional arguments group use `` :ref:`cli:tox-optional-arguments`  ``,
 - to refer to the run subcommand use `` :ref:`cli:tox-run`  ``,
 - to refer to flag `--magic` of the `run` sub-command use `` :ref:`cli:tox-run---magic`  ``.
-
-
```

### Comparing `sphinx_argparse_cli-1.8.3/src/sphinx_argparse_cli.egg-info/SOURCES.txt` & `sphinx_argparse_cli-1.9.0/src/sphinx_argparse_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,28 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 whitelist.txt
+.github/dependabot.yml
 .github/workflows/check.yml
 roots/test-basic/conf.py
 roots/test-basic/index.rst
 roots/test-basic/parser.py
 roots/test-complex/conf.py
 roots/test-complex/index.rst
 roots/test-complex/parser.py
+roots/test-description-empty/conf.py
+roots/test-description-empty/index.rst
+roots/test-description-empty/parser.py
+roots/test-description-set/conf.py
+roots/test-description-set/index.rst
+roots/test-description-set/parser.py
 roots/test-group-title-empty-prefixes/conf.py
 roots/test-group-title-empty-prefixes/index.rst
 roots/test-group-title-empty-prefixes/parser.py
 roots/test-group-title-prefix-custom/conf.py
 roots/test-group-title-prefix-custom/index.rst
 roots/test-group-title-prefix-custom/parser.py
 roots/test-group-title-prefix-custom-subcommands/conf.py
@@ -36,14 +43,20 @@
 roots/test-group-title-prefix-empty-subcommands/parser.py
 roots/test-group-title-prefix-prog-replacement/conf.py
 roots/test-group-title-prefix-prog-replacement/index.rst
 roots/test-group-title-prefix-prog-replacement/parser.py
 roots/test-group-title-prefix-subcommand-replacement/conf.py
 roots/test-group-title-prefix-subcommand-replacement/index.rst
 roots/test-group-title-prefix-subcommand-replacement/parser.py
+roots/test-hook/conf.py
+roots/test-hook/index.rst
+roots/test-hook/parser.py
+roots/test-hook-fail/conf.py
+roots/test-hook-fail/index.rst
+roots/test-hook-fail/parser.py
 roots/test-lower-upper-refs/conf.py
 roots/test-lower-upper-refs/index.rst
 roots/test-lower-upper-refs/parser.py
 roots/test-prog/conf.py
 roots/test-prog/index.rst
 roots/test-prog/parser.py
 roots/test-ref/conf.py
```

### Comparing `sphinx_argparse_cli-1.8.3/tests/complex.txt` & `sphinx_argparse_cli-1.9.0/tests/complex.txt`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/tests/complex_pre_310.txt` & `sphinx_argparse_cli-1.9.0/tests/complex_pre_310.txt`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/tests/conftest.py` & `sphinx_argparse_cli-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_argparse_cli-1.8.3/tests/test_logic.py` & `sphinx_argparse_cli-1.9.0/tests/test_logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,27 @@
 
 
 @pytest.mark.sphinx(buildername="html", testroot="complex")
 def test_complex_as_html(build_outcome: str) -> None:
     assert build_outcome
 
 
+@pytest.mark.sphinx(buildername="html", testroot="hook")
+def test_hook(build_outcome: str) -> None:
+    assert build_outcome
+
+
+@pytest.mark.sphinx(buildername="text", testroot="hook-fail")
+def test_hook_fail(app: SphinxTestApp, warning: StringIO) -> None:
+    app.build()
+    text = (Path(app.outdir) / "index.txt").read_text()
+    assert "Failed to hook argparse to get ArgumentParser" in warning.getvalue()
+    assert text == ""
+
+
 @pytest.mark.sphinx(buildername="text", testroot="prog")
 def test_prog_as_text(build_outcome: str) -> None:
     assert build_outcome == "magic - CLI interface\n*********************\n\n   magic\n"
 
 
 @pytest.mark.sphinx(buildername="text", testroot="title-set")
 def test_set_title_as_text(build_outcome: str) -> None:
@@ -69,14 +82,24 @@
 
 
 @pytest.mark.sphinx(buildername="text", testroot="title-empty")
 def test_empty_title_as_text(build_outcome: str) -> None:
     assert build_outcome == "   foo\n"
 
 
+@pytest.mark.sphinx(buildername="text", testroot="description-set")
+def test_set_description_as_text(build_outcome: str) -> None:
+    assert build_outcome == "foo - CLI interface\n*******************\n\nMy own description\n\n   foo\n"
+
+
+@pytest.mark.sphinx(buildername="text", testroot="description-empty")
+def test_empty_description_as_text(build_outcome: str) -> None:
+    assert build_outcome == "foo - CLI interface\n*******************\n\n   foo\n"
+
+
 @pytest.mark.sphinx(buildername="text", testroot="complex")
 @pytest.mark.prepare(directive_args=[":usage_width: 100"])
 def test_usage_width_default(build_outcome: str) -> None:
     assert "complex second [-h] [--flag] [--root] one pos_two\n" in build_outcome
 
 
 @pytest.mark.sphinx(buildername="text", testroot="complex")
@@ -120,22 +143,18 @@
         '<p>Flag <a class="reference internal" href="#prog---root"><span class="std std-ref">prog --root</span></a> and'
         ' positional <a class="reference internal" href="#prog-root"><span class="std std-ref">prog root</span></a>.'
         "</p>"
     )
     assert ref in build_outcome
 
 
-_REF_WARNING_STRING_IO = StringIO()  # could not find any better way to get the warning
-
-
-@pytest.mark.sphinx(buildername="text", testroot="ref-duplicate-label", warning=_REF_WARNING_STRING_IO)
-def test_ref_duplicate_label(build_outcome: tuple[str, str]) -> None:
+@pytest.mark.sphinx(buildername="text", testroot="ref-duplicate-label")
+def test_ref_duplicate_label(build_outcome: tuple[str, str], warning: StringIO) -> None:
     assert build_outcome
-    warnings = _REF_WARNING_STRING_IO.getvalue()
-    assert "duplicate label prog---help" in warnings
+    assert "duplicate label prog---help" in warning.getvalue()
 
 
 @pytest.mark.sphinx(buildername="html", testroot="group-title-prefix-default")
 def test_group_title_prefix_default(build_outcome: str) -> None:
     assert '<h2>prog positional arguments<a class="headerlink" href="#prog-positional-arguments"' in build_outcome
```

### Comparing `sphinx_argparse_cli-1.8.3/tox.ini` & `sphinx_argparse_cli-1.9.0/tox.ini`

 * *Files identical despite different names*

