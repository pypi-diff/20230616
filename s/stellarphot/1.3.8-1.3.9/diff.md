# Comparing `tmp/stellarphot-1.3.8.tar.gz` & `tmp/stellarphot-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellarphot-1.3.8.tar", last modified: Tue Dec  6 16:26:00 2022, max compression
+gzip compressed data, was "stellarphot-1.3.9.tar", last modified: Fri Jun 16 20:07:47 2023, max compression
```

## Comparing `stellarphot-1.3.8.tar` & `stellarphot-1.3.9.tar`

### file list

```diff
@@ -1,143 +1,134 @@
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.256318 stellarphot-1.3.8/
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.132966 stellarphot-1.3.8/.github/
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.145316 stellarphot-1.3.8/.github/workflows/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1229 2022-06-01 15:38:08.000000 stellarphot-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      732 2020-06-25 02:34:16.000000 stellarphot-1.3.8/.gitignore
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       71 2020-02-18 16:06:39.000000 stellarphot-1.3.8/.readthedocs.yml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      371 2020-02-18 16:06:39.000000 stellarphot-1.3.8/.rtd-environment.yml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1718 2022-10-18 15:08:51.000000 stellarphot-1.3.8/CHANGES.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      347 2022-10-18 13:26:31.000000 stellarphot-1.3.8/MANIFEST.in
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      439 2022-12-06 16:26:00.256515 stellarphot-1.3.8/PKG-INFO
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1930 2022-11-06 21:02:41.000000 stellarphot-1.3.8/README.md
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.149372 stellarphot-1.3.8/docs/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4581 2020-02-18 16:06:39.000000 stellarphot-1.3.8/docs/Makefile
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.133535 stellarphot-1.3.8/docs/_templates/
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.152067 stellarphot-1.3.8/docs/_templates/autosummary/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      250 2020-02-18 16:06:39.000000 stellarphot-1.3.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      251 2020-02-18 16:06:39.000000 stellarphot-1.3.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      252 2020-02-18 16:06:39.000000 stellarphot-1.3.8/docs/_templates/autosummary/module.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7320 2020-02-18 16:06:39.000000 stellarphot-1.3.8/docs/conf.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      490 2020-06-25 02:34:16.000000 stellarphot-1.3.8/docs/index.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4549 2020-02-18 16:06:39.000000 stellarphot-1.3.8/docs/make.bat
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.153000 stellarphot-1.3.8/docs/stellarphot/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1012 2022-10-18 12:08:32.000000 stellarphot-1.3.8/docs/stellarphot/index.rst
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.155830 stellarphot-1.3.8/licenses/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1482 2020-02-18 16:06:39.000000 stellarphot-1.3.8/licenses/LICENSE.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      372 2020-02-18 16:06:39.000000 stellarphot-1.3.8/licenses/README.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1659 2020-02-18 16:06:39.000000 stellarphot-1.3.8/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      132 2020-02-18 16:06:39.000000 stellarphot-1.3.8/pyproject.toml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1925 2022-12-06 16:26:00.257497 stellarphot-1.3.8/setup.cfg
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1039 2020-02-18 16:06:39.000000 stellarphot-1.3.8/setup.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.164051 stellarphot-1.3.8/stellarphot/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      926 2022-03-28 19:21:43.000000 stellarphot-1.3.8/stellarphot/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1476 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/_astropy_init.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.170544 stellarphot-1.3.8/stellarphot/analysis/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2021-05-23 20:38:12.000000 stellarphot-1.3.8/stellarphot/analysis/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.174269 stellarphot-1.3.8/stellarphot/analysis/data/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1829 2022-03-28 19:21:43.000000 stellarphot-1.3.8/stellarphot/analysis/data/exotic-to-mod-candidate.json
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      574 2022-03-28 19:21:43.000000 stellarphot-1.3.8/stellarphot/analysis/data/exotic-to-mod-known.json
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5106 2022-11-16 23:59:29.000000 stellarphot-1.3.8/stellarphot/analysis/data/tic-template-for-exotic-candidate.json
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3852 2022-11-16 23:59:29.000000 stellarphot-1.3.8/stellarphot/analysis/data/tic-template-for-exotic-known.json
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    13373 2022-12-06 15:44:28.000000 stellarphot-1.3.8/stellarphot/analysis/exotic.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.176449 stellarphot-1.3.8/stellarphot/analysis/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2021-05-23 20:38:12.000000 stellarphot-1.3.8/stellarphot/analysis/tests/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      249 2022-12-06 15:44:28.000000 stellarphot-1.3.8/stellarphot/analysis/tests/test_exotic.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    10169 2021-11-05 21:05:08.000000 stellarphot-1.3.8/stellarphot/analysis/tests/test_transit_fitting.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    16696 2022-06-01 15:38:08.000000 stellarphot-1.3.8/stellarphot/analysis/transit_fitting.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1166 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/conftest.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1306 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/coordinates.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      391 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/core.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.177429 stellarphot-1.3.8/stellarphot/data/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      246 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/data/README.rst
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.182188 stellarphot-1.3.8/stellarphot/differential_photometry/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       90 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7088 2022-12-02 16:36:57.000000 stellarphot-1.3.8/stellarphot/differential_photometry/aij_rel_fluxes.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7860 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/differential_photometry/catalog_search.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    21254 2022-11-16 23:59:29.000000 stellarphot-1.3.8/stellarphot/differential_photometry/magnitude_transforms.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.186213 stellarphot-1.3.8/stellarphot/differential_photometry/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.200957 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)   832320 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    28800 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    23040 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    11520 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/comp_stars.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    28800 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      251 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/mag_transform.csv
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    23040 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25920 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/variables.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5272 2021-11-18 18:30:03.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7885 2021-05-23 20:38:12.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/test_catalog_search.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    12415 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/test_magnitude_transforms.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1888 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/differential_photometry/tests/test_vsx_mags.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3858 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/differential_photometry/vsx_mags.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.205191 stellarphot-1.3.8/stellarphot/io/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      104 2022-12-01 16:43:37.000000 stellarphot-1.3.8/stellarphot/io/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9693 2022-11-02 16:15:53.000000 stellarphot-1.3.8/stellarphot/io/aavso_submission_schema.yml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    14033 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/io/aij.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7674 2022-12-02 16:36:57.000000 stellarphot-1.3.8/stellarphot/io/tess.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.208306 stellarphot-1.3.8/stellarphot/io/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/io/tests/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.210635 stellarphot-1.3.8/stellarphot/io/tests/data/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      909 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/io/tests/data/aij-sample-apertures.aperture
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      529 2021-05-23 20:38:12.000000 stellarphot-1.3.8/stellarphot/io/tests/data/apertures_as_table.csv
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2906 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/io/tests/test_aij_io.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1904 2022-12-01 16:43:37.000000 stellarphot-1.3.8/stellarphot/io/tests/test_tess_submission.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.224044 stellarphot-1.3.8/stellarphot/notebooks/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3021 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/notebooks/ObserveACP.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-10-18 12:48:28.000000 stellarphot-1.3.8/stellarphot/notebooks/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5385 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/notebooks/acp.py
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3719 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/notebooks/calculate_aavso_mags_draft.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5678 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/notebooks/comp-star-plots.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9575 2021-05-23 20:38:12.000000 stellarphot-1.3.8/stellarphot/notebooks/comp-stars-template.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9399 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/notebooks/example_interactive_plot.ipynb
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    21861 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/notebooks/get_apass_comp_mags.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    27859 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/notebooks/image-viewer-working-copy.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2777 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/notebooks/image_viewer_demo.ipynb
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.239690 stellarphot-1.3.8/stellarphot/notebooks/photometry/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1869 2022-12-01 16:45:55.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    10203 2022-11-17 19:42:08.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2501 2022-12-01 16:43:37.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4631 2022-12-02 16:58:13.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/03-photometry-template.ipynb
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4078 2022-12-06 16:24:20.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    19549 2022-12-06 16:24:20.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/06-transit-fit-template.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4377 2022-12-06 15:44:28.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6486 2022-10-20 16:49:16.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/Untitled.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-10-18 12:08:32.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9511 2022-11-08 16:25:08.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)   144711 2022-11-02 16:15:53.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5602 2022-11-08 16:21:56.000000 stellarphot-1.3.8/stellarphot/notebooks/photometry/transform-pared-back.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    23862 2022-10-27 15:13:04.000000 stellarphot-1.3.8/stellarphot/photometry.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4742 2021-11-05 21:05:08.000000 stellarphot-1.3.8/stellarphot/source_detection.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.244120 stellarphot-1.3.8/stellarphot/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      108 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/tests/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.245606 stellarphot-1.3.8/stellarphot/tests/data/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      160 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/tests/data/test_sources.csv
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      265 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/tests/make_wcs.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      919 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/tests/test_coordinates.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      299 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/tests/test_core.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7590 2021-05-23 20:38:12.000000 stellarphot-1.3.8/stellarphot/tests/test_detection.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4156 2021-05-23 20:38:12.000000 stellarphot-1.3.8/stellarphot/tests/test_photometry.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.246245 stellarphot-1.3.8/stellarphot/utils/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      148 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/utils/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      382 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/version.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.255101 stellarphot-1.3.8/stellarphot/visualization/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      123 2022-10-18 12:08:28.000000 stellarphot-1.3.8/stellarphot/visualization/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4553 2022-11-16 23:59:29.000000 stellarphot-1.3.8/stellarphot/visualization/aij_plots.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    23085 2022-12-02 16:36:57.000000 stellarphot-1.3.8/stellarphot/visualization/comparison_functions.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3128 2022-12-02 17:24:01.000000 stellarphot-1.3.8/stellarphot/visualization/fits_opener.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5848 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/visualization/multi_night_plots.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1838 2022-12-01 17:21:37.000000 stellarphot-1.3.8/stellarphot/visualization/photometry_widget_functions.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    19419 2022-12-01 16:43:37.000000 stellarphot-1.3.8/stellarphot/visualization/seeing_profile_functions.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.255862 stellarphot-1.3.8/stellarphot/visualization/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2020-06-25 02:34:16.000000 stellarphot-1.3.8/stellarphot/visualization/tests/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4237 2021-11-05 21:05:08.000000 stellarphot-1.3.8/stellarphot/visualization/tests/test_seeing_profile.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1641 2021-05-23 20:38:12.000000 stellarphot-1.3.8/stellarphot/visualization/transit_plots.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-12-06 16:26:00.168501 stellarphot-1.3.8/stellarphot.egg-info/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      439 2022-12-06 16:25:59.000000 stellarphot-1.3.8/stellarphot.egg-info/PKG-INFO
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4841 2022-12-06 16:26:00.000000 stellarphot-1.3.8/stellarphot.egg-info/SOURCES.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2022-12-06 16:25:59.000000 stellarphot-1.3.8/stellarphot.egg-info/dependency_links.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2022-06-01 15:46:16.000000 stellarphot-1.3.8/stellarphot.egg-info/not-zip-safe
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      226 2022-12-06 16:25:59.000000 stellarphot-1.3.8/stellarphot.egg-info/requires.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       12 2022-12-06 16:25:59.000000 stellarphot-1.3.8/stellarphot.egg-info/top_level.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1238 2021-11-05 21:05:08.000000 stellarphot-1.3.8/tox.ini
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.813825 stellarphot-1.3.9/
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.731347 stellarphot-1.3.9/.github/
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.745295 stellarphot-1.3.9/.github/workflows/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1229 2022-06-01 15:38:08.000000 stellarphot-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      753 2023-06-15 18:08:41.000000 stellarphot-1.3.9/.gitignore
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      633 2023-06-16 19:54:25.000000 stellarphot-1.3.9/.readthedocs.yml
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      241 2023-06-16 19:54:18.000000 stellarphot-1.3.9/.rtd-environment.yml
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     2283 2023-06-16 20:06:42.000000 stellarphot-1.3.9/CHANGES.rst
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      347 2022-10-18 13:26:31.000000 stellarphot-1.3.9/MANIFEST.in
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      439 2023-06-16 20:07:47.813998 stellarphot-1.3.9/PKG-INFO
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1930 2023-06-15 17:41:12.000000 stellarphot-1.3.9/README.md
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.748079 stellarphot-1.3.9/docs/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     4581 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/Makefile
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.731856 stellarphot-1.3.9/docs/_templates/
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.750235 stellarphot-1.3.9/docs/_templates/autosummary/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      250 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      251 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      252 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     7316 2023-06-15 18:08:41.000000 stellarphot-1.3.9/docs/conf.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      482 2023-06-15 18:08:41.000000 stellarphot-1.3.9/docs/index.rst
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     4549 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/make.bat
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.750917 stellarphot-1.3.9/docs/stellarphot/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1127 2023-06-15 18:08:41.000000 stellarphot-1.3.9/docs/stellarphot/index.rst
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.753086 stellarphot-1.3.9/licenses/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1482 2020-02-18 16:06:39.000000 stellarphot-1.3.9/licenses/LICENSE.rst
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      372 2020-02-18 16:06:39.000000 stellarphot-1.3.9/licenses/README.rst
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1659 2020-02-18 16:06:39.000000 stellarphot-1.3.9/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      132 2020-02-18 16:06:39.000000 stellarphot-1.3.9/pyproject.toml
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1920 2023-06-16 20:07:47.814967 stellarphot-1.3.9/setup.cfg
+-rwxr-xr-x   0 jv8699qa (145084326) 2132868096     1039 2020-02-18 16:06:39.000000 stellarphot-1.3.9/setup.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.756219 stellarphot-1.3.9/stellarphot/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1052 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1476 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/_astropy_init.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.760215 stellarphot-1.3.9/stellarphot/analysis/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096       53 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/analysis/__init__.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.762503 stellarphot-1.3.9/stellarphot/analysis/data/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1829 2022-03-28 19:21:43.000000 stellarphot-1.3.9/stellarphot/analysis/data/exotic-to-mod-candidate.json
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      574 2022-03-28 19:21:43.000000 stellarphot-1.3.9/stellarphot/analysis/data/exotic-to-mod-known.json
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     5106 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/analysis/data/tic-template-for-exotic-candidate.json
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     3852 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/analysis/data/tic-template-for-exotic-known.json
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    15542 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/analysis/exotic.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.764019 stellarphot-1.3.9/stellarphot/analysis/tests/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2021-05-23 20:38:12.000000 stellarphot-1.3.9/stellarphot/analysis/tests/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      249 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/analysis/tests/test_exotic.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    10169 2021-11-05 21:05:08.000000 stellarphot-1.3.9/stellarphot/analysis/tests/test_transit_fitting.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    20530 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/analysis/transit_fitting.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1166 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/conftest.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     2142 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/core.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.764705 stellarphot-1.3.9/stellarphot/data/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      246 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/data/README.rst
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.766761 stellarphot-1.3.9/stellarphot/differential_photometry/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      120 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/differential_photometry/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     7076 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/differential_photometry/aij_rel_fluxes.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     9557 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/differential_photometry/catalog_search.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    23388 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/differential_photometry/magnitude_transforms.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.769409 stellarphot-1.3.9/stellarphot/differential_photometry/tests/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/__init__.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.784519 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096   832320 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    28800 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    23040 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    11520 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/comp_stars.fits
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    28800 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      251 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/mag_transform.csv
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     5760 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    23040 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    25920 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/variables.fits
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     5272 2021-11-18 18:30:03.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     7885 2021-05-23 20:38:12.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_catalog_search.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    12412 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_magnitude_transforms.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1888 2023-06-15 17:36:47.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_vsx_mags.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     3858 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/differential_photometry/vsx_mags.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.787327 stellarphot-1.3.9/stellarphot/io/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      104 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/io/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     9693 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/io/aavso_submission_schema.yml
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    18826 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/io/aij.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    11551 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/io/tess.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.788735 stellarphot-1.3.9/stellarphot/io/tests/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/io/tests/__init__.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.790125 stellarphot-1.3.9/stellarphot/io/tests/data/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      909 2023-06-15 17:36:47.000000 stellarphot-1.3.9/stellarphot/io/tests/data/aij-sample-apertures.aperture
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      529 2021-05-23 20:38:12.000000 stellarphot-1.3.9/stellarphot/io/tests/data/apertures_as_table.csv
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     2906 2023-06-15 17:36:47.000000 stellarphot-1.3.9/stellarphot/io/tests/test_aij_io.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1904 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/io/tests/test_tess_submission.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.792566 stellarphot-1.3.9/stellarphot/notebooks/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     5801 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/notebooks/comp-star-plots.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     9803 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/notebooks/comp-stars-template.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    27859 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/notebooks/image-viewer-working-copy.ipynb
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.804339 stellarphot-1.3.9/stellarphot/notebooks/photometry/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1869 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    10203 2022-11-17 19:42:08.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     2501 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb
+-rwxr-xr-x   0 jv8699qa (145084326) 2132868096     4631 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/03-photometry-template.ipynb
+-rwxr-xr-x   0 jv8699qa (145084326) 2132868096     4078 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    19546 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/06-transit-fit-template.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     4377 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     7063 2023-06-16 19:34:31.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/0X-comps-star-plot (1).ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     6486 2022-10-20 16:49:16.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/Untitled.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     9511 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096   144711 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     5602 2023-06-16 20:04:46.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/transform-pared-back.ipynb
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    25806 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/photometry.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     6216 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/source_detection.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.807479 stellarphot-1.3.9/stellarphot/tests/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      108 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/tests/__init__.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.808226 stellarphot-1.3.9/stellarphot/tests/data/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      160 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/tests/data/test_sources.csv
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      265 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/tests/make_wcs.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      299 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/tests/test_core.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     7584 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/tests/test_detection.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     4156 2021-05-23 20:38:12.000000 stellarphot-1.3.9/stellarphot/tests/test_photometry.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      382 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/version.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.812136 stellarphot-1.3.9/stellarphot/visualization/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      298 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/visualization/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     4821 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/aij_plots.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    30006 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/comparison_functions.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     4294 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/fits_opener.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     7254 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/multi_night_plots.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     2537 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/photometry_widget_functions.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096    22372 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/seeing_profile_functions.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.813183 stellarphot-1.3.9/stellarphot/visualization/tests/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/visualization/tests/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     4237 2023-06-15 18:08:31.000000 stellarphot-1.3.9/stellarphot/visualization/tests/test_seeing_profile.py
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     3135 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/visualization/transit_plots.py
+drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.758942 stellarphot-1.3.9/stellarphot.egg-info/
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      439 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/PKG-INFO
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     4538 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/SOURCES.txt
+-rw-r--r--   0 jv8699qa (145084326) 2132868096        1 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/dependency_links.txt
+-rw-r--r--   0 jv8699qa (145084326) 2132868096        1 2022-06-01 15:46:16.000000 stellarphot-1.3.9/stellarphot.egg-info/not-zip-safe
+-rw-r--r--   0 jv8699qa (145084326) 2132868096      221 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/requires.txt
+-rw-r--r--   0 jv8699qa (145084326) 2132868096       12 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/top_level.txt
+-rw-r--r--   0 jv8699qa (145084326) 2132868096     1238 2021-11-05 21:05:08.000000 stellarphot-1.3.9/tox.ini
```

### Comparing `stellarphot-1.3.8/.github/workflows/build.yml` & `stellarphot-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/.gitignore` & `stellarphot-1.3.9/.gitignore`

 * *Files 24% similar despite different names*

```diff
@@ -47,17 +47,19 @@
 sdist
 develop-eggs
 .installed.cfg
 distribute-*.tar.gz
 
 # Other
 .cache
+.nova
 .tox
 .*.sw[op]
 *~
 .project
 .pydevproject
 .settings
 .vscode
+_personal_docs
 
 # Mac OSX
 .DS_Store
```

### Comparing `stellarphot-1.3.8/CHANGES.rst` & `stellarphot-1.3.9/CHANGES.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,40 @@
-1.1.2 (2022-10-18)
+1.3.9 (2023-06-16)
 ------------------
 
 New Features
 ^^^^^^^^^^^^
 
