# Comparing `tmp/uxarray-2023.5.0.dev0.tar.gz` & `tmp/uxarray-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxarray-2023.5.0.dev0.tar", last modified: Wed May 24 20:36:24 2023, max compression
+gzip compressed data, was "uxarray-2023.6.0.tar", last modified: Fri Jun 16 04:47:17 2023, max compression
```

## Comparing `uxarray-2023.5.0.dev0.tar` & `uxarray-2023.6.0.tar`

### file list

```diff
@@ -1,155 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/release_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/workflows/upstream-dev-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/ci/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/ci/upstream-dev-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/icons/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/icons/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/icons/science.svg
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/icons/tips.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/_static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (123)   348960 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/DOE_vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/EarthCube_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/NSF_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/PANGEO_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   241224 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/uxarray_temp_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/nsf.png
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/_static/thumbnails/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/thumbnails/default.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    30865 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples/000-template.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    61123 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples/001-read-grid-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples/002-access-grid-info.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples/003-area-calc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/gallery.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/internal_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/user_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/user_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/user_api/uxarray_api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/exodus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/exodus/mixed/
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/exodus/mixed/mixed.exo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/exodus/outCSne8/
--rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/exodus/outCSne8/outCSne8.g
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/mpas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/mpas/QU/
--rw-r--r--   0 runner    (1001) docker     (123)   178192 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/scrip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/scrip/outCSne8/
--rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/scrip/outCSne8/outCSne8.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/shp/
--rw-r--r--   0 runner    (1001) docker     (123)   162187 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/shp/grid_fire.shp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.724800 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    46371 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2510328 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1203548 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1203552 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50983 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.728800 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/
--rw-r--r--   0 runner    (1001) docker     (123)  1130591 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/grid.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v1.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v2.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v3.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.728800 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/
--rw-r--r--   0 runner    (1001) docker     (123)   181767 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30.ug
--rw-r--r--   0 runner    (1001) docker     (123)    49344 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc
--rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/
--rw-r--r--   0 runner    (1001) docker     (123)  2076807 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug
--rw-r--r--   0 runner    (1001) docker     (123)   518496 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/
--rw-r--r--   0 runner    (1001) docker     (123)    36983 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_exodus.py
--rw-r--r--   0 runner    (1001) docker     (123)    33115 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_mpas.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_scrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_ugrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/uxarray/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/uxarray/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/dataarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/uxarray/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_exodus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_mpas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_scrip.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_shapefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_ugrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/uxarray/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/utils/get_quadratureDG.py
--rw-r--r--   0 runner    (1001) docker     (123)    21470 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/uxarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.566514 uxarray-2023.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/ISSUE_TEMPLATE/release_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.github/workflows/upstream-dev-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-16 04:47:07.000000 uxarray-2023.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-16 04:47:07.000000 uxarray-2023.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-16 04:47:07.000000 uxarray-2023.6.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-16 04:47:07.000000 uxarray-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-16 04:47:17.566514 uxarray-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-16 04:47:07.000000 uxarray-2023.6.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-06-16 04:47:07.000000 uxarray-2023.6.0/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-16 04:47:07.000000 uxarray-2023.6.0/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 04:47:07.000000 uxarray-2023.6.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 04:47:07.000000 uxarray-2023.6.0/ci/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/icons/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/icons/science.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/icons/tips.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/_static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)   348960 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/logos/DOE_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/logos/EarthCube_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/logos/NSF_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/logos/PANGEO_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   241224 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/logos/uxarray_temp_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/images/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/_static/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_static/thumbnails/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/_templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/announcement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30865 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/examples/000-template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/examples/001-working-with-unstructured-grids.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/examples/002-grid-topology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/examples/003-area-calc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/gallery.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/getting-started/freq-asked-questions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/getting-started/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/getting-started/quick-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/internal_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/docs/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/user_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-06-16 04:47:07.000000 uxarray-2023.6.0/docs/user_api/uxarray_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 04:47:07.000000 uxarray-2023.6.0/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 04:47:07.000000 uxarray-2023.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:47:17.566514 uxarray-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-16 04:47:07.000000 uxarray-2023.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/test/meshfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/test/meshfiles/exodus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/test/meshfiles/exodus/mixed/
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/exodus/mixed/mixed.exo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.542513 uxarray-2023.6.0/test/meshfiles/exodus/outCSne8/
+-rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/exodus/outCSne8/outCSne8.g
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/test/meshfiles/mpas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.546513 uxarray-2023.6.0/test/meshfiles/mpas/QU/
+-rw-r--r--   0 runner    (1001) docker     (123)   178192 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/test/meshfiles/scrip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.546513 uxarray-2023.6.0/test/meshfiles/scrip/outCSne8/
+-rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/scrip/outCSne8/outCSne8.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.546513 uxarray-2023.6.0/test/meshfiles/shp/
+-rw-r--r--   0 runner    (1001) docker     (123)   162187 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/shp/grid_fire.shp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.538513 uxarray-2023.6.0/test/meshfiles/ugrid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.554513 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    46371 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2510328 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1203548 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1203552 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50983 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.558513 uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/
+-rw-r--r--   0 runner    (1001) docker     (123)  1130591 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/grid.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/v1.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/v2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/v3.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.558513 uxarray-2023.6.0/test/meshfiles/ugrid/outCSne30/
+-rw-r--r--   0 runner    (1001) docker     (123)   181767 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/outCSne30/outCSne30.ug
+-rw-r--r--   0 runner    (1001) docker     (123)    49344 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.562513 uxarray-2023.6.0/test/meshfiles/ugrid/outRLL1deg/
+-rw-r--r--   0 runner    (1001) docker     (123)  2076807 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug
+-rw-r--r--   0 runner    (1001) docker     (123)   518496 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.562513 uxarray-2023.6.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/
+-rw-r--r--   0 runner    (1001) docker     (123)    36983 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32989 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-16 04:47:07.000000 uxarray-2023.6.0/test/test_ugrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.562513 uxarray-2023.6.0/uxarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.562513 uxarray-2023.6.0/uxarray/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/core/dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37216 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/core/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.566514 uxarray-2023.6.0/uxarray/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/io/_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/io/_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/io/_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/io/_shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/io/_ugrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.566514 uxarray-2023.6.0/uxarray/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/utils/get_quadratureDG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21470 2023-06-16 04:47:07.000000 uxarray-2023.6.0/uxarray/utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:17.562513 uxarray-2023.6.0/uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-16 04:47:17.000000 uxarray-2023.6.0/uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-16 04:47:17.000000 uxarray-2023.6.0/uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:47:17.000000 uxarray-2023.6.0/uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:47:17.000000 uxarray-2023.6.0/uxarray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 04:47:17.000000 uxarray-2023.6.0/uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 04:47:17.000000 uxarray-2023.6.0/uxarray.egg-info/top_level.txt
```

### Comparing `uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/bug_report.md` & `uxarray-2023.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/feature_request.md` & `uxarray-2023.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/release_request.md` & `uxarray-2023.6.0/.github/ISSUE_TEMPLATE/release_request.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/.github/PULL_REQUEST_TEMPLATE.md` & `uxarray-2023.6.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,22 @@
       You may ignore this step if it is not applicable (comment out this section). -->
 ```Python
 import uxarray as ux
 
 grid_path = "/path/to/grid.nc"
 data_path = "/path/to/data.nc"
 
-uxgrid = ux.Grid(grid_path)
+uxds = ux.open_dataset(grid_path, data_path)
 
 # this is how you use this function
-some_output = uxgrid.some_function()
+some_output = uxds.some_function()
 
 # this is another way to use this function
-other_output = uxgrid.some_function(some_param = True)
+other_output = uxds.some_function(some_param = True)
+
 ```
 
 ## PR Checklist
 <!-- Please mark any checkboxes that do not apply to this PR as [N/A]. If an entire section doesn't
 apply to this PR, comment it out or delete it. -->
 
 **General**
```

### Comparing `uxarray-2023.5.0.dev0/.github/workflows/ci.yml` & `uxarray-2023.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/.github/workflows/pypi.yaml` & `uxarray-2023.6.0/.github/workflows/pypi.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 jobs:
   test-build:
     if: github.repository == 'UXARRAY/uxarray'
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v4.6.0
+        uses: actions/setup-python@v4.6.1
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools setuptools-scm wheel twine check-manifest
       - name: Build tarball and wheels
@@ -28,15 +28,15 @@
   publish:
     needs: test-build
     if: startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v4.6.0
+        uses: actions/setup-python@v4.6.1
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools setuptools-scm wheel twine check-manifest
       - name: Build tarball and wheels
```

### Comparing `uxarray-2023.5.0.dev0/.github/workflows/upstream-dev-ci.yml` & `uxarray-2023.6.0/.github/workflows/upstream-dev-ci.yml`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/.gitignore` & `uxarray-2023.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/.pre-commit-config.yaml` & `uxarray-2023.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/LICENSE` & `uxarray-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/PKG-INFO` & `uxarray-2023.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2023.5.0.dev0
+Version: 2023.6.0
 Summary: Unstructured grid model reading and recognizing with xarray.
 Home-page: https://github.com/UXARRAY/uxarray
 Maintainer: UXARRAY
 Maintainer-email: 
 Project-URL: Source, https://github.com/UXARRAY/uxarray
 Project-URL: Tracker, https://github.com/UXARRAY/uxarray/issues
 Classifier: Operating System :: OS Independent
@@ -26,36 +26,36 @@
 | **License**  |                                                                        [![License][license-badge]][repo-link]                |
 | **Citing**   |                                                                              [![DOI][doi-badge]][doi-link]                   |
 
 
 
 UXarray aims to address the geoscience community need for tools that enable
 standard data analysis techniques to operate directly on unstructured grid
-data. UXarray will provide Xarray styled functions to better read in and use
+data. UXarray provides Xarray styled functions to better read in and use
 unstructured grid datasets that follow standard conventions, including UGRID,
-SCRIP, Exodus and shapefile formats.  This effort is a result of the
+MPAS, SCRIP, and Exodus formats.  This effort is a result of the
 collaboration between Project Raijin (NCAR and Pennsylvania State University)
 and the SEATS Project (Argonne National Laboratory, UC Davis, and Lawrence
 Livermore National Laboratory). The UXarray team welcomes other community
 members to become part of this collaboration at any level of contribution.
 
 UXarray is implemented in pure Python and does not explicitly contain or require
 any compiled code. This makes UXarray more accessible to the general Python
 community. Any contributions to this repository in pure Python are welcome and
 documentation for contribution guidelines can be found when clicking `New Issue`
 under the `Issues` tab in the UXarray repository.
 
 # Why is the name "UXarray"?
 
 We have created UXarray based on [Xarray](https://docs.xarray.dev/en/stable/)
-(via composition of a Xarray dataset object), a Pangeo ecosystem package
+(via inheritance of Xarray Dataset and DataArray classes), a Pangeo ecosystem package
 commonly-used for structured grids recognition, to support reading and
 recognizing unstructured grid model outputs. We picked the name "UXarray"
-and preferred to capitalize the first two letters to emphasize it is Xarray
-for Unstructured grids.
+(pronounced "you-ex-array") and preferred to capitalize the first two letters to
+emphasize it builds upon Xarray for Unstructured grids.
 
 # UXarray Functionality
 
 The following intended functionality has been inspired by discussions with
 members of the scientific community, within the SEATS Project and Project
 Raijin, and on several community platforms such as [Xarray GitHub
 Repository](https://github.com/pydata/xarray/issues/4222). The UXarray team
```

### Comparing `uxarray-2023.5.0.dev0/README.md` & `uxarray-2023.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 | **License**  |                                                                        [![License][license-badge]][repo-link]                |
 | **Citing**   |                                                                              [![DOI][doi-badge]][doi-link]                   |
 
 
 
 UXarray aims to address the geoscience community need for tools that enable
 standard data analysis techniques to operate directly on unstructured grid
-data. UXarray will provide Xarray styled functions to better read in and use
+data. UXarray provides Xarray styled functions to better read in and use
 unstructured grid datasets that follow standard conventions, including UGRID,
