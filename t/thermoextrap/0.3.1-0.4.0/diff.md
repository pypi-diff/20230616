# Comparing `tmp/thermoextrap-0.3.1.tar.gz` & `tmp/thermoextrap-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermoextrap-0.3.1.tar", last modified: Thu May  4 19:38:10 2023, max compression
+gzip compressed data, was "thermoextrap-0.4.0.tar", last modified: Fri Jun 16 01:04:15 2023, max compression
```

## Comparing `thermoextrap-0.3.1.tar` & `thermoextrap-0.4.0.tar`

### file list

```diff
@@ -1,107 +1,102 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.874773 thermoextrap-0.3.1/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1491 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.editorconfig
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1324 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      104 2023-04-11 02:16:02.000000 thermoextrap-0.3.1/.gitmodules
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3681 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      371 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      163 2023-04-24 16:24:54.000000 thermoextrap-0.3.1/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1386 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9712 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-10 21:01:10.000000 thermoextrap-0.3.1/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      285 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11351 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9470 2023-05-04 19:38:10.873805 thermoextrap-0.3.1/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5362 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.769447 thermoextrap-0.3.1/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.770453 thermoextrap-0.3.1/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.772243 thermoextrap-0.3.1/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.799553 thermoextrap-0.3.1/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       11 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/environment/conda-spec.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      985 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      423 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      638 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      584 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      337 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       36 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      328 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      369 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6622 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.805756 thermoextrap-0.3.1/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      843 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/lint.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-05-04 19:38:10.874984 thermoextrap-0.3.1/setup.cfg
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.756856 thermoextrap-0.3.1/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.815184 thermoextrap-0.3.1/src/thermoextrap/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1583 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18791 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/adaptive_interp.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    17295 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/beta.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.842126 thermoextrap-0.3.1/src/thermoextrap/core/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/core/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4998 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/core/_attrs_utils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12082 2023-04-11 02:16:02.000000 thermoextrap-0.3.1/src/thermoextrap/core/_deprecate.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      322 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/core/sputils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3159 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/core/xrutils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    52780 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/data.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3513 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/docstrings.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.846590 thermoextrap-0.3.1/src/thermoextrap/gpr_active/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      717 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    89013 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/active_utils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    56361 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/gp_models.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3377 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/ig_active.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3003 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/sine_active.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10310 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/idealgas.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.857939 thermoextrap-0.3.1/src/thermoextrap/legacy/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      629 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9563 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/extrap.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18311 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/gpr.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16775 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/gpr_stack.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5547 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/ig.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16626 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/interp.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9580 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/old_scripts.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21063 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/recursive_interp.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8609 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/reweight.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10983 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/utilities.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12877 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/lnpi.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32051 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/models.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21933 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/recursive_interp.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18752 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/stack.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5827 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/volume.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4387 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/volume_idealgas.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.837724 thermoextrap-0.3.1/src/thermoextrap.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9470 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2488 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      360 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       13 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:38:09.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.869899 thermoextrap-0.3.1/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9072 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/tests/conftest.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.870737 thermoextrap-0.3.1/tests/lnpi_data/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   794879 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/tests/lnpi_data/sample_data.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23103 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_GPs.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    25332 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_active.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32495 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_beta.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2259 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_data.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1421 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_idealgas.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3437 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_lnPi.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2094 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/tests/test_stack.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7641 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_u_data.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2046 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/tests/test_u_equations.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2703 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_volume.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4154 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.248064 thermoextrap-0.4.0/
+-rw-r--r--   0 wpk      (42033)    36681     1489 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-03 20:14:50.000000 thermoextrap-0.4.0/.editorconfig
+-rw-r--r--   0 wpk      (42033)    36681     1367 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      104 2023-04-11 02:16:02.000000 thermoextrap-0.4.0/.gitmodules
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-05-03 20:14:50.000000 thermoextrap-0.4.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3683 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-05-03 20:14:50.000000 thermoextrap-0.4.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      371 2023-06-15 17:34:49.000000 thermoextrap-0.4.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033)    36681      163 2023-06-15 17:34:54.000000 thermoextrap-0.4.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681     1669 2023-06-16 01:01:08.000000 thermoextrap-0.4.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9838 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-10 21:01:10.000000 thermoextrap-0.4.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      285 2023-06-15 17:41:07.000000 thermoextrap-0.4.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681     9389 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681    10058 2023-06-16 01:04:15.247589 thermoextrap-0.4.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     5371 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.213311 thermoextrap-0.4.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-05-03 20:14:50.000000 thermoextrap-0.4.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.213932 thermoextrap-0.4.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.215132 thermoextrap-0.4.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-05-03 20:14:50.000000 thermoextrap-0.4.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-05-03 20:14:50.000000 thermoextrap-0.4.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-05-03 20:14:50.000000 thermoextrap-0.4.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.218407 thermoextrap-0.4.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      336 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/base.yaml
+-rw-r--r--   0 wpk      (42033)    36681      658 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681      225 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      648 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/docs.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.219805 thermoextrap-0.4.0/environment/lock/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/lock/py310.yaml
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/lock/py311.yaml
+-rw-r--r--   0 wpk      (42033)    36681       63 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/lock/py38.yaml
+-rw-r--r--   0 wpk      (42033)    36681       63 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/lock/py39.yaml
+-rw-r--r--   0 wpk      (42033)    36681      261 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/test-extras.txt
+-rw-r--r--   0 wpk      (42033)    36681      382 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      513 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      522 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/environment/typing.yaml
+-rw-r--r--   0 wpk      (42033)    36681    29653 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/noxfile.py
+-rw-r--r--   0 wpk      (42033)    36681     8115 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/pyproject.toml
+-rw-r--r--   0 wpk      (42033)    36681       38 2023-06-16 01:04:15.248176 thermoextrap-0.4.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.203909 thermoextrap-0.4.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.224749 thermoextrap-0.4.0/src/thermoextrap/
+-rw-r--r--   0 wpk      (42033)    36681     1583 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    18791 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/adaptive_interp.py
+-rw-r--r--   0 wpk      (42033)    36681    17295 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/beta.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.228971 thermoextrap-0.4.0/src/thermoextrap/core/
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/core/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     4998 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/core/_attrs_utils.py
+-rw-r--r--   0 wpk      (42033)    36681    12082 2023-04-11 02:16:02.000000 thermoextrap-0.4.0/src/thermoextrap/core/_deprecate.py
+-rw-r--r--   0 wpk      (42033)    36681      322 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/core/sputils.py
+-rw-r--r--   0 wpk      (42033)    36681     3159 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/core/xrutils.py
+-rw-r--r--   0 wpk      (42033)    36681    52780 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/data.py
+-rw-r--r--   0 wpk      (42033)    36681     3513 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/docstrings.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.231562 thermoextrap-0.4.0/src/thermoextrap/gpr_active/
+-rw-r--r--   0 wpk      (42033)    36681      717 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/gpr_active/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    89018 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/src/thermoextrap/gpr_active/active_utils.py
+-rw-r--r--   0 wpk      (42033)    36681    56361 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/gpr_active/gp_models.py
+-rw-r--r--   0 wpk      (42033)    36681     3377 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/gpr_active/ig_active.py
+-rw-r--r--   0 wpk      (42033)    36681     3003 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/gpr_active/sine_active.py
+-rw-r--r--   0 wpk      (42033)    36681    10310 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/idealgas.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.237179 thermoextrap-0.4.0/src/thermoextrap/legacy/
+-rw-r--r--   0 wpk      (42033)    36681      629 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     9563 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/extrap.py
+-rw-r--r--   0 wpk      (42033)    36681    18311 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/gpr.py
+-rw-r--r--   0 wpk      (42033)    36681    16775 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/gpr_stack.py
+-rw-r--r--   0 wpk      (42033)    36681     5547 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/ig.py
+-rw-r--r--   0 wpk      (42033)    36681    16626 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/interp.py
+-rw-r--r--   0 wpk      (42033)    36681     9585 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/old_scripts.py
+-rw-r--r--   0 wpk      (42033)    36681    21063 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/recursive_interp.py
+-rw-r--r--   0 wpk      (42033)    36681     8649 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/reweight.py
+-rw-r--r--   0 wpk      (42033)    36681    10983 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/src/thermoextrap/legacy/utilities.py
+-rw-r--r--   0 wpk      (42033)    36681    12877 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/lnpi.py
+-rw-r--r--   0 wpk      (42033)    36681    32056 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/src/thermoextrap/models.py
+-rw-r--r--   0 wpk      (42033)    36681    21933 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/recursive_interp.py
+-rw-r--r--   0 wpk      (42033)    36681    18752 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/stack.py
+-rw-r--r--   0 wpk      (42033)    36681     5827 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/volume.py
+-rw-r--r--   0 wpk      (42033)    36681     4387 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/src/thermoextrap/volume_idealgas.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.227125 thermoextrap-0.4.0/src/thermoextrap.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681    10058 2023-06-16 01:04:14.000000 thermoextrap-0.4.0/src/thermoextrap.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2338 2023-06-16 01:04:15.000000 thermoextrap-0.4.0/src/thermoextrap.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-06-16 01:04:14.000000 thermoextrap-0.4.0/src/thermoextrap.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681     1158 2023-06-16 01:04:14.000000 thermoextrap-0.4.0/src/thermoextrap.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       13 2023-06-16 01:04:14.000000 thermoextrap-0.4.0/src/thermoextrap.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-04 19:38:09.000000 thermoextrap-0.4.0/src/thermoextrap.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.245014 thermoextrap-0.4.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681     9072 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/tests/conftest.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.245439 thermoextrap-0.4.0/tests/lnpi_data/
+-rw-r--r--   0 wpk      (42033)    36681   794879 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/tests/lnpi_data/sample_data.json
+-rw-r--r--   0 wpk      (42033)    36681    23103 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/tests/test_GPs.py
+-rw-r--r--   0 wpk      (42033)    36681    25332 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/tests/test_active.py
+-rw-r--r--   0 wpk      (42033)    36681    32495 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/tests/test_beta.py
+-rw-r--r--   0 wpk      (42033)    36681     2259 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/tests/test_data.py
+-rw-r--r--   0 wpk      (42033)    36681     1421 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/tests/test_idealgas.py
+-rw-r--r--   0 wpk      (42033)    36681     3437 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/tests/test_lnPi.py
+-rw-r--r--   0 wpk      (42033)    36681     2094 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/tests/test_stack.py
+-rw-r--r--   0 wpk      (42033)    36681     7641 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/tests/test_u_data.py
+-rw-r--r--   0 wpk      (42033)    36681     2046 2023-05-03 20:14:51.000000 thermoextrap-0.4.0/tests/test_u_equations.py
+-rw-r--r--   0 wpk      (42033)    36681     2703 2023-04-10 21:01:11.000000 thermoextrap-0.4.0/tests/test_volume.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-16 01:04:15.246892 thermoextrap-0.4.0/tools/
+-rw-r--r--   0 wpk      (42033)    36681    21120 2023-06-16 01:00:54.000000 thermoextrap-0.4.0/tools/noxtools.py
```

### Comparing `thermoextrap-0.3.1/.cruft.json` & `thermoextrap-0.4.0/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8322368421052632%*

 * *Differences: {"'checkout'": "'feature/nox'",*

 * * "'commit'": "'49d100c749e6cfa2cba3460ed06e4a06be07cc63'",*

 * * "'context'": "{'cookiecutter': {'conda_channel': 'conda-forge'}}"}*

