# Comparing `tmp/specutils-1.9.0.tar.gz` & `tmp/specutils-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specutils-1.9.0.tar", last modified: Tue Oct 18 19:43:31 2022, max compression
+gzip compressed data, was "specutils-1.9.1.tar", last modified: Tue Nov 22 16:36:03 2022, max compression
```

## Comparing `specutils-1.9.0.tar` & `specutils-1.9.1.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.750897 specutils-1.9.0/
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.637355 specutils-1.9.0/.github/
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.649281 specutils-1.9.0/.github/workflows/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1909 2022-09-08 18:05:22.000000 specutils-1.9.0/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3642 2022-10-18 19:06:04.000000 specutils-1.9.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      791 2022-01-27 16:59:43.000000 specutils-1.9.0/.gitignore
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      195 2022-02-08 17:26:33.000000 specutils-1.9.0/.readthedocs.yml
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    15066 2022-10-18 19:40:45.000000 specutils-1.9.0/CHANGES.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      467 2020-03-04 17:43:46.000000 specutils-1.9.0/CITATION
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      279 2022-01-27 16:59:43.000000 specutils-1.9.0/MANIFEST.in
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5120 2022-10-18 19:43:31.751197 specutils-1.9.0/PKG-INFO
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4741 2022-01-27 16:59:43.000000 specutils-1.9.0/README.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      313 2022-02-08 17:26:33.000000 specutils-1.9.0/conftest.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.667501 specutils-1.9.0/docs/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4581 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/Makefile
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.672426 specutils-1.9.0/docs/_static/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)   115135 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/_static/logo.png
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4414 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/_static/logo_icon.ico
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    62134 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/_static/logo_icon.png
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      274 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/_static/specutils.css
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.637919 specutils-1.9.0/docs/_templates/
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.675556 specutils-1.9.0/docs/_templates/autosummary/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      250 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      251 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      252 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    13196 2022-03-28 16:55:39.000000 specutils-1.9.0/docs/analysis.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3398 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/arithmetic.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     8193 2022-02-08 17:26:33.000000 specutils-1.9.0/docs/conf.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3263 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/contributing.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5982 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/custom_loading.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    25730 2022-09-09 16:44:33.000000 specutils-1.9.0/docs/fitting.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1556 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/identify.rst
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.677503 specutils-1.9.0/docs/img/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    74630 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/img/quick_start.png
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    30470 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/img/read_1d.png
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4707 2022-02-17 21:36:06.000000 specutils-1.9.0/docs/index.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1321 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/installation.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4549 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/make.bat
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    18939 2022-10-18 19:29:55.000000 specutils-1.9.0/docs/manipulation.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2218 2022-10-18 19:06:04.000000 specutils-1.9.0/docs/nitpick-exceptions
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1819 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/releasing.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     8794 2022-09-08 18:05:22.000000 specutils-1.9.0/docs/spectral_cube.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12016 2022-03-28 16:55:39.000000 specutils-1.9.0/docs/spectral_regions.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    14404 2022-09-08 18:05:22.000000 specutils-1.9.0/docs/spectrum1d.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3818 2022-02-17 21:36:06.000000 specutils-1.9.0/docs/spectrum_collection.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)   148954 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/specutils_classes_diagrams.png
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    34869 2020-03-04 17:43:46.000000 specutils-1.9.0/docs/specutils_classes_diagrams.pptx
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5014 2022-01-27 16:59:43.000000 specutils-1.9.0/docs/types_of_spectra.rst
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.679188 specutils-1.9.0/licenses/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1480 2022-01-27 16:59:43.000000 specutils-1.9.0/licenses/LICENSE.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      372 2022-01-27 16:59:43.000000 specutils-1.9.0/licenses/README.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1659 2022-01-27 16:59:43.000000 specutils-1.9.0/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      134 2022-01-27 16:59:43.000000 specutils-1.9.0/pyproject.toml
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2473 2022-10-18 19:43:31.752752 specutils-1.9.0/setup.cfg
--rwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)     1958 2022-01-27 16:59:43.000000 specutils-1.9.0/setup.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.682043 specutils-1.9.0/specutils/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      467 2020-03-04 17:43:46.000000 specutils-1.9.0/specutils/CITATION
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1172 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      613 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/_astropy_init.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.687978 specutils-1.9.0/specutils/analysis/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      232 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/analysis/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    10368 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/analysis/correlation.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12050 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/analysis/flux.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5193 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/analysis/location.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2538 2022-09-08 18:05:22.000000 specutils-1.9.0/specutils/analysis/moment.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    10397 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/analysis/template_comparison.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6257 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/analysis/uncertainty.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      700 2020-03-04 17:43:46.000000 specutils-1.9.0/specutils/analysis/utils.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11181 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/analysis/width.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7073 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/conftest.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.689553 specutils-1.9.0/specutils/fitting/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       66 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/fitting/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4005 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/fitting/continuum.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    31366 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/fitting/fitmodels.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.691704 specutils-1.9.0/specutils/io/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       33 2020-03-04 17:43:46.000000 specutils-1.9.0/specutils/io/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1061 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/_list_of_loaders.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.694074 specutils-1.9.0/specutils/io/asdf/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      715 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/asdf/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1325 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/asdf/extension.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.639899 specutils-1.9.0/specutils/io/asdf/schemas/
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.640161 specutils-1.9.0/specutils/io/asdf/schemas/astropy.org/
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.640314 specutils-1.9.0/specutils/io/asdf/schemas/astropy.org/specutils/
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.696505 specutils-1.9.0/specutils/io/asdf/schemas/astropy.org/specutils/spectra/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      921 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectral_coord-1.0.0.yaml
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1282 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectrum1d-1.0.0.yaml
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      386 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectrum_list-1.0.0.yaml
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.697507 specutils-1.9.0/specutils/io/asdf/tags/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/asdf/tags/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3670 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/asdf/tags/spectra.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.698762 specutils-1.9.0/specutils/io/asdf/tags/tests/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/asdf/tags/tests/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2234 2022-09-08 18:05:22.000000 specutils-1.9.0/specutils/io/asdf/tags/tests/test_spectra.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      752 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/asdf/types.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.718615 specutils-1.9.0/specutils/io/default_loaders/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      189 2020-03-04 17:43:46.000000 specutils-1.9.0/specutils/io/default_loaders/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7672 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/aaomega_2df.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6897 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/apogee.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3189 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/ascii.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    17571 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/default_loaders/dc_common.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2726 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/default_loaders/galah.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7147 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/default_loaders/gama.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2677 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/generic_cube.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1837 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/default_loaders/generic_ecsv_reader.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1841 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/hst_cos.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1870 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/hst_stis.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    22649 2022-10-12 21:12:09.000000 specutils-1.9.0/specutils/io/default_loaders/jwst_reader.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3814 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/manga.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2031 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/muscles_sed.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1191 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/default_loaders/ozdes.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     8168 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/sdss.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6871 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/default_loaders/sixdfgs_reader.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2842 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/subaru_pfs_spec.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6715 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/tabular_fits.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.720405 specutils-1.9.0/specutils/io/default_loaders/tests/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2020-03-04 17:43:46.000000 specutils-1.9.0/specutils/io/default_loaders/tests/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1406 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/tests/test_apogee.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    14644 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/tests/test_jwst_reader.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2512 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/default_loaders/twodfgrs_reader.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3803 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/io/default_loaders/twoslaq_lrg.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    28052 2022-09-08 18:05:22.000000 specutils-1.9.0/specutils/io/default_loaders/wcs_fits.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      915 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/default_loaders/wigglez.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12949 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/parsing_utils.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     9014 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/io/registers.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.725706 specutils-1.9.0/specutils/manipulation/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      221 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/manipulation/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2577 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/manipulation/estimate_uncertainty.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11013 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/manipulation/extract_spectral_region.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2591 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/manipulation/manipulation.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7876 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/manipulation/model_replace.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    14576 2022-10-18 19:06:04.000000 specutils-1.9.0/specutils/manipulation/resample.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     9002 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/manipulation/smoothing.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    10543 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/manipulation/utils.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.730001 specutils-1.9.0/specutils/spectra/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      335 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/spectra/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3176 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/spectra/spectral_axis.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/spectra/spectral_coordinate.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11072 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/spectra/spectral_region.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    33492 2022-09-08 18:05:22.000000 specutils-1.9.0/specutils/spectra/spectrum1d.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11065 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/spectra/spectrum_collection.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      600 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/spectra/spectrum_list.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12606 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/spectra/spectrum_mixin.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.747696 specutils-1.9.0/specutils/tests/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      121 2020-03-04 17:43:46.000000 specutils-1.9.0/specutils/tests/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1017 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/tests/conftest.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      643 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/tests/coveragerc
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/tests/setup_package.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    39713 2022-09-08 18:05:22.000000 specutils-1.9.0/specutils/tests/test_analysis.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4065 2022-09-08 18:05:22.000000 specutils-1.9.0/specutils/tests/test_arithmetic.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    10909 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_continuum.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     9132 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_correlation.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    20886 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_dc_common_loaders.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    29370 2022-09-21 18:22:40.000000 specutils-1.9.0/specutils/tests/test_fitting.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7129 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_io.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    59297 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_loaders.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7304 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_manipulation.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4939 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/tests/test_model_replace.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12054 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_region_extract.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6331 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/tests/test_regions.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     8174 2022-09-08 18:05:22.000000 specutils-1.9.0/specutils/tests/test_resample.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4171 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_slicing.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     9167 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_smoothing.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7846 2022-09-08 18:05:22.000000 specutils-1.9.0/specutils/tests/test_spectral_axis.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    18617 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_spectrum1d.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7096 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_spectrum_collection.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    16889 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_template_comparison.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3489 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_unc.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2314 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/tests/test_utils.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.750274 specutils-1.9.0/specutils/utils/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       37 2020-03-04 17:43:46.000000 specutils-1.9.0/specutils/utils/__init__.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2530 2022-01-27 16:59:43.000000 specutils-1.9.0/specutils/utils/quantity_model.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11009 2022-02-17 21:36:06.000000 specutils-1.9.0/specutils/utils/wcs_utils.py
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      337 2022-10-18 19:43:31.000000 specutils-1.9.0/specutils/version.py
-drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-10-18 19:43:31.684190 specutils-1.9.0/specutils.egg-info/
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5120 2022-10-18 19:43:31.000000 specutils-1.9.0/specutils.egg-info/PKG-INFO
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4973 2022-10-18 19:43:31.000000 specutils-1.9.0/specutils.egg-info/SOURCES.txt
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        1 2022-10-18 19:43:31.000000 specutils-1.9.0/specutils.egg-info/dependency_links.txt
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       77 2022-10-18 19:43:31.000000 specutils-1.9.0/specutils.egg-info/entry_points.txt
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        1 2022-10-18 19:43:31.000000 specutils-1.9.0/specutils.egg-info/not-zip-safe
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      189 2022-10-18 19:43:31.000000 specutils-1.9.0/specutils.egg-info/requires.txt
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       10 2022-10-18 19:43:31.000000 specutils-1.9.0/specutils.egg-info/top_level.txt
--rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3085 2022-10-18 19:06:04.000000 specutils-1.9.0/tox.ini
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.630782 specutils-1.9.1/
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.506378 specutils-1.9.1/.github/
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.520169 specutils-1.9.1/.github/workflows/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1909 2022-09-08 18:05:22.000000 specutils-1.9.1/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3642 2022-10-18 19:06:04.000000 specutils-1.9.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      791 2022-01-27 16:59:43.000000 specutils-1.9.1/.gitignore
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      195 2022-02-08 17:26:33.000000 specutils-1.9.1/.readthedocs.yml
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    15277 2022-11-22 16:33:00.000000 specutils-1.9.1/CHANGES.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      467 2020-03-04 17:43:46.000000 specutils-1.9.1/CITATION
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      279 2022-01-27 16:59:43.000000 specutils-1.9.1/MANIFEST.in
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5120 2022-11-22 16:36:03.630966 specutils-1.9.1/PKG-INFO
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4741 2022-01-27 16:59:43.000000 specutils-1.9.1/README.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      313 2022-02-08 17:26:33.000000 specutils-1.9.1/conftest.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.538058 specutils-1.9.1/docs/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4581 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/Makefile
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.543874 specutils-1.9.1/docs/_static/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)   115135 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/_static/logo.png
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4414 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/_static/logo_icon.ico
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    62134 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/_static/logo_icon.png
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      274 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/_static/specutils.css
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.507258 specutils-1.9.1/docs/_templates/
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.546428 specutils-1.9.1/docs/_templates/autosummary/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      250 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      251 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      252 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    13196 2022-03-28 16:55:39.000000 specutils-1.9.1/docs/analysis.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3398 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/arithmetic.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     8193 2022-02-08 17:26:33.000000 specutils-1.9.1/docs/conf.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3263 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/contributing.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5982 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/custom_loading.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    25730 2022-09-09 16:44:33.000000 specutils-1.9.1/docs/fitting.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1556 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/identify.rst
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.548722 specutils-1.9.1/docs/img/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    74630 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/img/quick_start.png
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    30470 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/img/read_1d.png
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4707 2022-02-17 21:36:06.000000 specutils-1.9.1/docs/index.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1321 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/installation.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4549 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/make.bat
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    18939 2022-10-18 19:29:55.000000 specutils-1.9.1/docs/manipulation.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2218 2022-10-18 19:06:04.000000 specutils-1.9.1/docs/nitpick-exceptions
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1819 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/releasing.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     8794 2022-09-08 18:05:22.000000 specutils-1.9.1/docs/spectral_cube.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12016 2022-03-28 16:55:39.000000 specutils-1.9.1/docs/spectral_regions.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    14388 2022-11-22 16:30:22.000000 specutils-1.9.1/docs/spectrum1d.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3818 2022-02-17 21:36:06.000000 specutils-1.9.1/docs/spectrum_collection.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)   148954 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/specutils_classes_diagrams.png
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    34869 2020-03-04 17:43:46.000000 specutils-1.9.1/docs/specutils_classes_diagrams.pptx
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5014 2022-01-27 16:59:43.000000 specutils-1.9.1/docs/types_of_spectra.rst
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.551096 specutils-1.9.1/licenses/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1480 2022-01-27 16:59:43.000000 specutils-1.9.1/licenses/LICENSE.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      372 2022-01-27 16:59:43.000000 specutils-1.9.1/licenses/README.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1659 2022-01-27 16:59:43.000000 specutils-1.9.1/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      134 2022-01-27 16:59:43.000000 specutils-1.9.1/pyproject.toml
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2473 2022-11-22 16:36:03.631978 specutils-1.9.1/setup.cfg
+-rwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)     1958 2022-01-27 16:59:43.000000 specutils-1.9.1/setup.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.555751 specutils-1.9.1/specutils/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      467 2020-03-04 17:43:46.000000 specutils-1.9.1/specutils/CITATION
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1172 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      613 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/_astropy_init.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.567233 specutils-1.9.1/specutils/analysis/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      232 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/analysis/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    10368 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/analysis/correlation.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12050 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/analysis/flux.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5193 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/analysis/location.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2538 2022-09-08 18:05:22.000000 specutils-1.9.1/specutils/analysis/moment.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    10397 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/analysis/template_comparison.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6257 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/analysis/uncertainty.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      700 2020-03-04 17:43:46.000000 specutils-1.9.1/specutils/analysis/utils.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11181 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/analysis/width.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7073 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/conftest.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.569479 specutils-1.9.1/specutils/fitting/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       66 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/fitting/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4005 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/fitting/continuum.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    31366 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/fitting/fitmodels.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.572977 specutils-1.9.1/specutils/io/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       33 2020-03-04 17:43:46.000000 specutils-1.9.1/specutils/io/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1061 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/_list_of_loaders.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.575040 specutils-1.9.1/specutils/io/asdf/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      715 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/asdf/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1325 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/asdf/extension.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.510129 specutils-1.9.1/specutils/io/asdf/schemas/
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.510369 specutils-1.9.1/specutils/io/asdf/schemas/astropy.org/
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.510635 specutils-1.9.1/specutils/io/asdf/schemas/astropy.org/specutils/
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.577155 specutils-1.9.1/specutils/io/asdf/schemas/astropy.org/specutils/spectra/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      921 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectral_coord-1.0.0.yaml
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1282 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectrum1d-1.0.0.yaml
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      386 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectrum_list-1.0.0.yaml
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.577942 specutils-1.9.1/specutils/io/asdf/tags/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/asdf/tags/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3670 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/asdf/tags/spectra.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.578893 specutils-1.9.1/specutils/io/asdf/tags/tests/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/asdf/tags/tests/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2234 2022-09-08 18:05:22.000000 specutils-1.9.1/specutils/io/asdf/tags/tests/test_spectra.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      752 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/asdf/types.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.594969 specutils-1.9.1/specutils/io/default_loaders/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      189 2020-03-04 17:43:46.000000 specutils-1.9.1/specutils/io/default_loaders/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7672 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/aaomega_2df.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6897 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/apogee.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3189 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/ascii.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    18939 2022-11-22 16:30:22.000000 specutils-1.9.1/specutils/io/default_loaders/dc_common.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2726 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/default_loaders/galah.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7147 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/default_loaders/gama.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2677 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/generic_cube.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1837 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/default_loaders/generic_ecsv_reader.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1841 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/hst_cos.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1870 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/hst_stis.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    22649 2022-10-12 21:12:09.000000 specutils-1.9.1/specutils/io/default_loaders/jwst_reader.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3814 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/manga.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2031 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/muscles_sed.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1191 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/default_loaders/ozdes.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     8168 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/sdss.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6871 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/default_loaders/sixdfgs_reader.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2842 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/subaru_pfs_spec.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6715 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/tabular_fits.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.597106 specutils-1.9.1/specutils/io/default_loaders/tests/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2020-03-04 17:43:46.000000 specutils-1.9.1/specutils/io/default_loaders/tests/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1406 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/tests/test_apogee.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    14644 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/tests/test_jwst_reader.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2512 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/default_loaders/twodfgrs_reader.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3803 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/io/default_loaders/twoslaq_lrg.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    28052 2022-09-08 18:05:22.000000 specutils-1.9.1/specutils/io/default_loaders/wcs_fits.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      915 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/default_loaders/wigglez.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12949 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/parsing_utils.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     9014 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/io/registers.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.605020 specutils-1.9.1/specutils/manipulation/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      221 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/manipulation/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2577 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/manipulation/estimate_uncertainty.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11013 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/manipulation/extract_spectral_region.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2591 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/manipulation/manipulation.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7876 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/manipulation/model_replace.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    14576 2022-10-18 19:06:04.000000 specutils-1.9.1/specutils/manipulation/resample.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     9002 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/manipulation/smoothing.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    10543 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/manipulation/utils.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.610936 specutils-1.9.1/specutils/spectra/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      335 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/spectra/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3176 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/spectra/spectral_axis.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/spectra/spectral_coordinate.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11072 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/spectra/spectral_region.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    33670 2022-11-22 16:30:22.000000 specutils-1.9.1/specutils/spectra/spectrum1d.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11065 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/spectra/spectrum_collection.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      600 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/spectra/spectrum_list.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12606 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/spectra/spectrum_mixin.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.628215 specutils-1.9.1/specutils/tests/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      121 2020-03-04 17:43:46.000000 specutils-1.9.1/specutils/tests/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     1017 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/tests/conftest.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      643 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/tests/coveragerc
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        0 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/tests/setup_package.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    39713 2022-09-08 18:05:22.000000 specutils-1.9.1/specutils/tests/test_analysis.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4065 2022-09-08 18:05:22.000000 specutils-1.9.1/specutils/tests/test_arithmetic.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    10909 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_continuum.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     9132 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_correlation.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    20886 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_dc_common_loaders.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    29370 2022-09-21 18:22:40.000000 specutils-1.9.1/specutils/tests/test_fitting.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7129 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_io.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    59297 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_loaders.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7304 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_manipulation.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4939 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/tests/test_model_replace.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    12054 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_region_extract.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     6331 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/tests/test_regions.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     8174 2022-09-08 18:05:22.000000 specutils-1.9.1/specutils/tests/test_resample.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4171 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_slicing.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     9167 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_smoothing.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7846 2022-09-08 18:05:22.000000 specutils-1.9.1/specutils/tests/test_spectral_axis.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    18617 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_spectrum1d.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     7096 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_spectrum_collection.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    16889 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_template_comparison.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3489 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_unc.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2314 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/tests/test_utils.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.630337 specutils-1.9.1/specutils/utils/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       37 2020-03-04 17:43:46.000000 specutils-1.9.1/specutils/utils/__init__.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     2530 2022-01-27 16:59:43.000000 specutils-1.9.1/specutils/utils/quantity_model.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)    11009 2022-02-17 21:36:06.000000 specutils-1.9.1/specutils/utils/wcs_utils.py
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      337 2022-11-22 16:36:03.000000 specutils-1.9.1/specutils/version.py
+drwxr-xr-x   0 rosteen   (2591) STSCI\science  (1031)        0 2022-11-22 16:36:03.559593 specutils-1.9.1/specutils.egg-info/
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     5120 2022-11-22 16:36:03.000000 specutils-1.9.1/specutils.egg-info/PKG-INFO
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     4973 2022-11-22 16:36:03.000000 specutils-1.9.1/specutils.egg-info/SOURCES.txt
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        1 2022-11-22 16:36:03.000000 specutils-1.9.1/specutils.egg-info/dependency_links.txt
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       77 2022-11-22 16:36:03.000000 specutils-1.9.1/specutils.egg-info/entry_points.txt
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)        1 2022-11-22 16:36:03.000000 specutils-1.9.1/specutils.egg-info/not-zip-safe
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)      189 2022-11-22 16:36:03.000000 specutils-1.9.1/specutils.egg-info/requires.txt
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)       10 2022-11-22 16:36:03.000000 specutils-1.9.1/specutils.egg-info/top_level.txt
+-rw-r--r--   0 rosteen   (2591) STSCI\science  (1031)     3085 2022-10-18 19:06:04.000000 specutils-1.9.1/tox.ini
```

### Comparing `specutils-1.9.0/.github/workflows/ci_cron_weekly.yml` & `specutils-1.9.1/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/.github/workflows/ci_workflows.yml` & `specutils-1.9.1/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/.gitignore` & `specutils-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/CHANGES.rst` & `specutils-1.9.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+1.9.1 (2022-11-22)
+------------------
+
+Bug Fixes
+^^^^^^^^^
+
+- Add and subtract operations on Spectrum1D now allow for other operand's class
+  to handle the arithmetic if that class has special handling. [#988]
+
 1.9.0 (2022-10-18)
 ------------------
 
 Bug Fixes
 ^^^^^^^^^
 
 - Fix bug in fitting with weights if weights argument is set to 'unc'. [#979]
```

### Comparing `specutils-1.9.0/PKG-INFO` & `specutils-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specutils
-Version: 1.9.0
+Version: 1.9.1
 Summary: Package for spectroscopic astronomical data
 Home-page: https://specutils.readthedocs.io/
 Author: Specutils Developers
 Author-email: coordinators@astropy.org
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `specutils-1.9.0/README.rst` & `specutils-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/Makefile` & `specutils-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/_static/logo.png` & `specutils-1.9.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/_static/logo_icon.ico` & `specutils-1.9.1/docs/_static/logo_icon.ico`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/_static/logo_icon.png` & `specutils-1.9.1/docs/_static/logo_icon.png`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/analysis.rst` & `specutils-1.9.1/docs/analysis.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/arithmetic.rst` & `specutils-1.9.1/docs/arithmetic.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/conf.py` & `specutils-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/contributing.rst` & `specutils-1.9.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/custom_loading.rst` & `specutils-1.9.1/docs/custom_loading.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/fitting.rst` & `specutils-1.9.1/docs/fitting.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/identify.rst` & `specutils-1.9.1/docs/identify.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/img/quick_start.png` & `specutils-1.9.1/docs/img/quick_start.png`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/img/read_1d.png` & `specutils-1.9.1/docs/img/read_1d.png`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/index.rst` & `specutils-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/installation.rst` & `specutils-1.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/make.bat` & `specutils-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/manipulation.rst` & `specutils-1.9.1/docs/manipulation.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/nitpick-exceptions` & `specutils-1.9.1/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/releasing.rst` & `specutils-1.9.1/docs/releasing.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/spectral_cube.rst` & `specutils-1.9.1/docs/spectral_cube.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/spectral_regions.rst` & `specutils-1.9.1/docs/spectral_regions.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/spectrum1d.rst` & `specutils-1.9.1/docs/spectrum1d.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 .. note::
     The ``spectral_axis`` can also be provided as a :class:`~specutils.SpectralAxis` object,
     and in fact will internally convert the spectral_axis to :class:`~specutils.SpectralAxis` if it
     is provided as an array or `~astropy.units.Quantity`.
 
 .. note::
     The ``spectral_axis`` can be either ascending or descending, but must be monotonic
-    in either case. 
+    in either case.
 
 Reading from a File
 -------------------
 
 ``specutils`` takes advantage of the Astropy IO machinery and allows loading and
 writing to files. The example below shows loading a FITS file. While specutils
 has some basic data loaders, for more complicated or custom files, users are
@@ -93,15 +93,15 @@
 
 The :class:`~specutils.Spectrum1D` class supports uncertainties, and
 arithmetic operations performed with :class:`~specutils.Spectrum1D`
 objects will propagate uncertainties.
 
 Uncertainties are a special subclass of :class:`~astropy.nddata.NDData`, and their
 propagation rules are implemented at the class level. Therefore, users must
-specify the uncertainty type at creation time
+specify the uncertainty type at creation time.
 
 .. code-block:: python
 
     >>> from specutils import Spectrum1D
     >>> from astropy.nddata import StdDevUncertainty
 
     >>> spec = Spectrum1D(spectral_axis=np.arange(5000, 5010)*u.AA, flux=np.random.sample(10)*u.Jy, uncertainty=StdDevUncertainty(np.random.sample(10) * 0.1))
@@ -244,85 +244,85 @@
 any number of dimensions for `~specutils.Spectrum1D`, as long as the spectral
 axis is always the last.
 
 
 Slicing
 -------
 
-As seen above, `~specutils.Spectrum1D` supports slicing in the same way as any 
-other array-like object. Additionally, a `~specutils.Spectrum1D` can be sliced 
-along the spectral axis using world coordinates. 
+As seen above, `~specutils.Spectrum1D` supports slicing in the same way as any
+other array-like object. Additionally, a `~specutils.Spectrum1D` can be sliced
+along the spectral axis using world coordinates.
 
 .. code-block:: python
 
     >>> from specutils import Spectrum1D
 
     >>> spec = Spectrum1D(spectral_axis=np.arange(5000, 5010)*u.AA, flux=np.random.sample((5, 10))*u.Jy)
     >>> spec_slice = spec[5002*u.AA:5006*u.AA]
     >>> spec_slice.spectral_axis
     <SpectralAxis [5002., 5003., 5004., 5005.] Angstrom>
 
-It is also possible to slice on other axes using simple array indices at the 
+It is also possible to slice on other axes using simple array indices at the
 same time as slicing the spectral axis based on spectral values.
 
 .. code-block:: python
 
     >>> from specutils import Spectrum1D
 
     >>> spec = Spectrum1D(spectral_axis=np.arange(5000, 5010)*u.AA, flux=np.random.sample((5, 10))*u.Jy)
     >>> spec_slice = spec[2:4, 5002*u.AA:5006*u.AA]
     >>> spec_slice.shape
     (2, 4)
 
-If the `specutils.Spectrum1D` was created with a WCS that included spatial 
+If the `specutils.Spectrum1D` was created with a WCS that included spatial
 information, for example in case of a spectral cube with two spatial dimensions,
 the `specutils.Spectrum1D.crop` method can be used to subset the data based on
 the world coordinates. The inputs required are two sets up `astropy.coordinates`
 objects defining the upper and lower corner of the region desired. Note that if
 one of the coordinates is decreasing along an axis, the higher world coordinate
 value will apply to the lower bound input.
 
 .. code-block:: python
-    
+
     >>> from astropy.coordinates import SpectralCoord, SkyCoord
     >>> import astropy.units as u
 
     >>> lower = [SkyCoord(ra=201.1, dec=27.5, unit=u.deg), SpectralCoord(3000, unit=u.AA)]
     >>> upper = [SkyCoord(ra=201.08, dec=27.52, unit=u.deg), SpectralCoord(3100, unit=u.AA)]
     >>> cropped_spec = spec.crop(lower, upper) #doctest:+SKIP
 
 Collapsing
 ----------
 
-`~specutils.Spectrum1D` has built-in convenience methods for collapsing the 
+`~specutils.Spectrum1D` has built-in convenience methods for collapsing the
 flux array of the spectrum via various statistics. The available statistics are
-mean, median, sum, max, and min, and may be called either on a specific axis 
+mean, median, sum, max, and min, and may be called either on a specific axis
 (or axes) or over the entire flux array. The collapse methods currently respect
 the ``mask`` attribute of the `~specutils.Spectrum1D`, but do not propagate
 any ``uncertainty`` attached to the spectrum.
 
 .. code-block:: python
 
     >>> spec = Spectrum1D(spectral_axis=np.arange(5000, 5010)*u.AA, flux=np.random.sample((5, 10))*u.Jy)
     >>> spec.mean() # doctest: +IGNORE_OUTPUT
     <Quantity 0.4572145 Jy>
 
 The 'axis' argument of the collapse methods may either be an integer axis, or a
-string specifying either 'spectral', which will collapse along only the 
+string specifying either 'spectral', which will collapse along only the
 spectral axis, or 'spatial', which will collapse along all non-spectral axes.
 
 .. code-block:: python
 
     >>> spec.mean(axis='spatial') # doctest: +IGNORE_OUTPUT
-    <Spectrum1D(flux=<Quantity [0.39985669, ... 0.38041483] Jy>, 
+    <Spectrum1D(flux=<Quantity [0.39985669, ... 0.38041483] Jy>,
                 spectral_axis=<SpectralAxis ... [5000., ... 5009.]>
 
-Note that in this case, the result of the collapse operation is a 
-`~specutils.Spectrum1D` rather than an `astropy.units.Quantity`, because the 
-collapse operation left the spectral axis intact. 
+Note that in this case, the result of the collapse operation is a
+`~specutils.Spectrum1D` rather than an `astropy.units.Quantity`, because the
+collapse operation left the spectral axis intact.
 
 It is also possible to supply your own function for the collapse operation by
 calling `~specutils.Spectrum1D.collapse()` and providing a callable function
 to the ``method`` argument.
 
 .. code-block:: python
```

### Comparing `specutils-1.9.0/docs/spectrum_collection.rst` & `specutils-1.9.1/docs/spectrum_collection.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/specutils_classes_diagrams.png` & `specutils-1.9.1/docs/specutils_classes_diagrams.png`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/specutils_classes_diagrams.pptx` & `specutils-1.9.1/docs/specutils_classes_diagrams.pptx`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/docs/types_of_spectra.rst` & `specutils-1.9.1/docs/types_of_spectra.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/licenses/LICENSE.rst` & `specutils-1.9.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/licenses/TEMPLATE_LICENCE.rst` & `specutils-1.9.1/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/setup.cfg` & `specutils-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/setup.py` & `specutils-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/__init__.py` & `specutils-1.9.1/specutils/__init__.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/_astropy_init.py` & `specutils-1.9.1/specutils/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/analysis/correlation.py` & `specutils-1.9.1/specutils/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/analysis/flux.py` & `specutils-1.9.1/specutils/analysis/flux.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/analysis/location.py` & `specutils-1.9.1/specutils/analysis/location.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/analysis/moment.py` & `specutils-1.9.1/specutils/analysis/moment.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/analysis/template_comparison.py` & `specutils-1.9.1/specutils/analysis/template_comparison.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/analysis/uncertainty.py` & `specutils-1.9.1/specutils/analysis/uncertainty.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/analysis/utils.py` & `specutils-1.9.1/specutils/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/analysis/width.py` & `specutils-1.9.1/specutils/analysis/width.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/conftest.py` & `specutils-1.9.1/specutils/conftest.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/fitting/continuum.py` & `specutils-1.9.1/specutils/fitting/continuum.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/fitting/fitmodels.py` & `specutils-1.9.1/specutils/fitting/fitmodels.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/_list_of_loaders.py` & `specutils-1.9.1/specutils/io/_list_of_loaders.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/asdf/__init__.py` & `specutils-1.9.1/specutils/io/asdf/__init__.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/asdf/extension.py` & `specutils-1.9.1/specutils/io/asdf/extension.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectral_coord-1.0.0.yaml` & `specutils-1.9.1/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectral_coord-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectrum1d-1.0.0.yaml` & `specutils-1.9.1/specutils/io/asdf/schemas/astropy.org/specutils/spectra/spectrum1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/asdf/tags/spectra.py` & `specutils-1.9.1/specutils/io/asdf/tags/spectra.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/asdf/tags/tests/test_spectra.py` & `specutils-1.9.1/specutils/io/asdf/tags/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/asdf/types.py` & `specutils-1.9.1/specutils/io/asdf/types.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/aaomega_2df.py` & `specutils-1.9.1/specutils/io/default_loaders/aaomega_2df.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/apogee.py` & `specutils-1.9.1/specutils/io/default_loaders/apogee.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/ascii.py` & `specutils-1.9.1/specutils/io/default_loaders/ascii.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/dc_common.py` & `specutils-1.9.1/specutils/io/default_loaders/dc_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,25 @@
     "stdev": Purpose.ERROR_STDEV,
     "sigma": Purpose.ERROR_STDEV,
     "variance": Purpose.ERROR_VARIANCE,
     "spectrum": Purpose.SCIENCE,
 }
 
 
+def refresh_units(wcs):
+    """
+    Reparse unit strings to ensure aliases have been applied.
+
+    This is needed to handle legacy spellings that are used by existing surveys.
+    """
+    new_units = [u.Unit(str(cu)) for cu in wcs.wcs.cunit]
+    wcs.wcs.cunit = new_units
+    return wcs
+
+
 def add_labels(spec_list, use_purpose=False):
     not_labeled = 0
     label_set = set()
     for spec in spec_list:
         meta = spec.meta
         purpose = meta.get("purpose")
         if use_purpose:
@@ -252,14 +263,15 @@
     units_info=None,
     purpose_prefix=None,
     all_standard_units,
     all_keywords,
     valid_wcs,
     index=None,
     drop_wcs_axes=None,
+    fallback_header=None,
 ):
     spec_wcs_info = {}
     spec_units_info = {}
     if wcs_info is not None:
         spec_wcs_info.update(wcs_info)
     if units_info is not None:
         spec_units_info.update(units_info)