-SCRIP, Exodus and shapefile formats.  This effort is a result of the
+MPAS, SCRIP, and Exodus formats.  This effort is a result of the
 collaboration between Project Raijin (NCAR and Pennsylvania State University)
 and the SEATS Project (Argonne National Laboratory, UC Davis, and Lawrence
 Livermore National Laboratory). The UXarray team welcomes other community
 members to become part of this collaboration at any level of contribution.
 
 UXarray is implemented in pure Python and does not explicitly contain or require
 any compiled code. This makes UXarray more accessible to the general Python
 community. Any contributions to this repository in pure Python are welcome and
 documentation for contribution guidelines can be found when clicking `New Issue`
 under the `Issues` tab in the UXarray repository.
 
 # Why is the name "UXarray"?
 
 We have created UXarray based on [Xarray](https://docs.xarray.dev/en/stable/)
-(via composition of a Xarray dataset object), a Pangeo ecosystem package
+(via inheritance of Xarray Dataset and DataArray classes), a Pangeo ecosystem package
 commonly-used for structured grids recognition, to support reading and
 recognizing unstructured grid model outputs. We picked the name "UXarray"
-and preferred to capitalize the first two letters to emphasize it is Xarray
-for Unstructured grids.
+(pronounced "you-ex-array") and preferred to capitalize the first two letters to
+emphasize it builds upon Xarray for Unstructured grids.
 
 # UXarray Functionality
 
 The following intended functionality has been inspired by discussions with
 members of the scientific community, within the SEATS Project and Project
 Raijin, and on several community platforms such as [Xarray GitHub
 Repository](https://github.com/pydata/xarray/issues/4222). The UXarray team
```

### Comparing `uxarray-2023.5.0.dev0/docs/Makefile` & `uxarray-2023.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/images/icons/code.svg` & `uxarray-2023.6.0/docs/_static/images/icons/code.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/images/icons/tips.svg` & `uxarray-2023.6.0/docs/_static/images/icons/tips.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/images/logos/DOE_vertical.png` & `uxarray-2023.6.0/docs/_static/images/logos/DOE_vertical.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/images/logos/EarthCube_logo.png` & `uxarray-2023.6.0/docs/_static/images/logos/EarthCube_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/images/logos/NSF_logo.png` & `uxarray-2023.6.0/docs/_static/images/logos/NSF_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/images/logos/PANGEO_logo.png` & `uxarray-2023.6.0/docs/_static/images/logos/PANGEO_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/images/logos/uxarray_temp_logo.png` & `uxarray-2023.6.0/docs/_static/images/logos/uxarray_temp_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/images/nsf.png` & `uxarray-2023.6.0/docs/_static/images/nsf.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/_static/thumbnails/default.svg` & `uxarray-2023.6.0/docs/_static/thumbnails/default.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/conf.py` & `uxarray-2023.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/contributing.rst` & `uxarray-2023.6.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/examples/000-template.ipynb` & `uxarray-2023.6.0/docs/examples/000-template.ipynb`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/examples/002-access-grid-info.ipynb` & `uxarray-2023.6.0/docs/examples/001-working-with-unstructured-grids.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8796188640793904%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '## Grid Definition and Data Variables\\n'), (2, 'When "*

 * *            "working with Unstructured Grids, the grid definition and data variables\\n'), (3, "*

 * *            "'are often stored as separate files. This means that there are multiple\\n'), (4, "*

 * *            "'separate files that need to be read and linked together to represent the\\n'), (5, "*

 * *            "'entire dataset.\\n'), (7, 'For example, the following sample dataset is taken from "*

 * *            "the NOAA […]*

```diff
@@ -1,271 +1,368 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Accessing Grid Information\n",
+                "# Working with Unstructured Grid Data\n",
                 "\n",
-                "Unstructured grids can be represented in one of many different conventions\n",
-                "(UGRID, SCRIP, EXODUS, etc). These conventions have different definitions\n",
-                "and representations of the attributes and variables used to describe\n",
-                "the unstructured grid topology. Even more, the [UGRID conventions](\n",
-                "https://ugrid-conventions.github.io/ugrid-conventions/) does not\n",
-                "enforce standard variable namings for most of the attributes and variables\n",
-                "(other than just a few required ones).\n",
-                "\n",
-                "UXarray unifies all of these conventions at the data loading step by\n",
-                "representing grids in the UGRID convention regardless of the original grid\n",
-                "type that is read in from the file. Furthermore, it uses a set of\n",
-                "standardized names for topology attributes and variables, while still\n",
-                "providing the user with the original attribute names and variables that\n",
-                "came from the grid definition file.\n",
-                "\n",
-                "## Overview\n",
+                "UXarray offers support for loading and representing unstructured grids\n",
+                "by providing Xarray-like functionality paired with new routines that\n",
+                "are specifically written for operating on unstructured grids.\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Grid Definition and Data Variables\n",
                 "\n",
-                "This notebook will showcase the different methods available for accessing\n",
-                "the grid topology attributes and variables stored in the `UXarray.Grid`\n",
-                "object.\n",
+                "When working with Unstructured Grids, the grid definition and data variables\n",
+                "are often stored as separate files. This means that there are multiple\n",
+                "separate files that need to be read and linked together to represent the\n",
+                "entire dataset.\n",
+                "\n",
+                "For example, the following sample dataset is taken from the NOAA Geoflow project,\n",
+                "which is made up of 4 files: 1 grid definition and 3 data files. (Special thanks to John Clyne, Shilpi Gupta, and the VAPOR team for providing this data!)\n",
+                "\n",
+                "```\n",
+                "geoflow-small\n",
+                "\u2502   grid.nc\n",
+                "\u2502   v1.nc\n",
+                "\u2502   v2.nc\n",
+                "\u2502   v3.nc\n",
+                "```\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Grid Conventions\n",
                 "\n",
-                "For more details on how to load in data, check out our [previous usage\n",
-                "example](https://uxarray.readthedocs.io/en/latest/examples/read-grid-data.html)\n",
+                "Given the complexity of Unstructured Grids, there are many different ways of representing their underlying topology and structure. These representations are referred to as conventions, and they outline\n",
+                "the required connectivity variables, naming conventions, data types, and many other specifications. UXarray uses the [UGRID](http://ugrid-conventions.github.io/ugrid-conventions/)\n",
+                "conventions as a foundation for internally representing Unstructured Grids, converting any supported input grid format into the UGRID convention at the data loading step. Below is a list of supported formats and conventions that can be read in with UXarray:\n",
+                "* UGRID\n",
+                "* Model for Prediction Across Scales (MPAS)\n",
+                "* Exodus\n",
                 "\n",
-                "**Methods**\n",
-                "1. Indexing with Original Variable Names\n",
-                "2. Indexing with UXarray Variable Dictionary\n",
-                "3. UXarray's Standardized UGRID Names (Most convenient)"
+                "In addition to loading datasets, we also provide support for constructing a grid from user-defined primitives such as vertices, which is showcased in our other notebooks.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Data\n",
+                "## Reading Grid and Data Files\n",
+                "UXarray provides the `UxDataset` data structure, which is an unstructure grid-informed implementation of Xarray's `Dataset` class. The main addition is the introduction of the `uxgrid` property, which stores our grid topology dimensions, coordinates, variables and provides grid-specific functions.\n",
                 "\n",
-                "We will be using two grid files, both of which are in the UGRID convention.\n",
-                "However, the key difference between them is the names used to describe the\n",
-                "attributes and variables.\n",
-                "\n",
-                "Let us first read in the data:"
+                "Constructing a `UxDataset` can be done using our custom `open_dataset` and `open_mfdataset` methods, depending on whether one or multiple data files or objects are meant to be linked to a single grid.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {
-                "collapsed": false,
-                "jupyter": {
-                    "outputs_hidden": false
-                }
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import uxarray as ux\n",
-                "import xarray as xr"
+                "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {
-                "collapsed": false,
-                "jupyter": {
-                    "outputs_hidden": false
-                }
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "# Base data path\n",
-                "base_path = \"../../test/meshfiles/\"\n",
+                "base_path = \"../../test/meshfiles/ugrid/geoflow-small/\"\n",
                 "\n",
-                "# Path to Grid files\n",
-                "ugrid_01_path = base_path + \"/ugrid/outCSne30/outCSne30.ug\"\n",
-                "ugrid_02_path = base_path + \"/ugrid/geoflow-small/grid.nc\"\n",
+                "# Path to Grid file\n",
+                "grid_path = base_path + \"grid.nc\"\n",
                 "\n",
-                "# Load grid files and create UXarray Grid objects\n",
-                "ugrid_01_ds = xr.open_dataset(ugrid_01_path)\n",
-                "ugrid_02_ds = xr.open_dataset(ugrid_02_path)\n",
+                "# Paths to Data Variable files\n",
+                "var_names = ['v1.nc', 'v2.nc', 'v3.nc']\n",
                 "\n",
-                "ugrid_01 = ux.Grid(ugrid_01_ds)\n",
-                "ugrid_02 = ux.Grid(ugrid_02_ds)"
+                "data_paths = [base_path + name for name in var_names]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The output of the bottom cell showcases the slight differences\n",
-                "in variable names:"
+                "Loading a single data file with a grid is done using the `open_dataset` method. The resulting `UxDataset` only contains the data variables stored in `v1.nc`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\n",
-                        "Variable Names\n",
-                        "ugrid_01 variable names: ['Mesh2', 'Mesh2_face_nodes', 'Mesh2_node_x', 'Mesh2_node_y', 'nMesh2_face', 'nMaxMesh2_face_nodes', 'nMesh2_node']\n",
-                        "ugrid_02 variable names: ['mesh', 'mesh_face_nodes', 'mesh_depth', 'mesh_node_x', 'mesh_node_y', 'nMeshFaces', 'nFaceNodes', 'nMeshNodes', 'meshLayers']\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "# Extract variable names\n",
-                "ugrid_01_names = list(ugrid_01.ds.keys()) + \\\n",
-                "                 list(ugrid_01.ds.coords) + \\\n",
-                "                 list(ugrid_01.ds.dims)\n",
-                "ugrid_02_names = list(ugrid_02.ds.keys()) + \\\n",
-                "                 list(ugrid_02.ds.coords) + \\\n",
-                "                 list(ugrid_02.ds.dims)\n",
-                "\n",
-                "print(\"\\nAttribute and variable names for each grid:\")\n",
-                "print(\"ugrid_01 variable names:\", ugrid_01_names)\n",
-                "print(\"ugrid_02 variable names:\", ugrid_02_names)"
+                "uxds_single = ux.open_dataset(grid_path, data_paths[0])\n",
+                "uxds_single"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 1. Indexing with Original Variable Names\n",
-                "\n",
-                "The simplest approach is to use the original variable name as an index\n",
-                "into the grid dataset, `Grid.ds`. Since `ugrid_01` and `ugrid_02` have\n",
-                "different names for most of their topology attributes and variables, the\n",
-                "index for accessing them will be different for both grids."
+                "Similarly, if you wish to open multiple data files with a grid, you would use the `open_mfdataset` method. The resulting `UxDataset` contains all the data variables stored in `v1.nc`, `v2.nc`, and `v3.nc`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
-                "x_1 = ugrid_01.ds['Mesh2_node_x']\n",
-                "y_1 = ugrid_01.ds['Mesh2_node_y']\n",
-                "face_nodes_1 = ugrid_01.ds['Mesh2_face_nodes']\n",
-                "n_face_nodes_1 = ugrid_01.ds['nMaxMesh2_face_nodes']\n",
-                "\n",
-                "x_2 = ugrid_02.ds['mesh_node_x']\n",
-                "y_2 = ugrid_02.ds['mesh_node_y']\n",
-                "face_nodes_2 = ugrid_02.ds['mesh_face_nodes']\n",
-                "n_face_nodes_2 = ugrid_02.ds['nFaceNodes']"
+                "uxds_multiple = ux.open_mfdataset(grid_path, data_paths)\n",
+                "uxds_multiple"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "## Grid Topology"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 2. Indexing with UXarray Variable Dictionary\n",
+                "Each dataset contains the aforementioned `uxgrid` property, which is a `Grid` object and represents the grid topology that the data variables lie on. The `uxgrid` property can be used to execute grid specific functions and access grid topology dimensions, coordinates, and variables. A detailed overview of functionalities can be found in subsequent notebooks.\n",
                 "\n",
-                "UXarray provides a dictionary, `Grid.grid_var_names`, to map the original\n",
-                "topology attribute and variable names that come from the grid file into\n",
-                "a standardized set of names. In other words, the dictionary uses a\n",
-                "standardized set of UGRID attribute and variable names as keys, and the\n",
-                "original variable names that come from the grid file as values.\n",
-                "\n",
-                "This allows us to use the same index into either dataset. However, this\n",
-                "makes the indexing code much longer than the previous method."
+                "For both instances of `UxDataset` that contain single and multiple data sets (i.e. `uxds_single` and `uxds_multiple`), the `uxgrid` property contains the same grid information, however they are each instantiated separately.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
-                "var_names_dict = ugrid_01.grid_var_names\n",
-                "x_1 = ugrid_01.ds[var_names_dict['Mesh2_node_x']]\n",
-                "y_1 = ugrid_01.ds[var_names_dict['Mesh2_node_y']]\n",
-                "face_nodes_1 = ugrid_01.ds[var_names_dict['Mesh2_face_nodes']]\n",
-                "n_face_nodes_1 = ugrid_01.ds[var_names_dict['nMesh2_node']]\n",
+                "# check if the grids contain the same variables & information\n",
+                "print(uxds_single.uxgrid == uxds_multiple.uxgrid)\n",
                 "\n",
-                "var_names_dict = ugrid_02.grid_var_names\n",
-                "x_2 = ugrid_02.ds[var_names_dict['Mesh2_node_x']]\n",
-                "y_2 = ugrid_02.ds[var_names_dict['Mesh2_node_y']]\n",
-                "face_nodes_2 = ugrid_02.ds[var_names_dict['Mesh2_face_nodes']]\n",
-                "n_face_nodes_2 = ugrid_02.ds[var_names_dict['nMesh2_node']]"
+                "# check if the grids point to the same object in memory\n",
+                "print(uxds_single.uxgrid is uxds_multiple.uxgrid)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Please note, for instance, we accessed the actual variable `mesh_node_x`\n",
-                "of `ugrid_02` via indexing the dictionary with the standardized name\n",
-                "`Mesh2_node_x`, likewise in `ugrid_01`."
+                "Printing out the `uxgrid` property provides an overview of the original grid format, dimensions, coordinates, and connectivity variables."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
+            },
+            "outputs": [],
+            "source": [
+                "uxds_multiple.uxgrid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 3. UXarray's Standardized UGRID Names\n",
-                "The last way of accessing grid topology attributes and variables is to use\n",
-                "the standardized UGRID namings provided by UXarray. This method still\n",
-                "utilizes the dictionary, `grid_var_names`, under the hood to return a\n",
-                "reference to the variable or attribute that is stored withing\n",
-                "`UXarray.Grid.ds`.\n",
-                "\n",
-                "This eliminates the need to remember the original variable names and\n",
-                "needing to index through the `grid_var_names` dictionary. Because of this,\n",
-                "we find this as the most convenient approach."
+                "These dimensions, coordinates, and connectivity variables can be accessed with attributes using the same names as shown in the print-out. Below are a few examples."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
-                "x_1 = ugrid_01.Mesh2_node_x\n",
-                "y_1 = ugrid_01.Mesh2_node_y\n",
-                "face_nodes_1 = ugrid_01.Mesh2_face_nodes\n",
-                "n_face_nodes_1 = ugrid_01.nMesh2_node\n",
-                "\n",
-                "x_2 = ugrid_02.Mesh2_node_x\n",
-                "y_2 = ugrid_02.Mesh2_node_y\n",
-                "face_nodes_2 = ugrid_02.Mesh2_face_nodes\n",
-                "n_face_nodes_2 = ugrid_02.nMesh2_node"
+                "uxds_multiple.uxgrid.nMesh2_node"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
+            },
+            "outputs": [],
+            "source": [
+                "uxds_multiple.uxgrid.Mesh2_node_x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
+            },
+            "outputs": [],
+            "source": [
+                "uxds_multiple.uxgrid.Mesh2_face_nodes"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "collapsed": false
+            },
             "source": [
-                "In conclusion, there are three ways of accessing the grid attributes and\n",
-                "variables. Even though the UXarray developers recommend using the\n",
-                "standardized UGRID names method, users can find each various pros/cons with\n",
-                "each of these access ways."
+                "## Data Variables"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "While grid-specific variables and functions are stored under the `uxgrid` property, data variables that lie on the grid are stored directly in the `UxDataset` or `UxDataArray`. Most `Xarray` functions and operators can be executed on these data structures.\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "uxds_single.values"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "uxds_single.dims"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "uxds_single.coords"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "uxds_single.attrs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "uxds_single.min()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "uxds_single > 0"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "grid = uxds_single.uxgrid\n",
+                "foo = ux.UxDataArray(\n",
+                "    data = np.random.random(grid.nMesh2_face),\n",
+                "    dims = [\"nMesh2_face\"],\n",
+                "    uxgrid = grid\n",
+                ")\n",
+                "foo"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "uxds_new_var = uxds_single.assign({\"foo\" : foo})"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "uxds_new_var"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -278,12 +375,17 @@
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.10"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "8e8ae2f388051fced6c30f82a529eeca8cf1e059ab06a64326e2a2ad0ec3c36c"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `uxarray-2023.5.0.dev0/docs/examples/003-area-calc.ipynb` & `uxarray-2023.6.0/docs/examples/003-area-calc.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.833415404040404%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}, delete: ['attachments']}, 1: {'metadata': "*

 * *            "{replace: OrderedDict()}, delete: ['attachments']}, 2: {'execution_count': 1, "*

 * *            "'metadata': {'ExecuteTime': {'end_time': '2023-06-09T10:04:28.775400Z', 'start_time': "*

 * *            "'2023-06-09T10:04:28.705400Z'}, 'jupyter': OrderedDict([('outputs_hidden', "*

 * *            "False)])}}, 3: {'execution_count': 2, 'metadata': {'ExecuteTime': {'end_time': "*

 * *            "'2023-06-09T10:04:28. […]*

```diff
@@ -1,15 +1,12 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "# Face Area Calculations\n",
                 "\n",
                 "## Overview\n",
                 "\n",
                 "This notebook will showcase the different area calculation options provided by `uxarray`\n",
                 "\n",
@@ -21,98 +18,131 @@
                 "3. Getting Area of Individual Faces\n",
                 "4. Calculate Area of a Single Triangle in Cartesian Coordinates\n",
                 "5. Calculate Area from Multiple Faces in Spherical Coordinates\n",
                 "6. Area Calculation without Grid Object\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We will be using the `outCSne30.ug` grid file, which is encoded in the UGRID convention."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:02.171354Z",
-                    "start_time": "2023-04-19T09:57:02.144399Z"
+                    "end_time": "2023-06-09T10:04:28.775400Z",
+                    "start_time": "2023-06-09T10:04:28.705400Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "import uxarray as ux\n",
                 "import numpy as np\n",
                 "import xarray as xr"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:02.172124Z",
-                    "start_time": "2023-04-19T09:57:02.148439Z"
+                    "end_time": "2023-06-09T10:04:28.817401Z",
+                    "start_time": "2023-06-09T10:04:28.718401Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<uxarray.Grid>\n",
+                            "Original Grid Type: ugrid\n",
+                            "Grid Dimensions:\n",
+                            "  * nMesh2_face: 5400\n",
+                            "  * nMaxMesh2_face_nodes: 4\n",
+                            "  * nMesh2_node: 5402\n",
+                            "Grid Coordinate Variables:\n",
+                            "  * Mesh2_node_x: (5402,)\n",
+                            "  * Mesh2_node_y: (5402,)\n",
+                            "Grid Connectivity Variables:\n",
+                            "  * Mesh2_face_nodes: (5400, 4)\n",
+                            "  * nNodes_per_face: (5400,)"
+                        ]
+                    },
+                    "execution_count": 2,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "# Base data path\n",
                 "base_path = \"../../test/meshfiles/\"\n",
                 "\n",
                 "# Path to Grid files\n",
                 "ugrid_path = base_path + \"/ugrid/outCSne30/outCSne30.ug\"\n",
                 "\n",
                 "# Load grid files and create UXarray Grid objects\n",
                 "ugrid_ds = xr.open_dataset(ugrid_path)\n",
                 "\n",
                 "ugrid = ux.Grid(ugrid_ds)\n",
-                "ugrid.ds"
+                "ugrid"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## 1. Calculate Total Face Area\n",
-                "We can calculate the total face area by calling the function `Grid.calculate_total_face_area()`. Since our dataset lies on the unit sphere, our expected area is 4pi, which is approximatly 12.56"
+                "We can calculate the total face area by calling the function `Grid.calculate_total_face_area()`. Since our dataset lies on the unit sphere, our expected area is 4*pi, which is approximately 12.56"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.685968Z",
-                    "start_time": "2023-04-19T09:57:02.154548Z"
+                    "end_time": "2023-06-09T10:04:28.820400Z",
+                    "start_time": "2023-06-09T10:04:28.732401Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "12.566370614678554"
+                        ]
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "t4_area = ugrid.calculate_total_face_area()\n",
                 "t4_area"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## 2. Options for `Grid.calculate_total_face_area` Function\n",
                 "\n",
                 "By default, `Grid.calculate_total_face_area` uses a Triangular Quadrature Rule and an Order of 4. However, you can specify the Quadrature Rule and Order as follows:\n",
                 "\n",
                 "\n",
                 "**Order:**\n",
@@ -120,236 +150,329 @@
                 "       1 to 10              for gaussian\n",
                 "\n",
                 "       1, 4, 8, 10 and 12   for triangular\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.690062Z",
-                    "start_time": "2023-04-19T09:57:03.687612Z"
+                    "end_time": "2023-06-09T10:04:28.821401Z",
+                    "start_time": "2023-06-09T10:04:28.777401Z"
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "12.571403993719983"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "t1_area = ugrid.calculate_total_face_area(quadrature_rule=\"triangular\", order=1)\n",
                 "t1_area"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For the result above, notice that the area is slightly different than the first calculation we made.\n",
                 "\n",
                 "Now we use Triangular Quadrature Rule and Order 1\n",
                 "\n",
                 "Using a lower order is faster, but at the sacrifice of accuracy.\n",
                 "\n",
                 "Generally, gaussian quadrature rule is more accurate than the triangular quadrature rule. Additionally, a higher order comes at the cost of computation time, but produces a more accurate result. See `uxarray/get_quadratureDG.py` file for details on quadrature points and weights."
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## 3. Getting Area of Individual Faces\n",
                 "\n",
                 "We can access the Grid attribute `Grid.face_area` to access the individual face areas. If you have not run a face area calculation yet, it will run the `Grid.compute_face_areas` and cache the value.\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 5,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.693036Z",
-                    "start_time": "2023-04-19T09:57:03.690838Z"
+                    "end_time": "2023-06-09T10:04:28.827402Z",
+                    "start_time": "2023-06-09T10:04:28.810401Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([0.00211238, 0.00211285, 0.00210788, ..., 0.00210788, 0.00211285,\n",
+                            "       0.00211238])"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "ugrid.face_areas"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Now calculate the area again with the `Grid.compute_face_areas` function using arguments: quadrature_rule \"gaussian\" and order 4"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 6,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.696254Z",
-                    "start_time": "2023-04-19T09:57:03.693676Z"
+                    "end_time": "2023-06-09T10:04:28.904401Z",
+                    "start_time": "2023-06-09T10:04:28.896401Z"
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "12.566370614359112"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "all_face_areas = ugrid.compute_face_areas(quadrature_rule=\"gaussian\", order=4)\n",
                 "g4_area = all_face_areas.sum()\n",
                 "g4_area"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we compare the values with actual know value and report error for each of the three cases above."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
+            "execution_count": 7,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2023-06-09T10:04:28.950400Z",
+                    "start_time": "2023-06-09T10:04:28.904401Z"
+                }
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "(0.005033379360810386, 3.1938185429680743e-10, 6.039613253960852e-14)"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "actual_area = 4 * np.pi\n",
                 "diff_t4_area = np.abs(t4_area - actual_area)\n",
                 "diff_t1_area = np.abs(t1_area - actual_area)\n",
                 "diff_g4_area = np.abs(g4_area - actual_area)\n",
                 "\n",
                 "diff_t1_area, diff_t4_area, diff_g4_area"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "As we can see, it is clear that the Gaussian Quadrature Rule with Order 4 is the most accurate, and the Triangular Quadrature Rule with Order 1 is the least accurate.\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## 4. Calculate Area of a Single Triangle in Cartesian Coordinates\n",
                 "\n",
                 "For this section, we create a single triangle face with 3 vertices. By default, in `uxarray`, we assume that the coordinate system is spherical (lat / lon), however if you want to use cartesian coordinates, you must pass through `islatlon = False` into the `Grid` constructor.\n",
                 "\n",
                 "Assume the units in meters - this is a big triangle!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 8,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.703400Z",
-                    "start_time": "2023-04-19T09:57:03.696048Z"
+                    "end_time": "2023-06-09T10:04:28.958400Z",
+                    "start_time": "2023-06-09T10:04:28.921401Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<uxarray.Grid>\n",
+                            "Original Grid Type: From vertices\n",
+                            "Grid Dimensions:\n",
+                            "  * nMesh2_node: 3\n",
+                            "  * nMesh2_face: 1\n",
+                            "  * nMaxMesh2_face_nodes: 3\n",
+                            "Grid Coordinate Variables:\n",
+                            "  * Mesh2_node_x: (3,)\n",
+                            "  * Mesh2_node_y: (3,)\n",
+                            "Grid Connectivity Variables:\n",
+                            "  * Mesh2_face_nodes: (1, 3)\n",
+                            "  * nNodes_per_face: (1,)"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "verts = [[[0.57735027, -5.77350269e-01, -0.57735027],\n",
                 "         [0.57735027, 5.77350269e-01, -0.57735027],\n",
                 "         [-0.57735027, 5.77350269e-01, -0.57735027]]]\n",
                 "\n",
                 "# load our vertices into a UXarray Grid object\n",
                 "vgrid = ux.Grid(verts,\n",
                 "                vertices=True,\n",
                 "                islatlon=False,\n",
                 "                concave=False)\n",
                 "\n",
-                "vgrid.ds"
+                "vgrid"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 9,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.705404Z",
-                    "start_time": "2023-04-19T09:57:03.703896Z"
+                    "end_time": "2023-06-09T10:04:28.967401Z",
+                    "start_time": "2023-06-09T10:04:28.951402Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "1.0719419938548207"
+                        ]
+                    },
+                    "execution_count": 9,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "vgrid.calculate_total_face_area()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Additionally, if you are using a unit other than meters, you can update the units as follows"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 10,
             "metadata": {
-                "collapsed": false
+                "ExecuteTime": {
+                    "end_time": "2023-06-09T10:04:29.014400Z",
+                    "start_time": "2023-06-09T10:04:28.967401Z"
+                },
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "1.0475702709086985"
+                        ]
+                    },
+                    "execution_count": 10,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "# Set correct units for the x and y coordinates\n",
                 "vgrid.Mesh2_node_x.attrs[\"units\"] = \"km\"\n",
                 "vgrid.Mesh2_node_y.attrs[\"units\"] = \"km\"\n",
-                "vgrid.Mesh2_node_z.attrs[\"units\"] = \"km\"\n",
+                "vgrid._Mesh2_node_z.attrs[\"units\"] = \"km\"  # This is just a placeholder, UXarray does not support 3D meshes \n",
                 "\n",
                 "# Calculate the area of the triangle\n",
                 "area_gaussian = vgrid.calculate_total_face_area(\n",
                 "            quadrature_rule=\"gaussian\", order=5)\n",
                 "area_gaussian"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": []
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## 5. Calculate Area from Multiple Faces in Spherical Coordinates\n",
                 "\n",
                 "Similar to above, we can construct a `Grid` object with multiple faces by passing through a set of vertices. Here we define 3 six-sided faces."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 11,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.733266Z",
-                    "start_time": "2023-04-19T09:57:03.712481Z"
+                    "end_time": "2023-06-09T10:04:29.022400Z",
+                    "start_time": "2023-06-09T10:04:28.984401Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "faces_verts_ndarray = np.array([\n",
                 "    np.array([[150, 10, 0], [160, 20, 0], [150, 30, 0], [135, 30, 0], [125, 20, 0],\n",
                 "              [135, 10, 0]]),\n",
                 "    np.array([[125, 20, 0], [135, 30, 0], [125, 60, 0], [110, 60, 0], [100, 30, 0],\n",
@@ -357,89 +480,135 @@
                 "    np.array([[95, 10, 0], [105, 20, 0], [100, 30, 0], [85, 30, 0], [75, 20, 0],\n",
                 "              [85, 10, 0]]),\n",
                 "])"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We want our units to be spherical, so we pass through `islatlon=True`. Additionally, if `islatlon` is not passed through, it will default to spherical coordinates."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 12,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.733502Z",
-                    "start_time": "2023-04-19T09:57:03.715386Z"
+                    "end_time": "2023-06-09T10:04:29.046402Z",
+                    "start_time": "2023-06-09T10:04:29.001401Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<uxarray.Grid>\n",
+                            "Original Grid Type: From vertices\n",
+                            "Grid Dimensions:\n",
+                            "  * nMesh2_node: 14\n",
+                            "  * nMesh2_face: 3\n",
+                            "  * nMaxMesh2_face_nodes: 6\n",
+                            "Grid Coordinate Variables:\n",
+                            "  * Mesh2_node_x: (14,)\n",
+                            "  * Mesh2_node_y: (14,)\n",
+                            "Grid Connectivity Variables:\n",
+                            "  * Mesh2_face_nodes: (3, 6)\n",
+                            "  * nNodes_per_face: (3,)"
+                        ]
+                    },
+                    "execution_count": 12,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "verts_grid = ux.Grid(faces_verts_ndarray,\n",
                 "                     vertices=True,\n",
                 "                     islatlon=True,\n",
                 "                     concave=False)\n",
-                "verts_grid.ds"
+                "verts_grid"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 13,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-19T09:57:03.733582Z",
-                    "start_time": "2023-04-19T09:57:03.724024Z"
+                    "end_time": "2023-06-09T10:04:29.078400Z",
+                    "start_time": "2023-06-09T10:04:29.034401Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([0.14323746, 0.25118746, 0.12141312])"
+                        ]
+                    },
+                    "execution_count": 13,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "verts_grid.face_areas"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 6. Area Calculation without Grid Object\n",
                 "\n",
                 "If you want to compute the face area without using the `Grid` object, many of the functions for computing the face are can be accessed through `uxarray.helpers`\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 18,
             "metadata": {
-                "collapsed": false
+                "ExecuteTime": {
+                    "end_time": "2023-06-09T10:04:29.086401Z",
+                    "start_time": "2023-06-09T10:04:29.048402Z"
+                },
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
-                "from uxarray.helpers import calculate_face_area"
+                "from uxarray.utils.helpers import calculate_face_area"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "`Grid.calculate_face_area` takes in three coordinate variables (x, y, z) in the form of numpy arrays and the coordinate type (either spherical or artesian) and computes the face area from the set of points"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
+            "execution_count": 19,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2023-06-09T10:04:29.086401Z",
+                    "start_time": "2023-06-09T10:04:29.064401Z"
+                }
+            },
             "outputs": [],
             "source": [
                 "cart_x = np.array([\n",
                 "   0.577340924821405, 0.577340924821405, 0.577340924821405,\n",
                 "   0.577340924821405\n",
                 "])\n",
                 "cart_y = np.array([\n",
@@ -450,25 +619,48 @@
                 "   0.577366836872017, -0.577366836872017, 0.577366836872017,\n",
                 "   -0.577366836872017\n",
                 "])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
+            "execution_count": 20,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2023-06-09T10:04:29.095401Z",
+                    "start_time": "2023-06-09T10:04:29.081402Z"
+                }
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "2.0901881354848064"
+                        ]
+                    },
+                    "execution_count": 20,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "calculate_face_area(cart_x, cart_y, cart_z, coords_type=\"cartesian\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
@@ -478,9 +670,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.10"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 0
+    "nbformat_minor": 4
 }
```

### Comparing `uxarray-2023.5.0.dev0/docs/index.rst` & `uxarray-2023.6.0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 .. .. image:: _static/images/nsf.png
 ..    :scale: 100%
 ..   :align: right
 
 .. |
 .. |
 
-Uxarray Documentation
+UXarray Documentation
 =====================
 
-Uxarray aims to provide xarray styled functionality for unstructured grid datasets
-following ugrid conventions.
+UXarray provides Xarray-styled functionality for working with unstructured grids build around the
+`UGRID <http://ugrid-conventions.github.io/ugrid-conventions/>`_ conventions.
+
+
 
 .. grid:: 1 1 2 2
     :gutter: 2
 
     .. grid-item-card:: Getting Started
         :class-title: custom-title
         :class-body: custom-body
@@ -68,14 +70,15 @@
 
 
 .. toctree::
     :maxdepth: 2
     :hidden:
     :caption: For users
 
+    ANNOUNCEMENT! <announcement>
     Installation <installation>
     Getting Started <quickstart>
     Usage Examples <examples>
     API Reference <api>
     Tutorials <tutorials>
     Cite Uxarray <citation>
```

#### html2text {}

```diff
@@ -2,31 +2,32 @@
 26 08:45:00 2019. You can adapt this file completely to your liking, but it
 should at least contain the root `toctree` directive. .. module:: uxarray ..
 meta:: :description: Uxarray Python module :keywords: weather research and
 forecasting, model, weather, numerical weather prediction, model, matplotlib,
 cartopy, ncar, ucar, cisl, UC Davis, SEATs, ugrid, national center for
 atmospheric research, university corporation for atmospheric research .. ..
 image:: _static/images/nsf.png .. :scale: 100% .. :align: right .. | .. |
-Uxarray Documentation ===================== Uxarray aims to provide xarray
-styled functionality for unstructured grid datasets following ugrid
-conventions. .. grid:: 1 1 2 2 :gutter: 2 .. grid-item-card:: Getting Started :
-class-title: custom-title :class-body: custom-body :img-top: _static/images/
-icons/tips.svg :link: quickstart :link-type: doc A good place to start for new
-users .. grid-item-card:: Examples :class-title: custom-title :class-body:
-custom-body :img-top: _static/images/icons/science.svg :link: examples :link-
-type: doc A gallery of examples using uxarray .. grid-item-card:: Installation
-:class-title: custom-title :class-body: custom-body :img-top: _static/images/
-icons/download.svg :link: installation :link-type: doc Installation
-instructions for uxarray .. grid-item-card:: API :class-title: custom-title :
-class-body: custom-body :img-top: _static/images/icons/code.svg :link: api :
-link-type: doc See the complete uxarray API .. toctree:: :maxdepth: 2 :hidden:
-:caption: For users Installation  Getting Started  Usage Examples  API
-Reference  Tutorials  Cite Uxarray  .. toctree:: :maxdepth: 2 :hidden: :
-caption: For developers Contributor's Guide  .. toctree:: :maxdepth: 1 :hidden:
-:caption: Community GitHub Discussions
+UXarray Documentation ===================== UXarray provides Xarray-styled
+functionality for working with unstructured grids build around the `UGRID
+ugrid-conventions.github.io/ugrid-conventions/>`_ conventions. .. grid:: 1 1 2
+2 :gutter: 2 .. grid-item-card:: Getting Started :class-title: custom-title :
+class-body: custom-body :img-top: _static/images/icons/tips.svg :link:
+quickstart :link-type: doc A good place to start for new users .. grid-item-
+card:: Examples :class-title: custom-title :class-body: custom-body :img-top:
+_static/images/icons/science.svg :link: examples :link-type: doc A gallery of
+examples using uxarray .. grid-item-card:: Installation :class-title: custom-
+title :class-body: custom-body :img-top: _static/images/icons/download.svg :
+link: installation :link-type: doc Installation instructions for uxarray ..
+grid-item-card:: API :class-title: custom-title :class-body: custom-body :img-
+top: _static/images/icons/code.svg :link: api :link-type: doc See the complete
+uxarray API .. toctree:: :maxdepth: 2 :hidden: :caption: For users
+ANNOUNCEMENT!  Installation  Getting Started  Usage Examples  API Reference
+Tutorials  Cite Uxarray  .. toctree:: :maxdepth: 2 :hidden: :caption: For
+developers Contributor's Guide  .. toctree:: :maxdepth: 1 :hidden: :caption:
+Community GitHub Discussions
 github.com/UXARRAY/uxarray/discussions> GitHub Issues
 github.com/UXARRAY/uxarray/issues> Ugrid Conventions
 ugrid-conventions.github.io/ugrid-conventions/> -------------------- Supported
 By ============ .. raw:: html
            Project Raijin, entitled "Collaborative Research: EarthCube
            Capabilities: Raijin: Community Geoscience Analysis Tools for
 [NSF_Logo] Unstructured Mesh Data", was awarded by NSF 21-515 EarthCube (Award
```

### Comparing `uxarray-2023.5.0.dev0/docs/installation.rst` & `uxarray-2023.6.0/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 .. currentmodule:: uxarray
 
 .. _installation:
 
 Installation
 ============
 
-This installation guide includes only the Uxarray installation instructions. Please
-refer to `Uxarray Contributor's Guide <https://uxarray.readthedocs.io/en/latest/contributing.html>`_
-for detailed information about how to contribute to the uxarray project.
+This installation guide includes only the UXarray installation instructions. Please
+refer to `UXarray Contributor's Guide <https://uxarray.readthedocs.io/en/latest/contributing.html>`_
+for detailed information about how to contribute to the UXarray project.
 
-Installing Uxarray via Conda
+Installing UXarray via Conda
 ----------------------------
 
-The easiest way to install Uxarray along with its dependencies is via
+The easiest way to install UXarray along with its dependencies is via
 `Conda <https://conda.io/en/latest>`_::
 
     conda install -c conda-forge uxarray
 
 Note that the Conda package manager automatically installs all `required`
-dependencies of Uxarray, meaning it is not necessary to explicitly install
-Xarray or other required packages when installing Uxarray.
+dependencies of UXarray, meaning it is not necessary to explicitly install
+Xarray or other required packages when installing UXarray.
 
 If you are interested in learning more about how Conda environments work, please
 visit the `managing environments <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`_
 page of the Conda documentation.
 
-Installing Uxarray via PyPI
+Installing UXarray via PyPI
 ---------------------------
 
 An alternative to Conda is using pip::
 
     pip install uxarray
 
-Installing Uxarray from source (Github)
+Installing UXarray from source (Github)
 ---------------------------------------
 
-Installing Uxarray from source code is a fairly straightforward task, but
+Installing UXarray from source code is a fairly straightforward task, but
 doing so should not be necessary for most users. If you `are` interested in
-installing Uxarray from source, you will first need to get the latest version
+installing UXarray from source, you will first need to get the latest version
 of the code::
 
     git clone https://github.com/UXARRAY/uxarray.git
     cd uxarray
 
-Required dependencies for installing and testing Uxarray
+Required dependencies for installing and testing UXarray
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The following packages should be installed (in your active conda
 environment)::
 
     - Python 3.9+
     - `pytest <https://docs.pytest.org/en/stable/>`_  (For tests only)
@@ -55,37 +55,37 @@
 
 If you don't have these packages installed, the next section describes
 how to setup a conda environment with them.
 
 Creating a Conda environment
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The Uxarray source code includes a conda environment definition file
+The UXarray source code includes a conda environment definition file
 (:code:`environment.yml`) in the :code:`/ci` folder under the root
 directory that can be used to create a development environment
-containing all of the packages required to build Uxarray. The
+containing all of the packages required to build UXarray. The
 following commands should work on Windows, Linux, and macOS to create
 and activate a new conda environment from that file::
 
     conda env create -f ci/environment.yml
     conda activate uxarray_build
 
 Installing from source
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Once the dependencies listed above are installed, you can install
-Uxarray with running the following command from the root-directory::
+UXarray with running the following command from the root-directory::
 
     pip install .
 
 For compatibility purposes, we strongly recommend using Conda to
 configure your build environment as described above.
 
-Testing Uxarray source
+Testing UXarray source
 ^^^^^^^^^^^^^^^^^^^^^^
 
-A Uxarray code base can be tested from the root directory of the source
+A UXarray code base can be tested from the root directory of the source
 code repository using the following command (Explicit installation of the
 `pytest <https://docs.pytest.org/en/stable/>`_ package may be required, please
 see above)::
 
     pytest test
```

### Comparing `uxarray-2023.5.0.dev0/docs/make.bat` & `uxarray-2023.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/docs/user_api/uxarray_api.md` & `uxarray-2023.6.0/docs/user_api/uxarray_api.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,208 +1,300 @@
 Core (tier 1) functionality is indicated using regular text/list
 item style. \
 Secondary (tier 2) functionality is indicated using (*) in front.
 
-# class uxarray.Grid
+# 1. class ``uxarray.UxDataset``
 
-Describes an unstructured grid via [Dataset
-Accessor](https://docs.xarray.dev/en/stable/internals/extending-xarray.html)
-to a ``xarray.Dataset`` object.
-
-## uxarray.Grid Attributes
-
-- uxarray.Grid.ds: DataSet\
-  DataSet containing uxarray.Grid properties
-  `dims={nMesh2_node (total number of nodes),
-  nMesh2_face (number of faces),
-  MaxNumNodesPerFace (maximum number of nodes per face)}` \
-  `optional_dims={nMesh2_edge (number of edges, optional),
-  MaxNumFacesPerNode (max number of faces per node),Two, Three, Four}`
+The ``uxarray.UxDataset`` class inherits from ``xarray.Dataset``
+and A xarray.Dataset-like, and it is multi-dimensional, in
+memory, array database. It has the ``Grid`` object, ``uxgrid``, as a
+property to be unstructured grid-aware.
 
-- (*) uxarray.Grid.islatlon: boolean \
+## 1.1. UxDataset IO
+
+- uxarray.open_dataset(grid_filename_or_obj, [kwargs]) \
+  Open a single dataset, given a grid topology definition.
+
+- uxarray.open_mfdataset(grid_filename_or_obj, paths) \
+  Open multiple datasets, given a grid topology definition.
+
+## 1.2. UxDataset Attributes
+
+- UXDataset.uxgrid: ``uxarray.Grid`` \
+  ``uxarray.Grid`` property to make ``UxDataset`` unstructured grid-aware
+
+- UxDataset.source_datasets: str \
+  Property to keep track of the source data set files or object used to
+  instantiate this ``UxDataset`` (For diagnostics and reporting purposes).
+
+## 1.3. UxDataset Methods
+
+### 1.3.1. Implemented UxDataset Methods
+
+- UxDataset.info(self) \
+  Concise summary of UxDataset variables and attributes
+
+- np.float64 UxDataset.integrate(self, [quadrature_rule, order]) \
+  Integrate dataset variables over all the faces of the given mesh.
+
+### 1.3.2. Future UxDataset Methods
+
+- np.float64 UxDataset.integrate(self, [quadrature_rule, order, Grid region]) \
+  Integrate the dataset variables over a region, if specified.
+
+- UxDataset UxDataset.regrid(self, uxarray.Grid target_grid, opts) \
+  Regrid the dataset to the target_grid (by default via 1st order FV).
+
+- UxDataset UxDataset.zonal_mean(self, integer bin_count or bin_lats) \
+  Compute global zonal means over bincount latitudinal bands.
+
+- (*) UxDataset uxarray.UxDataset.composite(self, nodes) \
+  Produce composites of the DataArray at the specific locations via
+  stereographic projection.
+
+- (*) UxDataset UxDataset.snapshot(self, nodes) \
+  Produce snapshots of the DataArray at the specific locations via
+  stereographic projection.
+
+This list will be further populated ...
+
+# 2. class ``uxarray.UxDataArray``
+
+N-dimensional, ``xarray.DataArray``-like array. The
+``uxarray.UxDataArray`` class inherits from ``xarray.DataArray``. It has
+the ``Grid`` object, `uxgrid`, as a property to be unstructured grid-aware.
+
+## 2.1. UxDataArray Attributes
+
+### 2.1.1. Implemented UxDataArray Attributes
+
+- UXDataArray.uxgrid: ``uxarray.Grid`` \
+  ``uxarray.Grid`` property to make ``UxDataArray`` unstructured grid-aware
+
+### 2.1.2. Future UxDataArray Attributes
+
+- UxDataArray.type: enumeration {“vertexcentered”, “facecentered”,
+  “faceaverage”, “edgecentered”, “edgeorthogonal”, “edgeparallel”,
+  “cgll”, “dgll”} \
+  Where data is stored in this UxDataArray.
+
+- (*) UxDataArray.np: integer \
+  Polynomial order of data (when using UxDataArray.type = “cgll” or “dgll”)
+
+## 2.2. UxDataArray Methods
+
+### 2.2.1 Implemented UxDataArray Methods
+
+- UxDataArray.integrate(self, [quadrature_rule, order]) \
+  Integrate over all the faces of the given mesh.
+
+- ### 2.2.2 Future UxDataArray Methods
+
+- UxDataArray UxDataArray.divergence(self, UxDataArray other) \
+  Compute the divergence of the vector field defined by self and other.
+
+- UxDataArray UxDataArray.relative_vorticity(self, UxDataArray other) \
+  Compute the vertical component of the vorticity of the vector field defined
+  by self and other.
+
+- UxDataArray UxDataArray.laplacian(self) \
+  Compute the scalar Laplacian of the scalar field defined by self.
+
+- (UxDataArray, UxDataArray) UxDataArray.gradient(self) \
+  Compute the gradient of the scalar field defined by self in spherical
+  coordinates.
+
+- UxDataArray UxDataArray.scalardotgradient(self, UxDataArray v, UxDataArray q) \
+  Compute the dot product between a vector field (self, v) and the gradient
+  of a scalar field q.
+
+This list will be further populated ...
+
+# 3. class uxarray.Grid
+
+Describes an unstructured grid topology. It can be used standalone to explore
+an unstructured grid topology, or can be seen as the property of
+``uxarray.UxDataset`` and ``uxarray.DataArray`` to make them unstructured
+grid-aware data sets and arrays, respectively.
+
+## 3.1. Grid IO
+- uxarray.open_grid(grid_filename_or_obj, gridspec, [kwargs]) \
+  Create a ``Grid`` object from a grid topology definition.
+
+## 3.2. Grid Attributes
+
+### 3.2.1. Implemented Grid Attributes
+
+- Grid.isconcave: boolean \
+  A flag indicating the grid contains concave faces. If this flag is set,
+  then alternative algorithms may be needed for some of the operations below.
+
+- Grid.islatlon: boolean \
   A flag indicating the grid is a latitude longitude grid.
 
-- (*) uxarray.Grid.isconcave: boolean \
-  A flag indicating the grid contains concave faces.  If
-  this flag is set then alternative algorithms may be needed
-  for some of the operations below.
+- Grid.source_grid: str \
+  The source file or object for this Grid's definition (For diagnostics and
+  reporting purposes).
 
-- (*) uxarray.Grid.edgedual: uxarray.Grid \
-  The edge dual grid.
+- Grid.use_dual: boolean \
+  A flag indicating if the grid is a MPAS dual mesh.
 
-- uxarray.Grid.source_grid: string \
-  The source file for this uxarray.Grid's definition (For
-  diagnostics and reporting purposes).
-
-- uxarray.Grid.source_datasets: string \
-  The source file(s) for this uxarray.Grid's corresponding
-  data (For diagnostics and reporting purposes).
+- Grid.vertices: boolean \
+  A flag indicating if the grid is built via vertices.
 
-- (*) uxarray.Grid.vertexdual: uxarray.Grid \
-  The vertex dual grid.
+- Grid.Mesh2: np.float64 xarray.DataArray \
+  UGRID Attribute. Indicates the topology data of a 2D unstructured mesh (just
+  like the dummy variable "Mesh2" in the UGRID conventions).
 
-According to the UGRID specification, the UGRID file should
-contain a dummy variable with attribute cf_role and value
-“mesh_topology”.  This variable stores information on mesh
-topology, including relevant variable names.  The API will
-need to search for the variable containing this attribute
-and throw an error if it is missing.  Following the UGRID
-specification guide, the code below uses the name “Mesh2”
-for the dummy variable, but this could be different. The
-other names below are the ones used in the UGRID standards
-document, but they could be different.
+- Grid.Mesh2_face_x: np.float64 xarray.DataArray of size (nMesh2_face) \
+  UGRID Coordinate Variable. 2D longitude coordinate of face centers in degrees.
 
-- uxarray.Grid.Mesh2_node_x: np.float64 DataArray of size (nMesh2_node) \
-  2D longitude coordinate or 3D x coordinates for nodes on the sphere.
+- Grid.Mesh2_face_y: np.float64 xarray.DataArray of size (nMesh2_face) \
+  UGRID Coordinate Variable. 2D latitude coordinate of face centers in degrees.
 
-- uxarray.Grid.Mesh2_node_y: np.float64 DataArray of size (nMesh2_node) \
-  2D latitude coordinate or 3D y coordinates for nodes on the sphere.
+- Grid.Mesh2_node_x: np.float64 xarray.DataArray of size (nMesh2_node) \
+  UGRID Coordinate Variable. 2D longitude coordinate for nodes on the sphere in
+  degrees.
 
-- uxarray.Grid.Mesh2_node_z: np.float64 DataArray of size (nMesh2_node) \
-  (optional)
-  3D z coordinates for nodes on the sphere.
+- Grid.Mesh2_node_y: np.float64 xarray.DataArray of size (nMesh2_node) \
+  UGRID Coordinate Variable. 2D latitude coordinates for nodes on the sphere in
+  degrees.
 
-- (*) uxarray.Grid.Mesh2_node_coordinates: np.float64 DataArray of size
-  (nMesh2_node, Two or Three) \
-  Alternative storage mechanism for node information.
+- Grid.Mesh2_node_cart_x: np.float64 xarray.DataArray of size (nMesh2_node) \
+  Coordinate Variable. x coordinates for nodes in meters.
 
-- uxarray.Grid.Mesh2_face_nodes: integer DataArray of size
-  (nMesh2_face, MaxNumNodesPerFace) \
-  A DataArray of indices for each face node, corresponding to coordinates
-  in uxarray.Grid.node_*.  Faces can have arbitrary length, with
-  _FillValue=-1 used when faces have fewer nodes than MaxNumNodesPerFace.
-  Nodes are in counter-clockwise order.
+- Grid.Mesh2_node_cart_y: np.float64 xarray.DataArray of size (nMesh2_node) \
+  Coordinate Variable. y coordinates for nodes in meters.
 
-- uxarray.Grid.Mesh2_edge_nodes: integer DataArray of size (nMesh2_edge, Two)
+- Grid.Mesh2_node_cart_z: np.float64 xarray.DataArray of size (nMesh2_node) \
+  Coordinate Variable. z coordinates for nodes in meters.
+
+- Grid.nMaxMesh2_face_nodes: int
+  UGRID Dimension. Represents the maximum number of nodes that a face may contain.
+
+- Grid.nMaxMesh2_face_edges: int
+  Dimension. Represents the maximum number of edges per face.
+
+- Grid.nMesh2_edge: int
+  UGRID Dimension. Represents the total number of edges.
+
+- Grid.nMesh2_face: int
+  UGRID Dimension. Represents the total number of faces.
+
+- Grid.nMesh2_node: int
+  UGRID Dimension. Represents the total number of nodes.
+
+- Grid.nNodes_per_face: int
+  Dimension. Represents the number of non-fill-value nodes per face.
+
+- Grid.Mesh2_edge_nodes: int xarray.DataArray of size (nMesh2_edge, Two)
   (optional) \
-  A DataArray of indices for each edge.  Nodes are in arbitrary order.
+  UGRID Connectivity Variable. Maps every edge to the two nodes that it connects
+
+- Grid.Mesh2_face_edges: int xarray.DataArray of size (nMesh2_face,
+  nMaxMesh2_face_nodes) (optional) \
+  UGRID Connectivity Variable. Maps every face to its edges.
+
+- Grid.Mesh2_face_nodes: int xarray.DataArray of size
+  (nMesh2_face, MaxNumNodesPerFace) \
+  UGRID Connectivity Variable. Maps each face to its corner nodes.
+
+- Grid.face_areas: np.float64 xarray.DataArray of size (nMesh2_face) \
+  Provides areas for each face.
+
+- Grid.parsed_attrs: dict
+  Dictionary of parsed attributes from the source grid.
 
-- (*) uxarray.Grid.Mesh2_edge_types: integer DataArray of size (nMesh2_edge)
+### 3.2.2. Future Grid Attributes
+
+- Grid.Mesh2_node_z: np.float64 xarray.DataArray of size (nMesh2_node) \
+  (optional)
+  3D z coordinates for nodes on the sphere.
+
+- (*) Grid.edge_dual: Grid \
+  The edge dual grid.
+
+- (*) Grid.vertex_dual: Grid \
+  The vertex dual grid.
+
+- (*) Grid.Mesh2_edge_types: int DataArray of size (nMesh2_edge)
   (optional; not in UGRID standard) \
   A DataArray indicating the type of edge (0 = great circle arc, 1 = line of
   constant latitude)
 
-- uxarray.Grid.Mesh2_face_areas: np.float64 DataArray of size (nMesh2_face)
-  (optional; not in UGRID standard) \
-  A DataArray providing face areas for each face.
-
-- (*) uxarray.Grid.Mesh2_imask: integer DataArray of size (nMesh2_face)
+- (*) Grid.Mesh2_imask: int DataArray of size (nMesh2_face)
   (optional; not in UGRID standard) \
-  The integer mask for this grid (1 = face is active; 0 = face is inactive)
-
-- uxarray.Grid.Mesh2_face_edges: integer DataArray of size (nMesh2_face,
-  MaxNumNodesPerFace) (optional) \
-  A DataArray of indices indicating edges that are neighboring each face.
+  The int mask for this grid (1 = face is active; 0 = face is inactive)
 
-- uxarray.Grid.Mesh2_face_links: integer DataArray of size (nMesh2_face,
+- Grid.Mesh2_face_links: int DataArray of size (nMesh2_face,
   MaxNumNodesPerFace) (optional) \
   A DataArray of indices indicating faces that are neighboring each face.
 
-- uxarray.Grid.Mesh2_edge_faces: integer DataArray of size (nMesh2_edge,
+- Grid.Mesh2_edge_faces: int DataArray of size (nMesh2_edge,
   Two) (optional) \
   A DataArray of indices indicating faces that are neighboring each edge.
 
-- uxarray.Grid.Mesh2_node_faces: integer DataArray of size (nMesh2_node,
+- Grid.Mesh2_node_faces: int DataArray of size (nMesh2_node,
   MaxNumFacesPerNode) (optional) \
   A DataArray of indices indicating faces that are neighboring each node.
 
-- (*) uxarray.Grid.Mesh2_latlon_bounds: np.float64 DataArray of size
+- (*) Grid.Mesh2_latlon_bounds: np.float64 DataArray of size
   (nMesh2_face, Four) (optional; not in UGRID standard) \
   A DataArray of values indicating the latitude-longitude boundaries of
   each face.
 
-- (*) uxarray.Grid.Mesh2_overlapfaces_a: integer DataArray of size
+- (*) Grid.Mesh2_overlapfaces_a: int DataArray of size
   (nMesh2_face) (optional; not in UGRID standard) \
   A DataArray of indices storing the indices of the parent face from
   grid A, available when this Grid is a supermesh.
 
-- (*) uxarray.Grid.Mesh2_overlapfaces_b: integer DataArray of size
+- (*) Grid.Mesh2_overlapfaces_b: int DataArray of size
   (nMesh2_face) (optional; not in UGRID standard) \
   A DataArray of indices storing the indices of the parent face from
   grid B, available when this Grid is a supermesh.
 
-## uxarray.Grid  Functions
+## 3.3. Grid Methods
 
-- uxarray.Grid.__init__(self, xarray dataset) \
-  Populate Grid object with Xarray dataset.  The routine will automatically
-  detect if it is a UGrid, SCRIP, Exodus, or shape file.
+### 3.3.1. Implemented Grid Methods
 
-- (*) uxarray.Grid.__init__(self, string gridspec) \
-  Define a grid specified by gridspec string (analogous to the gridspec
-  used in ncremap for grid generation).
+- Grid.__init__(self, input_obj) \
+  Populate Grid object with input_object that can be one of xarray.Dataset,
+  ndarray, list, or tuple.  The routine will automatically recognize if it is
+  a UGRID, MPAS, SCRIP, or Exodus, or shape file.
 
-- uxarray.Grid.__init__(self, np.float64.list vertices) \
-  Create a grid with one face with vertices specified by the given argument.
+- Grid.copy(self) \
+  Return a deep copy of self.
 
-- uxarray.Grid.encode_as(self, string grid_type) \
+- Grid.encode_as(self, str grid_type) \
   Encode a `uxarray.Grid` as a `xarray.Dataset`in the specified grid type
-  (UGRID, SCRIP, Exodus, or SHP).
-
-- uxarray.Grid.calculatefaceareas(self) \
-  Calculate the area of all faces.
-
-- uxarray.Grid.build_node_face_connectivity(self) \
-  Build the node-face connectivity array.
-
-- uxarray.Grid.build_edge_face_connectivity(self) \
-  Build the edge-face connectivity array.
-
-- uxarray.Grid.buildlatlon_bounds(self) \
-  Build the array of latitude-longitude bounding boxes.
-
-- uxarray.Grid.validate(self) \
-  Validate that the grid conforms to the UGRID standards.
-
-## Additional xarray.DataArray Attributes
-
-- xarray.DataArray.grid: uxarray.Grid \
-  The grid associated with this xarray.DataArray.
+  (UGRID, SCRIP, Exodus).
 
-- xarray.type: enumeration {“vertexcentered”, “facecentered”,
-  “faceaverage”, “edgecentered”, “edgeorthogonal”, “edgeparallel”,
-  “cgll”, “dgll”} \
-  Where data is stored in this DataArray.
-
-- (*) xarray.np: integer \
-  Polynomial order of data (when using xarray.type = “cgll” or “dgll”)
-
-## Helper Functions
-
-- np.float64 uxarray.integrate(self, xarray.DataArray q,
-  uxarray.Grid region (optional)) \
-  Integrate the DataArray globally or over a specified region
-  (if specified).
-
-- xarray.DataSet uxarray.zonalmean(self, xarray.DataArray q,
-  integer bincount or binlats) \
-  Compute global zonal means over bincount latitudinal bands.
+- Grid.calculate_total_face_area(self, [quadrature_rule, order]) \
+  Calculate the total surface area of the whole mesh, i.e. sum of face areas.
 
-- xarray.DataSet uxarray.regrid(self, xarray.DataArray q,
-  uxarray.Grid targetgrid, opts) \
-  Regrid the data to the target grid (by default via 1st order FV).
+- Grid.compute_face_areas(self, [quadrature_rule, order]) \
+  Calculate the individual areas of all faces.
 
-- xarray.DataArray uxarray.divergence(xarray.DataArray u,
-  xarray.DataArray v) \
-  Compute the divergence of the vector field defined by u and v.
+### 3.3.2. Future Grid Methods
 
-- xarray.DataArray uxarray.relative_vorticity(xarray.DataArray u,
-  xarray.DataArray v) \
-  Compute the vertical component of the vorticity of the vector field defined by u and v.
+- (*) Grid.__init__(self, str gridspec) \
+  Define a grid specified by gridspec str (analogous to the gridspec
+  used in ncremap for grid generation).
 
-- xarray.DataArray uxarray.laplacian(xarray.DataArray q) \
-  Compute the scalar Laplacian of the scalar field q.
+- Grid.build_node_face_connectivity(self) \
+  Build the node-face connectivity array.
 
-- (xarray.DataArray, xarray.DataArray) uxarray.gradient(xarray.DataArray q) \
-  Compute the gradient of the scalar field q in spherical coordinates.
+- Grid.build_edge_face_connectivity(self) \
+  Build the edge-face connectivity array.
 
-- xarray.DataArray uxarray.scalardotgradient(xarray.DataArray u,
-  xarray.DataArray v, xarray.DataArray q) \
-  Compute the dot product between a vector field (u,v) and the gradient of a scalar field q.
+- Grid.build_lat_lon_bounds(self) \
+  Build the array of latitude-longitude bounding boxes.
 
-- (*) xarray.Grid uxarray.supermesh(uxarray.Grid a, uxarray.Grid b) \
-  Construct the supermesh, consisting of all face edges from Grids a and b.
+- Grid.encode_as(self, str grid_type) \
+  Encode a `uxarray.Grid` as a `xarray.Dataset`in the MPAS or SHP grid type.
 
-- (*) xarray.DataSet xarray.DataSet.snapshot(self, nodes) \
-  Produce snapshots of the DataArray at the specific locations via stereographic projection.
+- Grid.validate(self) \
+  Validate that the grid conforms to the UGRID standards.
 
-- (*) xarray.DataSet xarray.DataSet.composite(self, nodes) \
-  Produce composites of the DataArray at the specific locations via stereographic projection.
+- (*) Grid Grid.super_mesh(self, Grid other) \
+  Construct the super mesh, consisting of all face edges from Grids self and
+  other.
```

### Comparing `uxarray-2023.5.0.dev0/meta.yaml` & `uxarray-2023.6.0/meta.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% set version = "2023.05.0dev" %}
+{% set version = "2023.06.0" %}
 
 package:
   name: 'uxarray'
   version: {{ version }}
 
 build:
   noarch: python
```

### Comparing `uxarray-2023.5.0.dev0/setup.py` & `uxarray-2023.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/exodus/mixed/mixed.exo` & `uxarray-2023.6.0/test/meshfiles/exodus/mixed/mixed.exo`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/exodus/outCSne8/outCSne8.g` & `uxarray-2023.6.0/test/meshfiles/exodus/outCSne8/outCSne8.g`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc` & `uxarray-2023.6.0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/scrip/outCSne8/outCSne8.nc` & `uxarray-2023.6.0/test/meshfiles/scrip/outCSne8/outCSne8.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/shp/grid_fire.shp` & `uxarray-2023.6.0/test/meshfiles/shp/grid_fire.shp`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/README.md` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/README.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/grid.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/grid.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v1.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/v1.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v2.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/v2.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v3.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/geoflow-small/v3.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30.ug` & `uxarray-2023.6.0/test/meshfiles/ugrid/outCSne30/outCSne30.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug` & `uxarray-2023.6.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug` & `uxarray-2023.6.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc` & `uxarray-2023.6.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/test_api.py` & `uxarray-2023.6.0/test/test_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,81 +8,88 @@
 try:
     import constants
 except ImportError:
     from . import constants
 
 current_path = Path(os.path.dirname(os.path.realpath(__file__)))
 
-gridfile_ne30 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30.ug"
-dsfile_var2_ne30 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30_var2.nc"
-dsfiles_mf_ne30 = str(
-    current_path) + "/meshfiles/ugrid/outCSne30/outCSne30_*.nc"
-
-gridfile_geoflow = current_path / "meshfiles" / "ugrid" / "geoflow-small" / "grid.nc"
-
 
 class TestAPI(TestCase):
 
+    geoflow_data_path = current_path / "meshfiles" / "ugrid" / "geoflow-small"
+    gridfile_geoflow = current_path / "meshfiles" / "ugrid" / "geoflow-small" / "grid.nc"
+    geoflow_data_v1 = geoflow_data_path / "v1.nc"
+    geoflow_data_v2 = geoflow_data_path / "v2.nc"
+    geoflow_data_v3 = geoflow_data_path / "v3.nc"
+
+    gridfile_ne30 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30.ug"
+    dsfile_var2_ne30 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30_var2.nc"
+    dsfiles_mf_ne30 = str(
+        current_path) + "/meshfiles/ugrid/outCSne30/outCSne30_*.nc"
+
     def test_open_geoflow_dataset(self):
         """Loads a single dataset with its grid topology file using uxarray's
         open_dataset call."""
 
-        # Base data path
-        base_path = "test/meshfiles/ugrid/geoflow-small/"
-
-        # Path to Grid file
-        grid_path = base_path + "grid.nc"
-
         # Paths to Data Variable files
-        var_names = ['v1.nc', 'v2.nc', 'v3.nc']
-        data_paths = [base_path + name for name in var_names]
+        data_paths = [
+            self.geoflow_data_v1, self.geoflow_data_v2, self.geoflow_data_v3
+        ]
 
-        uxds_v1 = ux.open_dataset(grid_path, data_paths[0])
+        uxds_v1 = ux.open_dataset(self.gridfile_geoflow, data_paths[0])
 
-    #     TODO: Add asserts
+        # Ideally uxds_v1.uxgrid should NOT be None
+        with self.assertRaises(AssertionError):
+            nt.assert_equal(uxds_v1.uxgrid, None)
 
     def test_open_dataset(self):
         """Loads a single dataset with its grid topology file using uxarray's
         open_dataset call."""
 
-        uxds_var2_ne30 = ux.open_dataset(gridfile_ne30, dsfile_var2_ne30)
+        uxds_var2_ne30 = ux.open_dataset(self.gridfile_ne30,
+                                         self.dsfile_var2_ne30)
 
         nt.assert_equal(uxds_var2_ne30.uxgrid.Mesh2_node_x.size,
                         constants.NNODES_outCSne30)
         nt.assert_equal(len(uxds_var2_ne30.uxgrid._ds.data_vars),
                         constants.DATAVARS_outCSne30)
-        nt.assert_equal(uxds_var2_ne30.uxgrid.source_grid, gridfile_ne30)
-        nt.assert_equal(uxds_var2_ne30.source_datasets, str(dsfile_var2_ne30))
+        nt.assert_equal(uxds_var2_ne30.uxgrid.source_grid,
+                        str(self.gridfile_ne30))
+        nt.assert_equal(uxds_var2_ne30.source_datasets,
+                        str(self.dsfile_var2_ne30))
 
     def test_open_mf_dataset(self):
         """Loads multiple datasets with their grid topology file using
         uxarray's open_dataset call."""
 
-        uxds_mf_ne30 = ux.open_mfdataset(gridfile_ne30, dsfiles_mf_ne30)
+        uxds_mf_ne30 = ux.open_mfdataset(self.gridfile_ne30,
+                                         self.dsfiles_mf_ne30)
 
         nt.assert_equal(uxds_mf_ne30.uxgrid.Mesh2_node_x.size,
                         constants.NNODES_outCSne30)
         nt.assert_equal(len(uxds_mf_ne30.uxgrid._ds.data_vars),
                         constants.DATAVARS_outCSne30)
-        nt.assert_equal(uxds_mf_ne30.uxgrid.source_grid, gridfile_ne30)
-        nt.assert_equal(uxds_mf_ne30.source_datasets, dsfiles_mf_ne30)
+        nt.assert_equal(uxds_mf_ne30.uxgrid.source_grid,
+                        str(self.gridfile_ne30))
+        nt.assert_equal(uxds_mf_ne30.source_datasets, self.dsfiles_mf_ne30)
 
     def test_open_grid(self):
         """Loads only a grid topology file using uxarray's open_grid call."""
-        uxgrid = ux.open_grid(gridfile_geoflow)
+        uxgrid = ux.open_grid(self.gridfile_geoflow)
 
         nt.assert_almost_equal(uxgrid.calculate_total_face_area(),
                                constants.MESH30_AREA,
                                decimal=3)
 
     def test_copy_dataset(self):
         """Loads a single dataset with its grid topology file using uxarray's
         open_dataset call and make a copy of the object."""
 
-        uxds_var2_ne30 = ux.open_dataset(gridfile_ne30, dsfile_var2_ne30)
+        uxds_var2_ne30 = ux.open_dataset(self.gridfile_ne30,
+                                         self.dsfile_var2_ne30)
 
         # make a shallow and deep copy of the dataset object
         uxds_var2_ne30_copy_deep = uxds_var2_ne30.copy(deep=True)
         uxds_var2_ne30_copy = uxds_var2_ne30.copy(deep=False)
 
         # Ideally uxds_var2_ne30_copy.uxgrid should NOT be None
         with self.assertRaises(AssertionError):
@@ -96,25 +103,20 @@
         assert (uxds_var2_ne30_copy_deep.uxgrid == uxds_var2_ne30.uxgrid)
         assert (uxds_var2_ne30_copy_deep.uxgrid is not uxds_var2_ne30.uxgrid)
 
     def test_copy_dataarray(self):
         """Loads an unstructured grid and data using uxarray's open_dataset
         call and make a copy of the dataarray object."""
 
-        # Base data path
-        base_path = "test/meshfiles/ugrid/geoflow-small/"
-
-        # Path to Grid file
-        grid_path = base_path + "grid.nc"
-
         # Paths to Data Variable files
-        var_names = ['v1.nc', 'v2.nc', 'v3.nc']
-        data_paths = [base_path + name for name in var_names]
+        data_paths = [
+            self.geoflow_data_v1, self.geoflow_data_v2, self.geoflow_data_v3
+        ]
 
-        uxds_v1 = ux.open_dataset(grid_path, data_paths[0])
+        uxds_v1 = ux.open_dataset(self.gridfile_geoflow, data_paths[0])
 
         # get the uxdataarray object
         v1_uxdata_array = uxds_v1['v1']
 
         # make a shallow and deep copy of the dataarray object
         v1_uxdata_array_copy_deep = v1_uxdata_array.copy(deep=True)
         v1_uxdata_array_copy = v1_uxdata_array.copy(deep=False)
```

### Comparing `uxarray-2023.5.0.dev0/test/test_dataset.py` & `uxarray-2023.6.0/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/test_exodus.py` & `uxarray-2023.6.0/test/test_exodus.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/test_grid.py` & `uxarray-2023.6.0/test/test_grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,43 +108,43 @@
             faces_coords.append(face_coords)
 
         # Now consturct the grid using the faces_coords
         verts_cart = np.array(faces_coords)
         vgrid = ux.open_grid(verts_cart,
                              vertices=True,
                              islatlon=False,
-                             concave=False)
+                             isconcave=False)
 
         assert (vgrid.source_grid == "From vertices")
         assert (vgrid.nMesh2_face == 6)
         assert (vgrid.nMesh2_node == 8)
         vgrid.encode_as("ugrid")
 
         # Test the case when user created a nested one-face grid
         faces_verts_one = np.array([
             np.array([[150, 10], [160, 20], [150, 30], [135, 30], [125, 20],
                       [135, 10]])
         ])
         vgrid = ux.open_grid(faces_verts_one,
                              vertices=True,
                              islatlon=True,
-                             concave=False)
+                             isconcave=False)
         assert (vgrid.source_grid == "From vertices")
         assert (vgrid.nMesh2_face == 1)
         assert (vgrid.nMesh2_node == 6)
         vgrid.encode_as("ugrid")
 
         # Test the case when user created a one-face grid
         faces_verts_single_face = np.array([[150, 10], [160, 20], [150, 30],
                                             [135, 30], [125, 20], [135, 10]])
 
         vgrid = ux.open_grid(faces_verts_single_face,
                              vertices=True,
                              islatlon=True,
-                             concave=False)
+                             isconcave=False)
         assert (vgrid.source_grid == "From vertices")
         assert (vgrid.nMesh2_face == 1)
         assert (vgrid.nMesh2_node == 6)
         vgrid.encode_as("ugrid")
 
     def test_init_verts_different_input_datatype(self):
         """Create a uxarray grid from multiple face vertices with different
@@ -178,30 +178,30 @@
                             [[125, 20], [135, 30], [125, 60], [110, 60],
                              [100, 30], [105, 20]],
                             [[95, 10], [105, 20], [100, 30], [85, 30], [75, 20],
                              [85, 10]]]
         vgrid = ux.open_grid(faces_verts_list,
                              vertices=True,
                              islatlon=False,
-                             concave=False)
+                             isconcave=False)
         assert (vgrid.source_grid == "From vertices")
         assert (vgrid.nMesh2_face == 3)
         assert (vgrid.nMesh2_node == 14)
         vgrid.encode_as("ugrid")
 
         # Test initializing Grid from tuples
         faces_verts_tuples = [
             ((150, 10), (160, 20), (150, 30), (135, 30), (125, 20), (135, 10)),
             ((125, 20), (135, 30), (125, 60), (110, 60), (100, 30), (105, 20)),
             ((95, 10), (105, 20), (100, 30), (85, 30), (75, 20), (85, 10))
         ]
         vgrid = ux.open_grid(faces_verts_tuples,
                              vertices=True,
                              islatlon=False,
-                             concave=False)
+                             isconcave=False)
         assert (vgrid.source_grid == "From vertices")
         assert (vgrid.nMesh2_face == 3)
         assert (vgrid.nMesh2_node == 14)
         vgrid.encode_as("ugrid")
 
     def test_init_verts_fill_values(self):
         faces_verts_filled_values = [[[150, 10], [160, 20], [150, 30],
@@ -211,21 +211,21 @@
                                       [ux.INT_FILL_VALUE, ux.INT_FILL_VALUE]],
                                      [[95, 10], [105, 20], [100, 30], [85, 30],
                                       [ux.INT_FILL_VALUE, ux.INT_FILL_VALUE],
                                       [ux.INT_FILL_VALUE, ux.INT_FILL_VALUE]]]
         vgrid = ux.open_grid(faces_verts_filled_values,
                              vertices=True,
                              islatlon=False,
-                             concave=False)
+                             isconcave=False)
         assert (vgrid.source_grid == "From vertices")
         assert (vgrid.nMesh2_face == 3)
         assert (vgrid.nMesh2_node == 12)
 
-    def test_init_grid_var_attrs(self):
-        """Tests to see if accessing variables through set attributes is equal
+    def test_grid_properties(self):
+        """Tests to see if accessing variables through set properties is equal
         to using the dict."""
 
         # Dataset with standard UGRID variable names
         # Coordinates
         xr.testing.assert_equal(
             self.grid_CSne30.Mesh2_node_x, self.grid_CSne30._ds[
                 self.grid_CSne30.grid_var_names["Mesh2_node_x"]])