```diff
@@ -1,25 +1,25 @@
 {
-    "checkout": "feature/markdown",
-    "commit": "10a9fe1a4f0b341184e41953433c344020f92c72",
+    "checkout": "feature/nox",
+    "commit": "49d100c749e6cfa2cba3460ed06e4a06be07cc63",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
                 "docs/_static/css/*",
                 "docs/_static/js/*",
                 "changelog.d/templates/*.j2",
                 "changelog.d/templates/auto-changelog/*.jinja2"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
-            "conda_channel": "wpk-nist",
+            "conda_channel": "conda-forge",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
             "github_username": "usnistgov",
             "open_source_license": "NIST license",
             "project_name": "thermoextrap",
             "project_short_description": "Thermodynamic extrapolation",
```

### Comparing `thermoextrap-0.3.1/.editorconfig` & `thermoextrap-0.4.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/.gitignore` & `thermoextrap-0.4.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
+.nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 .hypothesis/
@@ -102,11 +103,14 @@
 .mypy_cache/
 
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
+.noxconfig.toml
+cruft.patch
 /docs/**/generated/
 /monkeytype.sqlite3
-/dist-conda/*
-!/dist-conda/Makefile
+/dist-conda/
+/tmp/
+/thermoextrap-feedstock*/
```

### Comparing `thermoextrap-0.3.1/.pre-commit-config.yaml` & `thermoextrap-0.4.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
       - id: black
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
           - black==23.3.0
-        exclude: ^README.md
+        # exclude: ^README.md
   - repo: https://github.com/nbQA-dev/nbQA
     rev: 1.7.0
     hooks:
       - id: nbqa-ruff
         additional_dependencies: [ruff]
       - id: nbqa-black
         additional_dependencies: [black]
```

### Comparing `thermoextrap-0.3.1/CHANGELOG.md` & `thermoextrap-0.4.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,37 @@
+<!-- markdownlint-disable MD024 -->
+
 # Changelog
 
 Changelog for `thermoextrap`
 
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/thermoextrap)
 
 <!-- scriv-insert-here -->
 
+## v0.4.0 — 2023-06-15
+
+### Added
+
+- Package now available on conda-forge
+
+- Now support python3.11
+- Bumped pymbar version to pymbar>=4.0
+
+### Changed
+
+- Switched from tox to nox for testing.
+
+### Deprecated
+
+- No longer support pymbar < 4.0
+
 ## v0.3.0 — 2023-05-03
 
 ### Changed
 
 - New linters via pre-commit
 - Development env now handled by tox
```

### Comparing `thermoextrap-0.3.1/CONTRIBUTING.md` & `thermoextrap-0.4.0/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,67 +39,81 @@
 <https://github.com/usnistgov/thermoextrap/issues>.
 
 If you are proposing a feature:
 
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
 - Remember that this is a volunteer-driven project, and that contributions are