@@ -267,38 +279,67 @@
     if spec_info is not None:
         spec_wcs_info.update(spec_info.get("wcs", {}))
         spec_units_info.update(spec_info.get("units", {}))
         purpose = spec_info.get("purpose")
     else:
         purpose = None
 
-    purpose = get_purpose(
-        header,
-        purpose=purpose,
-        purpose_prefix=purpose_prefix,
-        all_keywords=all_keywords,
-        index=index,
-    )
+    try:
+        purpose = get_purpose(
+            header,
+            purpose=purpose,
+            purpose_prefix=purpose_prefix,
+            all_keywords=all_keywords,
+            index=index,
+        )
+    except ValueError:
+        if fallback_header is None:
+            raise
+        purpose = get_purpose(
+            fallback_header,
+            purpose=purpose,
+            purpose_prefix=purpose_prefix,
+            all_keywords=all_keywords,
+            index=index,
+        )
 
     if purpose == Purpose.SKIP:
         return None
 
     if valid_wcs or not spec_wcs_info:
         wcs = WCS(header)
         if drop_wcs_axes is not None:
             if isinstance(drop_wcs_axes, Callable):
                 wcs = drop_wcs_axes(wcs)
             else:
                 wcs = wcs.dropaxis(drop_wcs_axes)
     else:
-        wcs = compute_wcs_from_keys_and_values(header, **spec_wcs_info)
+        try:
+            wcs = compute_wcs_from_keys_and_values(header, **spec_wcs_info)
+        except ValueError:
+            if fallback_header is None:
+                raise
+            wcs = compute_wcs_from_keys_and_values(
+                fallback_header, **spec_wcs_info
+            )
+
+    wcs = refresh_units(wcs)
 
     if all_standard_units:
         spec_units_info = {}
-    flux_unit = get_flux_units_from_keys_and_values(header, **spec_units_info)
+    try:
+        flux_unit = get_flux_units_from_keys_and_values(
+            header, **spec_units_info
+        )
+    except ValueError:
+        if fallback_header is None:
+            raise
+        flux_unit = get_flux_units_from_keys_and_values(
+            fallback_header, **spec_units_info
+        )
     flux = data * flux_unit
 
     meta = {"header": header, "purpose": PURPOSE_SPECTRA_MAP[purpose]}
 
     if purpose in CREATE_SPECTRA:
         spectrum = Spectrum1D(wcs=wcs, flux=flux, meta=meta)
         spectra_map[PURPOSE_SPECTRA_MAP[purpose]].append(spectrum)
@@ -375,24 +416,30 @@
     wcs,
     units,
     all_standard_units,
     all_keywords,
     valid_wcs,
     label=True,
     drop_wcs_axes=None,