@@ -295,29 +295,29 @@
         assert self.grid_CSne30_01 == self.grid_CSne30_02
 
     def test_ne(self):
         """Test Not Equals ('!=') operator."""
         assert self.grid_CSne30_01 != self.grid_RLL1deg
 
 
-class TestIntegrate(TestCase):
+class TestFaceAreas(TestCase):
 
     grid_CSne30 = ux.open_grid(gridfile_CSne30)
 
     def test_calculate_total_face_area_triangle(self):
         """Create a uxarray grid from vertices and saves an exodus file."""
 
         verts = [[[0.57735027, -5.77350269e-01, -0.57735027],
                   [0.57735027, 5.77350269e-01, -0.57735027],
                   [-0.57735027, 5.77350269e-01, -0.57735027]]]
 
         grid_verts = ux.open_grid(verts,
                                   vertices=True,
                                   islatlon=False,
-                                  concave=False)
+                                  isconcave=False)
 
         #calculate area
         area_gaussian = grid_verts.calculate_total_face_area(
             quadrature_rule="gaussian", order=5)
         nt.assert_almost_equal(area_gaussian, constants.TRI_AREA, decimal=3)
 
         area_triangular = grid_verts.calculate_total_face_area(
@@ -332,49 +332,47 @@
         nt.assert_almost_equal(area, constants.MESH30_AREA, decimal=3)
 
     def test_calculate_total_face_area_sphere(self):
         """Computes the total face area of an MPAS mesh that lies on a unit
         sphere, with an expected total face area of 4pi."""
         mpas_grid_path = current_path / 'meshfiles' / "mpas" / "QU" / 'mesh.QU.1920km.151026.nc'
 
-        ds = xr.open_dataset(mpas_grid_path)
-        primal_grid = ux.Grid(ds, use_dual=False)
-        dual_grid = ux.Grid(ds, use_dual=True)
+        primal_grid = ux.open_grid(mpas_grid_path, use_dual=False)
+        dual_grid = ux.open_grid(mpas_grid_path, use_dual=True)
 
         primal_face_area = primal_grid.calculate_total_face_area()
         dual_face_area = dual_grid.calculate_total_face_area()
 
         nt.assert_almost_equal(primal_face_area,
                                constants.UNIT_SPHERE_AREA,
                                decimal=3)
 
         nt.assert_almost_equal(dual_face_area,
                                constants.UNIT_SPHERE_AREA,
                                decimal=3)
 
-    def test_integrate(self):
-        xr_psi = xr.open_dataset(dsfile_vortex_CSne30)
-        xr_v2 = xr.open_dataset(dsfile_var2_CSne30)
-
-        integral_psi = self.grid_CSne30.integrate(xr_psi)
-        integral_var2 = self.grid_CSne30.integrate(xr_v2)
-
-        nt.assert_almost_equal(integral_psi, constants.PSI_INTG, decimal=3)
-        nt.assert_almost_equal(integral_var2, constants.VAR2_INTG, decimal=3)
-
-
-class TestFaceAreas(TestCase):
+    # TODO: Will depend on the decision for whether to provide integrate function
+    # from within `Grid` as well as UxDataset
+    # def test_integrate(self):
+    #     xr_psi = xr.open_dataset(dsfile_vortex_CSne30)
+    #     xr_v2 = xr.open_dataset(dsfile_var2_CSne30)
+    #
+    #     integral_psi = self.grid_CSne30.integrate(xr_psi)
+    #     integral_var2 = self.grid_CSne30.integrate(xr_v2)
+    #
+    #     nt.assert_almost_equal(integral_psi, constants.PSI_INTG, decimal=3)
+    #     nt.assert_almost_equal(integral_var2, constants.VAR2_INTG, decimal=3)
 
     def test_compute_face_areas_geoflow_small(self):
         """Checks if the GeoFlow Small can generate a face areas output."""
         grid_geoflow = ux.open_grid(gridfile_geoflow)
 
         grid_geoflow.compute_face_areas()
 
-    # removed test until fix to tranposed face nodes
+    # TODO: Add this test after fix to tranposed face nodes
     # def test_compute_face_areas_fesom(self):
     #     """Checks if the FESOM PI-Grid Output can generate a face areas
     #     output."""
     #     grid_fesom = ux.open_grid(gridfile_fesom)
     #
     #     grid_fesom.compute_face_areas()
 
@@ -384,18 +382,18 @@
                       [125, 20, 0], [135, 10, 0]]),
             np.array([[125, 20, 0], [135, 30, 0], [125, 60, 0], [110, 60, 0],
                       [100, 30, 0], [105, 20, 0]]),
             np.array([[95, 10, 0], [105, 20, 0], [100, 30, 0], [85, 30, 0],
                       [75, 20, 0], [85, 10, 0]]),
         ])
         # load our vertices into a UXarray Grid object