-  welcome :)
+  welcome!
 
 ## Get Started
 
 ### Environment setup
 
 [pipx]: https://github.com/pypa/pipx
 [condax]: https://github.com/mariusvniekerk/condax
 [mamba]: https://github.com/mamba-org/mamba
 [conda-fast-setup]:
   https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community
 [pre-commit]: https://pre-commit.com/
+[nox]: https://github.com/wntrblm/nox
+[noxopt]: https://github.com/rmorshea/noxopt
 [tox]: https://tox.wiki/en/latest/
-[tox-conda]: https://github.com/tox-dev/tox-conda
 [cruft]: https://github.com/cruft/cruft
-[conda-merge]: https://github.com/amitbeka/conda-merge
+[cog]: https://github.com/nedbat/cog
 [git-flow]: https://github.com/nvie/gitflow
 [scriv]: https://github.com/nedbat/scriv
 [conventional-style]: https://www.conventionalcommits.org/en/v1.0.0/
 [commitizen]: https://github.com/commitizen-tools/commitizen
 [nb_conda_kernels]: https://github.com/Anaconda-Platform/nb_conda_kernels
+[pyproject2conda]: https://github.com/wpk-nist-gov/pyproject2conda
 
 This project uses a host of tools to (hopefully) make development easier. We
 recommend installing some of these tools system wide. For this, we recommend
 using either [pipx] or [condax]. We mostly use conda/condax, but the choice is
 yours. For conda, we recommend actually using [mamba]. Alternatively, you can
 setup `conda` to use the faster `mamba` solver. See [here][conda-fast-setup] for
 details.
 
 Additional tools are:
 
 - [pre-commit]
-- [tox] and [tox-conda]
+- [nox] with [noxopt]
 - [cruft]
-- [conda-merge]
 - [scriv]
+- [commitizen] (optional)
+- [pyproject2conda] (optional)
+- [cog] (optional)
 
 These are setup using the following:
 
 ```console
-condax install pre-commit
-condax install tox
-condax inject tox tox-conda
-condax install cruft
-condax install conda-merge
-condax install commitizen
+condax/pipx install pre-commit
+condax/pipx install cruft
+condax/pipx install commitizen # optional
 pipx install scriv
+pipx install pyproject2conda # optional
+condax/pipx install cogapp # optional
 ```
 
-Alternatively, you can install these dependencies using:
+if using pipx, nox can be installed with:
 
-```console
-conda env update -n {env-name} environment/tools.yaml
+```bash
+pipx install nox
+pipx inject nox ruamel.yaml
+pipx inject nox noxopt
+```
+
+If using condax, you'll need to use:
+
+```bash
+condax install nox
+condax inject nox ruamel.yaml
+conda activate ~/.condax/nox
+pip install noxopt
 ```
 
 ### Getting the repo
 
 Ready to contribute? Here's how to set up `thermoextrap` for local development.
 
 - Fork the `thermoextrap` repo on GitHub.
@@ -123,57 +137,40 @@
   cd thermoextrap
   git submodule update --init --recursive
   ```
 
 - Create development environment. There are two options to create the
   development environment.
 
-  - The recommended method is to use tox by using either:
+  - The recommended method is to use nox. First you'll need to create the
+    environment files using:
 
     ```bash
-    tox -e dev
+    nox -e pyproject2conda
     ```
 
-    or
+    Then run:
 
     ```bash
-    make dev-env
+    nox -e dev
     ```
 
-    These create a development environment located at `.tox/dev`.
-
-    ```bash
-    make tox-ipykernel-display-name
-    ```
-
-    This will add a meaningful display name for the kernel (assuming you're
-    using [nb_conda_kernels])
+    This create a development environment located at `.nox/dev`.
 
   - Alternativley, you can create centrally located conda environmentment using
     the command:
 
     ```bash
-    make mamba-dev
+    conda/mamba env create -n {env-name} -f environment/dev.yaml
     ```
 
-    This will create a conda environment 'thermoextrap-env' in the default
-    location.
-
-    To install (an editable version) of the current package:
-
     ```bash
     pip install -e . --no-deps
     ```
 
-    or
-
-    ```bash
-    make install-dev
-    ```
-
 - Initiate [pre-commit] with:
 
   ```bash
   pre-commit install
   ```
 
   To update the recipe, periodically run:
@@ -206,24 +203,18 @@
 
   To run tests, use:
 
   ```bash
   pytest
   ```
 
-  To test against multiple python versions, use tox:
-
-  ```bash
-  tox
-  ```
-
-  or using the `make`:
+  To test against multiple python versions, use [nox]:
 
   ```bash
-  make test-all
+  nox -s test
   ```
 
   Additionally, you should run the following:
 
   ```bash
   make pre-commit-lint-markdown
   make pre-commit-codespell
@@ -251,152 +242,161 @@
   cz commit
   ```
 
 - Submit a pull request through the GitHub website.
 
 ### Dependency management
 
-Dependencies need to be placed in a few locations, which depend on the nature of
-the dependency.
-
-- Package dependency: `environment.yaml` and `dependencies` section of
-  `pyproject.toml`
-- Documentation dependency: `environment/docs-extras.yaml` and `test` section of
-  `pyproject.toml`
-- Development dependency: `environment/dev-extras.yaml` and `dev` section of
-  `pyproject.toml`
-
-Note that total yaml files are build using [conda-merge]. For example,
-`environment.yaml` is combined with `environment/docs-extras.yaml` to produce
-`environment/docs.yaml`. This is automated in the `Makefile`. You can also run,
-after doing any updates,
+We use [pyproject2conda] to handle conda `environment.yaml` files. This extracts
+the dependencies from `pyproject.toml`. See [pyproject2conda] for info. To make
+the `environment.yaml` files, run:
 
 ```bash
-make environment-files-build
+nox -s pyproject2conda -- [--pyproject2conda-force]
 ```
 
-which will rebuild all the needed yaml files.
+Where the option in brackets is optional.
 
 ## Pull Request Guidelines
 
 Before you submit a pull request, check that it meets these guidelines:
 
 - The pull request should include tests.
 - If the pull request adds functionality, the docs should be updated. Put your
   new functionality into a function with a docstring, and add the feature to the
   list in CHANGELOG.md. You should use [scriv] for this.
 - The pull request should work for Python 3.8, 3.9, 3.10.
 
-## Building the docs
+## ipykernel
 