+    fallback_header=None,
 ):
     spectra_map = {
         "sky": [],
         "combined": [],
         "unreduced": [],
         "normalised": [],
         "reduced": [],
     }
 
     with read_fileobj_or_hdulist(filename) as fits_file:
+        if fallback_header is not None:
+            if fallback_header is True:
+                fallback_header = 0
+            fallback_header = fits_file[fallback_header].header
+
         hdus = deepcopy(hdus)
         if hdus is not None:
             # extract hdu information and validate it
             cycle = hdus.pop("cycle", None)
             cycle_start = hdus.pop("cycle_start", None)
             purpose_prefix = hdus.pop("purpose_prefix", None)
             if len(hdus) != 0 and cycle is None:
@@ -441,14 +488,15 @@
                 wcs_info=wcs,
                 units_info=units,
                 purpose_prefix=hdu_purpose_prefix,
                 all_standard_units=all_standard_units,
                 all_keywords=all_keywords,
                 valid_wcs=valid_wcs,
                 drop_wcs_axes=drop_wcs_axes,
+                fallback_header=fallback_header,
             )
 
     if label:
         add_labels(spectra_map["combined"])
         add_labels(spectra_map["reduced"])
         add_labels(spectra_map["normalised"])
         add_labels(spectra_map["unreduced"], use_purpose=True)