-        verts_grid = ux.Grid(faces_verts_ndarray,
-                             vertices=True,
-                             islatlon=True,
-                             concave=False)
+        verts_grid = ux.open_grid(faces_verts_ndarray,
+                                  vertices=True,
+                                  islatlon=True,
+                                  isconcave=False)
 
         face_verts_areas = verts_grid.face_areas
 
         nt.assert_almost_equal(face_verts_areas.sum(),
                                constants.FACE_VERTS_AREA,
                                decimal=3)
 
@@ -487,21 +485,17 @@
 class TestConnectivity(TestCase):
     mpas_filepath = current_path / "meshfiles" / "mpas" / "QU" / "mesh.QU.1920km.151026.nc"
     exodus_filepath = current_path / "meshfiles" / "exodus" / "outCSne8" / "outCSne8.g"
     ugrid_filepath_01 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30.ug"
     ugrid_filepath_02 = current_path / "meshfiles" / "ugrid" / "outRLL1deg" / "outRLL1deg.ug"
     ugrid_filepath_03 = current_path / "meshfiles" / "ugrid" / "ov_RLL10deg_CSne4" / "ov_RLL10deg_CSne4.ug"
 
-    xrds_maps = xr.open_dataset(mpas_filepath)
-    xrds_exodus = xr.open_dataset(exodus_filepath)
-    xrds_ugrid = xr.open_dataset(ugrid_filepath_01)
-
-    grid_mpas = ux.Grid(xrds_maps)
-    grid_exodus = ux.Grid(xrds_exodus)
-    grid_ugrid = ux.Grid(xrds_ugrid)
+    grid_mpas = ux.open_grid(mpas_filepath)
+    grid_exodus = ux.open_grid(exodus_filepath)
+    grid_ugrid = ux.open_grid(ugrid_filepath_01)
 
     # used from constructing vertices
     f0_deg = [[120, -20], [130, -10], [120, 0], [105, 0], [95, -10], [105, -20]]
     f1_deg = [[120, 0], [120, 10], [115, 0],
               [ux.INT_FILL_VALUE, ux.INT_FILL_VALUE],
               [ux.INT_FILL_VALUE, ux.INT_FILL_VALUE],
               [ux.INT_FILL_VALUE, ux.INT_FILL_VALUE]]
