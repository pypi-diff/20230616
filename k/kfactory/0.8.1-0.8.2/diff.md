# Comparing `tmp/kfactory-0.8.1.tar.gz` & `tmp/kfactory-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.8.1.tar", last modified: Fri Jun 16 11:48:36 2023, max compression
+gzip compressed data, was "kfactory-0.8.2.tar", last modified: Fri Jun 16 19:57:19 2023, max compression
```

## Comparing `kfactory-0.8.1.tar` & `kfactory-0.8.2.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.364026 kfactory-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.348026 kfactory-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.348026 kfactory-0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-16 11:48:18.000000 kfactory-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-16 11:48:18.000000 kfactory-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 11:48:18.000000 kfactory-0.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.348026 kfactory-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-16 11:48:18.000000 kfactory-0.8.1/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-16 11:48:18.000000 kfactory-0.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-16 11:48:18.000000 kfactory-0.8.1/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-16 11:48:18.000000 kfactory-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-16 11:48:18.000000 kfactory-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 11:48:18.000000 kfactory-0.8.1/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-16 11:48:18.000000 kfactory-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-16 11:48:18.000000 kfactory-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-16 11:48:18.000000 kfactory-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-16 11:48:36.364026 kfactory-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-16 11:48:18.000000 kfactory-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.348026 kfactory-0.8.1/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 11:48:18.000000 kfactory-0.8.1/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.348026 kfactory-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.348026 kfactory-0.8.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.348026 kfactory-0.8.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.352026 kfactory-0.8.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/gdsfactory.md
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.352026 kfactory-0.8.1/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/notebooks/03_Enclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/pre.md
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-16 11:48:18.000000 kfactory-0.8.1/docs/source/waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.344026 kfactory-0.8.1/gds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.356026 kfactory-0.8.1/gds/gds_ref/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_circular.gds
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A180_AS1.gds
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A90_AS1.gds
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T180_TS1.gds
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T90_TS1.gds
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_euler.gds
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A180_R150.gds
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A90_R150.gds
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T180_R150.gds
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T90_R150.gds
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_s.gds
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/bend_s_euler.gds
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/straight_W500_L1000_LWG_EWGSTD.gds
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/taper.gds
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/waveguide.gds
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-16 11:48:18.000000 kfactory-0.8.1/gds/gds_ref/waveguide_W500_L1000_LWG_EWGSTD.gds
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-16 11:48:18.000000 kfactory-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:48:36.364026 kfactory-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.344026 kfactory-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.356026 kfactory-0.8.1/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.360026 kfactory-0.8.1/src/kfactory/cells/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.360026 kfactory-0.8.1/src/kfactory/cells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/dbu/straight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/straight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/cells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)   111992 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/kcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.360026 kfactory-0.8.1/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.360026 kfactory-0.8.1/src/kfactory/technology/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/technology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/technology/layer_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.360026 kfactory-0.8.1/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55806 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/utils/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/utils/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.360026 kfactory-0.8.1/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-06-16 11:48:18.000000 kfactory-0.8.1/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.356026 kfactory-0.8.1/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-16 11:48:36.000000 kfactory-0.8.1/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-16 11:48:36.000000 kfactory-0.8.1/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:48:36.000000 kfactory-0.8.1/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-16 11:48:36.000000 kfactory-0.8.1/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 11:48:36.000000 kfactory-0.8.1/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:48:36.364026 kfactory-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_netlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-16 11:48:18.000000 kfactory-0.8.1/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.391002 kfactory-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.371002 kfactory-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.371002 kfactory-0.8.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-16 19:56:58.000000 kfactory-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-16 19:56:58.000000 kfactory-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 19:56:58.000000 kfactory-0.8.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.371002 kfactory-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-16 19:56:58.000000 kfactory-0.8.2/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-16 19:56:58.000000 kfactory-0.8.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-16 19:56:58.000000 kfactory-0.8.2/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-16 19:56:58.000000 kfactory-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-16 19:56:58.000000 kfactory-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 19:56:58.000000 kfactory-0.8.2/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-16 19:56:58.000000 kfactory-0.8.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-16 19:56:58.000000 kfactory-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-16 19:56:58.000000 kfactory-0.8.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-16 19:57:19.391002 kfactory-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-16 19:56:58.000000 kfactory-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.371002 kfactory-0.8.2/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 19:56:58.000000 kfactory-0.8.2/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.371002 kfactory-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.371002 kfactory-0.8.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.375002 kfactory-0.8.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.375002 kfactory-0.8.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/gdsfactory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.375002 kfactory-0.8.2/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/pre.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-16 19:56:58.000000 kfactory-0.8.2/docs/source/waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.367002 kfactory-0.8.2/gds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.379002 kfactory-0.8.2/gds/gds_ref/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_circular.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A180_AS1.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A90_AS1.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T180_TS1.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T90_TS1.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_euler.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A180_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A90_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T180_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T90_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_s.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/bend_s_euler.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/straight_W500_L1000_LWG_EWGSTD.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/taper.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/waveguide.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-16 19:56:58.000000 kfactory-0.8.2/gds/gds_ref/waveguide_W500_L1000_LWG_EWGSTD.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-16 19:56:58.000000 kfactory-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 19:57:19.391002 kfactory-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.367002 kfactory-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.383002 kfactory-0.8.2/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.383002 kfactory-0.8.2/src/kfactory/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.383002 kfactory-0.8.2/src/kfactory/cells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/dbu/straight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/straight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/cells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113176 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/kcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.383002 kfactory-0.8.2/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.383002 kfactory-0.8.2/src/kfactory/technology/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/technology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/technology/layer_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.387002 kfactory-0.8.2/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55806 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/utils/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.387002 kfactory-0.8.2/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-06-16 19:56:58.000000 kfactory-0.8.2/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.383002 kfactory-0.8.2/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-16 19:57:19.000000 kfactory-0.8.2/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-16 19:57:19.000000 kfactory-0.8.2/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:57:19.000000 kfactory-0.8.2/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-16 19:57:19.000000 kfactory-0.8.2/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 19:57:19.000000 kfactory-0.8.2/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:57:19.391002 kfactory-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_netlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-16 19:56:58.000000 kfactory-0.8.2/tests/test_spiral.py
```

### Comparing `kfactory-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `kfactory-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `kfactory-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/.github/workflows/pages.yml` & `kfactory-0.8.2/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/.github/workflows/release.yml` & `kfactory-0.8.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/.github/workflows/test_code.yml` & `kfactory-0.8.2/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/.pre-commit-config.yaml` & `kfactory-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/CHANGELOG.md` & `kfactory-0.8.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 This project uses [*towncrier*](https://towncrier.readthedocs.io/) and the changes for the upcoming release can be found in <https://github.com/gdsfactory/kfactory/tree/main/changelog.d/>.
 
 <!-- towncrier release notes start -->
 
+## [0.8.2](https://github.com/gdsfactory/kfactory/tree/0.8.2) - 2023-06-16
+
+
+### Fixed
+
+- fix info settings
+
+
 ## [0.8.1](https://github.com/gdsfactory/kfactory/tree/0.8.1) - 2023-06-16
 
 
 ### Fixed
 
 - Make settings/infos in cells pydantic models and restrict types [#163](https://github.com/gdsfactory/kfactory/issues/163)
 - adjust minimum version of klayout to 0.28.post2
```

### Comparing `kfactory-0.8.1/LICENSE` & `kfactory-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/Makefile` & `kfactory-0.8.2/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/PKG-INFO` & `kfactory-0.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.8.1
+Version: 0.8.2
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.8.1
+# KFactory 0.8.2
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.1` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.2` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.8.1/README.md` & `kfactory-0.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# KFactory 0.8.1
+# KFactory 0.8.2
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.1` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.2` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.8.1/docs/mkdocs.yml` & `kfactory-0.8.2/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/_static/complex.png` & `kfactory-0.8.2/docs/source/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/_static/klive.webm` & `kfactory-0.8.2/docs/source/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/_static/waveguide.png` & `kfactory-0.8.2/docs/source/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/complex_cell.py` & `kfactory-0.8.2/docs/source/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/config.md` & `kfactory-0.8.2/docs/source/config.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/gdsfactory.md` & `kfactory-0.8.2/docs/source/gdsfactory.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/gen_ref_pages.py` & `kfactory-0.8.2/docs/source/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/intro.md` & `kfactory-0.8.2/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/notebooks/00_geometry.py` & `kfactory-0.8.2/docs/source/notebooks/00_geometry.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/notebooks/01_references.py` & `kfactory-0.8.2/docs/source/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/notebooks/02_DRC.py` & `kfactory-0.8.2/docs/source/notebooks/02_DRC.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/notebooks/03_Enclosures.py` & `kfactory-0.8.2/docs/source/notebooks/03_Enclosures.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/pre.md` & `kfactory-0.8.2/docs/source/pre.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/star.py` & `kfactory-0.8.2/docs/source/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/docs/source/waveguide.py` & `kfactory-0.8.2/docs/source/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_circular.gds` & `kfactory-0.8.2/gds/gds_ref/bend_circular.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A180_AS1.gds` & `kfactory-0.8.2/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A180_AS1.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A90_AS1.gds` & `kfactory-0.8.2/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A90_AS1.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T180_TS1.gds` & `kfactory-0.8.2/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T180_TS1.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T90_TS1.gds` & `kfactory-0.8.2/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T90_TS1.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_euler.gds` & `kfactory-0.8.2/gds/gds_ref/bend_euler.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A180_R150.gds` & `kfactory-0.8.2/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A180_R150.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A90_R150.gds` & `kfactory-0.8.2/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A90_R150.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T180_R150.gds` & `kfactory-0.8.2/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T180_R150.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T90_R150.gds` & `kfactory-0.8.2/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T90_R150.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_s.gds` & `kfactory-0.8.2/gds/gds_ref/bend_s.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/gds/gds_ref/bend_s_euler.gds` & `kfactory-0.8.2/gds/gds_ref/bend_s_euler.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/pyproject.toml` & `kfactory-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.8.1"
+version = "0.8.2"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.9.post2",
 	"scipy",
 	"ruamel.yaml",
@@ -232,15 +232,15 @@
 
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.8.1"
+current = "0.8.2"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `kfactory-0.8.1/src/kfactory/__init__.py` & `kfactory-0.8.2/src/kfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     dpolygon_from_array,
 )
 from . import cells, placer, routing, utils, port, pdk, technology
 from .conf import config
 
 # from .pdk import Pdk
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 logger = config.logger
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
```

### Comparing `kfactory-0.8.1/src/kfactory/cells/bezier.py` & `kfactory-0.8.2/src/kfactory/cells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/cells/circular.py` & `kfactory-0.8.2/src/kfactory/cells/circular.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/cells/dbu/straight.py` & `kfactory-0.8.2/src/kfactory/cells/dbu/straight.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     └──────────────────────────────┘
 
 The slabs and excludes can be given in the form of an
 [Enclosure][kfactory.utils.LayerEnclosure].
 """
 
 from ... import KCell, LayerEnum, cell, kdb
-from ...kcell import KCellInfo
+from ...kcell import Info
 from ...utils import LayerEnclosure
 
 __all__ = ["straight"]
 
 
 @cell
 def straight(
@@ -54,15 +54,15 @@
 
     c.shapes(layer).insert(kdb.Box(0, -width // 2, length, width // 2))
     c.create_port(trans=kdb.Trans(2, False, 0, 0), layer=layer, width=width)
     c.create_port(trans=kdb.Trans(0, False, length, 0), layer=layer, width=width)
 
     if enclosure is not None:
         enclosure.apply_minkowski_y(c, layer)
-    c.info = KCellInfo(
+    c.info = Info(
         **{
             "width_um": width * c.kcl.dbu,
             "length_um": length * c.kcl.dbu,
             "width_dbu": width,
             "length_dbu": length,
         }
     )
```

### Comparing `kfactory-0.8.1/src/kfactory/cells/dbu/taper.py` & `kfactory-0.8.2/src/kfactory/cells/dbu/taper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Taper definitions [dbu].
 
 TODO: Non-linear tapers
 """
 
 from ... import KCell, cell, kdb
-from ...kcell import KCellInfo
+from ...kcell import Info
 from ...utils import LayerEnclosure
 
 __all__ = ["taper"]
 
 
 @cell
 def taper(
@@ -54,15 +54,15 @@
     )
 
     c.create_port(trans=kdb.Trans(2, False, 0, 0), width=width1, layer=layer)
     c.create_port(trans=kdb.Trans(0, False, length, 0), width=width2, layer=layer)
 
     if enclosure is not None:
         enclosure.apply_minkowski_y(c, kdb.Region(c.bbox()))
-    c.info = KCellInfo(
+    c.info = Info(
         **{
             "width1_um": width1 * c.kcl.dbu,
             "width2_um": width2 * c.kcl.dbu,
             "length_um": length * c.kcl.dbu,
             "width1_dbu": width1,
             "width2_dbu": width2,
             "length_dbu": length,
```

### Comparing `kfactory-0.8.1/src/kfactory/cells/euler.py` & `kfactory-0.8.2/src/kfactory/cells/euler.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/cells/straight.py` & `kfactory-0.8.2/src/kfactory/cells/straight.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/cells/taper.py` & `kfactory-0.8.2/src/kfactory/cells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/conf.py` & `kfactory-0.8.2/src/kfactory/conf.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/kcell.py` & `kfactory-0.8.2/src/kfactory/kcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,57 @@
     | kdb.DCplxTrans
     | kdb.VCplxTrans
     | kdb.Vector
     | kdb.DVector
 )
 
 
+class KCellSettings(BaseModel):
+    class Config:
+        extra = "allow"
+        validate_assignment = True
+        frozen = True
+
+    @model_validator(mode="before")
+    def restrict_types(
+        cls, data: dict[str, Any]
+    ) -> dict[str, int | float | SerializableShape | str]:
+        for name, value in data.items():
+            if not isinstance(value, str | int | float | SerializableShape):
+                data[name] = str(value)
+        return data
+
+    def __getitem__(self, key: str) -> Any:
+        return getattr(self, key)
+
+
+class Info(BaseModel):
+    class Config:
+        extra = "allow"
+        validate_assignment = True
+
+    @model_validator(mode="before")
+    def restrict_types(
+        cls, data: dict[str, int | float | str]
+    ) -> dict[str, int | float | str]:
+        for name, value in data.items():
+            assert isinstance(value, str | int | float), (
+                "Values of the info dict only support int, float, or strings."
+                f"{name}: {value}, {type(value)}"
+            )
+
+        return data
+
+    def __getitem__(self, __key: str) -> Any:
+        return getattr(self, __key)
+
+    def __setitem__(self, __key: str, __val: str | int | float) -> None:
+        setattr(self, __key, __val)
+
+
 class PROPID(IntEnum):
     """Mapping for GDS properties."""
 
     NAME = 0
 
 
 class LockedError(AttributeError):
@@ -548,15 +591,15 @@
     yaml_tag = "!Port"
     name: str | None
     kcl: KCLayout
     width: int
     layer: int | LayerEnum
     _trans: kdb.Trans | None
     _dcplx_trans: kdb.DCplxTrans | None
-    info: dict[str, int | float | str]
+    info: Info = Info()
     port_type: str
     d: UMPort
 
     @overload
     def __init__(
         self,
         *,
@@ -634,15 +677,15 @@
         port: Port | None = None,
         kcl: KCLayout = kcl,
         info: dict[str, int | float | str] = {},
     ):
         """Create a port from dbu or um based units."""
         self.kcl = kcl
         self.d = UMPort(self)
-        self.info = info.copy()
+        self.info = Info(**info)
         if port is not None:
             self.name = port.name if name is None else name
 
             if port.dcplx_trans.is_complex():
                 self.dcplx_trans = port.dcplx_trans
             else:
                 self.trans = port.trans
@@ -699,48 +742,53 @@
 
         Args:
             trans: an optional transformation applied to the port to be copied
 
         Returns:
             port: a copy of the port
         """
+        info = self.info.model_dump()
+        for name, value in self.info:
+            info[name] = value
         if self._trans:
             if isinstance(trans, kdb.Trans):
                 _trans = trans * self.trans
                 return Port(
                     name=self.name,
                     trans=_trans,
                     layer=self.layer,
                     port_type=self.port_type,
                     width=self.width,
                     kcl=self.kcl,
+                    info=info,
                 )
             elif not trans.is_complex():
                 _trans = trans.s_trans().to_itype(self.kcl.dbu) * self.trans
                 return Port(
                     name=self.name,
                     trans=_trans,
                     layer=self.layer,
                     port_type=self.port_type,
                     width=self.width,
                     kcl=self.kcl,
+                    info=info,
                 )
         if isinstance(trans, kdb.Trans):
             dtrans = kdb.DCplxTrans(trans.to_dtype(self.kcl.dbu))
             _dtrans = dtrans * self.dcplx_trans
         else:
             _dtrans = trans * self.dcplx_trans
         return Port(
             name=self.name,
             dcplx_trans=_dtrans,
             dwidth=self.d.width,
             layer=self.layer,
             kcl=self.kcl,
             port_type=self.port_type,
-            info=self.info,
+            info=info,
         )
 
     @property
     def x(self) -> int:
         """X coordinate of the port in dbu."""
         return self.trans.disp.x
 
@@ -954,57 +1002,14 @@
         self.parent.width = int(value / self.parent.kcl.dbu)
         assert self.parent.width * self.parent.kcl.dbu == float(value), (
             "When converting to dbu the width does not match the desired width"
             f"({self.width} / {value})!"
         )
 
 
-class KCellSettings(BaseModel):
-    class Config:
-        extra = "allow"
-        validate_assignment = True
-        frozen = True
-
-    @model_validator(mode="before")
-    def restrict_types(
-        cls, data: dict[str, Any]
-    ) -> dict[str, int | float | SerializableShape | str]:
-        for name, value in data.items():
-            if not isinstance(value, str | int | float | SerializableShape):
-                data[name] = str(value)
-        return data
-
-    def __getitem__(self, key: str) -> Any:
-        return getattr(self, key)
-
-
-class KCellInfo(BaseModel):
-    class Config:
-        extra = "allow"
-        validate_assignment = True
-
-    @model_validator(mode="before")
-    def restrict_types(
-        cls, data: dict[str, int | float | str]
-    ) -> dict[str, int | float | str]:
-        for name, value in data.items():
-            assert isinstance(value, str | int | float), (
-                "Values of the info dict only support int, float, or strings."
-                f"{name}: {value}, {type(value)}"
-            )
-
-        return data
-
-    def __getitem__(self, __key: str) -> Any:
-        return getattr(self, __key)
-
-    def __setitem__(self, __key: str, __val: str | int | float) -> None:
-        setattr(self, __key, __val)
-
-
 class KCell:
     """KLayout cell and change its class to KCell.
 
     A KCell is a dynamic proxy for kdb.Cell. It has all the
     attributes of the official KLayout class. Some attributes have been adjusted
     to return KCell specific sub classes. If the function is listed here in the
     docs, they have been adjusted for KFactory specifically. This object will
@@ -1023,15 +1028,15 @@
         _locked: If set the cell shouldn't be modified anymore.
         ports: Manages the ports of the cell.
     """
 
     yaml_tag = "!KCell"
     _ports: Ports
     _settings: KCellSettings
-    _info: KCellInfo
+    _info: Info
     d: UMKCell
 
     def __init__(
         self,
         name: str | None = None,
         kcl: KCLayout = kcl,
         kdb_cell: kdb.Cell | None = None,
@@ -1047,15 +1052,15 @@
                 KLayout Cell
             ports: Attach an existing [Ports][kfactory.kcell.Ports] object to the KCell,
                 if `None` create an empty one.
         """
         self.kcl = kcl
         self.insts: Instances = Instances()
         self._settings: KCellSettings = KCellSettings()
-        self.info: KCellInfo = KCellInfo()
+        self.info: Info = Info()
         self._locked = False
         if name is None:
             _name = "Unnamed_!"
         else:
             _name = name
         self._kdb_cell = kdb_cell or kcl.create_cell(_name)
         if _name == "Unnamed_!":
@@ -1793,34 +1798,56 @@
                         f"kfactory:ports:{i}:dcplx_trans",
                         port._dcplx_trans.to_s(),
                         None,
                         True,
                     )
                 )
 
-        for name, setting in self.settings.model_dump().items():
+            info = port.info.model_dump()
+            for name, value in port.info:
+                info[name] = value
+
+            for name, value in info.items():
+                self.add_meta_info(
+                    kdb.LayoutMetaInfo(
+                        f"kfactory:ports:{i}:info:{name}",
+                        value,
+                        None,
+                        True,
+                    )
+                )
+
+        for name, setting in self.settings.model_copy().model_dump().items():
             self.add_meta_info(
                 kdb.LayoutMetaInfo(f"kfactory:settings:{name}", setting, None, True)
             )
         for name, info in self.info.model_dump().items():
             self.add_meta_info(
                 kdb.LayoutMetaInfo(f"kfactory:info:{name}", info, None, True)
             )
+        for name, info in self.info:
+            self.add_meta_info(
+                kdb.LayoutMetaInfo(f"kfactory:info:{name}", info, None, True)
+            )
 
     def get_meta_data(self) -> None:
         """Read metadata from the KLayout Layout object."""
-        port_dict = {}
+        port_dict: dict[str, Any] = {}
         settings = {}
         for meta in self.each_meta_info():
             if meta.name.startswith("kfactory:ports"):
-                i, _type = meta.name.removeprefix("kfactory:ports:").split(":")
+                i, _type = meta.name.removeprefix("kfactory:ports:").split(":", 1)
                 if i not in port_dict:
-                    port_dict[i] = {_type: meta.value}
-                else:
+                    port_dict[i] = {}
+                if not _type.startswith("info"):
                     port_dict[i][_type] = meta.value
+                else:
+                    if "info" not in port_dict[i]:
+                        port_dict[i]["info"] = {}
+                    port_dict[i]["info"][_type.removeprefix("info:")] = meta.value
             elif meta.name.startswith("kfactory:info"):
                 self.info[meta.name.removeprefix("kfactory:info:")] = meta.value
             elif meta.name.startswith("kfactory:settings"):
                 settings[meta.name.removeprefix("kfactory:settings:")] = meta.value
 
         self._settings = KCellSettings(**settings)
 
@@ -1837,14 +1864,15 @@
             _port = Port(
                 name=name,
                 width=width,
                 layer=layer,
                 trans=kdb.Trans.R0,
                 kcl=self.kcl,
                 port_type=port_type,
+                info=_d.get("info", {}),
             )
             if trans:
                 _port.trans = kdb.Trans.from_s(trans)
             elif dcplx_trans:
                 _port.dcplx_trans = kdb.DCplxTrans.from_s(dcplx_trans)
 
             self.add_port(_port, keep_mirror=True)
@@ -3111,14 +3139,18 @@
                 if set_name:
                     name = get_cell_name(f.__name__, **params)
                     cell.name = name
                 if set_settings:
                     settings = cell.settings.model_dump()
                     settings.update(params)
                     cell._settings = KCellSettings(**settings)
+                info = cell.info.model_dump()
+                for name, value in cell.info:
+                    info[name] = value
+                cell.info = Info(**info)
                 if check_instances:
                     if any(inst.is_complex() for inst in cell.each_inst()):
                         raise ValueError(
                             "Most foundries will not allow off-grid instances. Please "
                             "flatten them or add check_instances=False to the decorator"
                         )
                 if snap_ports:
```

### Comparing `kfactory-0.8.1/src/kfactory/pdk.py` & `kfactory-0.8.2/src/kfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/placer.py` & `kfactory-0.8.2/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/port.py` & `kfactory-0.8.2/src/kfactory/port.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/routing/electrical.py` & `kfactory-0.8.2/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/routing/manhattan.py` & `kfactory-0.8.2/src/kfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/routing/optical.py` & `kfactory-0.8.2/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/technology/layer_map.py` & `kfactory-0.8.2/src/kfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/typings.py` & `kfactory-0.8.2/src/kfactory/typings.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/utils/__init__.py` & `kfactory-0.8.2/src/kfactory/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/utils/enclosure.py` & `kfactory-0.8.2/src/kfactory/utils/enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/utils/fill.py` & `kfactory-0.8.2/src/kfactory/utils/fill.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/utils/simplify.py` & `kfactory-0.8.2/src/kfactory/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/utils/violations.py` & `kfactory-0.8.2/src/kfactory/utils/violations.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory/widgets/interactive.py` & `kfactory-0.8.2/src/kfactory/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.8.2/src/kfactory.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.8.1
+Version: 0.8.2
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.8.1
+# KFactory 0.8.2
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.1` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.2` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.8.1/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.8.2/src/kfactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/src/kfactory.egg-info/requires.txt` & `kfactory-0.8.2/src/kfactory.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/conftest.py` & `kfactory-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_cell.py` & `kfactory-0.8.2/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_cells.py` & `kfactory-0.8.2/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_cplxcells.py` & `kfactory-0.8.2/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_enclosure.py` & `kfactory-0.8.2/tests/test_enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_extrude.py` & `kfactory-0.8.2/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_meta.py` & `kfactory-0.8.2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_netlist.py` & `kfactory-0.8.2/tests/test_netlist.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_pdk.py` & `kfactory-0.8.2/tests/test_pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_ports.py` & `kfactory-0.8.2/tests/test_ports.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_rename.py` & `kfactory-0.8.2/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_routing.py` & `kfactory-0.8.2/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.8.1/tests/test_spiral.py` & `kfactory-0.8.2/tests/test_spiral.py`

 * *Files identical despite different names*