-We use [tox] to isolate the documentation build. Useful commands are as follows.
+The environments created by nox `dev` and `docs` will try to add meaningful
+display names for ipykernel (assuming you're using [nb_conda_kernels])
 
-- Build the docs:
+## Building the docs
 
-  ```bash
-  tox -e docs -- build
-  ```
+We use [nox] to isolate the documentation build. Specific tasks can be run with
 
-- Spellcheck the docs:
+```bash
+nox -s docs -- -d [commands]
+```
 
-  ```bash
-  tox -e docs -- spelling
-  ```
+where commands can be one of:
 
-- Create a release of the docs:
+- clean : remove old doc build
+- build/html : build html documentation
+- spelling : check spelling
+- linkcheck : check the links
+- symlink : rebuild symlinks from `examples` to `docs/examples`
+- release : make pages branch for documentation hosting (using
+  [ghp-import](https://github.com/c-w/ghp-import))
+- livehtml : Live documentation updates
+- open : open the documentation in a web browser
 
-  ```bash
-  tox -e docs -- release
-  ```
+## Testing with nox
 
-  If you make any changes to `docs/examples`, you should run:
+The basic command is:
 
-  ```bash
-  make docs-examples-symlink
-  ```
+```bash
+nox -s test -- [--test-opts] [--no-cov]
+```
 
-  to update symlinks from `docs/examples` to `examples`.
+where you can pass in additional pytest options (properly escaped) via
+`--test-opts`. For example:
 
-  After this, the docs can be pushed to the correct branch for distribution.
+```bash
+nox -s test -- --test-opts "'-v'"
+# or
+nox -s test -- --test-opts "\-v"
+```
 
-- Live documentation updates using
+## Building distribution for conda
 
-  ```bash
-  make docs-livehtml
-  ```
+[grayskull]: https://github.com/conda/grayskull
 
-## Using tox
+For the most part, we use [grayskull] to create the conda recipe. However, I've
+had issues getting it to play nice with `pyproject.toml` for some of the 'extra'
+variables. So, we use grayskull to build the majority of the recipe, and append
+the file `.recipe-append.yaml`. For some edge cases (install name different from
+package name, etc), you'll need to manually edit this file to create the final
+recipe.
 
-The package is setup to use tox to test, build and release pip and conda
-distributions, and release the docs. Most of these tasks have a command in the
-`Makefile`. To test against multiple versions, use:
+The basic command is:
 
 ```bash
-make test-all
+nox -s dist-conda -- -c [command]
 ```
 
-To build the documentation in an isolated environment, use:
+Where `command` is one of:
 
-```bash
-make docs-build
-```
+- clean
+- recipe : create recipe via [grayskull]
+- build : build the distribution
 
-To release the documentation use:
+To upload the recipe, you'll need to run an external command like:
 
 ```bash
-make docs-release release_args='-m "commit message" -r origin -p'
+nox -s dist-conda -- --dist-conda-run "anaconda upload PATH-TO-TARBALL"
 ```
 
-Where posargs is are passed to ghp-import. Note that the branch created is
-called `nist-pages`. This can be changed in `tox.ini`.
+## Building distribution for pypi
 
-To build the distribution, use:
+The basic command is:
 
 ```bash
-make dist-pypi-[build-testrelease-release]
+nox -s dist-pypi -- -p [command]
 ```
 
-where `build` build to distro, `testrelease` tests putting on `testpypi` and
-release puts the distro on pypi.
+where `command` is one of:
+
+- clean : clean out old distribution
+- build : build distribution (if specify only this, clean will be called first)
+- testrelease : upload to testpypi
+- release : upload to pypi
+
+## Testing pypi or conda installs
 
-To build the conda distribution, use:
+Run:
 
 ```bash
-make dist-conda-[recipe, build]
+nox -s testdist-pypi -- --version [version]
 ```
 
-where `recipe` makes the conda recipe (using grayskull), and `build` makes the
-distro. This can be manually added to a channel.
-
-To test the created distributions, you can use one of:
+to test a specific version from pypi and
 
 ```bash
-tox -e test-dist-[pypi, conda]-[local,remote]-py[38,39,...]
+nox -s testdist-conda -- --version [version]
 ```
 
-or
+to to likewise from conda.
+
+## Type checking
+
+Run:
 
 ```bash
-make test-dist-[pypi, conda]-[local,remote] py=[38, 39, 310]
+nox -s typing -- -m [commands] [options]
 ```
 
-where one options in the brackets should be choosen.
-
 ## Package version
 
 [setuptools_scm]: https://github.com/pypa/setuptools_scm
 
-Versioning is handled with [setuptools_scm].The pacakge version is set by the
-git tag. For convenience, you can override the version in the makefile (calling
-tox) by setting `version=v{major}.{minor}.{micro}`. This is useful for updating
-the docs, etc.
+Versioning is handled with [setuptools_scm].The package version is set by the
+git tag. For convenience, you can override the version with nox setting
+`--version ...`. This is useful for updating the docs, etc.
 
-## Creating conda recipe
+## Notes on [nox]
 
-[grayskull]: https://github.com/conda/grayskull
+One downside of using [tox] with this particular workflow is the need for
+multiple scripts/makefiles, while with [nox], most everything is self contained
+in the file `noxfile.py`. [nox] also is allows for a mix of conda and virtualenv
+environments.
 
-For the most part, we use [grayskull] to create the conda recipe. However, I've
-had issues getting it to play nice with `pyproject.toml` for some of the 'extra'
-variables. So, we use grayskull to build the majority of the recipe, and append
-the file `.recipe-append.yaml`. For some edge cases (install name different from
-package name, etc), you'll need to manually edit this file to create the final
-recipe.
+## Serving the documentation
+
+To view to documentation with js headers/footers, you'll need to serve them:
+
+```bash
+python -m http.server -d docs/_build/html
+```
+
+Then open the address `localhost:8000` in a webbrowser.
```

### Comparing `thermoextrap-0.3.1/LICENSE` & `thermoextrap-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/Makefile` & `thermoextrap-0.4.0/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 clean-pyc: ## remove Python file artifacts
 	find . -name '*.pyc' -exec rm -f {} +
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 	find . -name '__pycache__' -exec rm -fr {} +
 
 clean-test: ## remove test and coverage artifacts
-	rm -fr .tox/
+	rm -fr .nox/
 	rm -f .coverage
 	rm -fr htmlcov/
 	rm -fr .pytest_cache
 
 
 
 
@@ -99,15 +99,15 @@
 
 
 ################################################################################
 # my convenience functions
 ################################################################################
 .PHONY: user-venv user-autoenv-zsh user-all
 user-venv: ## create .venv file with name of conda env
-	echo $${PWD}/.tox/dev > .venv
+	echo $${PWD}/.nox/dev > .venv
 
 user-autoenv-zsh: ## create .autoenv.zsh files
 	echo conda activate $$(cat .venv) > .autoenv.zsh
 	echo conda deactivate > .autoenv_leave.zsh
 
 user-all: user-venv user-autoenv-zsh ## runs user scripts
 
@@ -115,14 +115,17 @@
 ################################################################################
 # Testing
 ################################################################################
 .PHONY: test coverage
 test: ## run tests quickly with the default Python
 	pytest -x -v
 
+test-accept: ## run tests and accept doctest results. (using pytest-accept)
+	DOCFILLER_SUB=False pytest -v --accept
+
 coverage: ## check code coverage quickly with the default Python
 	coverage run --source thermoextrap -m pytest
 	coverage report -m
 	coverage html
 	$(BROWSER) htmlcov/index.html
 
 
@@ -137,167 +140,117 @@
 	python -c 'import thermoextrap; print(thermoextrap.__version__)'
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
-ENVIRONMENTS = $(addsuffix .yaml,$(addprefix environment/, dev docs test))
-PRETTIER = bash scripts/run-prettier.sh
-
-environment/%.yaml: environment.yaml environment/%-extras.yaml ## create combined environment/{dev,docs,test}.yaml
-	conda-merge $^ > $@
-	$(PRETTIER) $@
-
-environment/dev.yaml: ## development environment yaml file
-environment/test.yaml: ## testing environment yaml file
-enviornment/docs.yaml: ## docs environment yaml file
-
-
-# special for linters
-environment/lint.yaml: environment.yaml $(addsuffix .yaml, $(addprefix environment/, test-extras lint-extras)) ## mypy environment
-	echo $^
-	conda-merge $^ > $@
-	$(PRETTIER) $@
-
-ENVIRONMENTS += environment/lint.yaml
-
 .PHONY: environment-files-clean
 environment-files-clean: ## clean all created environment/{dev,docs,test}.yaml
 	-rm $(ENVIRONMENTS) 2> /dev/null || true
 
 .PHONY: environment-files-build
-environment-files-build: $(ENVIRONMENTS) ## rebuild all environment files
+environment-files-build: pyproject.toml ## rebuild all environment files
+	nox -s pyproject2conda
+
+environment/%.yaml: pyproject.toml
+	nox -s pyproject2conda
 
 ################################################################################
 # virtual env
 ################################################################################
-.PHONY: mamba-env mamba-dev mamba-env-update mamba-dev-update
+.PHONY: mamba-env-update mamba-dev-update
 
-mamba-env: environment.yaml ## create base environment
+mamba-dev: environment/dev.yaml environment-files-build ## create development environment
 	mamba env create -f $<
 
-mamba-env-update: environment.yaml ## update base environment
-	mamba env update -f $<
-
-mamba-dev: environment/dev.yaml ## create development environment
-	mamba env create -f $<
-
-mamba-dev-update: environment/dev.yaml ## update development environment
+mamba-dev-update: environment/dev.yaml environment-files-build ## update development environment
 	mamba env update -f $<
 
 ################################################################################
-# TOX
+# NOX
 ###############################################################################
-tox_args?=-v
-version?=
-TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_args)
-
-.PHONY: tox-ipykernel-display-name
-tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
-	bash ./scripts/tox-ipykernel-display-name.sh thermoextrap
-
 ## dev env
+NOX=nox
 .PHONY: dev-env
-dev-env: environment/dev.yaml ## create development environment using tox
-	tox -e dev
+dev-env: environment/dev.yaml ## create development environment using nox
+	$(NOX) -e dev
 
 ## testing
 .PHONY: test-all
-test-all: environment/test.yaml ## run tests on every Python version with tox.  can pass posargs=...
-	$(TOX) -- $(posargs)
+test-all: environment/test.yaml ## run tests on every Python version with nox.
+	$(NOX) -s test
 
 ## docs
-.PHONY: docs-examples-symlink
-docs-examples-symlink: ## create symlinks to notebooks from /examples/ to /docs/examples.
-	bash ./scripts/docs-examples-symlinks.sh
-
-
 .PHONY: docs-build docs-release docs-clean docs-command
 docs-build: ## build docs in isolation
-	$(TOX) -e docs -- build
+	$(NOX) -s docs -- -d build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
-docs-release: ## release docs.  use release_args=... to override stuff
-	$(TOX) -e docs -- release
-docs-command: ## run command with command=...
-	$(TOX) -e docs -- command
+docs-release: ## release docs.
+	$(NOX) -s docs -- release
+docs-command: ## run arbitrary command with command=...
+	$(NOX) -s docs -- --docs-run $(command)
 
 .PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
 docs-spelling: ## run spell check with sphinx
-	$(TOX) -e docs -- spelling
+	$(NOX) -s docs -- -d spelling
 docs-livehtml: ## use autobuild for docs
-	$(TOX) -e docs -- livehtml
+	$(NOX) -s docs -- -d livehtml
 docs-open: ## open the build
-	$(BROWSER) docs/_build/html/index.html
+	$(NOX) -s docs -- -d open
 docs-linkcheck: ## check links
-	$(TOX) -e docs -- linkcheck
+	$(NOX) -s docs -- -d linkcheck
 
 docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/docs.yaml
 
-## linting
-.PHONY: lint-mypy lint-pyright lint-pytype lint-all lint-command
-lint-mypy: ## run mypy mypy_args=...
-	$(TOX) -e lint -- mypy
-lint-pyright: ## run pyright pyright_args=...
-	$(TOX) -e lint -- pyright
-lint-pytype: ## run pytype pytype_args=...
-	$(TOX) -e lint -- pytype
-lint-all:
-	$(TOX) -e lint -- all
-lint-command:
-	$(TOX) -e lint -- command
-
-lint-mypy lint-pyright lint-pytype lint-all lint-command: environment/lint.yaml
+## typing
+.PHONY: typing-mypy typing-pyright typing-pytype typing-all typing-command
+typing-mypy: ## run mypy mypy_args=...
+	$(NOX) -s typing -- -m mypy
+typing-pyright: ## run pyright pyright_args=...
+	$(NOX) -s typing -- -m pyright
+typing-pytype: ## run pytype pytype_args=...
+	$(NOX) -s typing -- -m pytype
+typing-all:
+	$(NOX) -s typing -- -m mypy pyright pytype
+typing-command:
+	$(NOX) -s typing -- --typing-run $(command)
+typing-mypy typing-pyright typing-pytype typing-all typing-command: environment/typing.yaml
 
 ## distribution
 .PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command
 
 dist-pypi-build: ## build dist
-	$(TOX) -e dist-pypi -- build
+	$(NOX) -s dist-pypi -- -p build
 dist-pypi-testrelease: ## test release on testpypi
-	$(TOX) -e dist-pypi -- testrelease
+	$(NOX) -s dist-pypi -- -p testrelease
 dist-pypi-release: ## release to pypi, can pass posargs=...
-	$(TOX) -e dist-pypi -- release
+	$(NOX) -s dist-pypi -- -p release
 dist-pypi-command: ## run command with command=...
-	$(TOX) -e dist-pypi -- command
+	$(NOX) -s dist-pypi -- --dist-pypi-run $(command)
 dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/dist-pypi.yaml
 
 .PHONY: dist-conda-recipe dist-conda-build dist-conda-command
 dist-conda-recipe: ## build conda recipe can pass posargs=...
-	$(TOX) -e dist-conda -- recipe
+	$(NOX) -s dist-conda -- -c recipe
 dist-conda-build: ## build conda recipe can pass posargs=...
-	$(TOX) -e dist-conda -- build
+	$(NOX) -s dist-conda -- -c build
 dist-conda-command: ## run command with command=...
-	$(TOX) -e dist-conda -- command
+	$(NOX) -s dist-conda -- -dist-conda-run $(command)
 dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
-## test distribution
-.PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
-
-py?=310
-testdist-pypi-remote: ## testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39.  Can specify version setting, eg,  TEST_VERSION='==0.1.0'.  Note that the the format should be '=={version}'.
-	$(TOX) -e $@-py$(py) -- $(posargs)
-testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
-	$(TOX) -e $@-py$(py) -- $(poasargs)
-testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
-	$(TOX) -e $@-py$(py) -- $(posargs)
-testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
-	$(TOX) -e $@-py$(py) -- $(poasargs)
-
-testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local: environment/test.yaml
-
 ## list all options
-.PHONY: tox-list
-tox-list:
-	$(TOX) -a
+.PHONY: nox-list
+nox-list:
+	$(NOX) --list
 
 
 ################################################################################
 # installation
 ################################################################################
 .PHONY: install install-dev
 install: ## install the package to the active Python's site-packages (run clean?)
```

### Comparing `thermoextrap-0.3.1/PKG-INFO` & `thermoextrap-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thermoextrap
-Version: 0.3.1
+Version: 0.4.0
 Summary: Thermodynamic extrapolation
 Author-email: Jacob Monroe <jacob.monroe@nist.gov>, William Krekelberg <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/thermoextrap
 Project-URL: documentation, https://pages.nist.gov/thermoextrap/
 Keywords: thermoextrap
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,25 +12,36 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: accel
 Provides-Extra: parallel
 Provides-Extra: viz
 Provides-Extra: mbar
 Provides-Extra: gpr
 Provides-Extra: openmm
 Provides-Extra: all
 Provides-Extra: test
+Provides-Extra: dev-extras
+Provides-Extra: typing-extras
+Provides-Extra: typing
+Provides-Extra: nox
+Provides-Extra: dev
+Provides-Extra: tools
+Provides-Extra: dev-complete
+Provides-Extra: docs
+Provides-Extra: dist-pypi
+Provides-Extra: dist-conda
 License-File: LICENSE
 
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
@@ -47,16 +58,16 @@
 [black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/thermoextrap
 [pypi-link]: https://pypi.org/project/thermoextrap
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/thermoextrap/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/thermoextrap
-[conda-badge]: https://img.shields.io/conda/v/wpk-nist/thermoextrap
-[conda-link]: https://anaconda.org/wpk-nist/thermoextrap
+[conda-badge]: https://img.shields.io/conda/v/conda-forge/thermoextrap
+[conda-link]: https://anaconda.org/conda-forge/thermoextrap
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/thermoextrap/blob/main/LICENSE
 
 <!-- other links -->
 
 [cmomy]: https://github.com/usnistgov/cmomy
 [gpr-link]:
@@ -109,15 +120,15 @@
 request for wanted features and suggestions!
 
 ## Quick start
 
 `thermoextrap` may be installed with either (recommended)
 
 ```bash
-conda install -c wpk-nist thermoextrap
+conda install -c conda-forge thermoextrap
 ```
 
 or
 
 ```bash
 pip install thermoextrap
 ```
@@ -185,25 +196,44 @@
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
+<!-- markdownlint-disable MD024 -->
+
 # Changelog
 
 Changelog for `thermoextrap`
 
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/thermoextrap)
 
 <!-- scriv-insert-here -->
 
+## v0.4.0 — 2023-06-15
+
+### Added
+
+- Package now available on conda-forge
+
+- Now support python3.11
+- Bumped pymbar version to pymbar>=4.0
+
+### Changed
+
+- Switched from tox to nox for testing.
+
+### Deprecated
+
+- No longer support pymbar < 4.0
+
 ## v0.3.0 — 2023-05-03
 
 ### Changed
 
 - New linters via pre-commit
 - Development env now handled by tox
```

### Comparing `thermoextrap-0.3.1/README.md` & `thermoextrap-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 [black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/thermoextrap
 [pypi-link]: https://pypi.org/project/thermoextrap
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/thermoextrap/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/thermoextrap
-[conda-badge]: https://img.shields.io/conda/v/wpk-nist/thermoextrap
-[conda-link]: https://anaconda.org/wpk-nist/thermoextrap
+[conda-badge]: https://img.shields.io/conda/v/conda-forge/thermoextrap
+[conda-link]: https://anaconda.org/conda-forge/thermoextrap
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/thermoextrap/blob/main/LICENSE
 
 <!-- other links -->
 
 [cmomy]: https://github.com/usnistgov/cmomy
 [gpr-link]:
@@ -78,15 +78,15 @@
 request for wanted features and suggestions!
 
 ## Quick start
 
 `thermoextrap` may be installed with either (recommended)
 
 ```bash
-conda install -c wpk-nist thermoextrap
+conda install -c conda-forge thermoextrap
 ```
 
 or
 
 ```bash
 pip install thermoextrap
 ```
```

### Comparing `thermoextrap-0.3.1/changelog.d/templates/auto-changelog/template.jinja2` & `thermoextrap-0.4.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/pyproject.toml` & `thermoextrap-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -19,80 +19,159 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["readme", "version"]
 requires-python = ">=3.8"
 dependencies = [
     "numpy >= 1.20",
     "xarray >= 0.16",
     "sympy",
     "scipy",
-    "cmomy >= 0.4",
+    "cmomy >= 0.5",
     "custom-inherit",
     "attrs",
     "module-utilities >= 0.2",
 ]
 
 [project.urls]
 homepage = "https://github.com/usnistgov/thermoextrap"
 documentation = "https://pages.nist.gov/thermoextrap/"
 
 [project.optional-dependencies]
 accel = ["bottleneck"]
-parallel = ["dask[complete]"]
+parallel = [
+    "dask[complete]", # p2c: -s dask
+
+]
 viz = ["matplotlib"]
-mbar = ["pymbar<4.0"]
-gpr = ["tensorflow", "tensorflow-probability", "gpflow"]
+mbar = ["pymbar>=4.0"]
+gpr = [
+    "tensorflow", # p2c: -p
+    "tensorflow-probability", # p2c: -p
+    "gpflow < 2.6.0", # p2c: -p
+
+]
 openmm = ["openmm"]
 all = [
     "thermoextrap[mbar]",
     "thermoextrap[gpr]",
     "thermoextrap[accel]",
     "thermoextrap[parallel]",
     "thermoextrap[viz]",
 ]
-test = ["pytest"]
+test = [
+    "pytest", #
+    "pytest-xdist",
+    "pytest-cov",
+    "pytest-sugar",
+    "pandas",
+    "thermoextrap[mbar]",
+    "thermoextrap[gpr]",
+]
+dev-extras = [
+    "pytest-accept", # p2c: -p
+    "setuptools-scm",
+    "ipython",
+    "ipykernel",
+]
+typing-extras = [
+    # "pytype; python_version < '3.11'",
+    "mypy",
+]
+typing = [
+    "thermoextrap[typing-extras]", #
+    "thermoextrap[test]",
+]
+nox = [
+    "nox",
+    "noxopt", # p2c: -p
+    "ruamel.yaml",
+]
+dev = [
+    "thermoextrap[test]", #
+    "thermoextrap[typing-extras]",
+    "thermoextrap[dev-extras]",
+    "thermoextrap[accel]",
+    "thermoextrap[viz]",
+]
+tools = [
+    "pre-commit", #
+    "cruft",
+    "scriv",
+]
+dev-complete = [
+    "thermoextrap[dev]", #
+    "thermoextrap[tools]",
+    "thermoextrap[nox]",
+]
+docs = [
+    "setuptools-scm", #
+    "ipython",
+    "pyenchant",
+    "ghp-import",
+    "sphinx",
+    "sphinx-copybutton",
+    "sphinxcontrib-spelling",
+    "sphinx-autobuild",
+    "myst-nb",
+    "sphinx-book-theme",
+    "autodocsumm",
+    "thermoextrap[viz]",
+    "thermoextrap[mbar]",
+    "thermoextrap[gpr]",
+]
+# to be parsed with pyproject2conda with --no-base option
+dist-pypi = ["twine", "build"]
+dist-conda = [
+    "anaconda-client", #
+    "grayskull",
+    "conda-build",
+    "conda-verify",
+    "boa",
+    "setuptools-scm",
+]
+
+[tool.pyproject2conda]
+channels = ["conda-forge"]
 
-# dev = []
-# docs = []
 ## grayskull still messes some things up, but use scripts/recipe-append.sh for this
 [tool.setuptools]
 zip-safe = true # if using mypy, must be False
 include-package-data = true
 license-files = ["LICENSE"]
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 ## include = []
 ## exclude = []
-##
 [tool.setuptools.dynamic]
 readme = { file = [
     "README.md",
     "CHANGELOG.md",
     "LICENSE"
 ], content-type = "text/markdown" }
 
 [tool.setuptools_scm]
 fallback_version = "999"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
-addopts = "--verbose"
-testpaths = ["tests"]
+addopts = "--doctest-modules --doctest-glob='*.md'"
+testpaths = ["tests", "README.md"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["thermoextrap"]
 
 [tool.ruff]
@@ -251,15 +330,15 @@
 
 [tool.mypy]
 files = ["src/thermoextrap"]
 show_error_codes = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unused_configs = true
-exclude = [".eggs", ".tox", "doc", "docs"]
+exclude = [".eggs", ".tox", "doc", "docs", ".nox"]
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = []
 
 [[tool.mypy.overrides]]
```

### Comparing `thermoextrap-0.3.1/src/thermoextrap/__init__.py` & `thermoextrap-0.4.0/src/thermoextrap/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/adaptive_interp.py` & `thermoextrap-0.4.0/src/thermoextrap/adaptive_interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/beta.py` & `thermoextrap-0.4.0/src/thermoextrap/beta.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/core/_attrs_utils.py` & `thermoextrap-0.4.0/src/thermoextrap/core/_attrs_utils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/core/_deprecate.py` & `thermoextrap-0.4.0/src/thermoextrap/core/_deprecate.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/core/xrutils.py` & `thermoextrap-0.4.0/src/thermoextrap/core/xrutils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/data.py` & `thermoextrap-0.4.0/src/thermoextrap/data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/docstrings.py` & `thermoextrap-0.4.0/src/thermoextrap/docstrings.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/gpr_active/__init__.py` & `thermoextrap-0.4.0/src/thermoextrap/gpr_active/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/gpr_active/active_utils.py` & `thermoextrap-0.4.0/src/thermoextrap/gpr_active/active_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,24 +243,24 @@
         pot = tot_pot - bias
         # Extract statistical inefficiencies for x and pot and pick largest
         # Can have multidimensional outputs, i.e., multiple columns of x
         # Handle by looping and taking maximum
         g_x = 0.0
         g_cross = 0.0
         for k in range(x.shape[1]):
-            this_g_x = timeseries.statisticalInefficiency(x[:, k])
-            this_g_cross = timeseries.statisticalInefficiency(x[:, k], pot)
+            this_g_x = timeseries.statistical_inefficiency(x[:, k])
+            this_g_cross = timeseries.statistical_inefficiency(x[:, k], pot)
             if this_g_x > g_x:
                 g_x = this_g_x
             if this_g_cross > g_cross:
                 g_cross = this_g_cross
-        g_pot = timeseries.statisticalInefficiency(pot)
+        g_pot = timeseries.statistical_inefficiency(pot)
         g_max = np.max([g_x, g_pot, g_cross])
         # Get indices of uncorrelated data and subsample everything
-        uncorr_inds = timeseries.subsampleCorrelatedData(np.arange(x.shape[0]), g_max)
+        uncorr_inds = timeseries.subsample_correlated_data(np.arange(x.shape[0]), g_max)
         x = x[uncorr_inds, :]
         bias = bias[uncorr_inds]
         pot = pot[uncorr_inds]
         # Get weights to remove bias during averaging
         logw = get_logweights(self.beta * bias)
         w = np.exp(logw)
         # Convert to xarray objects with dimensions named appropriately
```

### Comparing `thermoextrap-0.3.1/src/thermoextrap/gpr_active/gp_models.py` & `thermoextrap-0.4.0/src/thermoextrap/gpr_active/gp_models.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/gpr_active/ig_active.py` & `thermoextrap-0.4.0/src/thermoextrap/gpr_active/ig_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/gpr_active/sine_active.py` & `thermoextrap-0.4.0/src/thermoextrap/gpr_active/sine_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/idealgas.py` & `thermoextrap-0.4.0/src/thermoextrap/idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/__init__.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/extrap.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/extrap.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/gpr.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/gpr.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/gpr_stack.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/gpr_stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/ig.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/ig.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/interp.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/old_scripts.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/old_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         B = [B]
     B = np.array(B)
 
     if useMBAR:
         mbarObj = mbar.MBAR(np.array([refB * U]), [U.shape[0]])
         outval = np.zeros((len(B), x.shape[1]))
         for i in range(len(B)):
-            outval[i, :] = mbarObj.computeMultipleExpectations(x.T, B[i] * U)[0]
+            outval[i, :] = mbarObj.compute_multiple_expectations(x.T, B[i] * U)["mu"]
 
     else:
         # Compute what goes in the exponent and subtract out the maximum
         # Don't need to bother storing for later because compute ratio
         dBeta = B - refB
         dBetaU = (-1.0) * np.tensordot(dBeta, U, axes=0)
         dBetaUdiff = dBetaU - np.array([np.max(dBetaU, axis=1)]).T
```

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/recursive_interp.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/recursive_interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/reweight.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/reweight.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,17 +79,17 @@
             B = [B]
         B = np.array(B)
 
         if useMBAR:
             mbarObj = mbar.MBAR(np.array([refB * U]), [U.shape[0]])
             predictVals = np.zeros((len(B), x.shape[1]))
             for i in range(len(B)):
-                predictVals[i, :] = mbarObj.computeMultipleExpectations(x.T, B[i] * U)[
-                    0
-                ]
+                predictVals[i, :] = mbarObj.compute_multiple_expectations(
+                    x.T, B[i] * U
+                )["mu"]
 
         else:
             # Compute what goes in the exponent and subtract out the maximum
             # Don't need to bother storing for later because compute ratio
             dBeta = B - refB
             dBetaU = (-1.0) * np.tensordot(dBeta, U, axes=0)
             dBetaUdiff = dBetaU - np.array([np.max(dBetaU, axis=1)]).T
@@ -214,10 +214,12 @@
         B = np.array(B)
 
         allU = self.U.flatten()
         predictVals = np.zeros((len(B), self.x.shape[2]))
         x = np.reshape(self.x, (self.x.shape[0] * self.x.shape[1], self.x.shape[2]))
 
         for i in range(len(B)):
-            predictVals[i, :] = params.computeMultipleExpectations(x.T, B[i] * allU)[0]
+            predictVals[i, :] = params.compute_multiple_expectations(x.T, B[i] * allU)[
+                "mu"
+            ]
 
         return predictVals
```

### Comparing `thermoextrap-0.3.1/src/thermoextrap/legacy/utilities.py` & `thermoextrap-0.4.0/src/thermoextrap/legacy/utilities.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/lnpi.py` & `thermoextrap-0.4.0/src/thermoextrap/lnpi.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/models.py` & `thermoextrap-0.4.0/src/thermoextrap/models.py`

 * *Files identical despite different names*

```diff
@@ -1085,15 +1085,15 @@
         x = np.array(xv, order="c")
         x_flat = x.reshape(x.shape[0] * x.shape[1], -1)
 
         U = uv.values.reshape(-1)
 
         out = []
         for b in alpha.values:
-            out.append(mbar_obj.computeMultipleExpectations(x_flat.T, b * U)[0])
+            out.append(mbar_obj.compute_multiple_expectations(x_flat.T, b * U)["mu"])
 
         out = np.array(out)
         # reshape
         shape = (out.shape[0],) + x.shape[2:]
         out = xr.DataArray(
             out.reshape(shape), dims=(alpha.name,) + dims[2:]
         ).assign_coords(alpha=alpha)
```

### Comparing `thermoextrap-0.3.1/src/thermoextrap/recursive_interp.py` & `thermoextrap-0.4.0/src/thermoextrap/recursive_interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/stack.py` & `thermoextrap-0.4.0/src/thermoextrap/stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/volume.py` & `thermoextrap-0.4.0/src/thermoextrap/volume.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap/volume_idealgas.py` & `thermoextrap-0.4.0/src/thermoextrap/volume_idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/src/thermoextrap.egg-info/PKG-INFO` & `thermoextrap-0.4.0/src/thermoextrap.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thermoextrap
-Version: 0.3.1
+Version: 0.4.0
 Summary: Thermodynamic extrapolation
 Author-email: Jacob Monroe <jacob.monroe@nist.gov>, William Krekelberg <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/thermoextrap
 Project-URL: documentation, https://pages.nist.gov/thermoextrap/
 Keywords: thermoextrap
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,25 +12,36 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: accel
 Provides-Extra: parallel
 Provides-Extra: viz
 Provides-Extra: mbar
 Provides-Extra: gpr
 Provides-Extra: openmm
 Provides-Extra: all
 Provides-Extra: test
+Provides-Extra: dev-extras
+Provides-Extra: typing-extras
+Provides-Extra: typing
+Provides-Extra: nox
+Provides-Extra: dev
+Provides-Extra: tools
+Provides-Extra: dev-complete
+Provides-Extra: docs
+Provides-Extra: dist-pypi
+Provides-Extra: dist-conda
 License-File: LICENSE
 
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
@@ -47,16 +58,16 @@
 [black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/thermoextrap
 [pypi-link]: https://pypi.org/project/thermoextrap
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/thermoextrap/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/thermoextrap
-[conda-badge]: https://img.shields.io/conda/v/wpk-nist/thermoextrap
-[conda-link]: https://anaconda.org/wpk-nist/thermoextrap
+[conda-badge]: https://img.shields.io/conda/v/conda-forge/thermoextrap
+[conda-link]: https://anaconda.org/conda-forge/thermoextrap
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/thermoextrap/blob/main/LICENSE
 
 <!-- other links -->
 
 [cmomy]: https://github.com/usnistgov/cmomy
 [gpr-link]:
@@ -109,15 +120,15 @@
 request for wanted features and suggestions!
 
 ## Quick start
 
 `thermoextrap` may be installed with either (recommended)
 
 ```bash
-conda install -c wpk-nist thermoextrap
+conda install -c conda-forge thermoextrap
 ```
 
 or
 
 ```bash
 pip install thermoextrap
 ```
@@ -185,25 +196,44 @@
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
+<!-- markdownlint-disable MD024 -->
+
 # Changelog
 
 Changelog for `thermoextrap`
 
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/thermoextrap)
 
 <!-- scriv-insert-here -->
 
+## v0.4.0 — 2023-06-15
+
+### Added
+
+- Package now available on conda-forge
+
+- Now support python3.11
+- Bumped pymbar version to pymbar>=4.0
+
+### Changed
+
+- Switched from tox to nox for testing.
+
+### Deprecated
+
+- No longer support pymbar < 4.0
+
 ## v0.3.0 — 2023-05-03
 
 ### Changed
 
 - New linters via pre-commit
 - Development env now handled by tox
```

### Comparing `thermoextrap-0.3.1/src/thermoextrap.egg-info/SOURCES.txt` & `thermoextrap-0.4.0/src/thermoextrap.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,40 +9,33 @@
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
-environment.yaml
+noxfile.py
 pyproject.toml
-tox.ini
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
-environment/conda-spec.txt
-environment/dev-extras.yaml
+environment/base.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
 environment/dist-pypi.yaml
-environment/docs-extras.yaml
 environment/docs.yaml
-environment/lint-extras.yaml
-environment/lint.yaml
+environment/test-extras.txt
 environment/test-extras.yaml
 environment/test.yaml
-environment/tools.yaml
-scripts/dist-conda.mk
-scripts/dist-pypi.mk
-scripts/docs-examples-symlinks.sh
-scripts/lint.mk
-scripts/recipe-append.sh
-scripts/run-prettier.sh
-scripts/tox-ipykernel-display-name.sh
+environment/typing.yaml
+environment/lock/py310.yaml
+environment/lock/py311.yaml
+environment/lock/py38.yaml
+environment/lock/py39.yaml
 src/thermoextrap/__init__.py
 src/thermoextrap/adaptive_interp.py
 src/thermoextrap/beta.py
 src/thermoextrap/data.py
 src/thermoextrap/docstrings.py
 src/thermoextrap/idealgas.py
 src/thermoextrap/lnpi.py
@@ -84,8 +77,9 @@
 tests/test_data.py
 tests/test_idealgas.py
 tests/test_lnPi.py
 tests/test_stack.py
 tests/test_u_data.py
 tests/test_u_equations.py
 tests/test_volume.py
-tests/lnpi_data/sample_data.json
+tests/lnpi_data/sample_data.json
+tools/noxtools.py
```

### Comparing `thermoextrap-0.3.1/tests/conftest.py` & `thermoextrap-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/lnpi_data/sample_data.json` & `thermoextrap-0.4.0/tests/lnpi_data/sample_data.json`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_GPs.py` & `thermoextrap-0.4.0/tests/test_GPs.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_active.py` & `thermoextrap-0.4.0/tests/test_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_beta.py` & `thermoextrap-0.4.0/tests/test_beta.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_data.py` & `thermoextrap-0.4.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_idealgas.py` & `thermoextrap-0.4.0/tests/test_idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_lnPi.py` & `thermoextrap-0.4.0/tests/test_lnPi.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_stack.py` & `thermoextrap-0.4.0/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_u_data.py` & `thermoextrap-0.4.0/tests/test_u_data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_u_equations.py` & `thermoextrap-0.4.0/tests/test_u_equations.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.1/tests/test_volume.py` & `thermoextrap-0.4.0/tests/test_volume.py`

 * *Files identical despite different names*