@@ -646,46 +640,44 @@
             assert grid.nNodes_per_face.max() <= max_dimension
 
         # test on grid constructed from vertices
         verts = [
             self.f0_deg, self.f1_deg, self.f2_deg, self.f3_deg, self.f4_deg,
             self.f5_deg, self.f6_deg
         ]
-        grid_from_verts = ux.Grid(verts)
+        grid_from_verts = ux.open_grid(verts)
 
         # number of non-fill-value nodes per face
         expected_nodes_per_face = np.array([6, 3, 4, 6, 6, 4, 4], dtype=int)
         nt.assert_equal(grid_from_verts.nNodes_per_face.values,
                         expected_nodes_per_face)
 
     def test_edge_nodes_euler(self):
         """Verifies that (``nMesh2_edge``) follows euler's formula."""
         grid_paths = [
             self.exodus_filepath, self.ugrid_filepath_01,
             self.ugrid_filepath_02, self.ugrid_filepath_03
         ]
 
         for grid_path in grid_paths:
-            grid_xr = xr.open_dataset(grid_path)
-            grid_ux = ux.Grid(grid_xr)
+            grid_ux = ux.open_grid(grid_path)
 
             n_face = grid_ux.nMesh2_face
             n_node = grid_ux.nMesh2_node
             n_edge = grid_ux.nMesh2_edge
 
             # euler's formula (n_face = n_edges - n_nodes + 2)
             assert (n_face == n_edge - n_node + 2)
 
     def test_build_face_edges_connectivity_mpas(self):
         """Tests the construction of (``Mesh2_edge_nodes``) on an MPAS grid
         with known edge nodes."""
 
         # grid with known edge node connectivity