```

### Comparing `specutils-1.9.0/specutils/io/default_loaders/galah.py` & `specutils-1.9.1/specutils/io/default_loaders/galah.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/gama.py` & `specutils-1.9.1/specutils/io/default_loaders/gama.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/generic_cube.py` & `specutils-1.9.1/specutils/io/default_loaders/generic_cube.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/generic_ecsv_reader.py` & `specutils-1.9.1/specutils/io/default_loaders/generic_ecsv_reader.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/hst_cos.py` & `specutils-1.9.1/specutils/io/default_loaders/hst_cos.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/hst_stis.py` & `specutils-1.9.1/specutils/io/default_loaders/hst_stis.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/jwst_reader.py` & `specutils-1.9.1/specutils/io/default_loaders/jwst_reader.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/manga.py` & `specutils-1.9.1/specutils/io/default_loaders/manga.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/muscles_sed.py` & `specutils-1.9.1/specutils/io/default_loaders/muscles_sed.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/ozdes.py` & `specutils-1.9.1/specutils/io/default_loaders/ozdes.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/sdss.py` & `specutils-1.9.1/specutils/io/default_loaders/sdss.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/sixdfgs_reader.py` & `specutils-1.9.1/specutils/io/default_loaders/sixdfgs_reader.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/subaru_pfs_spec.py` & `specutils-1.9.1/specutils/io/default_loaders/subaru_pfs_spec.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/tabular_fits.py` & `specutils-1.9.1/specutils/io/default_loaders/tabular_fits.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/tests/test_apogee.py` & `specutils-1.9.1/specutils/io/default_loaders/tests/test_apogee.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/tests/test_jwst_reader.py` & `specutils-1.9.1/specutils/io/default_loaders/tests/test_jwst_reader.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/twodfgrs_reader.py` & `specutils-1.9.1/specutils/io/default_loaders/twodfgrs_reader.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/twoslaq_lrg.py` & `specutils-1.9.1/specutils/io/default_loaders/twoslaq_lrg.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/wcs_fits.py` & `specutils-1.9.1/specutils/io/default_loaders/wcs_fits.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/default_loaders/wigglez.py` & `specutils-1.9.1/specutils/io/default_loaders/wigglez.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/parsing_utils.py` & `specutils-1.9.1/specutils/io/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/io/registers.py` & `specutils-1.9.1/specutils/io/registers.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/manipulation/estimate_uncertainty.py` & `specutils-1.9.1/specutils/manipulation/estimate_uncertainty.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/manipulation/extract_spectral_region.py` & `specutils-1.9.1/specutils/manipulation/extract_spectral_region.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/manipulation/manipulation.py` & `specutils-1.9.1/specutils/manipulation/manipulation.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/manipulation/model_replace.py` & `specutils-1.9.1/specutils/manipulation/model_replace.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/manipulation/resample.py` & `specutils-1.9.1/specutils/manipulation/resample.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/manipulation/smoothing.py` & `specutils-1.9.1/specutils/manipulation/smoothing.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/manipulation/utils.py` & `specutils-1.9.1/specutils/manipulation/utils.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/spectra/spectral_axis.py` & `specutils-1.9.1/specutils/spectra/spectral_axis.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/spectra/spectral_region.py` & `specutils-1.9.1/specutils/spectra/spectral_region.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/spectra/spectrum1d.py` & `specutils-1.9.1/specutils/spectra/spectrum1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -669,21 +669,27 @@
     @radial_velocity.setter
     @deprecated('1.8.0', alternative='set_radial_velocity_to or shift_spectrum_to')
     def radial_velocity(self, val):
         self.shift_spectrum_to(radial_velocity=val)
 
     def __add__(self, other):
         if not isinstance(other, (NDCube, u.Quantity)):