-
 Other Changes and Additions
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
++ Old and redundant notebooks have been purged and bad references to `glowing-waffles` instead of `stellarphot` [#94]
++ Most functions are now linked to the documentation. [#90]
++ Many functions and classes that had missing documentation have now had docstrings added. [#100]
 
 Bug Fixes
 ^^^^^^^^^
 
++ Runs without errors on release version of astrowidgets (0.3.0) [#93]
++ Runs without errors on current numpy (1.24.3) and astropy (5.3). [#92]
+
+
+1.1.2 (2022-10-18)
+------------------
+
+New Features
+^^^^^^^^^^^^
+
+Other Changes and Additions
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Bug Fixes
+^^^^^^^^^
 + Simplify comparison notebook.
 
+
 1.1.1 (2022-10-18)
 ------------------
 
 New Features
 ^^^^^^^^^^^^
```

### Comparing `stellarphot-1.3.8/README.md` & `stellarphot-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/docs/Makefile` & `stellarphot-1.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/docs/conf.py` & `stellarphot-1.3.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes. To override the custom theme, set this to the
 # name of a builtin theme or the name of a custom theme in html_theme_path.
 #html_theme = None
 
 
 html_theme_options = {
-    'logotext1': 'glowing-waffles',  # white,  semi-bold
+    'logotext1': 'stellarphot',  # white,  semi-bold
     'logotext2': '',  # orange, light
     'logotext3': ':docs'   # white,  light
     }
 
 
 # Custom sidebar templates, maps document names to template names.
 #html_sidebars = {}
```

### Comparing `stellarphot-1.3.8/docs/make.bat` & `stellarphot-1.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/docs/stellarphot/index.rst` & `stellarphot-1.3.9/docs/stellarphot/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -17,11 +17,14 @@
 
 There may be additional fields.
 
 Reference/API
 =============
 
 .. automodapi:: stellarphot
-.. automodapi:: stellarphot.photometry
+.. automodapi:: stellarphot.analysis
+.. automodapi:: stellarphot.core
 .. automodapi:: stellarphot.differential_photometry
-.. automodapi:: stellarphot.visualization
 .. automodapi:: stellarphot.io
+.. automodapi:: stellarphot.photometry
+.. automodapi:: stellarphot.source_detection
+.. automodapi:: stellarphot.visualization
```

### Comparing `stellarphot-1.3.8/licenses/LICENSE.rst` & `stellarphot-1.3.9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/licenses/TEMPLATE_LICENCE.rst` & `stellarphot-1.3.9/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/setup.cfg` & `stellarphot-1.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 license_file = licenses/LICENSE.rst
 url = https://github.com/stellarphot/stellarphot
 edit_on_github = False
 github_project = stellarphot/stellarphot
 
 [options]
 install_requires = 
-	astropy >=5,<5.1
+	astropy >=5
 	astroquery
 	ccdproc
 	ginga
 	ipywidgets
 	bottleneck
 	photutils >=1
 	matplotlib
```

### Comparing `stellarphot-1.3.8/setup.py` & `stellarphot-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/_astropy_init.py` & `stellarphot-1.3.9/stellarphot/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/analysis/data/exotic-to-mod-candidate.json` & `stellarphot-1.3.9/stellarphot/analysis/data/exotic-to-mod-candidate.json`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/analysis/data/exotic-to-mod-known.json` & `stellarphot-1.3.9/stellarphot/analysis/data/exotic-to-mod-known.json`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/analysis/data/tic-template-for-exotic-candidate.json` & `stellarphot-1.3.9/stellarphot/analysis/data/tic-template-for-exotic-candidate.json`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/analysis/data/tic-template-for-exotic-known.json` & `stellarphot-1.3.9/stellarphot/analysis/data/tic-template-for-exotic-known.json`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/analysis/exotic.py` & `stellarphot-1.3.9/stellarphot/analysis/exotic.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 import ipywidgets as ipw
 from traitlets import observe, Bool
 
 from astroquery.mast import Catalogs
 from astropy.utils.data import get_pkg_data_filename
 
 
+__all__ = ['MyValid', 'get_tic_info', 'make_checker','validate_exposure_time',
+           'populate_TIC_boxes', 'populate_TOI_boxes', 'exotic_settings_widget',
+           'set_values_from_json_file', 'get_values_from_widget','generate_json_file_name']
+
+
 template_types = ['known', 'candidate']
 template_json = {}
 to_fill = {}
 
 for template in template_types:
     template_name = get_pkg_data_filename('data/tic-template-for-exotic-'
                                           f'{template}.json')
@@ -31,15 +36,23 @@
 
 # Nested keys are flattened by joining them with this character
 join_char = "😬"
 
 
 class MyValid(ipw.Button):
     """
-    A more compact indicator of valid entries.
+    A class containing a more compact indicator of valid entries based on ipywidgets
+    buton value.
+
+    Attributes
+    ----------
+
+    value : bool
+        Current value of the indicator.
+
     """
     value = Bool(False, help="Bool value").tag(sync=True)
 
     def __init__(self, **kwd):
         super().__init__(**kwd)
         self.layout.width = '40px'
         self._set_properties(None)
@@ -60,30 +73,37 @@
     at MAST.
 
     Parameters
     ----------
 
     TIC_ID : int
         9 or 10 digit TIC ID number.
+
+    Returns
+    -------
+
+    `astropy.table.Table`
+        Astropy table withinformation about the TIC object.
+
     """
     catalog_data = Catalogs.query_criteria(catalog="Tic", ID=TIC_ID)
     return catalog_data
 
 
 def make_checker(indicator_widget, value_widget):
     """
-    Build an observer thatchecks TIC number and, if it is a valid
+    Build an observer that checks TIC number and, if it is a valid
     TIC number, looks up information about the TIC object from
     MAST copy of TIC as priors for EXOTIC. It also sets the visible checkbox
     to the appropriate state.
 
     Parameters
     ----------
 
-    indicator_widget : MyCheck widget
+    indicator_widget : `~stellarphot.analysis.MyValid` widget
         The widget that indicates to the user whether or not the value is
         reasonable.
 
     value_widget: ipywidget
         This widget should be generated by exotic_settings_widget.
 
     Returns
@@ -115,14 +135,32 @@
                 indicator_widget.value = False
                 indicator_widget.tooltip = 'TIC numbers have 9 digits'
 
     return check_name
 
 
 def validate_exposure_time(indicator_widget, value_widget):
+    """ Validates the exposure time input.
+
+    Parameters
+    ----------
+    indicator_widget : `~stellarphot.analysis.MyValid` widget
+        The widget that indicates to the user whether or not the value is
+        reasonable.
+
+    value_widget: ipywidget
+        This widget should be generated by exotic_settings_widget.
+
+    Returns
+    -------
+    function
+        Function that will set the correct boolean value on the
+        indicator_widget to indicate if the value of the exposure time
+        is valid.  This can be used as an observer for an ipywidget
+    """
     def check_exposure(change):
         # Valid Exposure time is greater than zero
         if change['new'] > 0:
             if indicator_widget is not None:
                 indicator_widget.value = True
         else:
             if indicator_widget is not None:
@@ -130,14 +168,29 @@
     return check_exposure
 
 
 def populate_TIC_boxes(tic_info, value_widget):
     """
     Set the appropriate widget values given information pulled from
     MAST TIC.
+
+    Parameters
+    ----------
+
+    tic_info : dict
+        Dictionary of information about the TIC object.
+
+    value_widget: ipywidget
+        This widget should contain a 'candidate' key.
+
+    Returns
+    -------
+
+    None
+        Sets values of planetary parameters of `candidate` in ``value_widget`` in place.
     """
     # Match EXOTIC json keys to columns in the result returned from
     # astroquery
     exotic_tic = {
         "Star Effective Temperature (K)": "Teff",
         "Star Effective Temperature (+) Uncertainty": "epos_Teff",
         "Star Effective Temperature (-) Uncertainty": "eneg_Teff",
@@ -158,14 +211,29 @@
             value_widget['candidate'][exotic_key].value = tic_info[v][0]
 
 
 def populate_TOI_boxes(toi, exotic_widget):
     """
     Set the appropriate widget values given information pulled from
     MAST TIC.
+
+    Parameters
+    ----------
+
+    toi : `~stellarphot.io.tess.TOI`
+        Information about the TIC object.
+
+    exotic_widget:  ipywidget
+        This widget should be generated by exotic_settings_widget.
+
+    Returns
+    -------
+
+    None
+        Sets values of planetary parameters of `candidate` in ``exotic_widget`` in place.
     """
     # Match EXOTIC json keys to columns in the result returned from
     # astroquery
     exotic_toi = {
             "Planet Name": "tic_id",
             "Target Star RA": "coord",
             "Target Star Dec": "coordP",
@@ -201,14 +269,25 @@
 for k in validators:
     validators[k]['Exposure Time (s)'] = validate_exposure_time
 
 
 def exotic_settings_widget():
     """
     Generate a widget to enter (and store) settings for exotic.
+
+    Parameters
+    ----------
+
+    None
+
+    Returns
+    -------
+
+    ipywidget
+        Widget with settings for EXOTIC.
     """
 
     # We rely on some global variables:
     global to_fill, template_types
 
     # This dictionary will contain all of the widgets
     widget_list = {}
@@ -321,14 +400,19 @@
     ----------
 
     widget : ipywidget
         This widget should be generated by exotic_settings_widget.
 
     json_file : str
         File with settings for the widget.
+
+    Returns
+    -------
+    None
+        Sets values of parameters of widget in place.
     """
     with open(json_file) as f:
         input_values = json.load(f)
 
     planet_type = widget.planet_type.value
     for k, widget in widget.value_widget[planet_type].items():
         k1, k2 = k.split(join_char)
@@ -344,14 +428,21 @@
 
     exotic_widget : ipywidget
         This widget should be generated by exotic_settings_widget.
 
     key : str, either "known" or "candidate", optional
         Indicates which case to use for EXOTIC. If ``None``, use the ``planet_type``
         attribute of the ``exotic_widget``.
+
+    Returns
+    -------
+
+    dict
+        Value of modified template_json[key], where template_json is a global variable.
+
     """
     if not key:
         key = exotic_widget.planet_type.value
 
     for k, widget in exotic_widget.value_widget[key].items():
         k1, k2 = k.split(join_char)
         template_json[key][k1][k2] = widget.value
@@ -369,14 +460,18 @@
     exotic_widget : ipywidget
         This widget should be generated by exotic_settings_widget.
 
     key : str, either "known" or "candidate", optional
         Indicates which case to use for EXOTIC. If ``None``, use the ``planet_type``
         attribute of the ``exotic_widget``.
 
+    Returns
+    -------
+    str
+        Name of file to save settings to.
     """
     if not key:
         key = exotic_widget.planet_type.value
 
     get_values_from_widget(exotic_widget, key=key)
     user_info = 'user_info'
     planet = 'planetary_parameters'
```

### Comparing `stellarphot-1.3.8/stellarphot/analysis/tests/test_transit_fitting.py` & `stellarphot-1.3.9/stellarphot/analysis/tests/test_transit_fitting.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/conftest.py` & `stellarphot-1.3.9/stellarphot/conftest.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/aij_rel_fluxes.py` & `stellarphot-1.3.9/stellarphot/differential_photometry/aij_rel_fluxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,27 +33,27 @@
         of the comparison stars will necessarily be used. Stars in
         this table are excluded from the comparison set if, in any
         of the `star_data` for that comparison, the net counts are
         ``NaN`` or if the angular distance between the position in
         the `star_data` and the position in the `comp_stars` table
         is too large.
 
-    in_place : ``bool``, optional
+    in_place : bool,  optional
         If ``True``, add new columns to input table. Otherwise, return
         new table with those columns added.
 
-    coord_column : ``str``, optional
+    coord_column : str,  optional
         If provided, use this column to match comparison stars to coordinates.
         If not provided, the coordinates are generated with SkyCoord.
 
-    flux_column_name : ``str``, optional
+    flux_column_name : str,  optional
         If provided, use this column to find flux.
         If not provided, the column 'aperture_net_flux' is used.
 
-    star_id_column : ``str``, optional
+    star_id_column : str,  optional
         Name of the column that provides a unique identifier for each
         comparison star.
 
     Returns
     -------
 
     `astropy.table.Table` or None
```

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/catalog_search.py` & `stellarphot-1.3.9/stellarphot/differential_photometry/catalog_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,28 +22,28 @@
     """
     Given a WCS and list of coordinates check whether the coordinates
     are within the frame.
 
     Parameters
     ----------
 
-    frame_wcs : astropy WCS object
+    frame_wcs : `astropy.wcs.WCS`
         WCS for the image.
-    coordinates : astropy.coordinates.SkyCoord
+    coordinates : `astropy.coordinates.SkyCoord`
         Coordinate(s) whose position will be checked to see if they are in the
         field of view.
     padding : int, optional
         Coordinates need to be at least this many pixels in from the edge
         of the frame to be considered in the field of view. Default value
         is 0.
 
     Returns
     -------
 
-    numpy.ndarray of bool
+    `numpy.ndarray` of bool
         One value for each input coordinate; values are ``True`` if the
         coordinate was in the field of view, ``False`` otherwise.
 
     """
     x, y = frame_wcs.all_world2pix(coordinates.ra, coordinates.dec, 0)
     in_x = (x >= padding) & (x <= frame_wcs.pixel_shape[0] - padding)
     in_y = (y >= padding) & (y <= frame_wcs.pixel_shape[1] - padding)
@@ -59,25 +59,49 @@
     """
     Return the items from catalog that are within the search radius and
     (optionally) within the field of view of a frame.
 
     Parameters
     ----------
 
-    frame_wcs : astropy.wcs.WCS
+    frame_wcs : `astropy.wcs.WCS`
         WCS of the image of interest.
 
     shape : tuple of int
+        Shape of the image of interest.
+
+    desired_catalog : str
+        Name of the catalog to be searched.
+
+    ra_column : str, optional
+        Name of the column in the catalog that contains the RA values.
+        Default is 'RAJ2000'.
+
+    dec_column : str, optional
+        Name of the column in the catalog that contains the Dec values.
+        Default is 'DEJ2000'.
+
+    radius : float, optional
+        Radius, in degrees, around which to search. Default is 0.5.
+
+    clip_by_frame : bool, optional
+        If ``True``, only return items that are within the field of view
+        of the frame. Default is ``True``.
+
+    padding : int, optional
+        Coordinates need to be at least this many pixels in from the edge
+        of the frame to be considered in the field of view. Default value
+        is 100.
+
+    Returns
+    -------
+
+    `astropy.table.Table`
+        Table of catalog information for stars in the field of view.
 
-    Description: This function takes coordinate data from an image and a
-    catalog name and returns the positions of those stars.
-    Preconditions:frame_wcs is a WCS object, shape is tuple, list or array of
-    numerical values, desired_catalog is a string and radius is a numerical
-    value.
-    Postconditions:
     """
     rad = radius * units.deg
     if isinstance(frame_wcs_or_center, SkyCoord):
         # Center was passed in, just use it.
         center = frame_wcs_or_center
         if clip_by_frame:
             raise ValueError('To clip entries by frame you must use '
@@ -93,111 +117,149 @@
     # Vizier always returns list even if there is only one element. Grab that
     # element.
     cat = cat[0]
     cat_coords = SkyCoord(ra=cat[ra_column], dec=cat[dec_column])
     if clip_by_frame:
         in_fov = in_frame(frame_wcs_or_center, cat_coords, padding=padding)
     else:
-        in_fov = np.ones([len(cat_coords)], dtype=np.bool)
+        in_fov = np.ones([len(cat_coords)], dtype=bool)
     return cat[in_fov]
 
 
 def catalog_clean(catalog, remove_rows_with_mask=True,
                   **other_restrictions):
     """
     Return a catalog with only the rows that meet the criteria specified.
 
     Parameters
     ----------
 
-    catalog : astropy.Table
+    catalog : `astropy.table.Table`
         Table of catalog information. There are no restrictions on the columns.
+
     remove_rows_with_mask : bool, optional
         If ``True``, remove rows in which one or more of the values is masked.
+
     other_restrictions: dict, optional
         Key/value pairs in which the key is the name of a column in the
         catalog and the value is the criteria that values in that column
         must satisfy to be kept in the cleaned catalog. The criteria must be
         simple, beginning with a comparison operator and including a value.
         See Examples below.
+
+    Returns
+    -------
+
+    `astropy.table.Table`
+        Table of catalog information for stars in the field of view.
+
     """
 
     comparisons = {
         '<': np.less,
         '=': np.equal,
         '>': np.greater,
         '<=': np.less_equal,
         '>=': np.greater_equal,
         '!=': np.not_equal
     }
 
     recognized_comparison_ops = '|'.join(comparisons.keys())
-    keepers = np.ones([len(catalog)], dtype=np.bool)
+    keepers = np.ones([len(catalog)], dtype=bool)
 
     if remove_rows_with_mask and catalog.masked:
         for c in catalog.columns:
             keepers &= ~catalog[c].mask
 
     for column, restriction in other_restrictions.items():
         criteria_re = re.compile(r'({})([-+a-zA-Z0-9]+)'.format(recognized_comparison_ops))
         results = criteria_re.match(restriction)
         if not results:
             raise ValueError("Criteria {}{} not "
                              "understood.".format(column, restriction))
         comparison_func = comparisons[results.group(1)]
         comparison_value = results.group(2)
         new_keepers = comparison_func(catalog[column],
-                                      np.float(comparison_value))
+                                      float(comparison_value))
         keepers = keepers & new_keepers
 
     return catalog[keepers]
 
 
 def find_apass_stars(image_or_center,
                      radius=1,
                      max_mag_error=0.05,
                      max_color_error=0.1):
     """
     Get APASS data from Vizer.
 
     Parameters
-    ---------
+    ----------
 
     image_or_center : `astropy.nddata.CCDData` or `astropy.coordinates.SkyCoord`
         Either an image with a WCS (from which the RA/Dec will be extracted) or coordinate of
         the center.
 
     radius : float, optional
         Radius, in degrees, around which to search. Not needed if the first argument is an image.
+
+    max_mag_error : float, optional
+        Maximum error in magnitude to allow. Default is 0.05.
+
+    max_color_error : float, optional
+        Maximum error in color to allow. Default is 0.1.
+
+    Returns
+    -------
+
+    all_apass : `astropy.table.Table`
+        Table of all APASS stars in the field of view.
+
+    apass_lower_error : `astropy.table.Table`
+        Table of APASS stars in the field of view with errors lower than the specified values.
     """
     if isinstance(image_or_center, SkyCoord):
         # Center was passed in, just use it.
         cen_wcs = image_or_center
         shape = None
     else:
         cen_wcs = image_or_center.wcs
         shape = image_or_center.shape
-    # use the catalog_search function to find the apass stars in the frame of the image read above
+    # use the catalog_search function to find the APASS stars in the frame of the image read above
     all_apass = catalog_search(cen_wcs, shape, 'II/336/apass9',
                                ra_column='RAJ2000', dec_column='DEJ2000', radius=radius,
                                clip_by_frame=False)
 
-    # Creates a boolean array of the apass stars that have well defined
+    # Creates a boolean array of the APASS stars that have well defined
     # magnitudes and color.
     apass_lower_error = (all_apass['e_r_mag'] < max_mag_error) & (
         all_apass['e_B-V'] < max_color_error)
 
-    # create new table  of apass stars that meet error restrictions
+    # create new table of APASS stars that meet error restrictions
     apass_lower_error = all_apass[apass_lower_error]
 
     return all_apass, apass_lower_error
 
 
 def find_known_variables(image):
-    # Get any known variable stars from a new catalog search of VSX
+    """
+    Get any known variable stars in image field from the VSX catalog.
+
+    Parameters
+    ----------
+
+    image : `astropy.nddata.CCDData`
+        Image with a WCS.
+
+    Returns
+    -------
+
+    vsx : `astropy.table.Table`
+        Table of known variable stars in the field of view.
+    """
     try:
         vsx = catalog_search(image.wcs, image.shape, 'B/vsx/vsx',
                              ra_column='RAJ2000', dec_column='DEJ2000')
     except IndexError:
         raise RuntimeError('No variables found in this field of view '
                            f'centered on {image.wcs}')
     return vsx
@@ -207,20 +269,27 @@
     """
     Filter catalog by key/value pairs in arguments and return bool
     area ``True`` where values in catalog meet the criteria.
 
     Parameters
     ----------
 
-    catalog : astropy Table
+    catalog : `astropy.table.Table`
         Table whose values are to be filtered.
 
     kwd : key/value pairs, e.g. ``e_r_mag=0.1``
         The key must be the name of a column and the value the
         *upper limit* on the acceptable values.
+
+    Returns
+    -------
+
+    `numpy.ndarray` of bool
+        One value for each row in the catalog; values are ``True`` if the
+        row meets the criteria, ``False`` otherwise.
     """
     good_ones = np.ones(len(catalog), dtype='bool')
 
     for key, value in kwd.items():
         print(key, value, catalog[key] <= value)
         good_ones &= (catalog[key] <= value)
```

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/magnitude_transforms.py` & `stellarphot-1.3.9/stellarphot/differential_photometry/magnitude_transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,96 +9,168 @@
 from astropy.coordinates import SkyCoord, match_coordinates_sky
 from astropy import units as u
 
 from astroquery.vizier import Vizier
 
 
 __all__ = [
+    'f', 'get_cat', 'opts_to_str', 'calc_residual',
     'filter_transform',
     'calculate_transform_coefficients',
     'transform_magnitudes',
-    'transform_to_catalog'
+    'transform_to_catalog',
 ]
 
 
 def f(X, a, b, c, d, z):
+    """
+    Calculate the calibrated magnitudes from the instrumental magnitudes and colors.
+
+    Parameters
+    ----------
+
+    X : tuple of numpy.ndarray
+        The first element is an array of instrumental magnitudes,
+        the second is an array of colors.
+
+    a, b, c, d, z : float
+        Parameters of the fit.
+
+    Returns
+    -------
+    `numpy.ndarray`
+        Array of calibrated magnitudes.
+    """
     mag_inst, color = X
 
     return a * mag_inst + b * mag_inst ** 2 + c * color + d * color**2 + z
 
 
-# TODO: THIS SHOULD ALMOST CERTAINLY BE REPLACED
 def get_cat(image):
+    """
+    Get the APASS catalog entries within 1 degree of first object in
+    Astropy table 'image'.
+
+    Parameters
+    ----------
+
+    image : `astropy.table.Table`
+        Table containing the image information. Must have columns
+        ``RA`` and ``Dec``.
+
+    Returns
+    -------
+
+    `astropy.table.Table`
+        Table containing the APASS catalog entries within 1 degree of
+        first object in Astropy table.
+    """
     our_coords = SkyCoord(image['RA'], image['Dec'], unit='degree')
     # Get catalog via cone search
     Vizier.ROW_LIMIT = -1  # Set row_limit to have no limit
     desired_catalog = 'II/336/apass9'
     a_star = our_coords[0]
     rad = 1 * u.degree
     cat = Vizier.query_region(a_star, radius=rad, catalog=desired_catalog)
     cat = cat[0]
     cat_coords =  SkyCoord(cat['RAJ2000'], cat['DEJ2000'])
     return cat, cat_coords
 
 
 def opts_to_str(opts):
+    """
+    Convert the options from a fit to a string.
+
+    Parameters
+    ----------
+
+    opts : tuple of float
+        Options from a fit.
+
+    Returns
+    -------
+
+    str
+        String representation of the options.
+    """
     opt_names = ['a', 'b', 'c', 'd', 'z']
     names = []
     for name, value in zip(opt_names, opts):
         names.append(f'{name}={value:.4f}')
     return ', '.join(names)
 
 
 def calc_residual(new_cal, catalog):
+    """
+    Calculate the standard deviations of the residuals between
+    the new calibrated magnitude and the catalog magnitude.
+
+    Parameters
+    ----------
+
+    new_cal : `numpy.ndarray`
+        New calibrated magnitudes.
+
+    catalog : `numpy.ndarray`
+        Catalog magnitudes.
+
+    Returns
+    -------
+
+    float
+        Standard deviation of the residual.
+
+    """
     resid = new_cal - catalog
     return resid.std()
 
 
 def filter_transform(mag_data, output_filter,
                      g=None, r=None, i=None,
                      transform=None):
-    '''
+    """
     Transform SDSS magnitudes to BVRI using either the transforms from
     Jester et al or Ivezic et al.
 
     Parameters
     ----------
 
-    mag_data : astropy.table.Table
+    mag_data : `astropy.table.Table`
         Table containing ``g``, ``r`` and ``i`` magnitudes (or at least)
         those required to transform to the desired output filter.
+
     output_filter : 'B', 'V', 'R' or 'I'
         Filter for which magnitude should be calculated. Note that
         *case matters* here.
+
     g, r, i : str
         Name of column in table for that magnitude.
+
     transform : 'jester' or 'ivezic'
         Transform equations to use.
-    Description: This function impliments the transforms in
-        'A Comparison of SDSS Standard
 
     Returns
     -------
 
-    astropy.table.Column
+    `astropy.table.Column`
         Output transformed magnitudes as a table column
 
     Notes
     -----
 
     The transforms implemented in this function are taken from:
 
     Jester, et al, *The Sloan Digital Sky Survey View of the Palomar-Green Bright Quasar Survey*, AJ 130, p. 873 (2005)
     http://iopscience.iop.org/article/10.1086/432466/meta
 
     Ivezić et al, *A Comparison of SDSS Standard Star Catalog for Stripe 82 with Stetson's Photometric Standards*,
     The Future Of Photometric, Spectrophotometric And Polarimetric Standardization, ASP Conference Series 364, p. 165 (2007)
     http://aspbooks.org/custom/publications/paper/364-0165.html
 
-    '''
+    """
     supported_transforms = ['jester', 'ivezic']
     if transform not in supported_transforms:
         raise ValueError('Transform {} is not known. Must be one of '
                          '{}'.format(transform, supported_transforms))
     transform_ivezic = {
         'B': [0.2628, -0.7952, 1.0544, 0.0268],
         'V': [0.0688, -0.2056, -0.3838, -0.0534],
@@ -165,45 +237,55 @@
     """
     Calculate linear transform coefficients from input magnitudes to catalog
     magnitudes.
 
     Parameters
     ----------
 
-    input_mag : numpy array or astropy Table column
+    input_mag : `numpy.ndarray` or `astropy.table.Column`
         Input magnitudes; for example, instrumental magnitudes.
-    catalog_mag : numpy array or astropy Table column
+
+    catalog_mag : `numpy.ndarray` or `astropy.table.Column`
         Catalog (or reference) magnitudes; the magnitudes to which the
         input_mag will eventually be transformed.
-    color : numpy array or astropy Table column
+
+    color : `numpy.ndarray` or `astropy.table.Column`
         Colors to use in determining transform coefficients.
-    input_mag_error : numpy array or astropy Table column, optional
+
+    input_mag_error : `numpy.ndarray` or `astropy.table.Column`, optional
         Error in input magnitudes. Default is zero.
-    catalog_mag_error : numpy array or astropy Table column, optional
+
+    catalog_mag_error : `numpy.ndarray` or `astropy.table.Column`, optional
         Error in catalog magnitudes. Default is zero.
+
     faintest_mag_for_transform : float, optional
         If this is not ``None``, the magnitude of the faintest catalog stars
         to use in computing transform coefficients.
+
     order : int, optional
         Order of the polynomial fit to use in correcting for color.
+
     sigma : float, optional
         Value of sigma to use to reject outliers while fitting using
         sigma clipping.
+
     gain : float, optional
         If not ``None``, adjust the instrumental magnitude by
         -2.5 * log10(gain), i.e. gain correct the magnitude.
+
     verbose : bool, optional
         If ``True``, print some diagnostic information.
+
     extended_output : bool, optional
         If ``True``, return additional information.
 
     Returns
     -------
 
-    filtered_data : `~numpy.ma.core.MaskedArray`
+    filtered_data : `numpy.ma.core.MaskedArray`
         The data, with the mask set ``True`` for the data that was *omitted*
         from the fit.
 
     model : `astropy.modeling.FittableModel`
         Entries in the model are the coefficients in the fit made to the
         data. Since the model is always a polynomial, these are terms in
         a polynomial in the order of ascending power. In other words, the
@@ -304,23 +386,22 @@
     """
     Calculate catalog magnitudes and transform coefficients
     from instrumental magnitudes.
 
     Parameters
     ----------
 
-    input_mags : astropy Table
+    input_mags : `astropy.table.Table`
         Table which contains a column with instrumental magnitudes, i.e.
         -2.5 * log10(net_counts / exposure_time).
 
-    catalog : astropy Table
+    catalog : `astropy.table.Table`
         Table containing reference catalog of magnitudes and colors.
 
-
-    transform_catalog : astropy Table
+    transform_catalog : `astropy.table.Table`
         Table containing the reference catalog of magnitudes and colors
         to use in determining the transform coefficients. Can be the
         same table as ``catalog`` if desired.
 
     input_mag_column : str, optional
         Name of the column in ``input_mags`` with the magnitudes to be
         transformed.
@@ -343,14 +424,30 @@
     order : int, optional
         Order of the polynomial to use in fitting magnitude difference/color
         relationship.
 
     gain : float, optional
         If not ``None``, adjust the instrumental magnitude by
         -2.5 * log10(gain), i.e. gain correct the magnitude.
+
+    Returns
+    -------
+
+    our_cat_mags : `astropy.table.Column`
+        The calculated catalog magnitudes for the stars in ``input_mags``.
+
+    good_match_all : `numpy.ndarray`
+        Boolean array indicating which stars in ``input_mags`` have a match
+        in the catalog.
+
+    transforms : `astropy.modeling.FittableModel`
+        The coefficients of the transform. The coefficients are in the order
+        of ascending power, i.e. the coefficient ``ci`` is the coefficient
+        of the term ``x**i``.  Warning: This returns a namedtuple if the fit
+        fails.
     """
     catalog_all_coords = SkyCoord(catalog['RAJ2000'],
                                   catalog['DEJ2000'],
                                   unit='deg')
 
     transform_catalog_coords = SkyCoord(transform_catalog['RAJ2000'],
                                         transform_catalog['DEJ2000'],
@@ -416,15 +513,15 @@
     """
     Transform a set of intrumental magnitudes to a standard system using either
     instrumental colors or catalog colors.
 
     Parameters
     ----------
 
-    observed_magnitudes_grouped : astropy.table.Table group
+    observed_magnitudes_grouped : `astropy.table.Table`
         An astropy table, grouped by whatever you want that sepearates the data into
         data from just one image. BJD of the center of the observatory is one reasonable choice
 
     obs_mag_col : str
         Name of the column in `observed_magnitudes_grouped` that contains instrumental
         magnitudes.
 
@@ -440,32 +537,39 @@
 
     cat_color : tuple of two strings
         Names of the two columns in the caatalog that should be used to calculate color. The magnitude
         difference will be calculated in the ortder the fitlers are given. For example, if the value is
         ``('r_mag', 'i_mag')`` then the calculated color will be the ``r_mag`` column minus
         the ``i_mag`` column.
 
-    a_delta, b_delta, c_delta, d_delta : flt, optional
+    a_delta, b_delta, c_delta, d_delta : float, optional
         Range allowed in fitting for each of the parameters ``a``, ``b``, ``c``, and ``d``. Use ``1E-6`` to fix a parameter.
 
-    a_cen : flt, optional
+    a_cen : float, optional
         Center of range for the fitting parameter ``a``.
 
-    zero_point_range : tuple of flt, optional
+    zero_point_range : tuple of float, optional
         Range to which the value of the zero point is restricted in fitting to observed magnitudes.
 
     in_place : bool, optional
         If ``True``, add the calibrated magnitude to the input table, othewise return a copy.
 
     fit_diff : bool, optional
         If ``True``, fit the difference between the instrumental and catalog magnitude instead of the
         treating the catalog mag as the dependent variable.
 
     verbose: bool optional
         If ``True``, print additional output.
+
+    Returns
+    -------
+
+    `astropy.table.Table`
+        Table containing the calibrated magnitudes and the fit parameters.
+
     """
 
     if obs_error_column is None:
         print("are you sure you want to do that? Error weighting is important!")
 
     fit_bounds_lower = [
         a_cen - a_delta,     # a
```

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/comp_stars.fits` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/comp_stars.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/data/variables.fits` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/variables.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/test_catalog_search.py` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_catalog_search.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/test_magnitude_transforms.py` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_magnitude_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                               dec_start=45 * u.degree,
                               separation=10 * u.arcsec):
     """
     Generate RA/Dec coordinates for a set of stars.
     """
     # The plus one guarantees we'll have enough positions for
     # all of our stars.
-    max_index = np.int(np.sqrt(n_stars)) + 1
+    max_index = int(np.sqrt(n_stars)) + 1
 
     grids = np.mgrid[:max_index, :max_index]
     dec_grid, ra_grid = grids
     dec_offsets = separation * dec_grid
     ra_offsets = separation * ra_grid
     ra = (ra_start + ra_offsets).flatten()
     dec = (dec_start + dec_offsets).flatten()
```

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/tests/test_vsx_mags.py` & `stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_vsx_mags.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/differential_photometry/vsx_mags.py` & `stellarphot-1.3.9/stellarphot/differential_photometry/vsx_mags.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/io/aavso_submission_schema.yml` & `stellarphot-1.3.9/stellarphot/io/aavso_submission_schema.yml`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/io/aij.py` & `stellarphot-1.3.9/stellarphot/io/aij.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,22 +3,45 @@
 
 import astropy.units as u
 from astropy.coordinates import SkyCoord
 from astropy.table import Table, hstack
 
 import numpy as np
 
-__all__ = ['parse_aij_table', 'ApertureFileAIJ']
+__all__ = [ 'ApertureAIJ', 'MultiApertureAIJ', 'ApertureFileAIJ',
+           'generate_aij_table', 'parse_aij_table', 'Star']
 
 
 class ApertureAIJ:
     """
-    Represent the aperture information AstroImageJ saves.
+    Represents the aperture information AstroImageJ saves.
+
+    Attributes
+    ----------
+    backplane : bool
+        Not sure what this does but stellarphot doesn't use it. Default: False
+
+    radius : float
+        Aperture radius. Default: 15.0
+
+    rback1 : float
+        Inner annulus radius. Default: 27.0
+
+    rback2 : float
+        Outer annulus radius. Default: 41.0
+
+    removebackstars : bool
+        Whether to remove stars in the annulus from the photometry. Default: True
+
     """
     def __init__(self):
+        """
+        Initialize and set default values for the attributes of the aperture object instance.
+        """
+
         # Outer annulus radius
         self.rback2 = 41.0
 
         # Inner annulus radius
         self.rback1 = 27.0
 
         # Aperture radius
@@ -48,17 +71,56 @@
                  for attr in attributes]
 
         return all(equal)
 
 
 class MultiApertureAIJ:
     """
-    Represent the multi-aperture information that AstroImageJ saves
+    Multi-aperture information that AstroImageJ saves.
+
+    Attributes
+    ----------
+
+    absmagapertures : list
+        List of absolute magnitudes of the apertures.
+
+    apfwhmfactor : float
+        Factor to multiply the aperture radius by relative to the FWHM. Default: 1.4
+
+    centroidstar : list
+        List of booleans indicating whether the aperture is a centroid star.
+
+    decapertures : list
+        List of Declinations of the apertures.
+
+    isalignstar : list
+        List of booleans indicating whether the aperture is an alignment star.
+
+    isrefstar : list
+        List of booleans indicating whether the aperture is a reference star.
+
+    naperturesmax : float
+        Maximum number of apertures. Default: 1000
+
+    raapertures : list
+        List of Right Ascensions of the apertures.
+
+    usevarsizeap : bool
+        Whether to use variable size apertures. Default: False
+
+    xapertures : list
+        List of x positions of the apertures.
+
+    yapertures : list
+        List of y positions of the apertures.
     """
     def __init__(self):
+        """
+        Initialize and set default values for the attributes of the multi-aperture object instance.
+        """
         # Default values for these chosen to match AIJ defaults
         # They are not used by stellarphot
         self.naperturesmax = 1000
         self.apfwhmfactor = 1.4
         self.usevarsizeap = False
 
         # Each attribute below should be list-like, all of the same length
@@ -126,17 +188,29 @@
         equal = simple_eq + float_eq
 
         return all(equal)
 
 
 class ApertureFileAIJ:
     """
-    Represent AstroImageJ aperture file.
+    Class to represent AstroImageJ aperture file.
+
+    Attributes
+    ----------
+
+    aperture : `~stellarphot.io.ApertureAIJ`
+        Aperture information.
+`
+    multiaperture : `~stellarphot.io.MultiApertureAIJ`
+        Multi-aperture information.
     """
     def __init__(self):
+        """
+        Initialize the AstroImageJ aperture file instance.
+        """
         self.aperture = ApertureAIJ()
         self.multiaperture = MultiApertureAIJ()
 
     def __str__(self):
         lines = []
 
         top_level_attrib = vars(self)
@@ -158,22 +232,37 @@
         # Add a trailing blank line
         return '\n'.join(lines) + '\n'
 
     def __eq__(self, other):
         return (self.aperture == other.aperture) and (self.multiaperture == other.multiaperture)
 
     def write(self, file):
+        """
+        Write the aperture object to a file.
+
+        Parameters
+        ----------
+
+        file : str
+            Name of the file to write.
+        """
         p = Path(file)
         p.write_text(str(self))
 
     @classmethod
     def read(cls, file):
         """
-        Generate aperture object from file. Happily, each line is basically a path
+        Generate aperture object from file.  Each line is basically a path
         to an attribute name followed by a value.
+
+        Parameters
+        ----------
+
+        file : str
+            Name of the file to read.
         """
 
         # Make the instance to return
 
         aij_aps = cls()
 
         with open(file, 'r') as f:
@@ -200,15 +289,15 @@
     @classmethod
     def from_table(cls, aperture_table,
                    aperture_rad=None, inner_annulus=None, outer_annulus=None,
                    default_absmag=99.999, default_isalign=True,
                    default_centroidstar=True,
                    y_size=4096):
         """
-        Create an `stellarphot.io.ApertureFileAIJ` from a stellarphot aperture
+        Create an `~stellarphot.io.ApertureFileAIJ` from a stellarphot aperture
         table and info about the aperture sizes.
 
         Parameters
         ----------
 
         aperture_table : `astropy.table.Table`
             Table of aperture information.
@@ -217,15 +306,21 @@
             Radius of aperture.
 
         inner_annulus : number
             Inner radius of annulus.
 
         outer_annulus : number
             Outer radius of annulus.
+
+        Returns
+        -------
+        apAIJ: `~stellarphot.io.ApertureFileAIJ`
+            ApertureFileAIJ object representing the aperture table.
         """
+
         # Create the instance
         apAIJ = cls()
 
         # Populate aperture properties
         apAIJ.aperture.rback2 = outer_annulus
         apAIJ.aperture.rback1 = inner_annulus
         apAIJ.aperture.radius = aperture_rad
@@ -271,14 +366,32 @@
 
 def _is_comp(star_coord, comp_table):
     idx, d2d, _ = star_coord.match_to_catalog_sky(comp_table['coord'])
     return 'comparison' in comp_table['marker name'][idx]
 
 
 def generate_aij_table(table_name, comparison_table):
+    """
+    Generate an AIJ table from a stellarphot table and a comparison table.
+
+    Parameters
+    ----------
+
+    table_name : `astropy.table.Table`
+        Table of stellarphot photometry.
+
+    comparison_table : `astropy.table.Table`
+        Table of comparison star photometry.
+
+    Returns
+    -------
+
+    base_table : `astropy.table.Table`
+        Table of photometry in AIJ format.
+    """
     info_columns = {
         'date-obs': 'DATE_OBS',
         'airmass': 'AIRMASS',
         'BJD': 'BJD_MOBS',
         'exposure': 'EXPOSURE',
         'filter': 'FILTER',
         'aperture': 'Source_Radius',
@@ -336,14 +449,21 @@
     photometry table.
 
     Parameters
     ----------
 
     table_name : str
         Name of the table.
+
+    Returns
+    -------
+
+    stars : list
+        List of `Star` objects.
+
     """
 
     # Read in the raw table.
     if table_name.endswith('.csv'):
         # The table may have been edited and changed to csv.
         raw = Table.read(table_name)
     else:
@@ -384,14 +504,86 @@
             my_table.rename_column(spec, gen)
         stars.append(Star(my_table, idx + 1))
 
     return stars
 
 
 class Star(object):
+    """
+    A class for storing photometry for a single star.
+
+    Parameters
+    ----------
+
+    table : `astropy.table.Table`
+        Table of photometry for a single star.
+
+    id_num : int
+        ID number of the star.
+
+    Attributes
+    ----------
+
+    airmass : `astropy.units.Quantity`
+        Airmass at the time of observation.
+
+    bjd_tdb : `astropy.units.Quantity`
+        Midpoint of the exposure as barycentric Julian date in Barycentric Dynamical Time.
+
+    counts : `astropy.units.Quantity`
+        Net counts in the aperture.
+
+    dec : `astropy.units.Quantity`
+        Declination of the star.
+
+    error : `astropy.units.Quantity`
+        Error in the net counts.
+
+    exposure : `astropy.units.Quantity`
+        Exposure time of the observation.
+
+    id: int
+        ID number of the star.
+
+    jd_utc_end : `astropy.units.Quantity`
+        Julian date of the end of the observation.
+
+    jd_utc_mid : `astropy.units.Quantity`
+        Julian date of the middle of the observation.
+
+    jd_utc_start : `astropy.units.Quantity`
+        Julian date of the start of the observation.
+
+    magnitude : `astropy.units.Quantity`
+        Magnitude of the star.
+
+    magnitude_error : `astropy.units.Quantity`
+        Error in the magnitude of the star.
+
+    mjd_utc_end : `astropy.units.Quantity`
+        Modified Julian date of the end of the observation.
+
+    mjd_utc_mid : `astropy.units.Quantity`
+        Modified Julian date of the middle of the observation.
+
+    mjd_utc_start : `astropy.units.Quantity`
+        Modified Julian date of the start of the observation.
+
+    peak : `astropy.units.Quantity`
+        Peak counts in the aperture.
+
+    ra : `astropy.units.Quantity`
+        Right ascension of the star.
+
+    sky_per_pixel : `astropy.units.Quantity`
+        Sky brightness per pixel.
+
+    snr : `astropy.units.Quantity`
+        Signal-to-noise ratio of the star.
+    """
     def __init__(self, table, id_num):
         self._table = table
         self._table['DEC'].unit = u.degree
         self.id = id_num
 
     @property
     def airmass(self):
```

### Comparing `stellarphot-1.3.8/stellarphot/io/tests/data/aij-sample-apertures.aperture` & `stellarphot-1.3.9/stellarphot/io/tests/data/aij-sample-apertures.aperture`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/io/tests/data/apertures_as_table.csv` & `stellarphot-1.3.9/stellarphot/io/tests/data/apertures_as_table.csv`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/io/tests/test_aij_io.py` & `stellarphot-1.3.9/stellarphot/io/tests/test_aij_io.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/io/tests/test_tess_submission.py` & `stellarphot-1.3.9/stellarphot/io/tests/test_tess_submission.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/ObserveACP.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8126556776556777%*

 * *Differences: {"'cells'": "{0: {'cell_type': 'markdown', 'source': ['# Comparison star generator'], delete: "*

 * *            "['execution_count', 'outputs']}, 1: {'source': ['import re\\n', '\\n', 'import "*

 * *            "requests\\n', '\\n', 'from astropy.coordinates import SkyCoord\\n', '\\n', 'from "*

 * *            "stellarphot.visualization.comparison_functions import ComparisonViewer\\n']}, 2: "*

 * *            "{'cell_type': 'markdown', 'source': ['## Change the settings in this cell as "*

 * *            "needed'], delete: ['execu […]*

```diff
@@ -1,180 +1,116 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "from acp import *"
+                "# Comparison star generator"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 2,
-            "metadata": {},
-            "outputs": [],
             "source": [
-                "obj = ObserveACP(\"m34\", \"2019-02-24\")"
+                "import re\n",
+                "\n",
+                "import requests\n",
+                "\n",
+                "from astropy.coordinates import SkyCoord\n",
+                "\n",
+                "from stellarphot.visualization.comparison_functions import ComparisonViewer\n"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 3,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "40.52083333 42.76166667\n"
-                    ]
-                }
-            ],
             "source": [
-                "print(obj.ra, obj.dec)"
+                "## Change the settings in this cell as needed"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Filter b is already in list!\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/plain": [
-                            "['Rc', 'b', 'i', 'r']"
-                        ]
-                    },
-                    "execution_count": 4,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "obj.add_filter('Rc')\n",
-                "obj.add_filter(('b', 'i', 'r'))\n",
-                "obj.add_filter('b')\n",
+                "bright_mag_limit = 9\n",
+                "dim_mag_limit = 16\n",
+                "Cmag = 10\n",
                 "\n",
-                "obj.filters"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "['b', 'i', 'r']"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "obj.rm_filter('Rc')\n",
-                "obj.filters"
+                "# \ud83d\udc49 File to save apertures in\n",
+                "aperture_output_file = 'aperture_locations.csv'\n",
+                "\n",
+                "# \ud83d\udc49 File to exoplanet info in\n",
+                "tess_info_output_file = 'tess-info.pickle'"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "'2019-02-24'"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "obj.date"
+                "comp_viewer = ComparisonViewer(\n",
+                "                           target_mag=Cmag,\n",
+                "                           bright_mag_limit=bright_mag_limit,\n",
+                "                           dim_mag_limit=dim_mag_limit,\n",
+                "                           targets_from_file=None,\n",
+                "                           aperture_output_file=aperture_output_file,\n",
+                "                          )\n",
+                "comp_viewer.box"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "3"
-                        ]
-                    },
-                    "execution_count": 7,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "obj.count(3)\n",
-                "obj.imCount"
+                "import pickle\n",
+                "\n",
+                "with open(tess_info_output_file, 'wb') as f:\n",
+                "    pickle.dump(comp_viewer.toi_info, f)\n",
+                "    "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "obj.expose(90)\n",
-                "obj.count(3)\n",
-                "obj.repeat(1)\n",
-                "obj.wait_until(\"01:23:45\")\n",
-                "obj.write('name of text file')"
+                "comp_viewer.toi_info.tic_id"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
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
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.6.6"
+            "version": "3.10.6"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/calculate_aavso_mags_draft.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/03-photometry-template.ipynb`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.81065021494709%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, 'from pathlib import Path\\n'), (1, '\\n'), (2, 'import "*

 * *            "numpy as np\\n'), (3, '\\n'), (4, 'from ipyfilechooser import FileChooser\\n'), (5, "*

 * *            "'\\n'), (6, 'from astropy.nddata import CCDData\\n'), (7, 'from astropy.coordinates "*

 * *            "import SkyCoord, EarthLocation\\n'), (11, 'from stellarphot.photometry import *\\n'), "*

 * *            "(12, 'from stellarphot.source_detection import *\\n'), (13, 'from stellarphot import "*

 * *            " […]*

```diff
@@ -1,129 +1,161 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6d973d4c-b1db-4f8b-82a2-e64990c07776",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from astropy.coordinates import SkyCoord\n",
+                "from pathlib import Path\n",
+                "\n",
+                "import numpy as np\n",
+                "\n",
+                "from ipyfilechooser import FileChooser\n",
+                "\n",
+                "from astropy.nddata import CCDData\n",
+                "from astropy.coordinates import SkyCoord, EarthLocation\n",
                 "from astropy.table import Table\n",
                 "from astropy.time import Time\n",
-                "from astropy.timeseries import TimeSeries\n",
                 "\n",
-                "from matplotlib import pyplot as plt\n",
+                "from stellarphot.photometry import *\n",
+                "from stellarphot.source_detection import *\n",
+                "from stellarphot import Camera\n",
                 "\n",
-                "from stellarphot.differential_photometry import vsx_mags\n"
+                "from stellarphot.visualization.photometry_widget_functions import PhotometrySettings"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Settings are below "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "294fa9a6-5522-414b-ad96-73da98cb3eea",
             "metadata": {},
             "outputs": [],
             "source": [
-                "your_photometry_file = 'v0553 her-2022-06-03.csv'\n",
-                "comp_stars_file = 'apass-V0533-Her.csv'\n",
-                "name_of_variable = 'v0533 her'\n",
-                "\n",
-                "# Our filter names vs filter names in comparison star table\n",
-                "filter_mapping = dict(\n",
-                "    ip='SI',\n",
-                "    B='B'\n",
-                ")"
+                "ps = PhotometrySettings()\n",
+                "ps.box"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "110085f6-4c91-4e55-9ced-fb64936acf69",
             "metadata": {},
             "outputs": [],
             "source": [
-                "var_coord = SkyCoord.from_name(name_of_variable)\n",
+                "# A single dot means \"the folder this notebook is in\"\n",
+                "folder_with_images = ps.image_folder # '.'\n",
                 "\n",
-                "vc = dict(coords=var_coord)"
+                "# The file name below should be the one you made with the comp-star template\n",
+                "# Its name should end .fits\n",
+                "source_file_name = ps.aperture_locations # 'aperture_locations.fits'\n",
+                "\n",
+                "# Enter the aperture radius from the viewer seeing template here\n",
+                "aperture = ps.aperture_radius\n",
+                "\n",
+                "# Enter the object name here\n",
+                "object_name = ps.object_name\n",
+                "\n",
+                "# Enter date data was taken here\n",
+                "date = '2021-09-28'\n",
+                "\n",
+                "# Enter the name you want to give the photometry file, i.e. the file with star counts, here\n",
+                "photometry_file = f'{object_name}-{date}.csv'"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### More settings (no need to change these typically)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7cd3031f-59ef-4b21-bad9-0075fc9b679a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "your_photometry = Table.read(your_photometry_file)\n",
-                "your_photometry['RA'].unit = 'degree'\n",
-                "your_photometry['Dec'].unit = 'degree'\n",
+                "inner_annulus = aperture + 15\n",
+                "outer_annulus = inner_annulus + 15\n",
                 "\n",
-                "your_photometry['band'] = your_photometry['filter']\n",
+                "feder_cg_16m = Camera(gain=1.5, read_noise=10.0, dark_current=0.01)\n",
                 "\n",
-                "comp_stars = Table.read(comp_stars_file)\n",
-                "comp_stars['RAJ2000'].unit = 'degree'\n",
-                "comp_stars['DEJ2000'].unit = 'degree'\n",
-                "\n"
+                "max_adu = 50000"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "23411fe8-7cd2-455d-ac74-058ec5df9c37",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## The cell below does just one filter..."
+                "image_directory = Path(folder_with_images)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "77fd8792-f47b-41ef-a489-f82f05b4d68f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "this_filter = 'ip'\n",
-                "\n",
-                "this_phot = your_photometry[your_photometry['band'] == this_filter]\n",
-                "\n",
-                "this_phot_grp = this_phot.group_by('BJD')\n",
+                "sources = Table.read(source_file_name)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sources['coord'] = SkyCoord(ra=[c.split(',')[0] for c in sources['coord']],\n",
+                "                            dec=[c.split(',')[1] for c in sources['coord']],\n",
+                "                            unit='degree',\n",
+                "                            frame='icrs')\n",
+                "star_ra = sources['coord'].ra\n",
+                "star_dec = sources['coord'].dec\n",
                 "\n",
-                "times = []\n",
-                "cal_mag = []\n",
-                "cal_mag_err = []\n",
-                "for time, rows in zip(this_phot_grp.groups.keys, this_phot_grp.groups):\n",
-                "    mag, err = vsx_mags.calc_vmag(vc, rows, comp_stars, band=filter_mapping[this_filter], star_data_mag_column=f'mag_inst_{this_filter}')\n",
-                "    cal_mag.append(mag)\n",
-                "    cal_mag_err.append(err)\n",
-                "    times.append(time[0])"
+                "main_target_coords = sources[sources['star_id'] == 1]['coord']"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "5ec0ee07-89f5-495a-b1ed-549e61fdf73f",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Sample plot...."
+                "photometry_table = photometry_on_directory(\n",
+                "                        image_directory, object_name, \n",
+                "                        (star_ra, star_dec), \n",
+                "                        aperture, inner_annulus, outer_annulus, \n",
+                "                        max_adu, sources['star_id'], \n",
+                "                        feder_cg_16m,\n",
+                "                        observatory_location='feder',\n",
+                "                        bjd_coords=main_target_coords,\n",
+                "                        fwhm_by_fit=False                \n",
+                "                    )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ed95a387-bcbb-41f8-9aca-d872ba53baa9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.errorbar(times, cal_mag, yerr=cal_mag_err, fmt='s')\n",
-                "plt.grid()"
+                "photometry_table.write(photometry_file)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d88f4d8a-8fb4-46dd-838d-709adc75d3d2",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -137,13 +169,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.5"
+            "version": "3.10.6"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/comp-star-plots.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/comp-star-plots.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9726339285714286%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(8, 'from stellarphot.io import parse_aij_table\\n'), (10, "*

 * *            "'from stellarphot.visualization import multi_night\\n')], delete: [10, 8]}}, 1: "*

 * *            "{'attachments': OrderedDict()}, 3: {'attachments': OrderedDict()}, 5: {'attachments': "*

 * *            "OrderedDict()}, 9: {'attachments': OrderedDict()}, 12: {'attachments': "*

 * *            "OrderedDict()}, 14: {'attachments': OrderedDict()}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'SNdev2', 'name' […]*

```diff
@@ -12,22 +12,23 @@
                 "\n",
                 "import numpy as np\n",
                 "\n",
                 "%matplotlib inline\n",
                 "\n",
                 "#import matplotlib.pyplot as plt\n",
                 "\n",
-                "from glowing_waffles.io import parse_aij_table\n",
+                "from stellarphot.io import parse_aij_table\n",
                 "\n",
-                "from glowing_waffles.visualization import multi_night\n",
+                "from stellarphot.visualization import multi_night\n",
                 "\n",
                 "from astropy.table import Table, Column"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Set the name of your file in the cell below\n",
                 "\n",
                 "The function below can read in either a raw AIJ file or csv files with the same information."
             ]
@@ -40,14 +41,15 @@
             },
             "outputs": [],
             "source": [
                 "sources = parse_aij_table('')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Set EITHER the list of known variables or the list of comparison stars\n",
                 "\n",
                 "Do **NOT** set both.\n",
                 "\n",
@@ -75,14 +77,15 @@
                 "\n",
                 "if known_variables is not None and keepers is not None:\n",
                 "    raise ValueError('Only ONE of known_variables and keeps can be set. '\n",
                 "                     'The other should be set to None.')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Calculate comparison counts, AIJ-style\n",
                 "\n",
                 "Which is to say that we calculate the comparison counts as the unweighted sum of the counts of all of the comparison stars, exceluding any known variables from the set."
             ]
@@ -135,14 +138,15 @@
                 "    snr = gain * source.counts / err\n",
                 "    mag_e = 1/snr\n",
                 "    mags.append(mag)\n",
                 "    mag_err.append(mag_e)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Find unique date for each night\n",
                 "\n",
                 "We need to do this to group the data by night."
             ]
@@ -173,14 +177,15 @@
             },
             "outputs": [],
             "source": [
                 "means = [np.median(mag[np.isfinite(mag)]) for mag in mags]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Use second brightest star to scale brightness marker"
             ]
         },
         {
@@ -193,14 +198,15 @@
             "source": [
                 "means.sort()\n",
                 "brightest_mag = np.max([means[1], -10])\n",
                 "print(brightest_mag)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Plot the nights"
             ]
         },
         {
@@ -215,27 +221,27 @@
                 "multi_night(sources, unique_nights, night,\n",
                 "            brightest_mag, mags, mag_err)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 2",
+            "display_name": "SNdev2",
             "language": "python",
-            "name": "python2"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
-                "version": 2
+                "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.11"
+            "pygments_lexer": "ipython3",
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 0
 }
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/comp-stars-template.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9858346676997245%*

 * *Differences: {"'cells'": '{4: {\'source\': {insert: [(0, "directory_with_images = \'..\'\\n"), (2, \'# 👉 This '*

 * *            "could be any image from roughly the middle of the sequence.\\n'), (3, "*

 * *            '"sample_image_for_finding_stars = \'TIC_237205154.01-S001-R013-C001-rp.fit\'\\n"), '*

 * *            "(5, '# 👉 You will be able to use this name later to pull out the data you want\\n'), "*

 * *            '(6, "object_of_interest = \'TIC_237205154.01\'\\n"), (8, \'# 👉 Get these variable '*

 * *            'from ExoFOP-TESS or  […]*

```diff
@@ -53,32 +53,37 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "directory_with_images = '.'\n",
+                "directory_with_images = '..'\n",
                 "\n",
-                "#This could be any image from roughly the middle of the sequence.\n",
-                "sample_image_for_finding_stars = 'TIC_470127886.01-S001-R001-C001-rp.fit'\n",
+                "# \ud83d\udc49 This could be any image from roughly the middle of the sequence.\n",
+                "sample_image_for_finding_stars = 'TIC_237205154.01-S001-R013-C001-rp.fit'\n",
                 "\n",
-                "# This name should be one of the \"aliases\" for the object if it is a TIC object\n",
-                "object_of_interest = 'TYC 4612-401-1'\n",
+                "# \ud83d\udc49 You will be able to use this name later to pull out the data you want\n",
+                "object_of_interest = 'TIC_237205154.01'\n",
                 "\n",
-                "# Get these variable from ExoFOP-TESS or Exoplanet ETD\n",
-                "ra_object = '22:04:28.27'\n",
-                "dec_object = '81:33:57.42'\n",
+                "# \ud83d\udc49 Get these variable from ExoFOP-TESS or Exoplanet ETD\n",
+                " \n",
+                "ra_object = '19:34:19.97'\n",
+                "dec_object = '76:39:39.91'\n",
                 "\n",
-                "Cmag = 10.76 # Use TESS magnitude for this\n",
-                "depth = 13280 / 1000 # Depth should be in parts per thousand, ExoFOP gives it in ppm.\n",
+                "Cmag = 13.0024 # \ud83d\udc49 Use TESS magnitude from ExoFOP-TESSfor this\n",
+                "depth = 16908.821 / 1000 # \ud83d\udc49 Depth should be in parts per thousand, ExoFOP gives it in ppm.\n",
                 "\n",
+                "bright_mag_limit = 9\n",
+                "dim_mag_limit = 16\n",
+                "\n",
+                "# \ud83d\udc49 File to save apertures in\n",
                 "aperture_output_file = 'aperture_locations.fits'\n",
                 "\n",
-                "TESS_target = False  # change to False (capitalized) if this is NOT a TESS object\n",
+                "TESS_target = True  # change to False (capitalized) if this is NOT a TESS object\n",
                 "\n",
                 "if TESS_target:\n",
                 "    server = \"https://www.astro.louisville.edu\"\n",
                 "    gaia_aperture_url = server + f\"/cgi-bin/gaia_to_aij/upload_request.cgi?ra={ra_object}&dec={dec_object}&mag={Cmag}&depth={depth}\"\n",
                 "\n",
                 "    result = requests.get(gaia_aperture_url)\n",
                 "    links = re.search('href=\"(.+)\"', result.text.replace('\\n', ''), )\n",
@@ -111,16 +116,16 @@
                 "           directory_with_images=directory_with_images\n",
                 "           )\n",
                 "\n",
                 "apass, vsx_apass_angle, targets_apass_angle = match(ccd, targets_from_file, vsx)\n",
                 "\n",
                 "apass_good_coord, good_stars = mag_scale(Cmag, apass, vsx_apass_angle,\n",
                 "                                         targets_apass_angle,\n",
-                "                                         brighter_dmag=3,\n",
-                "                                         dimmer_dmag=2)\n",
+                "                                         brighter_dmag=Cmag - bright_mag_limit,\n",
+                "                                         dimmer_dmag=dim_mag_limit - Cmag)\n",
                 "\n",
                 "apass_comps = in_field(apass_good_coord, ccd, apass, good_stars)\n",
                 "\n",
                 "box, iw = viewer()\n",
                 "\n",
                 "make_markers(iw, ccd, targets_from_file, vsx, apass_comps,\n",
                 "             name_or_coord=coordinate)\n",
@@ -220,17 +225,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "new_vsx_mark = comp_table['marker name'] == 'VSX'\n",
+                "vsx_dict = {}\n",
                 "idx, _, _ = comp_table['coord'][new_vsx_mark].match_to_catalog_sky(vsx['coords'])\n",
                 "for our_name, vsx_name in zip(comp_table['id'][new_vsx_mark], vsx['Name'][idx]):\n",
-                "    print(f'Our id number: {our_name}, VSX name: {vsx_name}')"
+                "    print(f'Our id number: {our_name}, VSX name: {vsx_name}')\n",
+                "    vsx_dict[f'V{our_name}'] = vsx_name"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Label the stars with numbers"
@@ -238,30 +245,44 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "plot_names = []\n",
                 "for star in comp_table:\n",
                 "    star_id = star['id']\n",
                 "    if star['marker name'] == 'TESS Targets':\n",
-                "        iw._marker = functools.partial(iw.dc.Text, text=f'T{star_id}', fontsize=20, fontscale=False, color='green')\n",
+                "        label = f'T{star_id}'\n",
+                "        iw._marker = functools.partial(iw.dc.Text, text=label, fontsize=20, fontscale=False, color='green')\n",
                 "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
                 "\n",
                 "    elif star['marker name'] == 'APASS comparison':\n",
-                "        iw._marker = functools.partial(iw.dc.Text, text=f'C{star_id}', fontsize=20, fontscale=False, color='red')\n",
+                "        label = f'C{star_id}'\n",
+                "        iw._marker = functools.partial(iw.dc.Text, text=label, fontsize=20, fontscale=False, color='red')\n",
                 "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
                 "\n",
                 "    elif star['marker name'] == 'VSX':\n",
-                "        iw._marker = functools.partial(iw.dc.Text, text=f'V{star_id}', fontsize=20, fontscale=False, color='blue')\n",
+                "        label = f'V{star_id}'\n",
+                "        iw._marker = functools.partial(iw.dc.Text, text=label, fontsize=20, fontscale=False, color='blue')\n",
                 "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
                 "    else:\n",
+                "        label = f'U{star_id}'\n",
                 "        print(f\"Unrecognized marker name: {star['marker name']}\")\n",
-                "        "
+                "    plot_names.append(label)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "comp_table['plot_label'] = [plot_names]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -297,27 +318,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
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
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.3"
+            "version": "3.10.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/example_interactive_plot.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/comp-stars-template.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7678376793290786%*

 * *Differences: {"'cells'": "{4: {'metadata': {replace: OrderedDict()}, 'source': {insert: [(0, "*

 * *            '"directory_with_images = \'.\'\\n"), (2, \'#This could be any image from roughly the '*

 * *            'middle of the sequence.\\n\'), (3, "sample_image_for_finding_stars = '*

 * *            '\'TIC_470127886.01-S001-R001-C001-rp.fit\'\\n"), (5, \'# This name should be one of '*

 * *            'the "aliases" for the object if it is a TIC object\\n\'), (6, "object_of_interest = '*

 * *            '\'TYC 4612-401-1\'\\n"), (8, \'# Ge […]*

```diff
@@ -1,265 +1,332 @@
 {
     "cells": [
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Comparison star generator"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## For information about your TESS target\n",
+                "\n",
+                "1. Go to https://exofop.ipac.caltech.edu/tess/\n",
+                "2. Enter the TIC number in the TIC search box\n",
+                "2. Use the RA/Dec for the `ra` and `dec` variables in the cell below.\n",
+                "3. Use the \"TESS mag\" for the variable `Cmag` in the cell below.\n",
+                "4. Use the \"depth\" for the variable `depth` in the cell below."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "from __future__ import print_function, division\n",
-                "\n",
-                "import ipywidgets as ipw\n",
+                "import functools\n",
+                "import re\n",
+                "from pathlib import Path\n",
+                "import requests\n",
                 "\n",
                 "import numpy as np\n",
                 "\n",
-                "from skimage.measure import block_reduce\n",
+                "from astropy import units as u\n",
+                "from astropy.table import Table\n",
+                "from astropy.coordinates import SkyCoord\n",
+                "\n",
+                "from stellarphot.visualization.comparison_functions import (\n",
+                "    read_file, set_up, crossmatch_APASS2VSX, mag_scale, in_field, wrap, make_markers,\n",
+                "    viewer\n",
+                ")\n",
+                "from stellarphot.visualization.seeing_profile_functions import set_keybindings"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Change the settings in this cell as needed"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "directory_with_images = '.'\n",
+                "\n",
+                "#This could be any image from roughly the middle of the sequence.\n",
+                "sample_image_for_finding_stars = 'TIC_470127886.01-S001-R001-C001-rp.fit'\n",
                 "\n",
-                "from astropy.visualization import scale_image\n",
-                "from astropy.nddata import block_replicate\n",
-                "from ccdproc import CCDData\n",
+                "# This name should be one of the \"aliases\" for the object if it is a TIC object\n",
+                "object_of_interest = 'TYC 4612-401-1'\n",
                 "\n",
-                "from photutils.morphology import (centroid_com, centroid_1dg,\n",
-                "                                  centroid_2dg)\n",
+                "# Get these variable from ExoFOP-TESS or Exoplanet ETD\n",
+                "ra_object = '22:04:28.27'\n",
+                "dec_object = '81:33:57.42'\n",
                 "\n",
-                "import matplotlib.pyplot as plt\n",
+                "Cmag = 10.76 # Use TESS magnitude for this\n",
+                "depth = 13280 / 1000 # Depth should be in parts per thousand, ExoFOP gives it in ppm.\n",
                 "\n",
-                "# The nbagg backend is what allows the interactivity.\n",
-                "%matplotlib notebook"
+                "aperture_output_file = 'aperture_locations.fits'\n",
+                "\n",
+                "TESS_target = False  # change to False (capitalized) if this is NOT a TESS object\n",
+                "\n",
+                "if TESS_target:\n",
+                "    server = \"https://www.astro.louisville.edu\"\n",
+                "    gaia_aperture_url = server + f\"/cgi-bin/gaia_to_aij/upload_request.cgi?ra={ra_object}&dec={dec_object}&mag={Cmag}&depth={depth}\"\n",
+                "\n",
+                "    result = requests.get(gaia_aperture_url)\n",
+                "    links = re.search('href=\"(.+)\"', result.text.replace('\\n', ''), )\n",
+                "\n",
+                "    target_file_contents = requests.get(server + links[1])\n",
+                "    with open('gaia_stars.radec', 'wt') as f:\n",
+                "        f.write(target_file_contents.text)\n",
+                "    targets_from_file = read_file('gaia_stars.radec')\n",
+                "else:\n",
+                "    targets_from_file = []"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# This function really should be somewhere else eventually.\n",
-                "def scale_and_downsample(data, downsample=4,\n",
-                "                         min_percent=20,\n",
-                "                         max_percent=99.5):\n",
+                "coordinate = SkyCoord(ra=ra_object, dec=dec_object, unit=(\"hour\", \"degree\"))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ccd, vsx = \\\n",
+                "    set_up(sample_image_for_finding_stars,\n",
+                "           directory_with_images=directory_with_images\n",
+                "           )\n",
+                "\n",
+                "apass, vsx_apass_angle, targets_apass_angle = crossmatch_APASS2VSX(ccd, targets_from_file, vsx)\n",
                 "\n",
-                "    scaled_data = scale_image(data,\n",
-                "                              min_percent=min_percent,\n",
-                "                              max_percent=max_percent)\n",
+                "apass_good_coord, good_stars = mag_scale(Cmag, apass, vsx_apass_angle,\n",
+                "                                         targets_apass_angle,\n",
+                "                                         brighter_dmag=3,\n",
+                "                                         dimmer_dmag=2)\n",
                 "\n",
-                "    if downsample > 1:\n",
-                "        scaled_data = block_reduce(scaled_data,\n",
-                "                                   block_size=(downsample, downsample))\n",
-                "    return scaled_data\n",
-                "\n"
+                "apass_comps = in_field(apass_good_coord, ccd, apass, good_stars)\n",
+                "\n",
+                "box, iw = viewer()\n",
+                "\n",
+                "make_markers(iw, ccd, targets_from_file, vsx, apass_comps,\n",
+                "             name_or_coord=coordinate)\n",
+                "\n",
+                "box"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Get the table of marked stars."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "all_table = iw.get_markers(marker_name='all')\n",
+                "elims = np.array([name.startswith('elim')\n",
+                "                 for name in all_table['marker name']])\n",
+                "elim_table = all_table[elims]\n",
+                "comp_table = all_table[~elims]"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Remove any that are marked for elimination as comparisons."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# test_image contains the actual data\n",
-                "test_image = CCDData.read('M52-002R.fit')\n",
+                "index, d2d, d3d = elim_table['coord'].match_to_catalog_sky(comp_table['coord'])\n",
+                "comp_table.remove_rows(index)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Sort the table"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "if targets_from_file:\n",
+                "    target_coord = targets_from_file['coords'][0]\n",
+                "else:\n",
+                "    target_coord = SkyCoord(ra=ra_object, dec=dec_object, unit=(\"hour\", \"degree\"))\n",
                 "\n",
-                "# test_scaled is what is displayed later. It has been scaled to bring out the dim stars.\n",
-                "test_scaled = scale_and_downsample(test_image, downsample=1)\n",
+                "# Calculate how far each is from target\n",
+                "comp_table['separation'] = target_coord.separation(comp_table['coord'])\n",
                 "\n",
-                "# For testing, just working with a part of the image.\n",
+                "# Add dummy column for sorting in the order we want\n",
+                "comp_table['sort'] = np.zeros(len(comp_table))\n",
                 "\n",
-                "x_cut = slice(0, 1000)\n",
-                "y_cut = slice(0, 1500)\n",
+                "# Set sort order\n",
+                "apass_mark = comp_table['marker name'] == 'APASS comparison'\n",
+                "vsx_mark = comp_table['marker name'] == 'VSX'\n",
+                "tess_mark = ((comp_table['marker name'] == 'TESS Targets') | \n",
+                "        (comp_table['separation'] < 0.3 * u.arcsec))\n",
                 "\n",
-                "# Slice out the piece we are using for testing from the display image.\n",
-                "test_scaled = test_scaled[x_cut, y_cut]\n",
                 "\n",
-                "# Make sure we do the same cut from the data.\n",
-                "image_cut = test_image.data[x_cut, y_cut]\n",
+                "comp_table['sort'][apass_mark] = 2\n",
+                "comp_table['sort'][vsx_mark] = 1\n",
+                "comp_table['sort'][tess_mark] = 0\n",
                 "\n",
-                "# For photometry or center finding need to do at least a rough removal of\n",
-                "# the background in the image.\n",
-                "image_cut -= np.median(image_cut)\n",
+                "# Ensure the target is always first\n",
                 "\n",
-                "# We could mask out bad pixels....for now we will not.\n",
-                "mask = image_cut > 1e6\n",
-                "mask.sum()"
+                "\n",
+                "# Sort the table\n",
+                "comp_table.sort(['sort', 'separation'])\n",
+                "\n",
+                "# Assign the IDs\n",
+                "comp_table['id'] = range(1, len(comp_table) + 1)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Display information on variables"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "test_image.wcs"
+                "new_vsx_mark = comp_table['marker name'] == 'VSX'\n",
+                "idx, _, _ = comp_table['coord'][new_vsx_mark].match_to_catalog_sky(vsx['coords'])\n",
+                "for our_name, vsx_name in zip(comp_table['id'][new_vsx_mark], vsx['Name'][idx]):\n",
+                "    print(f'Our id number: {our_name}, VSX name: {vsx_name}')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## None of the code below should end up in the notebook \n",
-                "\n",
-                "Eventually it should all be in python modules we are importing from or encapsulted in a class."
+                "### Label the stars with numbers"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# Make the plot and display the scaled image. Stick with grayscale, but reversed.\n",
+                "for star in comp_table:\n",
+                "    star_id = star['id']\n",
+                "    if star['marker name'] == 'TESS Targets':\n",
+                "        iw._marker = functools.partial(iw.dc.Text, text=f'T{star_id}', fontsize=20, fontscale=False, color='green')\n",
+                "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
+                "\n",
+                "    elif star['marker name'] == 'APASS comparison':\n",
+                "        iw._marker = functools.partial(iw.dc.Text, text=f'C{star_id}', fontsize=20, fontscale=False, color='red')\n",
+                "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
+                "\n",
+                "    elif star['marker name'] == 'VSX':\n",
+                "        iw._marker = functools.partial(iw.dc.Text, text=f'V{star_id}', fontsize=20, fontscale=False, color='blue')\n",
+                "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
+                "    else:\n",
+                "        print(f\"Unrecognized marker name: {star['marker name']}\")\n",
+                "        "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "comp_table.write(aperture_output_file, overwrite=True)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Add 2.5 arcmin circle (do this after writing comparison table!)\n",
                 "\n",
-                "fig = plt.figure()\n",
-                "ax = fig.add_subplot(111)\n",
-                "ax.imshow(test_scaled, cmap='gray_r',)\n",
-                "\n",
-                "# Not quite sure why this is needed but it seems to be.\n",
-                "ax.set_xlim(0, test_scaled.shape[1])\n",
-                "ax.set_ylim(test_scaled.shape[0], 0)\n",
-                "\n",
-                "# Define functions to handle some of the possible events. There is no reason we \n",
-                "# need to actually handle all of these events, this is just to show the kind of \n",
-                "# things that are possible.\n",
-                "\n",
-                "def onclick(event):\n",
-                "    \"\"\"\n",
-                "    Display a circle around the star closest to the place the user clicked.\n",
-                "    \n",
-                "    What 'closest' really means here is the location found in a small region\n",
-                "    near the click using a method pulled from photutils.\n",
-                "    \"\"\"\n",
-                "    \n",
-                "    # Size of small region near the click.\n",
-                "    stamp_size = 20\n",
-                "    \n",
-                "    # Get the location of the click, rounded to the nearest pixel. Note\n",
-                "    # that the event.x is a number from 0 to 1 covering the whole drawing \n",
-                "    # canvas, but event.xdata is the position indicated in the units \n",
-                "    # on the axes.\n",
-                "    click_x_data = np.int(event.xdata)\n",
-                "    click_y_data = np.int(event.ydata)\n",
-                "    \n",
-                "    # Define a slice centered on the click\n",
-                "    slice_x = slice(click_x_data - stamp_size/2, click_x_data + stamp_size/2)\n",
-                "    slice_y = slice(click_y_data - stamp_size/2, click_y_data + stamp_size/2)\n",
-                "\n",
-                "    # IMPORTANT: the cutout is done from the DATA not from the displayed image.\n",
-                "    cutout = image_cut[slice_y, slice_x]\n",
-                "    \n",
-                "    # Use centroid_2dg form photutils to find the center of any Gaussian-like maxima\n",
-                "    # in the cutout.\n",
-                "    center_x, center_y = centroid_2dg(cutout, mask=mask[slice_y, slice_x])\n",
-                "\n",
-                "    # Really just changing the title for debugging to make sure something \n",
-                "    # happened.\n",
-                "    ax.set_title('button=%d, x=%d, y=%d, xdata=%f, ydata=%f'%(\n",
-                "        event.button, event.x, event.y, event.xdata, event.ydata))\n",
-                "    \n",
-                "    # More debugging.\n",
-                "    ax.set_xlabel('x=%f y=%f, cx=%f cy=%f' % (center_x, center_y, \n",
-                "                                           event.xdata + (center_x - stamp_size/2),\n",
-                "                                           event.ydata + (center_y - stamp_size/2)))\n",
-                "    \n",
-                "    # Add the marker in a few steps...\n",
-                "    \n",
-                "    # Calculate the x position of the centroid position in the larger\n",
-                "    # array (NOTE: this whole cutout thing could be improved by using\n",
-                "    # the Cutout2D class from astropy.nddata, I think)\n",
-                "    \n",
-                "    x_center_in_data = event.xdata + (center_x - stamp_size/2)\n",
-                "    y_center_in_data = event.ydata + (center_y - stamp_size/2)\n",
-                "\n",
-                "    # Draw the marker. Eventually probably need to use ax.scatter to\n",
-                "    # be able to change the size of the marker in some sensible way.\n",
-                "    ax.plot([x_center_in_data], \n",
-                "            [y_center_in_data], 'o', \n",
-                "            markerfacecolor='none', \n",
-                "            markeredgecolor='cyan',)\n",
-                "    \n",
-                "    display_cutout(cutout, ax)\n",
-                "    \n",
-                "    # Really no good reason for this.\n",
-                "    ax.set_ylabel('%f' % cutout.sum())\n",
-                "\n",
-                "# You can call this (and the other event handling functions) anything\n",
-                "# you want.\n",
-                "def on_key(event):\n",
-                "    plt.xlabel('you pressed {}'.format(event.key, event.xdata, event.ydata))\n",
-                "    \n",
-                "def off_key(event):\n",
-                "    plt.xlabel('you released {}'.format(event.key, event.xdata, event.ydata))\n",
-                "\n",
-                "# Drawing a new image for mouse movement events seems a little slow, at least\n",
-                "# if the plot is open for a while.\n",
-                "def mouse_moved(event):\n",
-                "    # Yuck. This code duplicates the click stuff above.\n",
-                "    stamp_size = 20\n",
-                "    click_x_data = np.int(event.xdata)\n",
-                "    click_y_data = np.int(event.ydata)\n",
-                "    slice_x = slice(click_x_data-stamp_size/2, click_x_data+stamp_size/2)\n",
-                "    slice_y = slice(click_y_data-stamp_size/2, click_y_data+stamp_size/2)\n",
-                "    cutout = image_cut[slice_y, slice_x]\n",
-                "    \n",
-                "    display_cutout(cutout, ax)\n",
-                "    plt.xlabel('you moved {}'.format(event.key, event.xdata, event.ydata))\n",
-                "\n",
-                "def display_cutout(cutout, ax, min_width=300):\n",
-                "    # Display a little zoom-in of the cutout. No good reason \n",
-                "    # for doing that, really. Use a different colormap so the cutout\n",
-                "    # stands out.\n",
-                "    \n",
-                "    # Scale up the cutout in size first so it isn't tiny...\n",
-                "    zoom_factor = min_width // max(cutout.shape)\n",
-                "    scaled_up = block_replicate(cutout, block_size=zoom_factor)\n",
-                "    # Display it.\n",
-                "    ax.imshow(scaled_up, cmap='viridis')\n",
-                "    \n",
-                "\n",
-                "# This is where the functions defined above get connected to specific \n",
-                "# events.\n",
-                "cid1 = fig.canvas.mpl_connect('button_press_event', onclick)\n",
-                "cid2 = fig.canvas.mpl_connect('key_press_event', on_key)\n",
-                "cid3 = fig.canvas.mpl_connect('key_release_event', off_key)\n",
-                "#cid4 = fig.canvas.mpl_connect('motion_notify_event', mouse_moved)"
+                "Otherwise the comparison table will contain an extra entry for this circle."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "if targets_from_file:\n",
+                "    target = targets_from_file[0]\n",
+                "    iw.marker = {'color': 'yellow', 'radius': 268, 'type': 'circle'}\n",
+                "    iw.add_markers(target, skycoord_colname='coords',\n",
+                "                   use_skycoord=True, marker_name='target')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 2",
+            "display_name": "Python 3",
             "language": "python",
-            "name": "python2"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
-                "version": 2
+                "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.11"
+            "pygments_lexer": "ipython3",
+            "version": "3.8.3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 0
+    "nbformat_minor": 4
 }
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/image-viewer-working-copy.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/image-viewer-working-copy.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8191633427073768%*

 * *Differences: {"'cells'": "{0: {'cell_type': 'code', 'source': {insert: [(0, 'from pathlib import Path\\n'), (1, "*

 * *            "'from astropy.coordinates import SkyCoord\\n'), (2, 'from astropy.table import "*

 * *            "Table\\n'), (3, 'from astropy.time import Time\\n'), (4, 'from astropy.timeseries "*

 * *            "import TimeSeries\\n'), (6, 'from matplotlib import pyplot as plt\\n'), (7, '\\n'), "*

 * *            "(8, 'from stellarphot.differential_photometry import vsx_mags\\n')], delete: [6, 5, "*

 * *            "4, 3, 2,  […]*

```diff
@@ -1,324 +1,299 @@
 {
     "cells": [
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Comparison star generator"
-            ]
-        },
-        {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6d973d4c-b1db-4f8b-82a2-e64990c07776",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## For information about your TESS target\n",
+                "from pathlib import Path\n",
+                "from astropy.coordinates import SkyCoord\n",
+                "from astropy.table import Table\n",
+                "from astropy.time import Time\n",
+                "from astropy.timeseries import TimeSeries\n",
                 "\n",
-                "1. Go to https://exofop.ipac.caltech.edu/tess/\n",
-                "2. Enter the TIC number in the TIC search box\n",
-                "2. Use the RA/Dec for the `ra` and `dec` variables in the cell below.\n",
-                "3. Use the \"TESS mag\" for the variable `Cmag` in the cell below.\n",
-                "4. Use the \"depth\" for the variable `depth` in the cell below."
+                "from matplotlib import pyplot as plt\n",
+                "\n",
+                "from stellarphot.differential_photometry import vsx_mags\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "294fa9a6-5522-414b-ad96-73da98cb3eea",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import functools\n",
-                "import re\n",
-                "from pathlib import Path\n",
-                "import requests\n",
+                "folder_with_files = '.'\n",
                 "\n",
-                "import numpy as np\n",
+                "your_photometry_file = 'some_name.csv'\n",
+                "comp_stars_file = 'apass-V0533-Her.csv'\n",
+                "name_of_variable = 'v0533 her'\n",
                 "\n",
-                "from astropy import units as u\n",
-                "from astropy.table import Table\n",
-                "from astropy.coordinates import SkyCoord\n",
+                "# Enter the check star label (2 or 3 digit number) below \n",
+                "check_star_label = '153'\n",
                 "\n",
-                "from stellarphot.visualization.comparison_functions import (\n",
-                "    read_file, set_up, match, mag_scale, in_field, wrap, make_markers,\n",
-                "    viewer\n",
-                ")\n",
-                "from stellarphot.visualization.seeing_profile_functions import set_keybindings"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Change the settings in this cell as needed"
+                "# Our filter names vs filter names in comparison star table\n",
+                "filter_mapping = dict(\n",
+                "    ip='SI',\n",
+                "    B='B'\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "ef5cce53-08f1-4de5-9814-23be33285f5b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "directory_with_images = '..'\n",
-                "\n",
-                "# \ud83d\udc49 This could be any image from roughly the middle of the sequence.\n",
-                "sample_image_for_finding_stars = 'TIC_237205154.01-S001-R013-C001-rp.fit'\n",
-                "\n",
-                "# \ud83d\udc49 You will be able to use this name later to pull out the data you want\n",
-                "object_of_interest = 'TIC_237205154.01'\n",
-                "\n",
-                "# \ud83d\udc49 Get these variable from ExoFOP-TESS or Exoplanet ETD\n",
-                " \n",
-                "ra_object = '19:34:19.97'\n",
-                "dec_object = '76:39:39.91'\n",
-                "\n",
-                "Cmag = 13.0024 # \ud83d\udc49 Use TESS magnitude from ExoFOP-TESSfor this\n",
-                "depth = 16908.821 / 1000 # \ud83d\udc49 Depth should be in parts per thousand, ExoFOP gives it in ppm.\n",
-                "\n",
-                "bright_mag_limit = 9\n",
-                "dim_mag_limit = 16\n",
-                "\n",
-                "# \ud83d\udc49 File to save apertures in\n",
-                "aperture_output_file = 'aperture_locations.fits'\n",
-                "\n",
-                "TESS_target = True  # change to False (capitalized) if this is NOT a TESS object\n",
-                "\n",
-                "if TESS_target:\n",
-                "    server = \"https://www.astro.louisville.edu\"\n",
-                "    gaia_aperture_url = server + f\"/cgi-bin/gaia_to_aij/upload_request.cgi?ra={ra_object}&dec={dec_object}&mag={Cmag}&depth={depth}\"\n",
-                "\n",
-                "    result = requests.get(gaia_aperture_url)\n",
-                "    links = re.search('href=\"(.+)\"', result.text.replace('\\n', ''), )\n",
-                "\n",
-                "    target_file_contents = requests.get(server + links[1])\n",
-                "    with open('gaia_stars.radec', 'wt') as f:\n",
-                "        f.write(target_file_contents.text)\n",
-                "    targets_from_file = read_file('gaia_stars.radec')\n",
-                "else:\n",
-                "    targets_from_file = []"
+                "p = Path(folder_with_files)\n",
+                "your_photometry_file = p / your_photometry_file\n",
+                "comp_stars_file = p / comp_stars_file"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "110085f6-4c91-4e55-9ced-fb64936acf69",
             "metadata": {},
             "outputs": [],
             "source": [
-                "coordinate = SkyCoord(ra=ra_object, dec=dec_object, unit=(\"hour\", \"degree\"))"
+                "var_coord = SkyCoord.from_name(name_of_variable)\n",
+                "\n",
+                "vc = dict(coords=var_coord)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "7cd3031f-59ef-4b21-bad9-0075fc9b679a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ccd, vsx = \\\n",
-                "    set_up(sample_image_for_finding_stars,\n",
-                "           directory_with_images=directory_with_images\n",
-                "           )\n",
-                "\n",
-                "apass, vsx_apass_angle, targets_apass_angle = match(ccd, targets_from_file, vsx)\n",
+                "your_photometry = Table.read(your_photometry_file)\n",
+                "your_photometry['RA'].unit = 'degree'\n",
+                "your_photometry['Dec'].unit = 'degree'\n",
                 "\n",
-                "apass_good_coord, good_stars = mag_scale(Cmag, apass, vsx_apass_angle,\n",
-                "                                         targets_apass_angle,\n",
-                "                                         brighter_dmag=Cmag - bright_mag_limit,\n",
-                "                                         dimmer_dmag=dim_mag_limit - Cmag)\n",
+                "your_photometry['band'] = your_photometry['filter']\n",
                 "\n",
-                "apass_comps = in_field(apass_good_coord, ccd, apass, good_stars)\n",
-                "\n",
-                "box, iw = viewer()\n",
-                "\n",
-                "make_markers(iw, ccd, targets_from_file, vsx, apass_comps,\n",
-                "             name_or_coord=coordinate)\n",
-                "\n",
-                "box"
+                "comp_stars = Table.read(comp_stars_file)\n",
+                "comp_stars['RAJ2000'].unit = 'degree'\n",
+                "comp_stars['DEJ2000'].unit = 'degree'\n",
+                "\n"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "cdab5216-9a6a-4db4-8508-f5e0b5dd0ece",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Get the table of marked stars."
+                "comp_stars_check_only = comp_stars[comp_stars['label'] == int(check_star_label)]\n",
+                "check_star_auid = comp_stars_check_only['auid'][0]\n",
+                "check_star_auid"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "aa43ad37-6ef2-4d29-b1cd-2b1652ac8ec9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "all_table = iw.get_markers(marker_name='all')\n",
-                "elims = np.array([name.startswith('elim')\n",
-                "                 for name in all_table['marker name']])\n",
-                "elim_table = all_table[elims]\n",
-                "comp_table = all_table[~elims]"
+                "comp_stars_no_check = comp_stars[comp_stars['auid'] != check_star_auid]"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "23411fe8-7cd2-455d-ac74-058ec5df9c37",
             "metadata": {},
             "source": [
-                "### Remove any that are marked for elimination as comparisons."
+                "## The cell below does just one filter..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "77fd8792-f47b-41ef-a489-f82f05b4d68f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "index, d2d, d3d = elim_table['coord'].match_to_catalog_sky(comp_table['coord'])\n",
-                "comp_table.remove_rows(index)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Sort the table"
+                "this_filter = 'ip'\n",
+                "\n",
+                "this_phot = your_photometry[your_photometry['band'] == this_filter]\n",
+                "                                                                                                                                                                                                                                                                                                                                                                                              \n",
+                "this_phot_grp = this_phot.group_by('BJD')\n",
+                "\n",
+                "times = []\n",
+                "cal_mag = []\n",
+                "cal_mag_err = []\n",
+                "for time, rows in zip(this_phot_grp.groups.keys, this_phot_grp.groups):\n",
+                "    mag, err = vsx_mags.calc_vmag(vc, rows, comp_stars_no_check, band=filter_mapping[this_filter], star_data_mag_column=f'mag_inst')\n",
+                "    cal_mag.append(mag)\n",
+                "    cal_mag_err.append(err)\n",
+                "    times.append(time[0])\n",
+                "    "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "cc814ba5-d71d-46ce-924c-3f0889b27729",
             "metadata": {},
             "outputs": [],
             "source": [
-                "if targets_from_file:\n",
-                "    target_coord = targets_from_file['coords'][0]\n",
-                "else:\n",
-                "    target_coord = SkyCoord(ra=ra_object, dec=dec_object, unit=(\"hour\", \"degree\"))\n",
-                "\n",
-                "# Calculate how far each is from target\n",
-                "comp_table['separation'] = target_coord.separation(comp_table['coord'])\n",
-                "\n",
-                "# Add dummy column for sorting in the order we want\n",
-                "comp_table['sort'] = np.zeros(len(comp_table))\n",
+                "from astropy.timeseries import TimeSeries\n",
+                "from astropy import units as u\n",
+                "from astropy.time import Time\n",
+                "import numpy as np\n",
                 "\n",
-                "# Set sort order\n",
-                "apass_mark = comp_table['marker name'] == 'APASS comparison'\n",
-                "vsx_mark = comp_table['marker name'] == 'VSX'\n",
-                "tess_mark = ((comp_table['marker name'] == 'TESS Targets') | \n",
-                "        (comp_table['separation'] < 0.3 * u.arcsec))\n",
+                "good_time = Time(times,scale = 'tdb', format= 'jd')\n",
                 "\n",
+                "series = TimeSeries(time=good_time, data=[cal_mag, cal_mag_err], names=['mag', 'err'])\n",
                 "\n",
-                "comp_table['sort'][apass_mark] = 2\n",
-                "comp_table['sort'][vsx_mark] = 1\n",
-                "comp_table['sort'][tess_mark] = 0\n",
+                "day = [np.floor(bjd.value) for bjd in series.time]\n",
+                "series['day'] = day\n",
                 "\n",
-                "# Ensure the target is always first\n",
+                "#series_grouped = series.group_by('day')\n",
                 "\n",
+                "table = Table(data=[times, cal_mag, cal_mag_err], names=['time', 'mag', 'err'])\n",
+                "table['day']  = day\n",
                 "\n",
-                "# Sort the table\n",
-                "comp_table.sort(['sort', 'separation'])\n",
+                "table = table.group_by('day')\n",
                 "\n",
-                "# Assign the IDs\n",
-                "comp_table['id'] = range(1, len(comp_table) + 1)"
+                "table_grouped = table\n",
+                "series_folded = series.fold(period=3.5*u.hour, epoch_time ='1963-01-30T00:00:00')\n"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "c2564919-46e9-4ce9-b6ec-a4dbf04a1a41",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Display information on variables"
+                "for group in table_grouped.groups: \n",
+                "    time0 = group['time'][0]\n",
+                "    plt.plot(label = group['day'])\n",
+                "    plt.errorbar(group['time']-time0,group['mag'], yerr=group['err'], fmt = 's', label = f'{time0:.2f}')\n",
+                "plt.grid()\n",
+                "plt.ylabel('Magnitude')\n",
+                "plt.xlabel('Time since begining of observation (Days)')\n",
+                "plt.legend()\n",
+                "plt.ylim(*plt.ylim()[::-1])\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "3498a8bc-c6d3-4cc5-be08-bdb3e1ccd3c1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "new_vsx_mark = comp_table['marker name'] == 'VSX'\n",
-                "vsx_dict = {}\n",
-                "idx, _, _ = comp_table['coord'][new_vsx_mark].match_to_catalog_sky(vsx['coords'])\n",
-                "for our_name, vsx_name in zip(comp_table['id'][new_vsx_mark], vsx['Name'][idx]):\n",
-                "    print(f'Our id number: {our_name}, VSX name: {vsx_name}')\n",
-                "    vsx_dict[f'V{our_name}'] = vsx_name"
+                "check = comp_stars[comp_stars['auid'] == check_star_auid]\n",
+                "check_coord = SkyCoord(ra=check['RAJ2000'][0], dec=check['DEJ2000'][0], unit='degree')"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "255bdf25-44c4-43f4-85c3-36d2c8a787e0",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Label the stars with numbers"
+                "your_coords = SkyCoord(ra=your_photometry['RA'], dec=your_photometry['Dec'])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "560ab802-170e-4ed2-9fb2-b7ca970fe6a9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_names = []\n",
-                "for star in comp_table:\n",
-                "    star_id = star['id']\n",
-                "    if star['marker name'] == 'TESS Targets':\n",
-                "        label = f'T{star_id}'\n",
-                "        iw._marker = functools.partial(iw.dc.Text, text=label, fontsize=20, fontscale=False, color='green')\n",
-                "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
-                "\n",
-                "    elif star['marker name'] == 'APASS comparison':\n",
-                "        label = f'C{star_id}'\n",
-                "        iw._marker = functools.partial(iw.dc.Text, text=label, fontsize=20, fontscale=False, color='red')\n",
-                "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
-                "\n",
-                "    elif star['marker name'] == 'VSX':\n",
-                "        label = f'V{star_id}'\n",
-                "        iw._marker = functools.partial(iw.dc.Text, text=label, fontsize=20, fontscale=False, color='blue')\n",
-                "        iw.add_markers(Table(data=[[star['x']+20], [star['y']-20]], names=['x', 'y']))\n",
-                "    else:\n",
-                "        label = f'U{star_id}'\n",
-                "        print(f\"Unrecognized marker name: {star['marker name']}\")\n",
-                "    plot_names.append(label)"
+                "check_coord.match_to_catalog_sky(your_coords)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "61f51fb1-14dd-4d77-ae25-e7bf62e591f9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "comp_table['plot_label'] = [plot_names]"
+                "your_photometry[28141]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "65d3dab3-c4bd-4206-8773-2dfa274df0be",
             "metadata": {},
             "outputs": [],
             "source": [
-                "comp_table.write(aperture_output_file, overwrite=True)"
+                "kc = dict(coords=check_coord)\n",
+                "this_filter = 'ip'\n",
+                "\n",
+                "this_phot = your_photometry[your_photometry['band'] == this_filter]\n",
+                "                                                                                                                                                                                                                                                                                                                                                                                              \n",
+                "this_phot_grp = this_phot.group_by('BJD')\n",
+                "\n",
+                "times = []\n",
+                "cal_mag_k = []\n",
+                "cal_mag_err_k = []\n",
+                "for time, rows in zip(this_phot_grp.groups.keys, this_phot_grp.groups):\n",
+                "    mag, err = vsx_mags.calc_vmag(kc, rows, comp_stars_no_check, band=filter_mapping[this_filter], star_data_mag_column=f'mag_inst')\n",
+                "    cal_mag_k.append(mag)\n",
+                "    cal_mag_err_k.append(err)\n",
+                "    times.append(time[0])\n",
+                "    "
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "811274f8-5138-4d51-9b47-217f7f40b956",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Add 2.5 arcmin circle (do this after writing comparison table!)\n",
+                "table_k = Table(data=[times, cal_mag_k, cal_mag_err_k], names=['time', 'mag', 'err'])\n",
+                "table_k['day']  = day\n",
+                "\n",
+                "table_k = table_k.group_by('day')\n",
                 "\n",
-                "Otherwise the comparison table will contain an extra entry for this circle."
+                "table_grouped_k = table_k"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "ec9f67a5-b11b-4509-a135-5bafc4f152a4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "if targets_from_file:\n",
-                "    target = targets_from_file[0]\n",
-                "    iw.marker = {'color': 'yellow', 'radius': 268, 'type': 'circle'}\n",
-                "    iw.add_markers(target, skycoord_colname='coords',\n",
-                "                   use_skycoord=True, marker_name='target')"
+                "for group in table_grouped_k.groups: \n",
+                "    time0 = group['time'][0]\n",
+                "    plt.plot(label = group['day'])\n",
+                "    plt.errorbar(group['time']-time0,group['mag'], yerr=group['err'], fmt = 's', label = f'{time0:.2f}')\n",
+                "plt.grid()\n",
+                "plt.ylabel('Magnitude')\n",
+                "plt.xlabel('Time since begining of observation (Days)')\n",
+                "plt.title('Check star')\n",
+                "plt.legend()\n",
+                "plt.ylim(15.2, 14.7)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "8c0be3a2-30c2-47c7-a8a5-d7d9c922e2b7",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -336,9 +311,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.6"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9347916666666667%*

 * *Differences: {"'cells'": "{1: {'source': ['### Choose photometry and aperture files']}, 3: {'source': ['box = "*

 * *            "ipw.VBox()\\n', 'box.children = [fo.file_chooser, fo2.file_chooser]\\n', 'box']}, 4: "*

 * *            "{'source': ['### Run the remaining cells']}, 5: {'source': {insert: [(0, "*

 * *            "'aperture_file = fo2.path\\n'), (1, 'photometry_file = fo.path\\n'), (3, 'output_file "*

 * *            '= photometry_file.stem + "-relative-flux" + photometry_file.suffix\')], delete: [8, '*

 * *            "7, 5, 4, 3,  […]*

```diff
@@ -1,91 +1,157 @@
 {
     "cells": [
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from astropy.coordinates import SkyCoord\n",
+                "import astropy.units as u\n",
+                "from astropy.table import Table\n",
+                "from astropy.time import Time\n",
+                "\n",
+                "import ipywidgets as ipw\n",
+                "\n",
+                "import matplotlib.pyplot as plt\n",
+                "\n",
+                "import numpy as np\n",
+                "\n",
+                "from stellarphot.differential_photometry.aij_rel_fluxes import *\n",
+                "from stellarphot.visualization.fits_opener import FitsOpener"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Comparison star generator"
+                "### Choose photometry and aperture files"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import re\n",
-                "\n",
-                "import requests\n",
-                "\n",
-                "from astropy.coordinates import SkyCoord\n",
-                "\n",
-                "from stellarphot.visualization.comparison_functions import ComparisonViewer\n"
+                "fo = FitsOpener(title=\"Select your photometry file\", filter_pattern=[\"*.csv\"])\n",
+                "fo2 = FitsOpener(title=\"Select your aperture file\", filter_pattern=[\"*.csv\", \"*.fits\"])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "box = ipw.VBox()\n",
+                "box.children = [fo.file_chooser, fo2.file_chooser]\n",
+                "box"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Change the settings in this cell as needed"
+                "### Run the remaining cells"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bright_mag_limit = 9\n",
-                "dim_mag_limit = 16\n",
-                "Cmag = 10\n",
+                "aperture_file = fo2.path\n",
+                "photometry_file = fo.path\n",
                 "\n",
-                "# \ud83d\udc49 File to save apertures in\n",
-                "aperture_output_file = 'aperture_locations.csv'\n",
-                "\n",
-                "# \ud83d\udc49 File to exoplanet info in\n",
-                "tess_info_output_file = 'tess-info.pickle'"
+                "output_file = photometry_file.stem + \"-relative-flux\" + photometry_file.suffix"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "comp_viewer = ComparisonViewer(\n",
-                "                           target_mag=Cmag,\n",
-                "                           bright_mag_limit=bright_mag_limit,\n",
-                "                           dim_mag_limit=dim_mag_limit,\n",
-                "                           targets_from_file=None,\n",
-                "                           aperture_output_file=aperture_output_file,\n",
-                "                          )\n",
-                "comp_viewer.box"
+                "photometry = Table.read(photometry_file)\n",
+                "del_rows = photometry['file'] == 'image_file.fits'\n",
+                "photometry = photometry[~del_rows]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pickle\n",
-                "\n",
-                "with open(tess_info_output_file, 'wb') as f:\n",
-                "    pickle.dump(comp_viewer.toi_info, f)\n",
-                "    "
+                "comp_table = Table.read(aperture_file)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "comp_table['coord'] = SkyCoord(ra=[c.split(',')[0] for c in comp_table['coord']],\n",
+                "                            dec=[c.split(',')[1] for c in comp_table['coord']],\n",
+                "                            unit='degree',\n",
+                "                            frame='icrs')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "comp_bool = comp_table['marker name'] == ['APASS comparison']\n",
+                "only_comp_stars = comp_table[comp_bool]\n",
+                "coords = only_comp_stars['coord']"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ra = [i.ra for i in coords]\n",
+                "dec = [i.dec for i in coords]\n",
+                "comp_coords = Table()\n",
+                "comp_coords['RA'] = ra * u.degree\n",
+                "comp_coords['Dec'] = dec * u.degree"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Calculate flux"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# calculate flux\n",
+                "flux_table = calc_aij_relative_flux(photometry, comp_coords)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "comp_viewer.toi_info.tic_id"
+                "flux_table.write(output_file, overwrite=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/photometry/03-photometry-template.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9676201063429324%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, 'import json\\n'), (2, 'import pickle\\n'), (4, 'import "*

 * *            "numpy as np \\n'), (6, 'from astropy.table import Table \\n'), (8, '#from "*

 * *            'try_json_editing_rev1 import whole_thing, generate_json_file_name, exotic_arguments, '*

 * *            "get_values_from_widget\\n'), (9, 'from stellarphot.analysis.exotic import "*

 * *            'generate_json_file_name, exotic_arguments, get_values_from_widget, '*

 * *            "exotic_settings_widget, populate_TOI_bo […]*

```diff
@@ -2,155 +2,153 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import json\n",
                 "from pathlib import Path\n",
+                "import pickle\n",
                 "\n",
-                "import numpy as np\n",
+                "import numpy as np \n",
                 "\n",
-                "from ipyfilechooser import FileChooser\n",
+                "from astropy.table import Table \n",
                 "\n",
-                "from astropy.nddata import CCDData\n",
-                "from astropy.coordinates import SkyCoord, EarthLocation\n",
-                "from astropy.table import Table\n",
-                "from astropy.time import Time\n",
-                "\n",
-                "from stellarphot.photometry import *\n",
-                "from stellarphot.source_detection import *\n",
-                "from stellarphot import Camera\n",
-                "\n",
-                "from stellarphot.visualization.photometry_widget_functions import PhotometrySettings"
+                "#from try_json_editing_rev1 import whole_thing, generate_json_file_name, exotic_arguments, get_values_from_widget\n",
+                "from stellarphot.analysis.exotic import generate_json_file_name, exotic_arguments, get_values_from_widget, exotic_settings_widget, populate_TOI_boxes\n",
+                "from stellarphot.visualization.fits_opener import FitsOpener"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Settings are below "
+                "# Instructions and Overview\n",
+                "\n",
+                "This notebook will do a different kind of fit to your exoplanet data. It takes longer to run than the fitting we've done so far, which is why we didn't begin with this type of fit."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ps = PhotometrySettings()\n",
-                "ps.box"
+                "fo = FitsOpener(title=\"Select your photometry/relative flux file\", filter_pattern=[\"*.csv\"])\n",
+                "\n",
+                "fo.file_chooser"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# A single dot means \"the folder this notebook is in\"\n",
-                "folder_with_images = ps.image_folder # '.'\n",
+                "input_data_file = fo.path\n",
+                "toi_info_file = \"tess-info.pickle\"\n",
                 "\n",
-                "# The file name below should be the one you made with the comp-star template\n",
-                "# Its name should end .fits\n",
-                "source_file_name = ps.aperture_locations # 'aperture_locations.fits'\n",
-                "\n",
-                "# Enter the aperture radius from the viewer seeing template here\n",
-                "aperture = ps.aperture_radius\n",
+                "with open(toi_info_file, 'rb') as f:\n",
+                "    tess_info = pickle.load(f)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "settings = exotic_settings_widget()\n",
                 "\n",
-                "# Enter the object name here\n",
-                "object_name = ps.object_name\n",
+                "exotic_data_file = 'data_for_exotic.csv'"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "inp_data = Table.read(input_data_file)\n",
+                "inp_data = inp_data[inp_data['star_id'] == 1]\n",
                 "\n",
-                "# Enter date data was taken here\n",
-                "date = '2021-09-28'\n",
+                "# inp_data = inp_data[inp_data['BJD'] > 2459795.75]\n",
                 "\n",
-                "# Enter the name you want to give the photometry file, i.e. the file with star counts, here\n",
-                "photometry_file = f'{object_name}-{date}.csv'"
+                "out_data = inp_data['BJD', 'relative_flux', 'relative_flux_error', 'airmass']\n",
+                "out_data.write(exotic_data_file, overwrite=True)"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### More settings (no need to change these typically)"
+                "settings.data_file_widget['candidate'].value = exotic_data_file\n",
+                "settings.data_file_widget['known'].value = exotic_data_file\n",
+                "populate_TOI_boxes(tess_info, settings.value_widget)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "inner_annulus = aperture + 15\n",
-                "outer_annulus = inner_annulus + 15\n",
-                "\n",
-                "feder_cg_16m = Camera(gain=1.5, read_noise=10.0, dark_current=0.01)\n",
-                "\n",
-                "max_adu = 50000"
+                "settings"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "image_directory = Path(folder_with_images)"
+                "settings_name = generate_json_file_name(settings)\n",
+                "contents = get_values_from_widget(settings)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sources = Table.read(source_file_name)"
+                "Path(contents['user_info']['Directory to Save Plots']).mkdir(exist_ok=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sources['coord'] = SkyCoord(ra=[c.split(',')[0] for c in sources['coord']],\n",
-                "                            dec=[c.split(',')[1] for c in sources['coord']],\n",
-                "                            unit='degree',\n",
-                "                            frame='icrs')\n",
-                "star_ra = sources['coord'].ra\n",
-                "star_dec = sources['coord'].dec\n",
-                "\n",
-                "main_target_coords = sources[sources['star_id'] == 1]['coord']"
+                "with open(settings_name, 'w') as f:\n",
+                "    json.dump(contents, f)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "photometry_table = photometry_on_directory(\n",
-                "                        image_directory, object_name, \n",
-                "                        (star_ra, star_dec), \n",
-                "                        aperture, inner_annulus, outer_annulus, \n",
-                "                        max_adu, sources['star_id'], \n",
-                "                        feder_cg_16m,\n",
-                "                        observatory_location='feder',\n",
-                "                        bjd_coords=main_target_coords,\n",
-                "                        fwhm_by_fit=False                \n",
-                "                    )"
+                "print('COPY AND PASTE THE LINE BELOW INTO AN EMPTY CELL TO RUN EXOTIC (include the exclamation point at the beginning):\\n\\n')\n",
+                "print(f'!exotic {\" \".join(exotic_arguments[whole_thing.planet_type.value])} {settings_name}')\n",
+                "print(\"\\n\\n\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "photometry_table.write(photometry_file)"
+                "!exotic --override --pre TIC_402828941-2022-08-03-SI.json"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/photometry/06-transit-fit-template.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/06-transit-fit-template.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'cells'": "{14: {'source': {insert: [(0, 'cycle_number = int((then - epoch) / period + 1)\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -203,15 +203,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "cycle_number = np.int((then - epoch) / period + 1)\n",
+                "cycle_number = int((then - epoch) / period + 1)\n",
                 "that_transit = cycle_number * period + epoch\n",
                 "that_transit"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/photometry/Untitled.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/notebooks/photometry/transform-pared-back.ipynb` & `stellarphot-1.3.9/stellarphot/notebooks/photometry/transform-pared-back.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/photometry.py` & `stellarphot-1.3.9/stellarphot/photometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 from astropy.time import Time
 
 from ccdproc import ImageFileCollection
 
 from astropy.stats import sigma_clipped_stats
 from astropy.nddata import NoOverlapError
 
-from .coordinates import convert_pixel_wcs
 from .source_detection import compute_fwhm
 
 __all__ = ['photutils_stellar_photometry',
            'faster_sigma_clip_stats',
            'find_too_close', 'clipped_sky_per_pix_stats',
-           'add_to_photometry_table', 'photometry_on_directory']
+           'add_to_photometry_table', 'photometry_on_directory',
+           'calculate_noise', 'find_times']
 
 
 def photutils_stellar_photometry(ccd_image, sources,
                                  aperture_radius, inner_annulus,
                                  outer_annulus, gain=1.0, N_R=0, N_dark_pp=0,
                                  reject_background_outliers=True):
     """
     Perform aperture photometry on an image, with a few options for estimating
     the local background from an annulus around the aperture.
 
     Parameters
     ----------
-    ccd_image : `~ccdproc.CCDData`
+    ccd_image : `ccdproc.CCDData`
         Image on which to perform aperture photometry.
 
-    sources : `~astropy.table.Table`
+    sources : `astropy.table.Table`
         Table of extracted sources. Assumed to be the output of
-        `~photutils.daofind()` source extraction function.
+        `photutils.daofind()` source extraction function.
 
     aperture_radius : float
         Radius of aperture(s) in pixels.
 
     inner_annulus : float
         Inner radius of the annulus in pixels.
 
@@ -60,15 +60,15 @@
 
     reject_background_outliers : bool, optional
         If ``True``, sigma clip the pixels in the annulus to reject outlying
         pixels (e.g. like stars in the annulus)
 
     Returns
     -------
-    phot_table : `~astropy.table.Table`
+    phot_table : `astropy.table.Table`
         Astropy table with columns for flux, x/y coordinates of center,
         RA/dec coordinates of center, sky background per pixel,
         net flux, aperture and annulus radii used, and flux error.
     """
 
     # check that the outer radius is greater or equal the inner radius
     # for annulus
@@ -118,15 +118,15 @@
     phot_table['inner_radius'] = \
         np.ones(len(phot_table['aperture_sum'])) * inner_annulus
     phot_table['outer_radius'] = \
         np.ones(len(phot_table['aperture_sum'])) * outer_annulus
 
     # Obtain RA/Dec coordinates and add them to table
     try:
-        ra, dec = convert_pixel_wcs(ccd_image, coords[0], coords[1], 1)
+        ra, dec = ccd_image.wcs.all_pix2world(coords[0], coords[1], 0)
         phot_table['RA_center'] = ra
         phot_table['Dec_center'] = dec
     except AttributeError:
         pass
 
     # Obtain flux error and add column to return table
     noise = np.sqrt(gain * net_flux + n_pix_ap * (1 + (n_pix_ap / n_pix_ann)) *
@@ -222,24 +222,31 @@
 
     Parameters
     ----------
 
     data : `astropy.nddata.CCDData`
         CCD image on which the annuli are defined.
 
-    annulus : photutils annulus
+    annulus : `photutils.CircularAnnulus`
         One or more annulus (of any shape) from photutils.
 
     sigma : float, optional
         Number of standard deviations from the central value a
         pixel must be to reject it.
 
     iters : int, optional
         Maximum number of sigma clip iterations to perform. Iterations stop
         automatically if no pixels are rejected.
+
+    Returns
+    -------
+
+    avg_sky_per_pix, med_sky_per_pix, std_sky_per_pix : `astropy.units.Quantity`
+        Average, median and standard deviation of the sky per pixel.
+
     """
     # Get a list of masks from the annuli
     # Use the 'center' method because then pixels are either in or out. To use
     # 'partial' or 'exact' we would need to do a weighted sigma clip and
     # I'm not sure how to do that.
     masks = annulus.to_mask(method='center')
 
@@ -269,36 +276,56 @@
                             fwhm_by_fit=True):
     """
     Calculate several columns for photometry table.
 
     Parameters
     ----------
 
-    phot : astropy.table.Table
+    phot : `astropy.table.Table`
         An astropy Table with raw photometry data in it (generated by
         `photutils.aperture_photometry`).
 
-    ccd : astropy.nddata.CCDData
+    ccd : `astropy.nddata.CCDData`
         Image on which photometry is being done.
 
-    annulus : photutils annulus
+    annulus : `photutils.CircularAnnulus`
         One or more annulus (of any shape) from photutils.
 
-    apertures : photutils apertures
+    apertures : `photutils.CircularAperture`
         One or more apertures (of any shape) from photutils.
 
     fname : str, optional
         Name of the image file on which photometry is being performed.
 
     star_ids : str or int, optional
         ID for each of the sources.
 
     gain : float, optional
         Gain, in electrons/ADU, of the camera that took the image. The gain
         is used in calculating the instrumental magnitude.
+
+    bjd_coords : `astropy.coordinates.SkyCoord`
+        Coordinates of the object of interest in the Barycentric Julian Date
+        frame. If not provided, the BJD column will not be added to the
+        photometry table.
+
+    observatory_location : str
+        Name of the observatory where the images were taken. If not provided,
+        the BJD column will not be added to the photometry table.
+
+    fwhm_by_fit : bool, optional
+        If ``True``, the FWHM will be calculated by fitting a Gaussian to
+        the star. If ``False``, the FWHM will be calculated by finding the
+        second moments of the light distribution. Default is ``True``.
+
+    Returns
+    -------
+
+    None
+        The input table is modified in place.
     """
     phot.rename_column('aperture_sum_0', 'aperture_sum')
     phot['aperture_sum'].unit = u.adu
     phot.rename_column('aperture_sum_1', 'annulus_sum')
     star_locs = ccd.wcs.all_pix2world(phot['xcenter'], phot['ycenter'], 0)
     star_coords = SkyCoord(ra=star_locs[0], dec=star_locs[1],
                            frame='icrs', unit='degree')
@@ -335,15 +362,15 @@
     phot['annulus_inner'] = annulus.r_in * u.pixel
     phot['annulus_outer'] = annulus.r_out * u.pixel
     phot['annulus_area'] = annulus.area  # * u.pixel * u.pixel
     phot['exposure'] = [ccd.header['exposure']] * len(phot) * u.second
     phot['date-obs'] = [ccd.header['DATE-OBS']] * len(phot)
     night = Time(ccd.header['DATE-OBS'], scale='utc')
     night.format = 'mjd'
-    phot['night'] = np.int(np.floor(night.value - 0.5))
+    phot['night'] = int(np.floor(night.value - 0.5))
     phot['aperture_net_flux'] = (phot['aperture_sum'] -
                                  (phot['aperture_area'] *
                                   phot['sky_per_pix_avg']))
 
     # This can happen, for example, when the object is faint
     # and centroiding is bad.
     bad_flux = phot['aperture_net_flux'] < 0
@@ -411,28 +438,49 @@
     max_adu : int
         Maximum allowed pixel value before a source is considered
         saturated.
 
     star_ids : array-like
         Unique identifier for each source in ``star_locs``.
 
-    camera : `stellarphot.Camera` object
+    camera : `~stellarphot.Camera`
         Camera object which has gain, read noise and dark current set.
 
     gain : float
         Gain, in electrons/ADU, of the camera that took the image. The gain
         is used in calculating the instrumental magnitude.
 
     read_noise : float
         Read noise of the camera in electrons. Used in the CCD equation
         to calculate error.
 
     dark_current : float
         Dark current, in electron/sec. Used in the CCD equation
         to calculate error.
+
+    bjd_coords : `astropy.coordinates.SkyCoord`
+        Coordinates of the object of interest in the Barycentric Julian Date
+        frame. If not provided, the BJD column will not be added to the
+        photometry table.
+
+    observatory_location : str
+        Name of the observatory where the images were taken. If not provided,
+        the BJD column will not be added to the photometry table.
+
+    fwhm_by_fit : bool, optional
+        If ``True``, the FWHM will be calculated by fitting a Gaussian to
+        the star. If ``False``, the FWHM will be calculated by finding the
+        second order moments of the light distribution. Default is ``True``.
+
+    Returns
+    -------
+
+    phot : `astropy.table.Table`
+        Table containing the photometry results.
+
     """
     ifc = ImageFileCollection(directory_with_images)
     phots = []
     missing_stars = []
     for a_ccd, fname in ifc.ccds(object=object_of_interest, return_fname=True):
         print('on image ', fname)
         try:
@@ -554,14 +602,67 @@
 
 
 def calculate_noise(gain=1.0, read_noise=0.0, dark_current_per_sec=0.0,
                     flux=0.0, sky_per_pix=0.0,
                     aperture_area=0, annulus_area=0,
                     exposure=0,
                     include_digitization=False):
+    """
+    Computes the noise in a photometric measurement.
+
+    This function computes the noise (in units of gain) in a photometric measurement using the
+    revised CCD equation from Collins et al (2017) AJ, 153, 77.  The equation is:
+
+    .. math::
+
+        \\sigma = \\sqrt{G \\cdot F + A \\cdot \\left(1 + \\frac{A}{B}\\right)\\cdot \\left[ G\\cdot S + D \\cdot t + R^2 + (0.289 G)^2\\right]}
+
+    where :math:`\sigma` is the noise, :math:`G` is the gain, :math:`F` is the flux,
+    :math:`A` is the aperture area in pixels, :math:`B` is the annulus area in pixels,
+    :math:`S` is the sky per pixel, :math:`D` is the dark current per second,
+    :math:`R` is the read noise, and :math:`t` is exposure time.
+
+    Note: The :math:`(0.289 G)^2` term is "digitization noise" and is optional.
+
+    Parameters
+    ----------
+
+    gain : float, optional
+        Gain of the CCD. In units of electrons per DN.
+
+    read_noise : float, optional
+        Read noise of the CCD in electrons.
+
+    dark_current_per_sec : float, optional
+        Dark current of the CCD in electrons per second.
+
+    flux : float, optional
+        Flux of the source in electrons.
+
+    sky_per_pix : float, optional
+        Sky per pixel in electrons.
+
+    aperture_area : int, optional
+        Area of the aperture in pixels.
+
+    annulus_area : int, optional
+        Area of the annulus in pixels.
+
+    exposure : int, optional
+        Exposure time in seconds.
+
+    include_digitization : bool, optional
+        Whether to include the digitization noise. Defaults to False.
+
+    Returns
+    -------
+
+    noise : float
+        The noise in the photometric measurement.
+    """
 
     try:
         no_annulus = (annulus_area == 0).all()
     except AttributeError:
         no_annulus = annulus_area == 0
 
     if no_annulus:
@@ -585,101 +686,54 @@
 
     if include_digitization:
         digitization = area_ratio * (gain * 0.289) ** 2
 
     return np.sqrt(poisson_source + sky + dark + rn_error + digitization)
 
 
-def find_times(phot_column, exposure,
-               ra=331.1170417, dec=81.5659444,
+def find_times(phot_column, exposure, ra, dec,
                latitude=46.86678, longitude=263.54672):
     """
-    Returns a numpy array of barycentric julien date times
+    Returns a numpy array of barycentric Julian date times
 
     Parameters
     ----------
 
-    phot_column : astropy Table column or numpy array
+    phot_column : `astropy.table.Column` or numpy array
         numpy array or column of observation dates from the photometry table
 
-    exposure : float; optional
+    exposure : float, optional
         exposure time in seconds
 
-    RA : float; optional
-        Right ascension in degree format, default is for TIC-470127886
+    RA : float
+        Right ascension in degree units
 
-    Dec : float; optional
-        Declination  in degree format, default is for TIC-470127886
+    Dec : float
+        Declination  in degree units
 
-    latitude : float; optional
-        latitude of the observatory, default is for Paul P. Feder Observatory
+    latitude : float, optional
+        latitude of the observatory in degrees North, default is for Paul P. Feder Observatory
 
-    longitude : float; optional
-        longitude of the observatory, default is for Paul P. Feder Observatory
+    longitude : float, optional
+        longitude of the observatory in degree East of Greenwich (0 to 360), default
+        is for Paul P. Feder Observatory
 
 
     Returns
     -------
 
-    new_time : numpy array
-        array of barycentric times by julien date
+    numpy array
+        array of times in barycentric Julian date
 
     """
     location = EarthLocation(lat=latitude, lon=longitude)
 
     times = Time(phot_column, scale='utc', format='isot', location=location)
     ip_peg = SkyCoord(ra=ra, dec=dec, unit='degree')
     ltt_bary = times.light_travel_time(ip_peg)
     times_tdb = times.tdb
     time_barycenter = times_tdb + ltt_bary
 
-    #adjust to midpoint of exposure
+    # Adjust to midpoint of exposure
     bary_time = time_barycenter + exposure / 2
 
-    new_time = bary_time.jd
-
-    return new_time
-
-
-# ra=331.1170417, dec=81.5659444, latitude=46.86678, longitude=263.54672
-def find_bjd_mid_exposure(utc_times, exposure=0,
-                          coords=None, location=None):
-    """
-    Returns a numpy array of barycentric Julian date times
-
-    Parameters
-    ----------
-
-    phot_column : `astropy.table.Column` of `astropy.times.Time`  or numpy array
-        numpy array or column of observation dates/times.
-
-    exposure : float; optional
-        exposure time in seconds
-
-    coords : `astropy.coordinates.SkyCoord`
-        Ra/Dec of the object to be used for the light travel time
-        calculation.
-
-    location: `astropy.coordinates.EarthLocation`
-        Location of the observatory.
-
-    Returns
-    -------
-
-    new_time : numpy array
-        array of barycentric times by Julian date
-
-    """
-    location = EarthLocation(lat=latitude, lon=longitude)
-    ip_peg = SkyCoord(ra=[ra], dec=[dec], unit='degree')
-
-    if coords is None or observatory_location is None:
-        raise ValueError
-    times = Time(phot_column, scale='utc', format='isot', location=location)
-    ltt_bary = times.light_travel_time(coords)
-    times_tdb = times.tdb
-    time_barycenter = times_tdb + ltt_bary
-
-    # adjust to midpoint of exposure
-    bary_time = time_barycenter + exposure * u.second / 2
-
-    return bary_time.jd
+    return bary_time.jd
```

### Comparing `stellarphot-1.3.8/stellarphot/source_detection.py` & `stellarphot-1.3.9/stellarphot/source_detection.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,23 +12,33 @@
 from astropy import units as u
 
 __all__ = ['source_detection', 'compute_fwhm']
 
 
 def _fit_2dgaussian(data):
     """
-    Fit a 2d Gaussian to data.
+    Fit a 2D Gaussian to data.
 
-    Written as a replace for functionality that was removed from
+    Written as a replacement for functionality that was removed from
     photutils.
 
-    Keep this private so we don't have to support it....
+    This function will be kept private so we don't have to support it.
 
     Copy/pasted from
     https://github.com/astropy/photutils/pull/1064/files#diff-9e64908ff7ac552845b4831870a749f397d73c681d218267bd9087c7757e6dd4R285
+
+    Parameters
+    ----------
+    data : array-like
+        The 2D array of data to fit.
+
+    Returns
+    -------
+    gfit : `astropy.modeling.Model`
+        The best-fit 2D Gaussian model.
     """
     props = data_properties(data - np.min(data))
 
     init_const = 0.  # subtracted data minimum above
     init_amplitude = np.ptp(data)
 
     g_init = (Const2D(init_const)
@@ -46,14 +56,53 @@
     return gfit
 
 
 def compute_fwhm(ccd, sources, fwhm_estimate=5,
                  x_column='xcenter', y_column='ycenter',
                  fit=True,
                  sky_per_pix_avg=0):
+    """
+    Computes the FWHM in both x and y directions of sources in an image.
+
+    Parameters
+    ----------
+
+    ccd : `astropy.nddata.CCDData`
+        The CCD Image array.
+
+    sources : `astropy.table.Table`
+        An astropy table of the positions of sources in the image.
+
+    fwhm_estimate : float, optional
+        The initial guess for the FWHM of the sources in the image.
+
+    x_column : str, optional
+        The name of the column in `sources` that contains the x positions
+        of the sources.
+
+    y_column : str, optional
+        The name of the column in `sources` that contains the y positions
+        of the sources.
+
+    fit : bool, optional
+        If ``True``, fit a 2D Gaussian to each source to estimate its FWHM. If
+        ``False``, estimate the FWHM of each source by computing the second
+        moments of its light distribution using photutils.
+
+    sky_per_pix_avg : float or array-like of float, optional
+        Sky background to subtract before centroiding.
+
+    Returns
+    -------
+
+    fwhm_x, fwhm_y : array-like of float
+        The FWHM of each source in the x and y directions.
+
+    """
+
     fwhm_x = []
     fwhm_y = []
     for source in sources:
         x = source[x_column]
         y = source[y_column]
         sky = sky_per_pix_avg
         # Cutout2D needs no units on the center position, so remove unit
@@ -96,17 +145,17 @@
                      threshold=10.0, find_fwhm=True,
                      sky_per_pix_avg=None):
     """
     Returns an astropy table containing the position of sources
     within the image.
 
     Parameters
-    ----------------
+    ----------
 
-    ccd : numpy.ndarray
+    ccd : `astropy.nddata.CCDData`
         The CCD Image array.
 
     fwhm : float, optional
         Full-width half-max of stars in the image.
 
     sigma : float, optional.
         The number of standard deviations to use as the lower and
@@ -116,25 +165,26 @@
         The number of iterations to perform sigma clipping
 
     threshold : float, optional.
         The absolute image value above which to select sources.
 
     find_fwhm : bool, optional
         If ``True``, estimate the FWHM of each source by fitting a 2D Gaussian
-        to it.
+        to it. If ``False``, estimate the FWHM of each source by computing
+        the second moments of its light distribution.
 
     sky_per_pix_avg : float or array-like of float
         Sky background to subtract before centroiding.
 
     Returns
-    -----------
+    -------
 
-    sources
-        an astropy table of the positions of sources in the image.
-        If `find_fwhm` is ``True``, includes a column called ``FWHM``.
+    sources: `astropy.table.Table`
+        A table of the positions of sources in the image.  If `find_fwhm` is
+        ``True``, includes a column called ``FWHM``.
     """
     mean, median, std = sigma_clipped_stats(ccd, sigma=sigma, maxiters=iters)
     daofind = DAOStarFinder(fwhm=fwhm, threshold=threshold * std)
     sources = daofind(ccd - median)
     print(sources)
     if find_fwhm:
         x, y = compute_fwhm(ccd, sources, fwhm_estimate=fwhm,
```

### Comparing `stellarphot-1.3.8/stellarphot/tests/test_detection.py` & `stellarphot-1.3.9/stellarphot/tests/test_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     inner_annulus = 2 * aperture
     outer_annulus = 3 * aperture
     # Add some large pixel values to the annulus for each source.
     # adding these moves the average pixel value by quite a bit,
     # so we'll only get the correct net flux if these are removed.
     for source in fake_image.sources:
-        center_px = (np.int(source['x_mean']), np.int(source['y_mean']))
+        center_px = (int(source['x_mean']), int(source['y_mean']))
         begin = center_px[0] + inner_annulus + 1
         end = begin + (outer_annulus - inner_annulus - 1)
         # Yes, x and y are deliberately reversed below.
         image[center_px[1], begin:end] = 100 * fake_image.mean_noise
 
     phot = photutils_stellar_photometry(image,
                                         found_sources, aperture,
```

### Comparing `stellarphot-1.3.8/stellarphot/tests/test_photometry.py` & `stellarphot-1.3.9/stellarphot/tests/test_photometry.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot/visualization/aij_plots.py` & `stellarphot-1.3.9/stellarphot/visualization/aij_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,21 +27,29 @@
         half width half max, 1/2 * FWHM
 
     plot_title : optional, string
         title of plot
 
     file_name : optional, string
         if entered, file will save as png with this name
+
     gap : number
         the distance between the aperture and the inner annulus
+
     annulus_width : number
         the distance between the inner and outer annulus
 
     figsize : tuple of int, optional
         Size of figure.
+
+    Returns
+    -------
+
+    `matplotlib.pyplot.figure`
+        The figure object containing the seeing plot.
     """
     if radius is None:
         radius = HWHM * 4
 
     fig = plt.figure(figsize=figsize)
     plt.grid(True)
     inner_annulus = radius + gap
@@ -91,33 +99,43 @@
 
     # save plot as png
     if file_name:
         safe_name = file_name.replace(" ", "-")
         plt.savefig(f"{safe_name + '-seeing-profile'}.png")
     return fig
 
+
 def plot_predict_ingress_egress(ingress_time, egress_time, end_line=1,
                                 ingress_x_pos=1, egress_x_pos=1, labels_y_pos=1):
     """
     Parameters
     ----------
-    ingress_time : number
+    ingress_time : float
         the beginning of an exoplanet transit
 
-    egress_time : number
+    egress_time : float
         the end of an exoplanet transit
 
-    ingress_x_pos : number
+    end_line : float
+        offset to move the vertical lines
+
+    ingress_x_pos : float
         offset to center ingress label
 
-    egress_x_pos : number
+    egress_x_pos : float
         offset to center egress label
 
-    labels_y_pos : number
+    labels_y_pos : float
         offset to move ingress and egress labels
+
+    Returns
+    -------
+
+    None
+        Directly adds lines and labels to the current plot.
     """
     ymin, ymax = plt.ylim()
 
     # create a vertical line at the ingress time and label it
     plt.vlines(ingress_time, ymin - end_line, ymax,
                linestyle=(0, (5, 10)), color='red')
     plt.annotate("Predicted Ingress", (ingress_time - ingress_x_pos,
```

### Comparing `stellarphot-1.3.8/stellarphot/visualization/comparison_functions.py` & `stellarphot-1.3.9/stellarphot/visualization/comparison_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from stellarphot.differential_photometry import *
 from stellarphot.io import TessSubmission, TOI, TessTargetFile
 from stellarphot.photometry import *
 from stellarphot.visualization.seeing_profile_functions import set_keybindings
 from stellarphot.visualization.fits_opener import FitsOpener
 
 
-__all__ = ['read_file', 'set_up', 'match', 'mag_scale',
-           'in_field', 'make_markers', 'wrap']
+__all__ = ['read_file', 'set_up', 'crossmatch_APASS2VSX', 'mag_scale',
+           'in_field', 'make_markers', 'wrap', 'ComparisonViewer']
 
 DESC_STYLE = {"description_width": "initial"}
 
 
 def read_file(radec_file):
     """
     Read an AIJ radec file with target and/or comp positions
@@ -54,28 +54,37 @@
     target_table = Table.from_pandas(df)
     ra = target_table['RA']
     dec = target_table['Dec']
     target_table['coords'] = SkyCoord(ra=ra, dec=dec, unit=(u.hour, u.degree))
     return target_table
 
 
-def set_up(sample_image_for_finding_stars,
-           directory_with_images='.'):
+def set_up(sample_image_for_finding_stars, directory_with_images='.'):
     """
-    Find known variable in the field of view and read sample image.
+    Read in sample image and find known variables in the field of view.
 
     Parameters
     ----------
 
     sample_image_for_finding_stars : str
-        Name or URL of a fits image of the field of view.
+        Name or URL of a FITS image of the field of view.
 
     directory_with_images : str, optional
         Folder in which the image is located. Ignored if the sample image
         is a URL.
+
+    Returns
+    -------
+
+    ccd: `astropy.nddata.CCDData`
+        Sample image.
+
+    vsx: `astropy.table.Table`
+        Table with known variables in the field of view.
+
     """
     if sample_image_for_finding_stars.startswith('http'):
         path = sample_image_for_finding_stars
     else:
         path = Path(directory_with_images) / sample_image_for_finding_stars
 
     ccd = CCDData.read(path)
@@ -87,46 +96,99 @@
         ra = vsx['RAJ2000']
         dec = vsx['DEJ2000']
         vsx['coords'] = SkyCoord(ra=ra, dec=dec, unit=(u.hour, u.degree))
 
     return ccd, vsx
 
 
-def match(CCD, RD, vsx):
+def crossmatch_APASS2VSX(CCD, RD, vsx):
     """
-    Find APASS stars in FOV and matches APASS stars to VSX and
-    APASS to input targets.
+    Find APASS stars in FOV and matches APASS stars to VSX and APASS to input targets.
+
+    Parameters
+    ----------
+
+    CCD : `astropy.nddata.CCDData`
+        Sample image.
+
+    RD : `astropy.table.Table`
+        Table with target information, including a
+        `astropy.coordinates.SkyCoord` column.
+
+    vsx : `astropy.table.Table`
+        Table with known variables in the field of view.
+
+    Returns
+    -------
+
+    apass : `astropy.table.Table`
+        Table with APASS stars in the field of view.
+
+    v_angle : `astropy.units.Quantity`
+        Angular separation between APASS stars and VSX stars.
+
+    RD_angle : `astropy.units.Quantity`
+        Angular separation between APASS stars and input targets.
     """
-    apass, apass_in_bright = find_apass_stars(
-        CCD)
+    apass, apass_in_bright = find_apass_stars(CCD)
     ra = apass['RAJ2000']
     dec = apass['DEJ2000']
     apass['coords'] = SkyCoord(ra=ra, dec=dec, unit=(u.hour, u.degree))
     apass_coord = apass['coords']
 
     if vsx:
         v_index, v_angle, v_dist = \
             apass_coord.match_to_catalog_sky(vsx['coords'])
     else:
         v_angle = []
+
     if RD:
         RD_index, RD_angle, RD_dist = \
             apass_coord.match_to_catalog_sky(RD['coords'])
     else:
         RD_angle = []
+
     return apass, v_angle, RD_angle
 
 
 def mag_scale(cmag, apass, v_angle, RD_angle,
               brighter_dmag=0.44, dimmer_dmag=0.75):
     """
     Select comparison stars that are 1) not close the VSX stars or to other
     target stars and 2) fall within a particular magnitude range.
 
+    Parameters
+    ----------
+
+    cmag : float
+        Magnitude of the target star.
+
+    apass : `astropy.table.Table`
+        Table with APASS stars in the field of view.
+
+    v_angle : `astropy.units.Quantity`
+        Angular separation between APASS stars and VSX stars.
 
+    RD_angle : `astropy.units.Quantity`
+        Angular separation between APASS stars and input targets.
+
+    brighter_dmag : float, optional
+        Maximum difference in magnitude between the target and comparison stars.
+
+    dimmer_dmag : float, optional
+        Minimum difference in magnitude between the target and comparison stars.
+
+    Returns
+    -------
+
+    apass_good_coord : `astropy.coordinates.SkyCoord`
+        Coordinates of the comparison stars.
+
+    good_stars : `astropy.table.Table`
+        Table with the comparison stars.
     """
     high_mag = apass['r_mag'] < cmag + dimmer_dmag
     low_mag = apass['r_mag'] > cmag - brighter_dmag
     if v_angle:
         good_v_angle = v_angle > 1.0 * u.arcsec
     else:
         good_v_angle = True
@@ -140,34 +202,81 @@
     good_apass = apass[good_stars]
     apass_good_coord = good_apass['coords']
     return apass_good_coord, good_stars
 
 
 def in_field(apass_good_coord, ccd, apass, good_stars):
     """
-    Return apass stars in the field of view
+    Return APASS stars in the field of view.
+
+    Parameters
+    ----------
+
+    apass_good_coord : `astropy.coordinates.SkyCoord`
+        Coordinates of the comparison stars.
+
+    ccd : `astropy.nddata.CCDData`
+        Sample image.
+
+    apass : `astropy.table.Table`
+        Table with APASS stars in the field of view.
+
+    good_stars : `astropy.table.Table`
+        Table with the comparison stars.
+
+    Returns
+    -------
+
+    ent : `astropy.table.Table`
+        Table with APASS stars in the field of view.
     """
     apassx, apassy = ccd.wcs.all_world2pix(
         apass_good_coord.ra, apass_good_coord.dec, 0)
     ccdx, ccdy = ccd.shape
 
     xin = (apassx < ccdx) & (0 < apassx)
     yin = (apassy < ccdy) & (0 < apassy)
     xy_in = xin & yin
     apass_good_coord[xy_in]
     nt = apass[good_stars]
     ent = nt[xy_in]
     return ent
 
 
-def make_markers(iw, ccd, RD, vsx, ent,
-                 name_or_coord=None):
+def make_markers(iw, ccd, RD, vsx, ent, name_or_coord=None):
     """
-    Add markers for APASS, TESS targets, VSX.
-    Also center on object/coordinate.
+    Add markers for APASS, TESS targets, VSX.  Also center on object/coordinate.
+
+    Parameters
+    ----------
+
+    iw : `astrowidgets.ImageWidget`
+        Ginga widget.
+
+    ccd : `astropy.nddata.CCDData`
+        Sample image.
+
+    RD : `astropy.table.Table`
+        Table with target information, including a
+        `astropy.coordinates.SkyCoord` column.
+
+    vsx : `astropy.table.Table`
+        Table with known variables in the field of view.
+
+    ent : `astropy.table.Table`
+        Table with APASS stars in the field of view.
+
+    name_or_coord : str or `astropy.coordinates.SkyCoord`, optional
+        Name or coordinates of the target.
+
+    Returns
+    -------
+
+    None
+        Markers are added to the image in Ginga widget.
     """
     iw.load_nddata(ccd)
     iw.zoom_level = 'fit'
 
     try:
         iw.reset_markers()
     except AttributeError:
@@ -189,17 +298,28 @@
         iw.add_markers(vsx, skycoord_colname='coords',
                        use_skycoord=True, marker_name='VSX')
     iw.marker = {'type': 'circle', 'color': 'red', 'radius': 10}
     iw.add_markers(ent, skycoord_colname='coords',
                    use_skycoord=True, marker_name='APASS comparison')
     iw.marker = {'type': 'cross', 'color': 'red', 'radius': 6}
 
+
 def wrap(imagewidget, outputwidget):
     """
-    Make the bits that let you click to select/deselect comparisons
+    Utility function to let you click to select/deselect comparisons.
+
+    Parameters
+    ----------
+
+    imagewidget : `astrowidgets.ImageWidget`
+        Ginga widget.
+
+    outputwidget : `ipywidgets.Output`
+        Output widget for printing information.
+
     """
     def cb(viewer, event, data_x, data_y):
         i = imagewidget._viewer.get_image()
 
         try:
             imagewidget.next_elim += 1
         except AttributeError:
@@ -238,23 +358,86 @@
                 print('sorry try again')
                 imagewidget._viewer.onscreen_message('Click closer to a star')
 
     return cb
 
 
 class ComparisonViewer:
+    """
+    A class to store an instance of the comparison viewer.
+
+    Attributes
+    ----------
+
+    target_mag : float
+        Magnitude of the target.
+
+    bright_mag_limit : float
+        Bright magnitude limit for APASS stars.
+
+    dim_mag_limit : float
+        Dim magnitude limit for APASS stars.
+
+    targets_from_file : str
+        File with target information.
+
+    tess_submission : `~stellarphot.io.TessSubmission`
+        Instance of the TESS submission class.
+
+    target_coord : `astropy.coordinates.SkyCoord`
+        Coordinates of the target.
+
+    box : `ipywidgets.Box`
+        Box containing the widgets.
+
+    iw : `ginga.util.grc.RemoteClient`
+        Ginga widget.
+
+    aperture_output_file : str
+        File to save aperture information to.
+    """
     def __init__(self,
                  file="",
                  directory='.',
                  target_mag=10,
                  bright_mag_limit=8,
                  dim_mag_limit=17,
                  targets_from_file=None,
                  object_coordinate=None,
                  aperture_output_file=None):
+        """
+        Initializes an instance of the ComparisonViewer class.
+
+        Parameters
+        ----------
+
+        file : str, optional
+            File to open. Defaults to "".
+
+        directory : str, optional
+            Directory to open file from. Defaults to '.'.
+
+        target_mag : float, optional
+            Magnitude of the target. Defaults to 10.
+
+        bright_mag_limit : float, optional
+            Bright magnitude limit for APASS stars. Defaults to 8.
+
+        dim_mag_limit : float, optional
+            Dim magnitude limit for APASS stars.  Defaults to 17.
+
+        targets_from_file : str, optional
+            File with target information.  Defaults to None.
+
+        object_coordinate : `astropy.coordinates.SkyCoord`, optional
+            Coordinates of the target. Defaults to None.
+
+        aperture_output_file : str, optional
+            File to save aperture information to.  Defaults to None.
+        """
 
         self._label_name = 'labels'
         self._circle_name = 'target circle'
         self._file_chooser = FitsOpener()
 
         self._directory = directory
         self.target_mag = target_mag
@@ -273,38 +456,48 @@
             self._file_chooser.set_file(file, directory=directory)
             self._set_file(None)
 
         self._make_observers()
 
     def _init(self):
         """
-        Some initialization needs to be defered until a file is chosen.
+        Handles aspects of initialization that need to be defered until a file is chosen.
         """
         if self.tess_submission is not None:
             self._tess_object_info.layout.visibility = "visible"
         self.ccd, self.vsx = \
             set_up(self._file_chooser.path.name,
                    directory_with_images=self._file_chooser.path.parent
                    )
 
-        apass, vsx_apass_angle, targets_apass_angle = match(self.ccd,
-                                                            self.targets_from_file,
-                                                            self.vsx)
+        apass, vsx_apass_angle, targets_apass_angle = crossmatch_APASS2VSX(self.ccd,
+                                                                            self.targets_from_file,
+                                                                            self.vsx)
 
         apass_good_coord, good_stars = mag_scale(self.target_mag, apass, vsx_apass_angle,
                                                  targets_apass_angle,
                                                  brighter_dmag=self.target_mag - self.bright_mag_limit,
                                                  dimmer_dmag=self.dim_mag_limit - self.target_mag)
 
         apass_comps = in_field(apass_good_coord, self.ccd, apass, good_stars)
         make_markers(self.iw, self.ccd, self.targets_from_file, self.vsx, apass_comps,
                      name_or_coord=self.target_coord)
 
     @property
     def variables(self):
+        """
+        Return a dictionary of the variables in the class.
+
+        Returns
+        -------
+
+        our_vsx : `astropy.table.Table`
+            Table of the variables in the class.
+
+        """
         comp_table = self.generate_table()
         new_vsx_mark = comp_table['marker name'] == 'VSX'
         idx, _, _ = comp_table['coord'][new_vsx_mark].match_to_catalog_sky(self.vsx['coords'])
         our_vsx = self.vsx[idx]
         our_vsx['star_id'] = comp_table['star_id'][new_vsx_mark]
         return our_vsx
 
@@ -501,23 +694,46 @@
         inner_box.children = [iw, legend]
         box.children = [self._file_chooser.file_chooser, self.object_name, self._tess_object_info, header,
                         inner_box, controls, self.tess_save_toggle, self._tess_save_box]
 
         return box, iw
 
     def save_tess_files(self, button=None):
+        """
+        Save the TESS files.
+
+        Parameters
+        ----------
+
+        button : `ipywidgets.Button`, optional
+            The button that was clicked.
+
+        Returns
+        -------
+
+        None
+            Button to save TESS file set to true (triggering action).
+        """
         if self._field_name.value:
             self.tess_field_view()
             self.iw.save(self._field_name.value, overwrite=True)
 
         if self._zoom_name.value:
             self.tess_field_zoom_view()
             self.iw.save(self._zoom_name.value, overwrite=True)
 
     def generate_table(self):
+        """
+        Generate the table of stars to use for the aperture file.
+
+        Returns
+        -------
+        comp_table : `astropy.table.Table`
+            Table of stars to use for the aperture file.
+        """
         try:
             all_table = self.iw.get_all_markers()
         except AttributeError:
             all_table = self.iw.get_markers(marker_name='all')
 
         elims = np.array([name.startswith('elim')
                          for name in all_table['marker name']])
@@ -553,14 +769,23 @@
 
         # Assign the IDs
         comp_table['star_id'] = range(1, len(comp_table) + 1)
 
         return comp_table
 
     def show_labels(self):
+        """
+        Show the labels for the stars.
+
+        Returns
+        -------
+
+        None
+            Labels for the stars are shown.
+        """
         plot_names = []
         comp_table = self.generate_table()
 
         original_mark = self.iw._marker
         for star in comp_table:
             star_id = star['star_id']
             if star['marker name'] == 'TESS Targets':
@@ -583,54 +808,116 @@
             else:
                 label = f'U{star_id}'
                 print(f"Unrecognized marker name: {star['marker name']}")
             plot_names.append(label)
         self.iw._marker = original_mark
 
     def remove_labels(self):
+        """
+        Remove the labels for the stars.
+
+        Returns
+        -------
+
+        None
+            Labels for the stars are removed.
+        """
         try:
             try:
                 self.iw.remove_markers(marker_name=self._label_name)
             except AttributeError:
                 self.iw.remove_markers_by_name(marker_name=self._label_name)
         except ValueError:
             # No labels, keep going
             pass
 
     def show_circle(self,
                     radius=2.5 * u.arcmin,
                     pixel_scale=0.56 * u.arcsec / u.pixel):
+        """
+        Show a circle around the target.
+
+        Parameters
+        ----------
+
+        radius : `astropy.units.Quantity`, optional
+            Radius of circle. The default is ``2.5*u.arcmin``.
+
+        pixel_scale : `astropy.units.Quantity`, optional
+            Pixel scale of image. The default is ``0.56*u.arcsec/u.pixel``.
+
+        Returns
+        -------
+
+        None
+            Circle is shown around the target.
+        """
         radius_pixels = np.round((radius / pixel_scale).to(u.pixel).value,
                                  decimals=0)
         orig_marker = self.iw.marker
         self.iw.marker = {'color': 'yellow',
                           'radius': radius_pixels,
                           'type': 'circle'}
         self.iw.add_markers(Table(data=[[self.target_coord]], names=['coords']),
                             skycoord_colname='coords',
                             use_skycoord=True, marker_name=self._circle_name)
         self.iw.marker = orig_marker
 
     def remove_circle(self):
+        """
+        Remove the circle around the target.
+
+        Returns
+        -------
+
+        None
+            Circle is removed from the image.
+        """
         try:
             self.iw.remove_markers(marker_name=self._circle_name)
         except AttributeError:
             self.iw.remove_markers_by_name(marker_name=self._circle_name)
 
     def tess_field_view(self):
+        """
+        Show the whole TESS field of view including circle around target, but hide labels.
+
+        Returns
+        -------
+
+        None
+            Shows image as described above.
+        """
+
         # Show whole field of view
         self.iw.zoom_level = 'fit'
 
         # Show the circle
         self.show_circle()
 
-        # Turn of labels -- too cluttered
+        # Turn off labels -- too cluttered
         self.remove_labels()
 
     def tess_field_zoom_view(self, width=6 * u.arcmin):
+        """
+        Zoom in on the TESS field of view.
+
+        Parameters
+        ----------
+
+        width : `astropy.units.Quantity`, optional
+            Width of field of view. The default is ``6*u.arcmin``.
+
+        Returns
+        -------
+
+        None
+            Zooms in on the image as described above.
+        """
+
         # Turn off labels -- too cluttered
         self.remove_labels()
 
         left_side = self.ccd.wcs.pixel_to_world(0, self.ccd.shape[1]/2)
         right_side = self.ccd.wcs.pixel_to_world(self.ccd.shape[0], self.ccd.shape[1]/2)
         fov = left_side.separation(right_side)
 
@@ -639,10 +926,7 @@
         self.iw.zoom_level = "fit"
 
         # Then set it to what we actually want...
         self.iw.zoom_level = self.iw.zoom_level / view_ratio
 
         # Show the circle
         self.show_circle()
-
-
-
```

### Comparing `stellarphot-1.3.8/stellarphot/visualization/fits_opener.py` & `stellarphot-1.3.9/stellarphot/visualization/fits_opener.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,54 @@
 
 from astropy.io import fits
 from astropy.nddata import CCDData
 
 from ipyfilechooser import FileChooser
 
 
+__all__ = ['FitsOpener']
+
+
 class FitsOpener:
+    """ A class to open FITS files and display them in an `astrowidgets.ImageWidget`.
+
+    Attributes
+    ----------
+
+    ccd : `astropy.nddata.CCDData`
+        The selected FITS file as a CCDData object.
+
+    file_chooser : `ipyfilechooser.FileChooser`
+        The actual FileChooser widget.
+
+    header : dict
+        The header of the selected FITS file.
+
+    path : `pathlib.Path`
+        The path to the selected FITS file.
+
+    register_callback : function, optional
+        A function that takes one argument. This function will be called when the
+        selected file changes.
+    """
     def __init__(self, title="Choose an image", filter_pattern=None, **kwargs):
+        """
+        Initializes an instance of the FitsOpener class, which is a wrapper around
+        the `ipyfilechooser.FileChooser` widget that (if no `filter_pattern` is given)
+        defaults to showing only FITS files.
+
+        Parameters
+        ----------
+
+        title : str, optional
+            The title of the FileChooser widget. The default is "Choose an image".
+
+        filter_pattern : str, optional
+            The filter pattern to use for the FileChooser widget. The default is None,
+        """
         self._fc = FileChooser(title=title, **kwargs)
         if not filter_pattern:
             self._fc.filter_pattern = ['*.fit*', '*.fit*.[bg]z']
         else:
             self._fc.filter_pattern = filter_pattern
 
         self._header = {}
@@ -88,25 +126,25 @@
             The widget into which to load the image.
         """
         with warnings.catch_warnings():
             image_widget.load_fits(str(self.path))
 
     def set_file(self, file, directory=None):
         """
-        Set the selected file of the ``FileChooser`` to be the input file.
+        Set the selected file of the `ipyfilechooser.FileChooser` to be the input file.
 
         Parameters
         ----------
 
         file : Path-like
             The file to be set as selected. Can be a string or a pathlib.Path.
             Cannot contain any directory information.
 
         directory : Path-like, optional
             Directory the file is in. The default value is the current directory of the
-            ``FileChooser``.
+            `ipyfilechooser.FileChooser`.
         """
         if directory is None:
             directory = self._fc.selected_path
 
         self._fc.reset(directory, file)
         self._fc._apply_selection()
```

### Comparing `stellarphot-1.3.8/stellarphot/visualization/multi_night_plots.py` & `stellarphot-1.3.9/stellarphot/visualization/multi_night_plots.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,50 @@
 
 def plot_magnitudes(mags=None, errors=None, times=None,
                     source=None, night=None, ref_mag=0,
                     alpha=0.25, y_range=None):
     """
     Plot one night of magnitude data for one source, overlaying a rolling
     mean and indication of mean/deviation.
+
+    Parameters
+    ----------
+
+    mags : array of floats, optional
+        Magnitudes of source.
+
+    errors : array of floats, optional
+        Errors on magnitudes.
+
+    times : array-like, optional
+        Times of observations.
+
+    source : `~stellarphot.source.Source`, optional
+        Source object.
+
+    night : float, optional
+        Night of observations.
+
+    ref_mag : float, optional
+        Reference magnitude of source. Default is 0.
+
+    alpha : float, optional
+        Alpha value for error bars. Default is 0.25.
+
+    y_range : tuple
+        Range of y-axis. Default is None.
+
+    Returns
+    -------
+
+    mean : float
+        Mean magnitude of source.
+
+    std : float
+        Standard deviation of magnitudes.
     """
     mean = np.nanmean(mags)
     std = np.nanstd(mags)
 
     working_times = times
     plt.errorbar(working_times, mags, yerr=errors, fmt='o', alpha=alpha,
                  label='night: {}'.format(night))
@@ -60,15 +96,46 @@
     return mean, std
 
 
 def multi_night(sources, unique_nights, night,
                 brightest_mag, mags, mag_err,
                 uniform_ylim=True):
     """
-    Plot magnitude vs time data for several sources over several nights
+    Plot magnitude vs time data for several sources over several nights.
+
+    Parameters
+    ----------
+
+    sources : list
+        List of `~stellarphot.source.Source` objects.
+
+    unique_nights : list
+        List of unique nights.
+
+    night : array-like
+        Array of nights.
+
+    brightest_mag : float
+        Brightest magnitude of sources.
+
+    mags : array-like
+        Array of magnitudes.
+
+    mag_err : array-like
+        Array of magnitude errors.
+
+    uniform_ylim : bool, optional
+        If True, use the median and median absolute deviation of the
+        magnitudes to set the y-axis range for each source. Default is True.
+
+    Returns
+    -------
+
+    None
+        Generates a plot of magnitude vs time for each source.
     """
     number_of_nights = len(unique_nights)
 
     for source in sources:
         f = plt.figure(figsize=(5 * number_of_nights, 5))
 
         night_means = []
```

### Comparing `stellarphot-1.3.8/stellarphot/visualization/seeing_profile_functions.py` & `stellarphot-1.3.9/stellarphot/visualization/seeing_profile_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,35 +16,46 @@
 
 import matplotlib.pyplot as plt
 
 from stellarphot.io import TessSubmission
 from stellarphot.visualization import seeing_plot
 from stellarphot.visualization.fits_opener import FitsOpener
 
-__all__ = ['set_keybindings', 'box', 'make_show_event']
+__all__ = ['set_keybindings', 'find_center', 'radial_profile',
+            'find_hwhm', 'RadialProfile', 'box', 'SeeingProfileWidget']
 
 desc_style = {"description_width": "initial"}
 
 
 def set_keybindings(image_widget, scroll_zoom=False):
     """
     Set image widget keyboard bindings. The bindings are:
 
     + Pan by click-and-drag or with arrow keys.
     + Zoom by scrolling or using the ``+``/``-`` keys.
-    + Adjust contrast by Ctrl-left click and drag; reset with
-      shift-right-click.
+    + Adjust contrast by Ctrl-right click and drag
+    + Reset contrast with shift-right-click.
 
     Any existing key bindings are removed.
 
     Parameters
     ----------
 
-    image_widget : astrowidgets.ImageWidget
+    image_widget : `astrowidgets.ImageWidget`
         Image widget on which to set the key bindings.
+
+    scroll_zoom : bool, optional
+        If True, zooming can be done by scrolling the mouse wheel.
+        Default is False.
+
+    Returns
+    -------
+
+    None
+        Adds key bindings to the image widget.
     """
     bind_map = image_widget._viewer.get_bindmap()
     # Displays the event map...
     # bind_map.eventmap
     bind_map.clear_event_map()
     bind_map.map_event(None, (), 'ms_left', 'pan')
     if scroll_zoom:
@@ -77,27 +88,34 @@
     """
     Find the centroid of a star from an initial guess of its position. Originally
     written to find star from a mouse click.
 
     Parameters
     ----------
 
-    image : numpy array or CCDData
+    image : `astropy.nddata.CCDData` or numpy array
         Image containing the star.
 
     center_guess : array or tuple
         The position, in pixels, of the initial guess for the position of
         the star. The coordinates should be horizontal first, then vertical,
         i.e. opposite the usual Python convention for a numpy array.
 
     cutout_size : int, optional
         The default width of the cutout to use for finding the star.
 
     max_iters : int, optional
         Maximum number of iterations to go through in finding the center.
+
+    Returns
+    -------
+
+    cen : array
+        The position of the star, in pixels, as found by the centroiding
+        algorithm.
     """
     pad = cutout_size // 2
     x, y = center_guess
 
     # Keep track of iterations
     cnt = 0
 
@@ -143,44 +161,49 @@
     """
     Construct a radial profile of a chunk of width ``size`` centered
     at ``center`` from image ``data`.
 
     Parameters
     ----------
 
-    data : numpy array or CCDData
+    data : `astropy.nddata.CCDData` or numpy array
         Image data
+
     center : list-like
         x, y position of the center in pixel coordinates, i.e. horizontal
         coordinate then vertical.
+
     size : int, optional
         Width of the rectangular cutout to use in constructing the profile.
+
     return_scaled : bool, optional
         If ``True``, return an average radius and profile, otherwise
         it is cumulative. Not at all clear what a "cumulative" radius
         means, tbh.
 
     Returns
     -------
 
     r_exact : numpy array
         Exact radius of center of each pixels from profile center.
+
     ravg : numpy array
-        Average radius of pixels in each bin.
+        Average radius in pixels used in constructing profile.
+
     radialprofile : numpy array
         Radial profile.
     """
     yd, xd = np.indices((size, size))
 
     sub_image = Cutout2D(data, center, size, mode='strict')
     sub_center = sub_image.center_cutout
 
     r = np.sqrt((xd - sub_center[0])**2 + (yd - sub_center[1])**2)
     r_exact = r.copy()
-    r = r.astype(np.int)
+    r = r.astype(int)
 
     sub_data = sub_image.data
 
     tbin = np.bincount(r.ravel(), sub_data.ravel())
     rbin = np.bincount(r.ravel(), r_exact.ravel())
     nr = np.bincount(r.ravel())
     if return_scaled:
@@ -191,16 +214,32 @@
         ravg = rbin
 
     return r_exact, ravg, radialprofile
 
 
 def find_hwhm(r, intensity):
     """
-    Estimate HWHM from normalized, angle-averaged intensity profile.
+    Estimate the half-width half-max from normalized, angle-averaged intensity profile.
+
+    Parameters
+    ----------
+
+    r : array
+        Radius of each pixel from the center of the star.
+
+    intensity : array
+        Normalized intensity at each radius.
+
+    Returns
+    -------
+
+    r_half : float
+        Radius at which the intensity is 50% the maximum
     """
+
     # Make the bold assumption that intensity decreases monotonically
     # so that we just need to find the first place where intensity is
     # less than 0.5 to estimate the HWHM.
     less_than_half = intensity < 0.5
     half_index = np.arange(len(less_than_half))[less_than_half][0]
     before_half = half_index - 1
 
@@ -215,19 +254,88 @@
 
     r_half = r_less - (I_less - I_half) / (I_less - I_more) * (r_less - r_more)
 
     return r_half
 
 
 class RadialProfile:
+    """
+    Class to hold radial profile information for a star.
+
+    Parameters
+    ----------
+
+    data : numpy array
+        Image data.
+
+    x : int
+        x position of the star.
+
+    y : int
+        y position of the star.
+
+    Attributes
+    ----------
+
+    cen : tuple
+        x, y position of the center of the star.
+
+    data : numpy array
+        Image data.
+
+    FWHM : float
+        Full-width half-max of the radial profile.
+
+    profile_size : int
+        Size of the cutout used to construct the radial profile.
+
+    radius_values : numpy array
+        Radius values for the radial profile.
+
+    r_exact : numpy array
+        Exact radius of center of each pixels from profile center.
+
+    ravg : numpy array
+        Average radius in pixels used in constructing profile.
+
+    """
     def __init__(self, data, x, y):
+        """
+        Initialize the radial profile object instance.  Sets the center
+        of the star and the image data.
+
+        Parameters
+        ----------
+
+        data : numpy array
+            Image data.
+
+        x : int
+            x position of the star.
+
+        y : int
+            y position of the star.
+
+
+        """
         self.cen = find_center(data, (x, y), cutout_size=30)
         self.data = data
 
     def profile(self, profile_size):
+        """
+        Construct the radial profile of the star.  Sets
+        ``r_exact``, ``ravg``, and ``radialprofile`` attributes.
+
+        Parameters
+        ----------
+
+        profile_size : int
+            Size of the cutout to use in constructing the profile.
+
+        """
         self.profile_size = profile_size
         self.r_exact, self.ravg, self.radialprofile = (
             radial_profile(self.data,
                            self.cen,
                            size=profile_size)
         )
 
@@ -246,21 +354,41 @@
     def radius_values(self):
         return np.arange(len(self.radialprofile))
 
 
 def box(imagewidget):
     """
     Compatibility layer for older versions of the photometry notebooks.
+
+    Parameters
+    ----------
+
+    imagewidget : `astrowidgets.ImageWidget`
+        ImageWidget instance to use for the seeing profile.
+
+    Returns
+    -------
+
+    box : `ipywidgets.VBox`
+        Box containing the seeing profile widget.
     """
     return SeeingProfileWidget(imagewidget=imagewidget).box
 
 
 class SeeingProfileWidget:
     """
-    Build a widget for measuring the seeing profile of stars in an image.
+    A class for storing an instance of a widget displaying the seeing profile of stars in an image.
+
+    Parameters
+    ----------
+    imagewidget : `astrowidgets.ImageWidget`, optional
+        ImageWidget instance to use for the seeing profile.
+
+    width : int, optional
+        Width of the seeing profile widget.
     """
     def __init__(self, imagewidget=None, width=500):
         if not imagewidget:
             imagewidget = ImageWidget(image_width=width,
                                       image_height=width,
                                       use_opencv=True)
 
@@ -404,16 +532,18 @@
                 # Rough location of click in original image
                 x = int(np.floor(event.data_x))
                 y = int(np.floor(event.data_y))
 
                 rad_prof = RadialProfile(data, x, y)
 
                 try:
-                    # Remove previous marker
-                    self.iw.remove_markers_by_name(self._aperture_name)
+                    try: # Remove previous marker
+                        self.iw.remove_markers(marker_name=self._aperture_name)
+                    except AttributeError:
+                        self.iw.remove_markers_by_name(marker_name=self._aperture_name)
                 except ValueError:
                     # No markers yet, keep going
                     pass
 
                 # ADD MARKER WHERE CLICKED
                 self.iw.add_markers(Table(data=[[rad_prof.cen[0]], [rad_prof.cen[1]]],
                                           names=['x', 'y']),
@@ -432,14 +562,15 @@
                 # Set this AFTER the radial profile has been created to avoid an attribute
                 # error.
                 self.ap_t.value = aperture_radius
             else:
                 # User changed aperture
                 aperture_radius = aperture
                 rad_prof = self.rad_prof
+
             # DISPLAY THE SCALED PROFILE
             self.out.clear_output(wait=True)
             with self.out:
                 # sub_med += med
                 self._seeing_plot_fig = seeing_plot(rad_prof.r_exact, rad_prof.scaled_exact_counts,
                             rad_prof.ravg,
                             rad_prof.scaled_profile, rad_prof.HWHM,
```

### Comparing `stellarphot-1.3.8/stellarphot/visualization/tests/test_seeing_profile.py` & `stellarphot-1.3.9/stellarphot/visualization/tests/test_seeing_profile.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.8/stellarphot.egg-info/SOURCES.txt` & `stellarphot-1.3.9/stellarphot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 docs/stellarphot/index.rst
 licenses/LICENSE.rst
 licenses/README.rst
 licenses/TEMPLATE_LICENCE.rst
 stellarphot/__init__.py
 stellarphot/_astropy_init.py
 stellarphot/conftest.py
-stellarphot/coordinates.py
 stellarphot/core.py
 stellarphot/photometry.py
 stellarphot/source_detection.py
 stellarphot/version.py
 stellarphot.egg-info/PKG-INFO
 stellarphot.egg-info/SOURCES.txt
 stellarphot.egg-info/dependency_links.txt
@@ -69,44 +68,37 @@
 stellarphot/io/aij.py
 stellarphot/io/tess.py
 stellarphot/io/tests/__init__.py
 stellarphot/io/tests/test_aij_io.py
 stellarphot/io/tests/test_tess_submission.py
 stellarphot/io/tests/data/aij-sample-apertures.aperture
 stellarphot/io/tests/data/apertures_as_table.csv
-stellarphot/notebooks/ObserveACP.ipynb
 stellarphot/notebooks/__init__.py
-stellarphot/notebooks/acp.py
-stellarphot/notebooks/calculate_aavso_mags_draft.ipynb
 stellarphot/notebooks/comp-star-plots.ipynb
 stellarphot/notebooks/comp-stars-template.ipynb
-stellarphot/notebooks/example_interactive_plot.ipynb
-stellarphot/notebooks/get_apass_comp_mags.ipynb
 stellarphot/notebooks/image-viewer-working-copy.ipynb
-stellarphot/notebooks/image_viewer_demo.ipynb
 stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb
 stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb
 stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb
 stellarphot/notebooks/photometry/03-photometry-template.ipynb
 stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb
 stellarphot/notebooks/photometry/06-transit-fit-template.ipynb
 stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb
+stellarphot/notebooks/photometry/0X-comps-star-plot (1).ipynb
 stellarphot/notebooks/photometry/Untitled.ipynb
 stellarphot/notebooks/photometry/__init__.py
 stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb
 stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb
 stellarphot/notebooks/photometry/transform-pared-back.ipynb
 stellarphot/tests/__init__.py
 stellarphot/tests/make_wcs.py
-stellarphot/tests/test_coordinates.py
 stellarphot/tests/test_core.py
 stellarphot/tests/test_detection.py
 stellarphot/tests/test_photometry.py
 stellarphot/tests/data/test_sources.csv
-stellarphot/utils/__init__.py
 stellarphot/visualization/__init__.py
 stellarphot/visualization/aij_plots.py
 stellarphot/visualization/comparison_functions.py
 stellarphot/visualization/fits_opener.py
 stellarphot/visualization/multi_night_plots.py
 stellarphot/visualization/photometry_widget_functions.py
 stellarphot/visualization/seeing_profile_functions.py
```

### Comparing `stellarphot-1.3.8/tox.ini` & `stellarphot-1.3.9/tox.ini`

 * *Files identical despite different names*