-        mpas_grid_xr = xr.open_dataset(self.mpas_filepath)
-        mpas_grid_ux = ux.Grid(mpas_grid_xr)
+        mpas_grid_ux = ux.open_grid(self.mpas_filepath)
         edge_nodes_expected = mpas_grid_ux._ds['Mesh2_edge_nodes'].values
 
         # arrange edge nodes in the same manner as Grid._build_edge_node_connectivity
         edge_nodes_expected.sort(axis=1)
         edge_nodes_expected = np.unique(edge_nodes_expected, axis=0)
 
         # construct edge nodes
@@ -704,16 +696,15 @@
     def test_build_face_edges_connectivity(self):
         """Generates Grid.Mesh2_edge_nodes from Grid.Mesh2_face_nodes."""
         ug_filename_list = [
             self.ugrid_filepath_01, self.ugrid_filepath_02,
             self.ugrid_filepath_03
         ]
         for ug_file_name in ug_filename_list:
-            xr_ds = xr.open_dataset(ug_file_name)
-            tgrid = ux.Grid(xr_ds)
+            tgrid = ux.open_grid(ug_file_name)
 
             mesh2_face_nodes = tgrid._ds["Mesh2_face_nodes"]
 
             tgrid._build_face_edges_connectivity()
             mesh2_face_edges = tgrid._ds.Mesh2_face_edges
             mesh2_edge_nodes = tgrid._ds.Mesh2_edge_nodes
 
@@ -740,16 +731,15 @@
 
             for i in range(len(reverted_mesh2_edge_nodes)):
                 self.assertTrue(
                     np.array_equal(reverted_mesh2_edge_nodes[i],
                                    original_face_nodes_connectivity[i]))
 
     def test_build_face_edges_connectivity_mpas(self):
-        xr_ds = xr.open_dataset(self.mpas_filepath)
-        tgrid = ux.Grid(xr_ds)
+        tgrid = ux.open_grid(self.mpas_filepath)
 
         mesh2_face_nodes = tgrid._ds["Mesh2_face_nodes"]
 
         tgrid._build_face_edges_connectivity()
         mesh2_face_edges = tgrid._ds.Mesh2_face_edges
         mesh2_edge_nodes = tgrid._ds.Mesh2_edge_nodes
 
@@ -767,15 +757,15 @@
         self.assertEqual(mesh2_edge_nodes.sizes["nMesh2_edge"], num_edges)
 
     def test_build_face_edges_connectivity_fillvalues(self):
         verts = [
             self.f0_deg, self.f1_deg, self.f2_deg, self.f3_deg, self.f4_deg,
             self.f5_deg, self.f6_deg
         ]
-        uds = ux.Grid(verts)
+        uds = ux.open_grid(verts)
         uds._build_face_edges_connectivity()
         n_face = len(uds._ds["Mesh2_face_edges"].values)
         n_node = uds.nMesh2_node
         n_edge = len(uds._ds["Mesh2_edge_nodes"].values)
 
         self.assertEqual(7, n_face)
         self.assertEqual(21, n_node)
```

### Comparing `uxarray-2023.5.0.dev0/test/test_helpers.py` & `uxarray-2023.6.0/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/test_mpas.py` & `uxarray-2023.6.0/test/test_mpas.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,17 @@
     def test_dual_to_ugrid_conversion(self):
         """Verifies that the Dual-Mesh was converted properly."""
 
         # dual-mesh encoded in the UGRID conventions
         ds = _read_mpas(self.mpas_xr_ds, use_dual=True)
 
         # check for correct dimensions
-        expected_ugrid_dims = ['nMesh2_node', "nMesh2_face", "Three"]
+        expected_ugrid_dims = [
+            'nMesh2_node', "nMesh2_face", "nMaxMesh2_face_nodes"
+        ]
         for dim in expected_ugrid_dims:
             assert dim in ds.sizes
 
         # check for correct length of coordinates
         assert len(ds['Mesh2_node_x']) == len(ds['Mesh2_node_y'])
         assert len(ds['Mesh2_face_x']) == len(ds['Mesh2_face_y'])
```

### Comparing `uxarray-2023.5.0.dev0/test/test_scrip.py` & `uxarray-2023.6.0/test/test_scrip.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/test/test_ugrid.py` & `uxarray-2023.6.0/test/test_ugrid.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/uxarray/core/api.py` & `uxarray-2023.6.0/uxarray/core/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 
 from uxarray.core.dataset import UxDataset
 
 
 def open_grid(grid_filename_or_obj: Union[str, Path, xr.DataArray, np.ndarray,
                                           list, tuple],
               gridspec: Optional[str] = None,
+              vertices: Optional[list] = None,
               islatlon: Optional[bool] = False,
               isconcave: Optional[bool] = False,
               use_dual: Optional[bool] = False,
-              **kwargs: Dict[str, Any]) -> xr.Dataset:
-    """Creates a ``uxarray.core.Grid`` object from a grid topology definition.
+              **kwargs: Dict[str, Any]) -> Grid:
+    """Creates a ``uxarray.Grid`` object from a grid topology definition.
 
     Parameters
     ----------
 
     grid_filename_or_obj : string, xarray.Dataset, ndarray, list, tuple, required
         String or Path object as a path to a netCDF file or an OpenDAP URL that
         stores the unstructured grid topology/definition. It is read similar to
@@ -37,14 +38,17 @@
 
     isconcave: bool, optional
         Specify if this grid has concave elements (internal checks for this are possible)
 
     gridspec: str, optional
         Specifies gridspec
 
+    vertices: bool, optional
+        Whether to create grid from vertices
+
     source_grid: str, optional
         Path or URL to the source grid file. For diagnostic/reporting purposes only.
 
     use_dual: bool, optional
             Specify whether to use the primal (use_dual=False) or dual (use_dual=True) mesh if the file type is mpas
 
     **kwargs : Dict[str, Any]