-            other = u.Quantity(other, unit=self.unit)
+            try:
+                other = u.Quantity(other, unit=self.unit)
+            except TypeError:
+                return NotImplemented
 
         return self.add(other)
 
     def __sub__(self, other):
         if not isinstance(other, NDCube):
-            other = u.Quantity(other, unit=self.unit)
+            try:
+                other = u.Quantity(other, unit=self.unit)
+            except TypeError:
+                return NotImplemented
 
         return self.subtract(other)
 
     def __mul__(self, other):
         if not isinstance(other, NDCube):
             other = u.Quantity(other)
```

### Comparing `specutils-1.9.0/specutils/spectra/spectrum_collection.py` & `specutils-1.9.1/specutils/spectra/spectrum_collection.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/spectra/spectrum_list.py` & `specutils-1.9.1/specutils/spectra/spectrum_list.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/spectra/spectrum_mixin.py` & `specutils-1.9.1/specutils/spectra/spectrum_mixin.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/conftest.py` & `specutils-1.9.1/specutils/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/coveragerc` & `specutils-1.9.1/specutils/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_analysis.py` & `specutils-1.9.1/specutils/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_arithmetic.py` & `specutils-1.9.1/specutils/tests/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_continuum.py` & `specutils-1.9.1/specutils/tests/test_continuum.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_correlation.py` & `specutils-1.9.1/specutils/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_dc_common_loaders.py` & `specutils-1.9.1/specutils/tests/test_dc_common_loaders.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_fitting.py` & `specutils-1.9.1/specutils/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_io.py` & `specutils-1.9.1/specutils/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_loaders.py` & `specutils-1.9.1/specutils/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_manipulation.py` & `specutils-1.9.1/specutils/tests/test_manipulation.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_model_replace.py` & `specutils-1.9.1/specutils/tests/test_model_replace.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_region_extract.py` & `specutils-1.9.1/specutils/tests/test_region_extract.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_regions.py` & `specutils-1.9.1/specutils/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_resample.py` & `specutils-1.9.1/specutils/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_slicing.py` & `specutils-1.9.1/specutils/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_smoothing.py` & `specutils-1.9.1/specutils/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_spectral_axis.py` & `specutils-1.9.1/specutils/tests/test_spectral_axis.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_spectrum1d.py` & `specutils-1.9.1/specutils/tests/test_spectrum1d.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_spectrum_collection.py` & `specutils-1.9.1/specutils/tests/test_spectrum_collection.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_template_comparison.py` & `specutils-1.9.1/specutils/tests/test_template_comparison.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_unc.py` & `specutils-1.9.1/specutils/tests/test_unc.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/tests/test_utils.py` & `specutils-1.9.1/specutils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/utils/quantity_model.py` & `specutils-1.9.1/specutils/utils/quantity_model.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils/utils/wcs_utils.py` & `specutils-1.9.1/specutils/utils/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/specutils.egg-info/PKG-INFO` & `specutils-1.9.1/specutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specutils
-Version: 1.9.0
+Version: 1.9.1
 Summary: Package for spectroscopic astronomical data
 Home-page: https://specutils.readthedocs.io/
 Author: Specutils Developers
 Author-email: coordinators@astropy.org
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `specutils-1.9.0/specutils.egg-info/SOURCES.txt` & `specutils-1.9.1/specutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `specutils-1.9.0/tox.ini` & `specutils-1.9.1/tox.ini`

 * *Files identical despite different names*