@@ -52,57 +56,60 @@
         [xarray
         docs](https://xarray.pydata.org/en/stable/generated/xarray.open_dataset.html)
         for accepted keyword arguments.
 
     Returns
     -------
 
-    object : uxarray.core.Grid
-        Dataset with the unstructured grid.
+    uxgrid : uxarray.Grid
+        Initialized Grid Object from Input Grid File
 
     Examples
     --------
 
     Open dataset with a grid topology file
 
     >>> import uxarray as ux
     >>> uxgrid = ux.open_grid("grid_filename.g")
     """
 
-    ## Grid definition
+    # Grid definition
     if isinstance(grid_filename_or_obj,
                   (list, tuple, np.ndarray, xr.DataArray)):
         uxgrid = Grid(grid_filename_or_obj,
                       gridspec=gridspec,
+                      vertices=vertices,
                       islatlon=islatlon,
                       isconcave=isconcave,
+                      source_grid=str(grid_filename_or_obj),
                       use_dual=use_dual)
     else:
         grid_ds = xr.open_dataset(grid_filename_or_obj,
                                   decode_times=False,
                                   **kwargs)  # type: ignore
 
         uxgrid = Grid(grid_ds,
                       gridspec=gridspec,
+                      vertices=vertices,
                       islatlon=islatlon,
                       isconcave=isconcave,
-                      source_grid=grid_filename_or_obj,
+                      source_grid=str(grid_filename_or_obj),
                       use_dual=use_dual)
 
     return uxgrid
 
 
 def open_dataset(grid_filename_or_obj: str,
                  filename_or_obj: str,
                  gridspec: Optional[str] = None,
                  vertices: Optional[list] = None,
                  islatlon: Optional[bool] = False,
                  isconcave: Optional[bool] = False,
                  use_dual: Optional[bool] = False,
-                 **kwargs: Dict[str, Any]) -> xr.Dataset:
+                 **kwargs: Dict[str, Any]) -> UxDataset:
     """Wraps ``xarray.open_dataset()``, given a grid topology definition with a
     single dataset file or object with corresponding data.
 
     Parameters
     ----------
 
     grid_filename_or_obj : string, required
@@ -120,14 +127,17 @@
 
     isconcave: bool, optional
         Specify if this grid has concave elements (internal checks for this are possible)
 
     gridspec: str, optional
         Specifies gridspec
 
+    vertices: bool, optional
+        Whether to create grid from vertices
+
     source_grid: str, optional
         Path or URL to the source grid file. For diagnostic/reporting purposes only.
 
     use_dual: bool, optional
             Specify whether to use the primal (use_dual=False) or dual (use_dual=True) mesh if the file type is mpas
 
     **kwargs : Dict[str, Any]
@@ -135,55 +145,51 @@
         [xarray
         docs](https://xarray.pydata.org/en/stable/generated/xarray.open_dataset.html)
         for accepted keyword arguments.
 
     Returns
     -------
 
-    object : uxarray.core.UxDataset
-        Dataset with the unstructured grid.
+    uxds : uxarray.UxDataset
+        Dataset with linked `uxgrid` property of type `Grid`.
 
     Examples
     --------
 
     Open dataset with a grid topology file
 
     >>> import uxarray as ux
     >>> ux_ds = ux.open_dataset("grid_filename.g", "grid_filename_vortex.nc")
     """
 
-    grid_ds = xr.open_dataset(grid_filename_or_obj,
-                              decode_times=False,
-                              **kwargs)  # type: ignore
-    ds = xr.open_dataset(filename_or_obj, decode_times=False,
-                         **kwargs)  # type: ignore
-
     ## Grid definition
-    uxgrid = Grid(grid_ds,
-                  gridspec=gridspec,
-                  vertices=vertices,
-                  islatlon=islatlon,
-                  isconcave=isconcave,
-                  source_grid=grid_filename_or_obj,
-                  use_dual=use_dual)
+    uxgrid = open_grid(grid_filename_or_obj,
+                       gridspec=gridspec,
+                       vertices=vertices,
+                       islatlon=islatlon,
+                       isconcave=isconcave,
+                       use_dual=use_dual)
 
     ## UxDataset
+    ds = xr.open_dataset(filename_or_obj, decode_times=False,
+                         **kwargs)  # type: ignore
+
     uxds = UxDataset(ds, uxgrid=uxgrid, source_datasets=str(filename_or_obj))
 
     return uxds
 
 
 def open_mfdataset(grid_filename_or_obj: str,
                    paths: Union[str, os.PathLike],
                    gridspec: Optional[str] = None,
                    vertices: Optional[list] = None,
                    islatlon: Optional[bool] = False,
                    isconcave: Optional[bool] = False,
                    use_dual: Optional[bool] = False,
-                   **kwargs: Dict[str, Any]) -> xr.Dataset:
+                   **kwargs: Dict[str, Any]) -> UxDataset:
     """Wraps ``xarray.open_mfdataset()``, given a single grid topology file
     with multiple dataset paths with corresponding data.
 
     Parameters
     ----------
 
     grid_filename_or_obj : string, required
@@ -200,14 +206,17 @@
 
     isconcave: bool, optional
         Specify if this grid has concave elements (internal checks for this are possible)
 
     gridspec: str, optional
         Specifies gridspec
 
+    vertices: bool, optional
+        Whether to create grid from vertices
+
     source_grid: str, optional
         Path or URL to the source grid file. For diagnostic/reporting purposes only.
 
     use_dual: bool, optional
             Specify whether to use the primal (use_dual=False) or dual (use_dual=True) mesh if the file type is mpas
 
     **kwargs : Dict[str, Any]
@@ -215,37 +224,40 @@
         [xarray
         docs](https://xarray.pydata.org/en/stable/generated/xarray.open_mfdataset.html)
         for accepted keyword arguments.
 
     Returns
     -------
 
-    object : uxarray.core.UxDataset
+    object : uxarray.UxDataset
         Dataset with the unstructured grid.
 
     Examples
     --------
 
     Open grid file along with multiple data files (two or more)
 
     >>> import uxarray as ux
+
+    1. Open from an explicit list of dataset files
+
     >>> ux_ds = ux.open_mfdataset("grid_filename.g", "grid_filename_vortex_1.nc", "grid_filename_vortex_2.nc")
-    """
 
-    grid_ds = xr.open_dataset(grid_filename_or_obj,
-                              decode_times=False,
-                              **kwargs)  # type: ignore
-    ds = xr.open_mfdataset(paths, decode_times=False, **kwargs)  # type: ignore
+    2. Open from a string glob
+
+    >>> ux_ds = ux.open_mfdataset("grid_filename.g", "grid_filename_vortex_*.nc")
+    """
 
     ## Grid definition
-    uxgrid = Grid(grid_ds,
-                  gridspec=gridspec,
-                  vertices=vertices,
-                  islatlon=islatlon,
-                  isconcave=isconcave,
-                  source_grid=grid_filename_or_obj,
-                  use_dual=use_dual)
+    uxgrid = open_grid(grid_filename_or_obj,
+                       gridspec=gridspec,
+                       vertices=vertices,
+                       islatlon=islatlon,
+                       isconcave=isconcave,
+                       use_dual=use_dual)
 
     ## UxDataset
+    ds = xr.open_mfdataset(paths, decode_times=False, **kwargs)  # type: ignore
+
     uxds = UxDataset(ds, uxgrid=uxgrid, source_datasets=str(paths))
 
     return uxds
```

### Comparing `uxarray-2023.5.0.dev0/uxarray/core/dataset.py` & `uxarray-2023.6.0/uxarray/core/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,38 @@
 from typing import Optional, IO
 
 from uxarray.core.dataarray import UxDataArray
 from uxarray.core.grid import Grid
 
 
 class UxDataset(xr.Dataset):
+    """A ``xarray.Dataset``-like, multi-dimensional, in memory, array database.
+    Inherits from ``xarray.Dataset`` and has its own unstructured grid-aware
+    dataset operators and attributes through the ``uxgrid`` accessor.
+
+    Parameters
+    ----------
+    uxgrid : uxarray.Grid, optional
+        The ``Grid`` object that makes this array aware of the unstructured
+        grid topology it belongs to.
+
+        If ``None``, it needs to be an instance of ``uxarray.Grid``.
+
+    Other Parameters
+    ----------------
+    *args:
+        Arguments for the ``xarray.Dataset`` class
+    **kwargs:
+        Keyword arguments for the ``xarray.Dataset`` class
+
+    Notes
+    -----
+    See `xarray.Dataset <https://docs.xarray.dev/en/stable/generated/xarray.Dataset.html>`__
+    for further information about Datasets.
+    """
 
     # expected instance attributes, required for subclassing with xarray (as of v0.13.0)
     __slots__ = (
         '_uxgrid',
         '_source_datasets',
     )
 
@@ -27,133 +51,171 @@
 
         self._uxgrid = None
         self._source_datasets = source_datasets
         # setattr(self, 'source_datasets', source_datasets)
 
         if uxgrid is not None and not isinstance(uxgrid, Grid):
             raise RuntimeError(
-                "uxarray.core.UxDataset.__init__: uxgrid can be either None or "
-                "an instance of the uxarray.core.Grid class")
+                "uxarray.UxDataset.__init__: uxgrid can be either None or "
+                "an instance of the `uxarray.Grid` class")
         else:
             self.uxgrid = uxgrid
 
         super().__init__(*args, **kwargs)
 
     def __getitem__(self, key):
-        """Override to check if the result is an instance of xarray.DataArray.
-
-        If so, convert to UxDataArray.
-        """
+        """Override to make sure the result is an instance of
+        ``uxarray.UxDataArray`` or ``uxarray.UxDataset``."""
 
         value = super().__getitem__(key)
 
         if isinstance(value, xr.DataArray):
             value = UxDataArray(value, uxgrid=self.uxgrid)
+        elif isinstance(value, xr.Dataset):
+            value = UxDataset(value,
+                              uxgrid=self.uxgrid,
+                              source_datasets=self.source_datasets)
 
         return value
 
-    def __setitem__(self, key, value):
-        """Override to check if the value being set is an instance of
-        xarray.DataArray.
-
-        If so, convert to UxDataArray.
-        """
-        if isinstance(value, xr.DataArray):
-            value = UxDataArray(value, uxgrid=self.uxgrid)
-            # works with the value below also.
-            # value = value.to_dataarray()
-
-        super().__setitem__(key, value)
+    # def __setitem__(self, key, value):
+    #     """Override to make sure the `value` is an instance of
+    #     ``uxarray.UxDataArray``."""
+    #     if isinstance(value, xr.DataArray):
+    #         value = UxDataArray(value, uxgrid=self.uxgrid)
+    #
+    #     if isinstance(value, UxDataArray):
+    #         value = value.to_dataarray()
+    #
+    #     super().__setitem__(key, value)
 
     @property
     def source_datasets(self):
+        """Property to keep track of the source data sets used to instantiate
+        this ``uxarray.UxDataset``.
+
+        Can be used as metadata for diagnosis purposes.
+
+        Examples
+        --------
+        uxds = ux.open_dataset(grid_path, data_path)
+        uxds.source_datasets
+        """
         return self._source_datasets
 
     # a setter function
     @source_datasets.setter
     def source_datasets(self, source_datasets_input):
         self._source_datasets = source_datasets_input
 
     @property
     def uxgrid(self):
+        """``uxarray.Grid`` property for ``uxarray.UxDataset`` to make it
+        unstructured grid-aware.
+
+        Examples
+        --------
+        uxds = ux.open_dataset(grid_path, data_path)
+        uxds.uxgrid
+        """
         return self._uxgrid
 
     # a setter function
     @uxgrid.setter
     def uxgrid(self, ugrid_obj):
         self._uxgrid = ugrid_obj
 
-    def _construct_dataarray(self, name) -> UxDataArray:
-        """Override to check if the result is an instance of xarray.DataArray.
+    def _calculate_binary_op(self, *args, **kwargs):
+        """Override to make the result a complete instance of
+        ``uxarray.UxDataset``."""
+        ds = super()._calculate_binary_op(*args, **kwargs)
 
-        If so, convert to UxDataArray.
-        """
+        if isinstance(ds, UxDataset):
+            ds.uxgrid = self.uxgrid
+            ds.source_datasets = self.source_datasets
+        else:
+            ds = UxDataset(ds,
+                           uxgrid=self.uxgrid,
+                           source_datasets=self.source_datasets)
+
+        return ds
+
+    def _construct_dataarray(self, name) -> UxDataArray:
+        """Override to make the result an instance of
+        ``uxarray.UxDataArray``."""
         xarr = super()._construct_dataarray(name)
         return UxDataArray(xarr, uxgrid=self.uxgrid)
 
     @classmethod
     def _construct_direct(cls, *args, **kwargs):
+        """Override to make the result an ``uxarray.UxDataset`` class."""
+
         return cls(xr.Dataset._construct_direct(*args, **kwargs))
 
     def _copy(self, **kwargs):
         """Override to make the result a complete instance of
-        uxarray.Dataset."""
+        ``uxarray.UxDataset``."""
         copied = super()._copy(**kwargs)
 
         deep = kwargs.get('deep', None)
 
         if deep == True:
             # Reinitialize the uxgrid assessor
             copied.uxgrid = self.uxgrid.copy()  # deep copy
         else:
             # Point to the existing uxgrid object
             copied.uxgrid = self.uxgrid
 
         return copied
 
     def _replace(self, *args, **kwargs):
+        """Override to make the result a complete instance of
+        ``uxarray.UxDataset``."""
         ds = super()._replace(*args, **kwargs)
 
         if isinstance(ds, UxDataset):
             ds.uxgrid = self.uxgrid
             ds.source_datasets = self.source_datasets
         else:
             ds = UxDataset(ds,
                            uxgrid=self.uxgrid,
                            source_datasets=self.source_datasets)
 
         return ds
 
     @classmethod
     def from_dataframe(cls, dataframe):
-        """Convert to a UxDataset instead of an xarray.Dataset."""
+        """Override to make the result a ``uxarray.UxDataset`` class."""
+
         return cls(
             {
                 col: ('index', dataframe[col].values)
                 for col in dataframe.columns
             },
             coords={'index': dataframe.index})
 
     @classmethod
     def from_dict(cls, data, **kwargs):
-        """Convert to a UxDataset instead of an xarray.Dataset."""
+        """Override to make the result a ``uxarray.UxDataset`` class."""
+
         return cls({key: ('index', val) for key, val in data.items()},
                    coords={'index': range(len(next(iter(data.values()))))},
                    **kwargs)
 
     def info(self, buf: IO = None, show_attrs=False) -> None:
-        """
-        Concise summary of a Dataset variables and attributes including
-        grid topology information stored in the (``uxgrid``) accessor
+        """Concise summary of Dataset variables and attributes including grid
+        topology information stored in the ``uxgrid`` property.
+
         Parameters
         ----------
         buf : file-like, default: sys.stdout
             writable buffer
         show_attrs : bool
             Flag to select whether to show attributes
+
         See Also
         --------
         pandas.DataFrame.assign
         ncdump : netCDF's ncdump
         """
         if buf is None:  # pragma: no cover
             buf = sys.stdout
@@ -218,21 +280,28 @@
         >>> integral = uxds.integrate()
         """
         integral = 0.0
 
         # call function to get area of all the faces as a np array
         face_areas = self.uxgrid.compute_face_areas(quadrature_rule, order)
 
-        # TODO: Fix this requirement. It should be applicable to
-        # TODO: either all variables of dataset or a dataarray instead.
+        # TODO: Should we fix this requirement? Shouldn't it be applicable to
+        # TODO: all variables of dataset or a dataarray instead?
         var_key = list(self.keys())
         if len(var_key) > 1:
             # warning: print message
             print(
                 "WARNING: The dataset has more than one variable, using the first variable for integration"
             )
 
         var_key = var_key[0]
         face_vals = self[var_key].to_numpy()
         integral = np.dot(face_areas, face_vals)
 
         return integral
+
+    def to_array(self) -> UxDataArray:
+        """Override to make the result an instance of
+        ``uxarray.UxDataArray``."""
+
+        xarr = super().to_array()
+        return UxDataArray(xarr, uxgrid=self.uxgrid)
```

### Comparing `uxarray-2023.5.0.dev0/uxarray/core/grid.py` & `uxarray-2023.6.0/uxarray/core/grid.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""uxarray grid module."""
+"""uxarray.core.grid module."""
 import xarray as xr
 import numpy as np
 
 # reader and writer imports
 from uxarray.io._exodus import _read_exodus, _encode_exodus
 from uxarray.io._mpas import _read_mpas
 from uxarray.io._ugrid import _read_ugrid, _encode_ugrid
@@ -11,54 +11,57 @@
 from uxarray.utils.helpers import (get_all_face_area_from_coords,
                                    parse_grid_type, node_xyz_to_lonlat_rad,
                                    node_lonlat_rad_to_xyz, close_face_nodes)
 from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 
 class Grid:
-    """
-    Examples
+    """Unstructured grid topology definition.
+
+    Can be used standalone to explore an unstructured grid topology, or
+    can be seen as the property of ``uxarray.UxDataset`` and ``uxarray.DataArray``
+    to make them unstructured grid-aware data sets and arrays.
+
+    Parameters
     ----------
+    input_obj : xarray.Dataset, ndarray, list, tuple, required
+        Input ``xarray.Dataset`` or vertex coordinates that form faces.
 
-    Open an exodus file with Uxarray Grid object
+    Other Parameters
+    ----------------
+    gridspec: bool, optional
+        Specifies gridspec
+    islatlon : bool, optional
+        Specify if the grid is lat/lon based
+    isconcave: bool, optional
+        Specify if this grid has concave elements (internal checks for this are possible)
+    use_dual: bool, optional
+        Specify whether to use the primal (use_dual=False) or dual (use_dual=True) mesh if the file type is mpas
 
-    >>> xarray_obj = xr.open_dataset("filename.g")
-    >>> mesh = ux.Grid(xarray_obj)
+    Raises
+    ------
+        RuntimeError
+            If specified file not found or recognized
 
-    Encode as the UGRID format
+    Examples
+    ----------
 
-    >>> mesh.encode_as("ugrid")
-    """
+    >>> import uxarray as ux
 
-    def __init__(self, input_obj, **kwargs):
-        """Initialize grid variables, decide if loading happens via file, verts
-        or gridspec.
+    1. Open a grid file with `uxarray.open_grid()`:
 
-        Parameters
-        ----------
-        input_obj : xarray.Dataset, ndarray, list, tuple, required
-            Input xarray.Dataset or vertex coordinates that form faces.
+    >>> uxgrid = ux.open_grid("filename.g")
 
-        Other Parameters
-        ----------------
-        gridspec: bool, optional
-            Specifies gridspec
-        islatlon : bool, optional
-            Specify if the grid is lat/lon based
-        isconcave: bool, optional
-            Specify if this grid has concave elements (internal checks for this are possible)
-        use_dual: bool, optional
-            Specify whether to use the primal (use_dual=False) or dual (use_dual=True) mesh if the file type is mpas
+    2. Open an unstructured grid dataset file with
+    `uxarray.open_dataset()`, then access `Grid` info:
 
-        Raises
-        ------
-            RuntimeError
-                If specified file not found or recognized
-        """
+    >>> uxds = ux.open_dataset("filename.g")
+    """
 
+    def __init__(self, input_obj, **kwargs):
         # initialize internal variable names
         self.__init_grid_var_names__()
 
         # initialize face_area variable
         self._face_areas = None
 
         # TODO: fix when adding/exercising gridspec
@@ -71,14 +74,15 @@
         ]
         for key in kwargs_list:
             setattr(self, key, kwargs.get(key, None))
 
         # check if initializing from verts:
         if isinstance(input_obj, (list, tuple, np.ndarray)):
             input_obj = np.asarray(input_obj)
+            self.mesh_type = "From vertices"
             # grid with multiple faces
             if input_obj.ndim == 3:
                 self.__from_vert__(input_obj)
                 self.source_grid = "From vertices"
             # grid with a single face
             elif input_obj.ndim == 2:
                 input_obj = np.array([input_obj])
@@ -94,21 +98,20 @@
         # TODO: re-add gridspec initialization when implemented
         elif isinstance(input_obj, xr.Dataset):
             self.mesh_type = parse_grid_type(input_obj)
             self.__from_ds__(dataset=input_obj)
         else:
             raise RuntimeError("Dataset is not a valid input type.")
 
-        # initialize convenience attributes
-        self.__init_grid_var_attrs__()
-
-        # construct connectivity
-        self._build_edge_node_connectivity()
+        # {"Standardized Name" : "Original Name"}
+        self._inverse_grid_var_names = {
+            v: k for k, v in self.grid_var_names.items()
+        }
 
-        # build face dimension, possibly safeguard for large datasets
+        # construct nNodes_per_Face
         self._build_nNodes_per_face()
 
     def __init_grid_var_names__(self):
         """Populates a dictionary for storing uxarray's internal representation
         of xarray object.
 
         Note ugrid conventions are flexible with names of variables, see:
@@ -122,49 +125,14 @@
             "Mesh2_face_nodes": "Mesh2_face_nodes",
             # initialize dims
             "nMesh2_node": "nMesh2_node",
             "nMesh2_face": "nMesh2_face",
             "nMaxMesh2_face_nodes": "nMaxMesh2_face_nodes"
         }
 
-    def __init_grid_var_attrs__(self) -> None:
-        """Initialize attributes for directly accessing UGRID dimensions and
-        variables.
-
-        Examples
-        ----------
-        Assuming the mesh node coordinates for longitude are stored with an input
-        name of 'mesh_node_x', we store this variable name in the `grid_var_names`
-        dictionary with the key 'Mesh2_node_x'. In order to access it, we do:
-
-        >>> x = grid._ds[grid.grid_var_names["Mesh2_node_x"]]
-
-        With the help of this function, we can directly access it through the
-        use of a standardized name based on the UGRID conventions
-
-        >>> x = grid.Mesh2_node_x
-        """
-
-        # Iterate over dict to set access attributes
-        for key, value in self.grid_var_names.items():
-            # Set Attributes for Data Variables
-            if self._ds.data_vars is not None:
-                if value in self._ds.data_vars:
-                    setattr(self, key, self._ds[value])
-
-            # Set Attributes for Coordinates
-            if self._ds.coords is not None:
-                if value in self._ds.coords:
-                    setattr(self, key, self._ds[value])
-
-            # Set Attributes for Dimensions
-            if self._ds.dims is not None:
-                if value in self._ds.dims:
-                    setattr(self, key, len(self._ds[value]))
-
     def __from_vert__(self, dataset):
         """Create a grid with faces constructed from vertices specified by the
         given argument.
 
         Parameters
         ----------
         dataset : ndarray, list, tuple, required
@@ -279,14 +247,269 @@
             else:
                 self._ds = _read_mpas(dataset)
         else:
             raise RuntimeError("unknown mesh type")
 
         dataset.close()
 
+    def __repr__(self):
+        """Constructs a string representation of the contents of a ``Grid``."""
+
+        prefix = "<uxarray.Grid>\n"
+        original_grid_str = f"Original Grid Type: {self.mesh_type}\n"
+        dims_heading = "Grid Dimensions:\n"
+        dims_str = ""
+        # if self.grid_var_names["Mesh2_node_x"] in self._ds:
+        #     dims_str += f"  * nMesh2_node: {self.nMesh2_node}\n"
+        # if self.grid_var_names["Mesh2_face_nodes"] in self._ds:
+        #     dims_str += f"  * nMesh2_face: {self.nMesh2_face}\n"
+        #     dims_str += f"  * nMesh2_face: {self.nMesh2_face}\n"
+
+        for key, value in zip(self._ds.dims.keys(), self._ds.dims.values()):
+            if key in self._inverse_grid_var_names:
+                dims_str += f"  * {self._inverse_grid_var_names[key]}: {value}\n"
+
+        if "nMesh2_edge" in self._ds.dims:
+            dims_str += f"  * nMesh2_edge: {self.nMesh2_edge}\n"
+
+        if "nMaxMesh2_face_edges" in self._ds.dims:
+            dims_str += f"  * nMaxMesh2_face_edges: {self.nMaxMesh2_face_edges}\n"
+
+        coord_heading = "Grid Coordinate Variables:\n"
+        coords_str = ""
+        if self.grid_var_names["Mesh2_node_x"] in self._ds:
+            coords_str += f"  * Mesh2_node_x: {self.Mesh2_node_x.shape}\n"
+            coords_str += f"  * Mesh2_node_y: {self.Mesh2_node_y.shape}\n"
+        if "Mesh2_node_cart_x" in self._ds:
+            coords_str += f"  * Mesh2_node_cart_x: {self.Mesh2_node_cart_x.shape}\n"
+            coords_str += f"  * Mesh2_node_cart_y: {self.Mesh2_node_cart_y.shape}\n"
+            coords_str += f"  * Mesh2_node_cart_z: {self.Mesh2_node_cart_z.shape}\n"
+        if "Mesh2_face_x" in self._ds:
+            coords_str += f"  * Mesh2_face_x: {self.Mesh2_face_x.shape}\n"
+            coords_str += f"  * Mesh2_face_y: {self.Mesh2_face_y.shape}\n"
+
+        connectivity_heading = "Grid Connectivity Variables:\n"
+        connectivity_str = ""
+        if self.grid_var_names["Mesh2_face_nodes"] in self._ds:
+            connectivity_str += f"  * Mesh2_face_nodes: {self.Mesh2_face_nodes.shape}\n"
+        if "Mesh2_edge_nodes" in self._ds:
+            connectivity_str += f"  * Mesh2_edge_nodes: {self.Mesh2_edge_nodes.shape}\n"
+        if "Mesh2_face_edges" in self._ds:
+            connectivity_str += f"  * Mesh2_face_edges: {self.Mesh2_face_edges.shape}\n"
+        connectivity_str += f"  * nNodes_per_face: {self.nNodes_per_face.shape}\n"
+
+        return prefix + original_grid_str + dims_heading + dims_str + coord_heading + coords_str + \
+            connectivity_heading + connectivity_str
+
+    # attribute properties
+
+    @property
+    def parsed_attrs(self):
+        """Dictionary of parsed attributes from the source grid."""
+        return self._ds.attrs
+
+    @property
+    def Mesh2(self):
+        """UGRID Attribute ``Mesh2``, which indicates the topology data of a 2D
+        unstructured mesh."""
+        return self._ds[self.grid_var_names["Mesh2"]]
+
+    # dimension properties
+
+    @property
+    def nMesh2_node(self):
+        """UGRID Dimension ``nMesh2_node``, which represents the total number
+        of nodes."""
+        return self._ds[self.grid_var_names["Mesh2_node_x"]].shape[0]
+
+    @property
+    def nMesh2_face(self):
+        """UGRID Dimension ``nMesh2_face``, which represents the total number
+        of faces."""
+        return self._ds[self.grid_var_names["Mesh2_face_nodes"]].shape[0]
+
+    @property
+    def nMesh2_edge(self):
+        """UGRID Dimension ``nMesh2_edge``, which represents the total number
+        of edges."""
+
+        if "Mesh2_edge_nodes" not in self._ds:
+            self._build_edge_node_connectivity(repopulate=True)
+
+        return self._ds['Mesh2_edge_nodes'].shape[0]
+
+    @property
+    def nMaxMesh2_face_nodes(self):
+        """UGRID Dimension ``nMaxMesh2_face_nodes``, which represents the
+        maximum number of faces nodes that a face may contain."""
+        return self.Mesh2_face_nodes.shape[1]
+
+    @property
+    def nMaxMesh2_face_edges(self):
+        """Dimension ``nMaxMesh2_face_edges``, which represents the maximum
+        number of edges per face.
+
+        Equivalent to ``nMaxMesh2_face_nodes``
+        """
+
+        if "Mesh2_face_edges" not in self._ds:
+            self._build_face_edges_connectivity()
+
+        return self._ds["Mesh2_face_edges"].shape[1]
+
+    @property
+    def nNodes_per_face(self):
+        """Dimension Variable ``nNodes_per_face``, which contains the number of
+        non-fill-value nodes per face.
+
+        Dimensions (``nMesh2_nodes``) and DataType ``INT_DTYPE``.
+        """
+        return self._ds["nNodes_per_face"]
+
+    # coordinate properties
+
+    @property
+    def Mesh2_node_x(self):
+        """UGRID Coordinate Variable ``Mesh2_node_x``, which contains the
+        longitude of each node in degrees.
+
+        Dimensions (``nMesh2_node``)
+        """
+        return self._ds[self.grid_var_names["Mesh2_node_x"]]
+
+    @property
+    def Mesh2_node_cart_x(self):
+        """Coordinate Variable ``Mesh2_node_cart_x``, which contains the x
+        location in meters.
+
+        Dimensions (``nMesh2_node``)
+        """
+        if "Mesh2_node_cart_x" not in self._ds:
+            self._populate_cartesian_xyz_coord()
+        return self._ds['Mesh2_node_cart_x']
+
+    @property
+    def Mesh2_face_x(self):
+        """UGRID Coordinate Variable ``Mesh2_face_x``, which contains the
+        longitude of each face center.
+
+        Dimensions (``nMesh2_face``)
+        """
+        if "Mesh2_face_x" in self._ds:
+            return self._ds["Mesh2_face_x"]
+        else:
+            return None
+
+    @property
+    def Mesh2_node_y(self):
+        """UGRID Coordinate Variable ``Mesh2_node_y``, which contains the
+        latitude of each node.
+
+        Dimensions (``nMesh2_node``)
+        """
+        return self._ds[self.grid_var_names["Mesh2_node_y"]]
+
+    @property
+    def Mesh2_node_cart_y(self):
+        """Coordinate Variable ``Mesh2_node_cart_y``, which contains the y
+        location in meters.
+
+        Dimensions (``nMesh2_node``)
+        """
+        if "Mesh2_node_cart_y" not in self._ds:
+            self._populate_cartesian_xyz_coord()
+        return self._ds['Mesh2_node_cart_y']
+
+    @property
+    def Mesh2_face_y(self):
+        """UGRID Coordinate Variable ``Mesh2_face_y``, which contains the
+        latitude of each face center.
+
+        Dimensions (``nMesh2_face``)
+        """
+        if "Mesh2_face_y" in self._ds:
+            return self._ds["Mesh2_face_y"]
+        else:
+            return None
+
+    @property
+    def _Mesh2_node_z(self):
+        """Coordinate Variable ``_Mesh2_node_z``, which contains the level of
+        each node. It is only a placeholder for now as a protected attribute.
+        UXarray does not support this yet and only handles the 2D flexibile
+        meshes.
+
+        If we introduce handling of 3D meshes in the future, it might be only
+        levels, i.e. the same level(s) for all nodes, instead of separate
+        level for each node that ``_Mesh2_node_z`` suggests.
+
+        Dimensions (``nMesh2_node``)
+        """
+        if self.grid_var_names["Mesh2_node_z"] in self._ds:
+            return self._ds[self.grid_var_names["Mesh2_node_z"]]
+        else:
+            return None
+
+    @property
+    def Mesh2_node_cart_z(self):
+        """Coordinate Variable ``Mesh2_node_cart_z``, which contains the z
+        location in meters.
+
+        Dimensions (``nMesh2_node``)
+        """
+        if "Mesh2_node_cart_z" not in self._ds:
+            self._populate_cartesian_xyz_coord()
+        return self._ds['Mesh2_node_cart_z']
+
+    # connectivity properties
+
+    @property
+    def Mesh2_face_nodes(self):
+        """UGRID Connectivity Variable ``Mesh2_face_nodes``, which maps each
+        face to its corner nodes.
+
+        Dimensions (``nMesh2_face``, ``nMaxMesh2_face_nodes``) and
+        DataType ``INT_DTYPE``.
+
+        Faces can have arbitrary length, with _FillValue=-1 used when faces
+        have fewer nodes than MaxNumNodesPerFace.
+
+        Nodes are in counter-clockwise order.
+        """
+
+        return self._ds[self.grid_var_names["Mesh2_face_nodes"]]
+
+    @property
+    def Mesh2_edge_nodes(self):
+        """UGRID Connectivity Variable ``Mesh2_edge_nodes``, which maps every
+        edge to the two nodes that it connects.
+
+        Dimensions (``nMesh2_edge``, ``Two``) and DataType
+        ``INT_DTYPE``.
+
+        Nodes are in arbitrary order.
+        """
+        if "Mesh2_edge_nodes" not in self._ds:
+            self._build_edge_node_connectivity()
+
+        return self._ds['Mesh2_edge_nodes']
+
+    @property
+    def Mesh2_face_edges(self):
+        """UGRID Connectivity Variable ``Mesh2_face_edges``, which maps every
+        face to its edges.
+
+        Dimensions (``nMesh2_face``, ``nMaxMesh2_face_nodes``) and
+        DataType ``INT_DTYPE``.
+        """
+        if "Mesh2_face_edges" not in self._ds:
+            self._build_face_edges_connectivity()
+
+        return self._ds["Mesh2_face_edges"]
+
     def copy(self):
         """Returns a deep copy of this grid."""
         return Grid(xr.Dataset(self._ds),
                     gridspec=self.gridspec,
                     vertices=self.vertices,
                     islatlon=self.islatlon,
                     isconcave=self.isconcave,
@@ -392,15 +615,15 @@
         z = np.zeros((self.nMesh2_node))
 
         # call func to cal face area of all nodes
         x = self.Mesh2_node_x.data
         y = self.Mesh2_node_y.data
         # check if z dimension
         if self.Mesh2.topology_dimension > 2:
-            z = self.Mesh2_node_z.data
+            z = self._Mesh2_node_z.data
 
         # Note: x, y, z are np arrays of type float
         # Using np.issubdtype to check if the type is float
         # if not (int etc.), convert to float, this is to avoid numba errors
         x, y, z = (arr.astype(float)
                    if not np.issubdtype(arr[0], np.floating) else arr
                    for arr in (x, y, z))
@@ -459,57 +682,59 @@
     def face_areas(self):
         """Declare face_areas as a property."""
         # if self._face_areas is not None: it allows for using the cached result
         if self._face_areas is None:
             self.compute_face_areas()
         return self._face_areas
 
-    def integrate(self, var_ds, quadrature_rule="triangular", order=4):
-        """Integrates a xarray.Dataset over all the faces of the given mesh.
-
-        Parameters
-        ----------
-        var_ds : Xarray dataset, required
-            Xarray dataset containing values to integrate on this grid
-        quadrature_rule : str, optional
-            Quadrature rule to use. Defaults to "triangular".
-        order : int, optional
-            Order of quadrature rule. Defaults to 4.
-
-        Returns
-        -------
-        Calculated integral : float
-
-        Examples
-        --------
-        Open grid file only
-
-        >>> xr_grid = xr.open_dataset("grid.ug")
-        >>> grid = ux.Grid.(xr_grid)
-        >>> var_ds = xr.open_dataset("centroid_pressure_data_ug")
-
-        # Compute the integral
-        >>> integral_psi = grid.integrate(var_ds)
-        """
-        integral = 0.0
-
-        # call function to get area of all the faces as a np array
-        face_areas = self.compute_face_areas(quadrature_rule, order)
-
-        var_key = list(var_ds.keys())
-        if len(var_key) > 1:
-            # warning: print message
-            print(
-                "WARNING: The xarray dataset file has more than one variable, using the first variable for integration"
-            )
-        var_key = var_key[0]
-        face_vals = var_ds[var_key].to_numpy()
-        integral = np.dot(face_areas, face_vals)
-
-        return integral
+    # TODO: Make a decision on whether to provide Dataset- or DataArray-specific
+    # functions from within Grid
+    # def integrate(self, var_ds, quadrature_rule="triangular", order=4):
+    #     """Integrates a xarray.Dataset over all the faces of the given mesh.
+    #
+    #     Parameters
+    #     ----------
+    #     var_ds : Xarray dataset, required
+    #         Xarray dataset containing values to integrate on this grid
+    #     quadrature_rule : str, optional
+    #         Quadrature rule to use. Defaults to "triangular".
+    #     order : int, optional
+    #         Order of quadrature rule. Defaults to 4.
+    #
+    #     Returns
+    #     -------
+    #     Calculated integral : float
+    #
+    #     Examples
+    #     --------
+    #     Open grid file only
+    #
+    #     >>> xr_grid = xr.open_dataset("grid.ug")
+    #     >>> grid = ux.Grid.(xr_grid)
+    #     >>> var_ds = xr.open_dataset("centroid_pressure_data_ug")
+    #
+    #     # Compute the integral
+    #     >>> integral_psi = grid.integrate(var_ds)
+    #     """
+    #     integral = 0.0
+    #
+    #     # call function to get area of all the faces as a np array
+    #     face_areas = self.compute_face_areas(quadrature_rule, order)
+    #
+    #     var_key = list(var_ds.keys())
+    #     if len(var_key) > 1:
+    #         # warning: print message
+    #         print(
+    #             "WARNING: The xarray dataset file has more than one variable, using the first variable for integration"
+    #         )
+    #     var_key = var_key[0]
+    #     face_vals = var_ds[var_key].to_numpy()
+    #     integral = np.dot(face_areas, face_vals)
+    #
+    #     return integral
 
     def _build_edge_node_connectivity(self, repopulate=False):
         """Constructs the UGRID connectivity variable (``Mesh2_edge_nodes``)
         and stores it within the internal (``Grid._ds``) and through the
         attribute (``Grid.Mesh2_edge_nodes``).
 
         Additionally, the attributes (``inverse_indices``) and
@@ -589,18 +814,14 @@
                     INT_DTYPE(0),
                 "inverse_indices":
                     inverse_indices,
                 "fill_value_mask":
                     fill_value_mask
             })
 
-        # set standardized attributes
-        setattr(self, "Mesh2_edge_nodes", self._ds['Mesh2_edge_nodes'])
-        setattr(self, "nMesh2_edge", edge_nodes_unique.shape[0])
-
     def _build_face_edges_connectivity(self):
         """Constructs the UGRID connectivity variable (``Mesh2_face_edges``)
         and stores it within the internal (``Grid._ds``) and through the
         attribute (``Grid.Mesh2_face_edges``)."""
         if ("Mesh2_edge_nodes" not in self._ds or
                 "inverse_indices" not in self._ds['Mesh2_edge_nodes'].attrs):
             self._build_edge_node_connectivity(repopulate=True)
@@ -617,18 +838,14 @@
                     "face_edges_connectivity",
                 "start_index":
                     INT_DTYPE(0),
                 "long_name":
                     "Maps every edge to the two nodes that it connects",
             })
 
-        # set standardized attributes
-        setattr(self, "nMaxMesh2_face_edges", inverse_indices.shape[1])
-        setattr(self, "Mesh2_face_edges", self._ds["Mesh2_face_edges"])
-
     def _populate_cartesian_xyz_coord(self):
         """A helper function that populates the xyz attribute in
         UXarray.Grid._ds. This function is called when we need to use the
         cartesian coordinates for each node to do the calculation but the input
         data only has the "Mesh2_node_x" and "Mesh2_node_y" in degree.
 
         Note
@@ -757,29 +974,20 @@
                 "units": "degrees_north",
             })
 
     def _build_nNodes_per_face(self):
         """Constructs ``nNodes_per_face``, which contains the number of non-
         fill-value nodes for each face in ``Mesh2_face_nodes``"""
 
-        # Triangular Mesh (No Fill Values)
-        if not hasattr(self, "nMaxMesh2_face_nodes"):
-            nMaxMesh2_face_nodes = self.Mesh2_face_nodes.shape[1]
-            setattr(self, "nMaxMesh2_face_nodes", nMaxMesh2_face_nodes)
-
         # padding to shape [nMesh2_face, nMaxMesh2_face_nodes + 1]
         closed = np.ones((self.nMesh2_face, self.nMaxMesh2_face_nodes + 1),
                          dtype=INT_DTYPE) * INT_FILL_VALUE
 
         closed[:, :-1] = self.Mesh2_face_nodes.copy()
 
         nNodes_per_face = np.argmax(closed == INT_FILL_VALUE, axis=1)
 
         # add to internal dataset
         self._ds["nNodes_per_face"] = xr.DataArray(
             data=nNodes_per_face,
             dims=["nMesh2_face"],
             attrs={"long_name": "number of non-fill value nodes for each face"})
-
-        # standardized attribute
-
-        setattr(self, "nNodes_per_face", self._ds["nNodes_per_face"])
```

### Comparing `uxarray-2023.5.0.dev0/uxarray/io/_exodus.py` & `uxarray-2023.6.0/uxarray/io/_exodus.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/uxarray/io/_mpas.py` & `uxarray-2023.6.0/uxarray/io/_mpas.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,17 +192,18 @@
     _replace_zeros(cellsOnVertex)
 
     # convert to zero-indexed
     _to_zero_index(cellsOnVertex)
 
     out_ds["Mesh2_face_nodes"] = xr.DataArray(
         data=cellsOnVertex,
-        dims=["nMesh2_face", "Three"],
+        dims=["nMesh2_face", "nMaxMesh2_face_nodes"],
         attrs={
             "cf_role": "face_node_connectivity",
+            "_FillValue": INT_FILL_VALUE,
             "start_index": INT_DTYPE(0)
         })
 
     # vertex indices that saddle a given edge
     cellsOnEdge = np.array(in_ds['cellsOnEdge'].values, dtype=INT_DTYPE)
 
     # replace missing/zero values with fill values
@@ -240,22 +241,22 @@
         out_ds.attrs['sphere_radius'] = in_ds.sphere_radius
     else:
         warnings.warn("Missing Required Attribute: 'sphere_radius'")
 
     # typically a random string used for tracking mesh provenance
     if 'mesh_id' in in_ds.attrs:
         out_ds.attrs['mesh_id'] = in_ds.mesh_id
-    else:
-        warnings.warn("Missing Required Attribute: 'mesh_id'")
+    # else:
+    #     warnings.warn("Missing Required Attribute: 'mesh_id'")
 
     # defines the version of the MPAS Mesh specification the mesh conforms to
     if 'mesh_spec' in in_ds.attrs:
         out_ds.attrs['mesh_spec'] = in_ds.mesh_spec
-    else:
-        warnings.warn("Missing Required Attribute: 'mesh_spec'")
+    # else:
+    #     warnings.warn("Missing Required Attribute: 'mesh_spec'")
 
     # defines if the mesh describes points that lie on the surface of a sphere or not
     if "on_a_sphere" in in_ds.attrs:
         out_ds.attrs['on_a_sphere'] = in_ds.on_a_sphere
         # required attributes if mesh does not lie on a sphere
         if in_ds.on_a_sphere == "NO":
             # defines if the mesh has any periodic boundaries
```

### Comparing `uxarray-2023.5.0.dev0/uxarray/io/_scrip.py` & `uxarray-2023.6.0/uxarray/io/_scrip.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/uxarray/io/_ugrid.py` & `uxarray-2023.6.0/uxarray/io/_ugrid.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/uxarray/utils/get_quadratureDG.py` & `uxarray-2023.6.0/uxarray/utils/get_quadratureDG.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/uxarray/utils/helpers.py` & `uxarray-2023.6.0/uxarray/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.5.0.dev0/uxarray.egg-info/PKG-INFO` & `uxarray-2023.6.0/uxarray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2023.5.0.dev0
+Version: 2023.6.0
 Summary: Unstructured grid model reading and recognizing with xarray.
 Home-page: https://github.com/UXARRAY/uxarray
 Maintainer: UXARRAY
 Maintainer-email: 
 Project-URL: Source, https://github.com/UXARRAY/uxarray
 Project-URL: Tracker, https://github.com/UXARRAY/uxarray/issues
 Classifier: Operating System :: OS Independent
@@ -26,36 +26,36 @@
 | **License**  |                                                                        [![License][license-badge]][repo-link]                |
 | **Citing**   |                                                                              [![DOI][doi-badge]][doi-link]                   |
 
 
 
 UXarray aims to address the geoscience community need for tools that enable
 standard data analysis techniques to operate directly on unstructured grid
-data. UXarray will provide Xarray styled functions to better read in and use
+data. UXarray provides Xarray styled functions to better read in and use
 unstructured grid datasets that follow standard conventions, including UGRID,
-SCRIP, Exodus and shapefile formats.  This effort is a result of the
+MPAS, SCRIP, and Exodus formats.  This effort is a result of the
 collaboration between Project Raijin (NCAR and Pennsylvania State University)
 and the SEATS Project (Argonne National Laboratory, UC Davis, and Lawrence
 Livermore National Laboratory). The UXarray team welcomes other community
 members to become part of this collaboration at any level of contribution.
 
 UXarray is implemented in pure Python and does not explicitly contain or require
 any compiled code. This makes UXarray more accessible to the general Python
 community. Any contributions to this repository in pure Python are welcome and
 documentation for contribution guidelines can be found when clicking `New Issue`
 under the `Issues` tab in the UXarray repository.
 
 # Why is the name "UXarray"?
 
 We have created UXarray based on [Xarray](https://docs.xarray.dev/en/stable/)
-(via composition of a Xarray dataset object), a Pangeo ecosystem package
+(via inheritance of Xarray Dataset and DataArray classes), a Pangeo ecosystem package
 commonly-used for structured grids recognition, to support reading and
 recognizing unstructured grid model outputs. We picked the name "UXarray"
-and preferred to capitalize the first two letters to emphasize it is Xarray
-for Unstructured grids.
+(pronounced "you-ex-array") and preferred to capitalize the first two letters to
+emphasize it builds upon Xarray for Unstructured grids.
 
 # UXarray Functionality
 
 The following intended functionality has been inspired by discussions with
 members of the scientific community, within the SEATS Project and Project
 Raijin, and on several community platforms such as [Xarray GitHub
 Repository](https://github.com/pydata/xarray/issues/4222). The UXarray team
```

### Comparing `uxarray-2023.5.0.dev0/uxarray.egg-info/SOURCES.txt` & `uxarray-2023.6.0/uxarray.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .github/workflows/pre-commit.yml
 .github/workflows/pypi.yaml
 .github/workflows/upstream-dev-ci.yml
 ci/docs.yml
 ci/environment.yml
 ci/upstream-dev-environment.yml
 docs/Makefile
+docs/announcement.rst
 docs/api.rst
 docs/citation.rst
 docs/conf.py
 docs/contributing.rst
 docs/examples.rst
 docs/gallery.yml
 docs/index.rst
@@ -45,17 +46,20 @@
 docs/_static/images/logos/EarthCube_logo.png
 docs/_static/images/logos/NSF_logo.png
 docs/_static/images/logos/PANGEO_logo.png
 docs/_static/images/logos/uxarray_temp_logo.png
 docs/_static/thumbnails/default.svg
 docs/_templates/breadcrumbs.html
 docs/examples/000-template.ipynb
-docs/examples/001-read-grid-data.ipynb
-docs/examples/002-access-grid-info.ipynb
+docs/examples/001-working-with-unstructured-grids.ipynb
+docs/examples/002-grid-topology.ipynb
 docs/examples/003-area-calc.ipynb
+docs/getting-started/freq-asked-questions.rst
+docs/getting-started/overview.rst
+docs/getting-started/quick-install.rst
 docs/internal_api/index.rst
 docs/user_api/index.rst
 docs/user_api/uxarray_api.md
 test/__init__.py
 test/constants.py
 test/test_api.py
 test/test_dataset.py
```

