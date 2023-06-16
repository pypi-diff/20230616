# Comparing `tmp/mlcalcdriver-1.4.0.tar.gz` & `tmp/mlcalcdriver-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcalcdriver-1.4.0.tar", last modified: Thu May 12 21:06:27 2022, max compression
+gzip compressed data, was "mlcalcdriver-1.4.1.tar", last modified: Fri Jun 16 19:08:54 2023, max compression
```

## Comparing `mlcalcdriver-1.4.0.tar` & `mlcalcdriver-1.4.1.tar`

### file list

```diff
@@ -1,188 +1,198 @@
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/.github/
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/.github/workflows/
--rw-r--r--   0 oliviermt  (1026) staff       (20)     1259 2021-12-10 21:34:04.000000 mlcalcdriver-1.4.0/.github/workflows/python-package.yml
--rw-r--r--   0 oliviermt  (1026) staff       (20)     1223 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/.gitignore
--rw-r--r--   0 oliviermt  (1026) staff       (20)      658 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/.pep8speaks.yml
--rw-r--r--   0 oliviermt  (1026) staff       (20)       48 2022-02-09 20:52:21.000000 mlcalcdriver-1.4.0/.pyup.yml
--rw-r--r--   0 oliviermt  (1026) staff       (20)    35149 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/LICENSE
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2658 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/PKG-INFO
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2185 2022-05-12 20:51:50.000000 mlcalcdriver-1.4.0/README.md
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/
--rw-r--r--   0 oliviermt  (1026) staff       (20)      230 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/.buildinfo
--rw-r--r--   0 oliviermt  (1026) staff       (20)        0 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/.nojekyll
--rw-r--r--   0 oliviermt  (1026) staff       (20)      688 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/Makefile
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_modules/
--rw-r--r--   0 oliviermt  (1026) staff       (20)     4937 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/_modules/index.html
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/base/
--rw-r--r--   0 oliviermt  (1026) staff       (20)    42890 2022-05-12 20:46:45.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/base/job.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    97977 2022-05-12 20:46:45.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/base/posinp.html
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/calculators/
--rw-r--r--   0 oliviermt  (1026) staff       (20)    12601 2022-05-12 20:46:45.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/calculators/calculator.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    38307 2022-05-12 20:46:45.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/calculators/schnetpack.html
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/interfaces/
--rw-r--r--   0 oliviermt  (1026) staff       (20)     9195 2022-05-12 20:46:45.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/interfaces/ase_interface.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    10219 2022-05-12 20:46:45.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/workflows/
--rw-r--r--   0 oliviermt  (1026) staff       (20)    24450 2022-05-12 20:46:45.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/workflows/geopt.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    40427 2022-05-12 20:46:45.000000 mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/workflows/phonon.html
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_sources/
--rw-r--r--   0 oliviermt  (1026) staff       (20)      170 2021-12-10 21:34:04.000000 mlcalcdriver-1.4.0/docs/_sources/ase_interface.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)      136 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/_sources/base.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)      120 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/_sources/calculator.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)      215 2022-05-12 19:27:02.000000 mlcalcdriver-1.4.0/docs/_sources/calculators.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       90 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/_sources/geopt.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       54 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/_sources/globals.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)      438 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/_sources/index.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)      517 2022-05-12 20:55:16.000000 mlcalcdriver-1.4.0/docs/_sources/interfaces.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       61 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/_sources/job.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       87 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/_sources/phonon.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       90 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/_sources/posinp.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)      140 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/_sources/schnet_interface.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       95 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/_sources/schnetcalc.rst.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)      159 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/_sources/workflows.rst.txt
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_static/
--rw-r--r--   0 oliviermt  (1026) staff       (20)    14692 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/_static/basic.css
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_static/css/
--rw-r--r--   0 oliviermt  (1026) staff       (20)     3275 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/badge_only.css
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/
--rw-r--r--   0 oliviermt  (1026) staff       (20)    87624 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 oliviermt  (1026) staff       (20)    67312 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 oliviermt  (1026) staff       (20)    86288 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 oliviermt  (1026) staff       (20)    66444 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 oliviermt  (1026) staff       (20)   165742 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 oliviermt  (1026) staff       (20)   444379 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 oliviermt  (1026) staff       (20)   165548 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 oliviermt  (1026) staff       (20)    98024 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 oliviermt  (1026) staff       (20)    77160 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 oliviermt  (1026) staff       (20)   323344 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 oliviermt  (1026) staff       (20)   193308 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 oliviermt  (1026) staff       (20)   309728 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 oliviermt  (1026) staff       (20)   184912 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 oliviermt  (1026) staff       (20)   328412 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 oliviermt  (1026) staff       (20)   195704 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 oliviermt  (1026) staff       (20)   309192 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 oliviermt  (1026) staff       (20)   182708 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 oliviermt  (1026) staff       (20)   129674 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/css/theme.css
--rw-r--r--   0 oliviermt  (1026) staff       (20)     9758 2022-03-16 20:02:08.000000 mlcalcdriver-1.4.0/docs/_static/doctools.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)      355 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/_static/documentation_options.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)      286 2022-03-16 20:02:08.000000 mlcalcdriver-1.4.0/docs/_static/file.png
--rw-r--r--   0 oliviermt  (1026) staff       (20)   287630 2022-03-16 20:02:08.000000 mlcalcdriver-1.4.0/docs/_static/jquery-3.5.1.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)    89476 2022-03-16 20:02:08.000000 mlcalcdriver-1.4.0/docs/_static/jquery.js
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/_static/js/
--rw-r--r--   0 oliviermt  (1026) staff       (20)      934 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/js/badge_only.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)     4370 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2734 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/js/html5shiv.min.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)     5023 2022-03-16 20:02:13.000000 mlcalcdriver-1.4.0/docs/_static/js/theme.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)    10854 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/_static/language_data.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)       90 2022-03-16 20:02:08.000000 mlcalcdriver-1.4.0/docs/_static/minus.png
--rw-r--r--   0 oliviermt  (1026) staff       (20)       90 2022-03-16 20:02:08.000000 mlcalcdriver-1.4.0/docs/_static/plus.png
--rw-r--r--   0 oliviermt  (1026) staff       (20)     4846 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/_static/pygments.css
--rw-r--r--   0 oliviermt  (1026) staff       (20)    16793 2022-03-16 20:02:08.000000 mlcalcdriver-1.4.0/docs/_static/searchtools.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)    19530 2022-03-16 20:02:08.000000 mlcalcdriver-1.4.0/docs/_static/underscore.js
--rw-r--r--   0 oliviermt  (1026) staff       (20)     7169 2022-05-12 20:57:29.000000 mlcalcdriver-1.4.0/docs/ase_interface.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)     5341 2022-05-12 20:57:29.000000 mlcalcdriver-1.4.0/docs/base.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    11101 2022-05-12 20:57:29.000000 mlcalcdriver-1.4.0/docs/calculator.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)     6388 2022-05-12 21:01:55.000000 mlcalcdriver-1.4.0/docs/calculators.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    24446 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/genindex.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    14232 2022-05-12 20:57:29.000000 mlcalcdriver-1.4.0/docs/geopt.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    16804 2022-05-12 20:57:29.000000 mlcalcdriver-1.4.0/docs/globals.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    12331 2022-05-12 21:04:45.000000 mlcalcdriver-1.4.0/docs/index.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)     5838 2022-05-12 21:04:45.000000 mlcalcdriver-1.4.0/docs/interfaces.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    14803 2022-05-12 20:57:30.000000 mlcalcdriver-1.4.0/docs/job.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)     1441 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/objects.inv
--rw-r--r--   0 oliviermt  (1026) staff       (20)    16522 2022-05-12 20:57:30.000000 mlcalcdriver-1.4.0/docs/phonon.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    45912 2022-05-12 20:57:30.000000 mlcalcdriver-1.4.0/docs/posinp.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)     7185 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/py-modindex.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)     9024 2022-05-12 20:57:30.000000 mlcalcdriver-1.4.0/docs/schnet_interface.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    11395 2022-05-12 20:57:30.000000 mlcalcdriver-1.4.0/docs/schnetcalc.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)     4034 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/search.html
--rw-r--r--   0 oliviermt  (1026) staff       (20)    15533 2022-05-12 21:04:46.000000 mlcalcdriver-1.4.0/docs/searchindex.js
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/docs/source/
--rw-r--r--   0 oliviermt  (1026) staff       (20)      170 2021-12-10 21:34:04.000000 mlcalcdriver-1.4.0/docs/source/ase_interface.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)      136 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/source/base.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)      120 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/source/calculator.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)      215 2022-05-12 19:27:02.000000 mlcalcdriver-1.4.0/docs/source/calculators.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2438 2022-05-12 20:48:00.000000 mlcalcdriver-1.4.0/docs/source/conf.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)       90 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/source/geopt.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)       54 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/source/globals.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)      438 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/source/index.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)      517 2022-05-12 20:55:16.000000 mlcalcdriver-1.4.0/docs/source/interfaces.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)       61 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/source/job.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)       87 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/source/phonon.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)       90 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/source/posinp.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)      140 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/source/schnet_interface.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)       95 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/docs/source/schnetcalc.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)      159 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/docs/source/workflows.rst
--rw-r--r--   0 oliviermt  (1026) staff       (20)     5206 2022-05-12 20:57:30.000000 mlcalcdriver-1.4.0/docs/workflows.html
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/mlcalcdriver/
--rw-r--r--   0 oliviermt  (1026) staff       (20)       82 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/mlcalcdriver/__init__.py
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/mlcalcdriver/base/
--rw-r--r--   0 oliviermt  (1026) staff       (20)      143 2019-10-30 20:27:44.000000 mlcalcdriver-1.4.0/mlcalcdriver/base/__init__.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)    10343 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/mlcalcdriver/base/job.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)    26319 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/mlcalcdriver/base/posinp.py
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/
--rw-r--r--   0 oliviermt  (1026) staff       (20)      623 2022-05-12 19:20:08.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/__init__.py
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/ase_calculators/
--rw-r--r--   0 oliviermt  (1026) staff       (20)       87 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/ase_calculators/__init__.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2448 2022-05-12 19:20:08.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/ase_calculators/asespkcalculator.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2479 2020-01-17 16:07:46.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/calculator.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     4414 2021-12-10 21:34:04.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/ensemble.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     8763 2022-05-12 19:55:35.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/schnetpack.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     9012 2022-05-12 20:39:37.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/schnetpack_patch.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     1565 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/mlcalcdriver/calculators/utils.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2926 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/mlcalcdriver/globals.py
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/mlcalcdriver/interfaces/
--rw-r--r--   0 oliviermt  (1026) staff       (20)      179 2022-05-12 19:20:08.000000 mlcalcdriver-1.4.0/mlcalcdriver/interfaces/__init__.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)      966 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/mlcalcdriver/interfaces/ase_interface.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     7924 2022-05-12 21:04:38.000000 mlcalcdriver-1.4.0/mlcalcdriver/interfaces/atoms_to_patches.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     1426 2021-12-10 21:34:04.000000 mlcalcdriver-1.4.0/mlcalcdriver/interfaces/schnetpack_interface.py
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/mlcalcdriver/workflows/
--rw-r--r--   0 oliviermt  (1026) staff       (20)       87 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/mlcalcdriver/workflows/__init__.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     6073 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/mlcalcdriver/workflows/geopt.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)    10422 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/mlcalcdriver/workflows/phonon.py
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/mlcalcdriver.egg-info/
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2658 2022-05-12 21:06:26.000000 mlcalcdriver-1.4.0/mlcalcdriver.egg-info/PKG-INFO
--rw-r--r--   0 oliviermt  (1026) staff       (20)     4849 2022-05-12 21:06:26.000000 mlcalcdriver-1.4.0/mlcalcdriver.egg-info/SOURCES.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)        1 2022-05-12 21:06:26.000000 mlcalcdriver-1.4.0/mlcalcdriver.egg-info/dependency_links.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       53 2022-05-12 21:06:26.000000 mlcalcdriver-1.4.0/mlcalcdriver.egg-info/requires.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       13 2022-05-12 21:06:26.000000 mlcalcdriver-1.4.0/mlcalcdriver.egg-info/top_level.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       47 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/pytest.ini
--rw-r--r--   0 oliviermt  (1026) staff       (20)      305 2022-05-12 19:20:08.000000 mlcalcdriver-1.4.0/requirements_dev.txt
--rw-r--r--   0 oliviermt  (1026) staff       (20)       38 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/setup.cfg
--rw-r--r--   0 oliviermt  (1026) staff       (20)      785 2022-05-12 20:52:24.000000 mlcalcdriver-1.4.0/setup.py
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/tests/
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/tests/models/
--rw-r--r--   0 oliviermt  (1026) staff       (20)  1857323 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/models/H2O_forces_model
--rw-r--r--   0 oliviermt  (1026) staff       (20)  1856737 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/models/H2O_model
--rw-r--r--   0 oliviermt  (1026) staff       (20)  1856737 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/models/ani1_N2_model
--rw-r--r--   0 oliviermt  (1026) staff       (20)  1856737 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/models/myN2_model
--rw-r--r--   0 oliviermt  (1026) staff       (20)    85275 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/models/wacsf_model
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/tests/posinp_angles/
--rw-r--r--   0 oliviermt  (1026) staff       (20)       96 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_angles/gra2.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      162 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/posinp_angles/gra4_red.xyz
-drwxr-xr-x   0 oliviermt  (1026) staff       (20)        0 2022-05-12 21:06:27.000000 mlcalcdriver-1.4.0/tests/posinp_files/
--rw-r--r--   0 oliviermt  (1026) staff       (20)      143 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/tests/posinp_files/H2O_atomic.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)       82 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_files/H2O_unrelaxed.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      148 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_files/H2Orelaxed.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)       58 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_files/N2.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)       60 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_files/N2_unrelaxed.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      191 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/tests/posinp_files/additional_atom.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      334 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/tests/posinp_files/free.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      188 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/tests/posinp_files/free_reduced.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      154 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/tests/posinp_files/missing_atom.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)       83 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_files/perio1.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)       85 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_files/perio2.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      193 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_files/periodic.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)       82 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/posinp_files/reduced.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      192 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/tests/posinp_files/surface.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)      193 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/posinp_files/surface2.xyz
--rw-r--r--   0 oliviermt  (1026) staff       (20)     1657 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/test_angles.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)      990 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/test_calculators.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2182 2019-10-23 19:39:54.000000 mlcalcdriver-1.4.0/tests/test_geopt.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)      796 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/test_interface.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     1552 2019-12-09 20:12:03.000000 mlcalcdriver-1.4.0/tests/test_job.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2274 2021-06-29 17:54:07.000000 mlcalcdriver-1.4.0/tests/test_phonon.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     8277 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/test_posinp.py
--rw-r--r--   0 oliviermt  (1026) staff       (20)     2668 2022-02-09 20:52:22.000000 mlcalcdriver-1.4.0/tests/test_schnetpack.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/.github/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/.github/workflows/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1257 2023-06-16 19:07:06.000000 mlcalcdriver-1.4.1/.github/workflows/python-package.yml
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1223 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/.gitignore
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      658 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/.pep8speaks.yml
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       48 2022-01-13 18:56:41.000000 mlcalcdriver-1.4.1/.pyup.yml
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    35149 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/LICENSE
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2439 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/PKG-INFO
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2015 2023-06-16 19:07:06.000000 mlcalcdriver-1.4.1/README.md
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      230 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/.buildinfo
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/.nojekyll
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      688 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/Makefile
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4937 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/index.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    42890 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/job.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    97977 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/posinp.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/ase_calculators/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    13223 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/ase_calculators/asespkcalculator.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    12601 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/calculator.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    25087 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/ensemble.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    38307 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/schnetpack.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9195 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/ase_interface.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10219 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    24450 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/geopt.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    40427 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/phonon.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_sources/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      170 2021-12-10 20:14:37.000000 mlcalcdriver-1.4.1/docs/_sources/ase_interface.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      109 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/_sources/asespkcalc.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      136 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/base.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      120 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/calculator.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      215 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_sources/calculators.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       93 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/_sources/ensemble.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/geopt.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       54 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/globals.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      438 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/index.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      517 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_sources/interfaces.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/job.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/phonon.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/posinp.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      140 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/schnet_interface.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       95 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/schnetcalc.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      159 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/workflows.rst.txt
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_static/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14692 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/basic.css
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_static/css/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     3275 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/css/badge_only.css
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    87624 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    67312 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    86288 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    66444 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   165742 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   444379 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   165548 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    98024 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    77160 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   323344 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   193308 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   309728 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   184912 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   328412 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   195704 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   309192 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   182708 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   129674 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/css/theme.css
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9758 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/doctools.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      355 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/documentation_options.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      286 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/file.png
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   287630 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/jquery-3.5.1.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    89476 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/jquery.js
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_static/js/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      934 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/js/badge_only.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4370 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2734 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/js/html5shiv.min.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5023 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/js/theme.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10854 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/language_data.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/minus.png
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/plus.png
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4846 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/pygments.css
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16793 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/searchtools.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    68420 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/_static/underscore-1.13.1.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    19530 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/underscore.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7169 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/ase_interface.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10423 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/asespkcalc.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5341 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/base.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    11101 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/calculator.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     6388 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/calculators.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    18549 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/ensemble.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    24446 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/genindex.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14232 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/geopt.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16804 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/globals.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    12331 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/index.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5838 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/interfaces.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14803 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/job.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1441 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/objects.inv
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16522 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/phonon.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    45912 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/posinp.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7185 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/py-modindex.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9024 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/schnet_interface.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    11395 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/schnetcalc.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4034 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/search.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    15533 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/searchindex.js
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/source/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      170 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/source/ase_interface.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      109 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/source/asespkcalc.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      136 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/base.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      120 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/calculator.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      215 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/source/calculators.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2438 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/source/conf.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       93 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/source/ensemble.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/geopt.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       54 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/globals.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      438 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/index.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      517 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/source/interfaces.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/job.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/phonon.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/posinp.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      140 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/schnet_interface.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       95 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/schnetcalc.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      159 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/workflows.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5206 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/workflows.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/mlcalcdriver/__init__.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/base/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      143 2022-01-21 22:08:52.000000 mlcalcdriver-1.4.1/mlcalcdriver/base/__init__.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10343 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/base/job.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    26319 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/base/posinp.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      623 2022-04-26 18:24:40.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/__init__.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/ase_calculators/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/ase_calculators/__init__.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2448 2022-03-18 20:53:07.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/ase_calculators/asespkcalculator.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2479 2022-01-21 22:12:51.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/calculator.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4414 2022-01-21 22:13:25.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/ensemble.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     8763 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/schnetpack.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9012 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/schnetpack_patch.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1565 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/utils.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2926 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/globals.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      179 2022-04-26 18:24:40.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/__init__.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      966 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/ase_interface.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7924 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/atoms_to_patches.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1426 2021-12-10 20:14:39.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/schnetpack_interface.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/workflows/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/mlcalcdriver/workflows/__init__.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     6073 2022-01-21 22:13:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/workflows/geopt.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10422 2023-02-23 19:49:26.000000 mlcalcdriver-1.4.1/mlcalcdriver/workflows/phonon.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2439 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/PKG-INFO
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5169 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/SOURCES.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)        1 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/dependency_links.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/requires.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       13 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/top_level.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       47 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/pytest.ini
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      271 2023-06-16 19:07:06.000000 mlcalcdriver-1.4.1/requirements_dev.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       38 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/setup.cfg
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      745 2023-06-16 19:08:51.000000 mlcalcdriver-1.4.1/setup.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/tests/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/tests/models/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1857323 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/H2O_forces_model
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/H2O_model
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/ani1_N2_model
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/myN2_model
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    85275 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/wacsf_model
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/tests/posinp_angles/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       96 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_angles/gra2.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      162 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_angles/gra4_red.xyz
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/tests/posinp_files/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      143 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/H2O_atomic.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/H2O_unrelaxed.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      148 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/H2Orelaxed.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       58 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/N2.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       60 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/N2_unrelaxed.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      191 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/additional_atom.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      334 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/free.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      188 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/free_reduced.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      154 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/missing_atom.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       83 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/perio1.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       85 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/perio2.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      193 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/posinp_files/periodic.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/posinp_files/reduced.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      192 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/posinp_files/surface.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      193 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/posinp_files/surface2.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1657 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/test_angles.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      990 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/test_calculators.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2182 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/test_geopt.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      796 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/test_interface.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1552 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/test_job.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2274 2023-02-23 19:49:26.000000 mlcalcdriver-1.4.1/tests/test_phonon.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     8277 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/test_posinp.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2668 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/test_schnetpack.py
```

### Comparing `mlcalcdriver-1.4.0/.github/workflows/python-package.yml` & `mlcalcdriver-1.4.1/.github/workflows/python-package.yml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.9]
+        python-version: ["3.10"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `mlcalcdriver-1.4.0/.gitignore` & `mlcalcdriver-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/.pep8speaks.yml` & `mlcalcdriver-1.4.1/.pep8speaks.yml`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/LICENSE` & `mlcalcdriver-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/PKG-INFO` & `mlcalcdriver-1.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: mlcalcdriver
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package to drive atomic calculations using machine learned models.
 Home-page: https://github.com/OMalenfantThuot/ML_Calc_Driver
 Author: Olivier Malenfant-Thuot
 Author-email: malenfantthuotolivier@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Machine Learning Calculations Driver (ML\_Calc\_Driver)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Build Status](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver.svg?branch=master&kill_cache=1)](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver)
@@ -21,15 +20,15 @@
 [![python](https://img.shields.io/pypi/pyversions/mlcalcdriver.svg)](https://www.python.org/)
 [![PyUp](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver/shield.svg?kill_cache=1)](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver)
 
 ML\_Calc\_Driver is a driver to emulate DFT calculations using machine learned predictive models.
 To use this package, one needs an already trained model, that can predict energy or forces from an input atomic geometry.
 Supported systems depends on the model, this package should not be a limitation.
 
-This package is tested with python 3.8 and 3.9.
+This package is tested with python 3.10.
 
 Credit to [mmoriniere](https://gitlab.com/mmoriniere) for the [MyBigDFT package](https://gitlab.com/mmoriniere/MyBigDFT)
 which served as a foundation for this work. Some classes have been directly adapted from MyBigDFT.
 
 **Dependencies scanned by [PyUp.io](https://pyup.io/)**
 
 ## Documentation
@@ -48,22 +47,18 @@
 
 `pip install -U mlcalcdriver`
 
 ### From sources
 
 ```
 git clone git@github.com:OMalenfantThuot/ML_Calc_Driver.git
-cd ML_Calc_Driver
+cd ML_Calc_Driver/
+pip install -r requirements_dev.txt
 pip install .
 ```
 To modify the sources, instead of `pip install .`, use
 
 ```
-pip install -r requirements_dev.txt
 pip install -e .
 ```
 
-### To use with [SchetPack](https://github.com/atomistic-machine-learning/schnetpack) trained models (only supported models at the time)
-
-`pip install schnetpack`
-
```

### Comparing `mlcalcdriver-1.4.0/README.md` & `mlcalcdriver-1.4.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![python](https://img.shields.io/pypi/pyversions/mlcalcdriver.svg)](https://www.python.org/)
 [![PyUp](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver/shield.svg?kill_cache=1)](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver)
 
 ML\_Calc\_Driver is a driver to emulate DFT calculations using machine learned predictive models.
 To use this package, one needs an already trained model, that can predict energy or forces from an input atomic geometry.
 Supported systems depends on the model, this package should not be a limitation.
 
-This package is tested with python 3.8 and 3.9.
+This package is tested with python 3.10.
 
 Credit to [mmoriniere](https://gitlab.com/mmoriniere) for the [MyBigDFT package](https://gitlab.com/mmoriniere/MyBigDFT)
 which served as a foundation for this work. Some classes have been directly adapted from MyBigDFT.
 
 **Dependencies scanned by [PyUp.io](https://pyup.io/)**
 
 ## Documentation
@@ -34,20 +34,16 @@
 
 `pip install -U mlcalcdriver`
 
 ### From sources
 
 ```
 git clone git@github.com:OMalenfantThuot/ML_Calc_Driver.git
-cd ML_Calc_Driver
+cd ML_Calc_Driver/
+pip install -r requirements_dev.txt
 pip install .
 ```
 To modify the sources, instead of `pip install .`, use
 
 ```
-pip install -r requirements_dev.txt
 pip install -e .
 ```
-
-### To use with [SchetPack](https://github.com/atomistic-machine-learning/schnetpack) trained models (only supported models at the time)
-
-`pip install schnetpack`
```

### Comparing `mlcalcdriver-1.4.0/docs/Makefile` & `mlcalcdriver-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/index.html` & `mlcalcdriver-1.4.1/docs/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/base/job.html` & `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/job.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/base/posinp.html` & `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/posinp.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/calculators/calculator.html` & `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/calculator.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/calculators/schnetpack.html` & `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/schnetpack.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/interfaces/ase_interface.html` & `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/ase_interface.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html` & `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/workflows/geopt.html` & `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/geopt.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_modules/mlcalcdriver/workflows/phonon.html` & `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/phonon.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_sources/interfaces.rst.txt` & `mlcalcdriver-1.4.1/docs/_sources/interfaces.rst.txt`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/basic.css` & `mlcalcdriver-1.4.1/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/badge_only.css` & `mlcalcdriver-1.4.1/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.eot` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.svg` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.ttf` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.woff` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/fontawesome-webfont.woff2` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-bold-italic.woff` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-bold-italic.woff2` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-bold.woff` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-bold.woff2` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-normal-italic.woff` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-normal-italic.woff2` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-normal.woff` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/fonts/lato-normal.woff2` & `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/css/theme.css` & `mlcalcdriver-1.4.1/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/doctools.js` & `mlcalcdriver-1.4.1/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/jquery-3.5.1.js` & `mlcalcdriver-1.4.1/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/jquery.js` & `mlcalcdriver-1.4.1/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/js/badge_only.js` & `mlcalcdriver-1.4.1/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/js/html5shiv-printshiv.min.js` & `mlcalcdriver-1.4.1/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/js/html5shiv.min.js` & `mlcalcdriver-1.4.1/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/js/theme.js` & `mlcalcdriver-1.4.1/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/language_data.js` & `mlcalcdriver-1.4.1/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/pygments.css` & `mlcalcdriver-1.4.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/searchtools.js` & `mlcalcdriver-1.4.1/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/_static/underscore.js` & `mlcalcdriver-1.4.1/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/ase_interface.html` & `mlcalcdriver-1.4.1/docs/ase_interface.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/base.html` & `mlcalcdriver-1.4.1/docs/base.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/calculator.html` & `mlcalcdriver-1.4.1/docs/calculator.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/calculators.html` & `mlcalcdriver-1.4.1/docs/calculators.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/genindex.html` & `mlcalcdriver-1.4.1/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/geopt.html` & `mlcalcdriver-1.4.1/docs/geopt.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/globals.html` & `mlcalcdriver-1.4.1/docs/globals.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/index.html` & `mlcalcdriver-1.4.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/interfaces.html` & `mlcalcdriver-1.4.1/docs/interfaces.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/job.html` & `mlcalcdriver-1.4.1/docs/job.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/objects.inv` & `mlcalcdriver-1.4.1/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/phonon.html` & `mlcalcdriver-1.4.1/docs/phonon.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/posinp.html` & `mlcalcdriver-1.4.1/docs/posinp.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/py-modindex.html` & `mlcalcdriver-1.4.1/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/schnet_interface.html` & `mlcalcdriver-1.4.1/docs/schnet_interface.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/schnetcalc.html` & `mlcalcdriver-1.4.1/docs/schnetcalc.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/search.html` & `mlcalcdriver-1.4.1/docs/search.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/searchindex.js` & `mlcalcdriver-1.4.1/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/source/conf.py` & `mlcalcdriver-1.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/source/interfaces.rst` & `mlcalcdriver-1.4.1/docs/source/interfaces.rst`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/docs/workflows.html` & `mlcalcdriver-1.4.1/docs/workflows.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/base/job.py` & `mlcalcdriver-1.4.1/mlcalcdriver/base/job.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/base/posinp.py` & `mlcalcdriver-1.4.1/mlcalcdriver/base/posinp.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/calculators/__init__.py` & `mlcalcdriver-1.4.1/mlcalcdriver/calculators/__init__.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/calculators/ase_calculators/asespkcalculator.py` & `mlcalcdriver-1.4.1/mlcalcdriver/calculators/ase_calculators/asespkcalculator.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/calculators/calculator.py` & `mlcalcdriver-1.4.1/mlcalcdriver/calculators/calculator.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/calculators/ensemble.py` & `mlcalcdriver-1.4.1/mlcalcdriver/calculators/ensemble.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/calculators/schnetpack.py` & `mlcalcdriver-1.4.1/mlcalcdriver/calculators/schnetpack.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/calculators/schnetpack_patch.py` & `mlcalcdriver-1.4.1/mlcalcdriver/calculators/schnetpack_patch.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/calculators/utils.py` & `mlcalcdriver-1.4.1/mlcalcdriver/calculators/utils.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/globals.py` & `mlcalcdriver-1.4.1/mlcalcdriver/globals.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/interfaces/ase_interface.py` & `mlcalcdriver-1.4.1/mlcalcdriver/interfaces/ase_interface.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/interfaces/atoms_to_patches.py` & `mlcalcdriver-1.4.1/mlcalcdriver/interfaces/atoms_to_patches.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/interfaces/schnetpack_interface.py` & `mlcalcdriver-1.4.1/mlcalcdriver/interfaces/schnetpack_interface.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/workflows/geopt.py` & `mlcalcdriver-1.4.1/mlcalcdriver/workflows/geopt.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver/workflows/phonon.py` & `mlcalcdriver-1.4.1/mlcalcdriver/workflows/phonon.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver.egg-info/PKG-INFO` & `mlcalcdriver-1.4.1/mlcalcdriver.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: mlcalcdriver
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package to drive atomic calculations using machine learned models.
 Home-page: https://github.com/OMalenfantThuot/ML_Calc_Driver
 Author: Olivier Malenfant-Thuot
 Author-email: malenfantthuotolivier@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Machine Learning Calculations Driver (ML\_Calc\_Driver)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Build Status](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver.svg?branch=master&kill_cache=1)](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver)
@@ -21,15 +20,15 @@
 [![python](https://img.shields.io/pypi/pyversions/mlcalcdriver.svg)](https://www.python.org/)
 [![PyUp](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver/shield.svg?kill_cache=1)](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver)
 
 ML\_Calc\_Driver is a driver to emulate DFT calculations using machine learned predictive models.
 To use this package, one needs an already trained model, that can predict energy or forces from an input atomic geometry.
 Supported systems depends on the model, this package should not be a limitation.
 
-This package is tested with python 3.8 and 3.9.
+This package is tested with python 3.10.
 
 Credit to [mmoriniere](https://gitlab.com/mmoriniere) for the [MyBigDFT package](https://gitlab.com/mmoriniere/MyBigDFT)
 which served as a foundation for this work. Some classes have been directly adapted from MyBigDFT.
 
 **Dependencies scanned by [PyUp.io](https://pyup.io/)**
 
 ## Documentation
@@ -48,22 +47,18 @@
 
 `pip install -U mlcalcdriver`
 
 ### From sources
 
 ```
 git clone git@github.com:OMalenfantThuot/ML_Calc_Driver.git
-cd ML_Calc_Driver
+cd ML_Calc_Driver/
+pip install -r requirements_dev.txt
 pip install .
 ```
 To modify the sources, instead of `pip install .`, use
 
 ```
-pip install -r requirements_dev.txt
 pip install -e .
 ```
 
-### To use with [SchetPack](https://github.com/atomistic-machine-learning/schnetpack) trained models (only supported models at the time)
-
-`pip install schnetpack`
-
```

### Comparing `mlcalcdriver-1.4.0/mlcalcdriver.egg-info/SOURCES.txt` & `mlcalcdriver-1.4.1/mlcalcdriver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 requirements_dev.txt
 setup.py
 .github/workflows/python-package.yml
 docs/.buildinfo
 docs/.nojekyll
 docs/Makefile
 docs/ase_interface.html
+docs/asespkcalc.html
 docs/base.html
 docs/calculator.html
 docs/calculators.html
+docs/ensemble.html
 docs/genindex.html
 docs/geopt.html
 docs/globals.html
 docs/index.html
 docs/interfaces.html
 docs/job.html
 docs/objects.inv
@@ -29,23 +31,27 @@
 docs/search.html
 docs/searchindex.js
 docs/workflows.html
 docs/_modules/index.html
 docs/_modules/mlcalcdriver/base/job.html
 docs/_modules/mlcalcdriver/base/posinp.html
 docs/_modules/mlcalcdriver/calculators/calculator.html
+docs/_modules/mlcalcdriver/calculators/ensemble.html
 docs/_modules/mlcalcdriver/calculators/schnetpack.html
+docs/_modules/mlcalcdriver/calculators/ase_calculators/asespkcalculator.html
 docs/_modules/mlcalcdriver/interfaces/ase_interface.html
 docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html
 docs/_modules/mlcalcdriver/workflows/geopt.html
 docs/_modules/mlcalcdriver/workflows/phonon.html
 docs/_sources/ase_interface.rst.txt
+docs/_sources/asespkcalc.rst.txt
 docs/_sources/base.rst.txt
 docs/_sources/calculator.rst.txt
 docs/_sources/calculators.rst.txt
+docs/_sources/ensemble.rst.txt
 docs/_sources/geopt.rst.txt
 docs/_sources/globals.rst.txt
 docs/_sources/index.rst.txt
 docs/_sources/interfaces.rst.txt
 docs/_sources/job.rst.txt
 docs/_sources/phonon.rst.txt
 docs/_sources/posinp.rst.txt
@@ -59,14 +65,15 @@
 docs/_static/jquery-3.5.1.js
 docs/_static/jquery.js
 docs/_static/language_data.js
 docs/_static/minus.png
 docs/_static/plus.png
 docs/_static/pygments.css
 docs/_static/searchtools.js
+docs/_static/underscore-1.13.1.js
 docs/_static/underscore.js
 docs/_static/css/badge_only.css
 docs/_static/css/theme.css
 docs/_static/css/fonts/Roboto-Slab-Bold.woff
 docs/_static/css/fonts/Roboto-Slab-Bold.woff2
 docs/_static/css/fonts/Roboto-Slab-Regular.woff
 docs/_static/css/fonts/Roboto-Slab-Regular.woff2
@@ -84,18 +91,20 @@
 docs/_static/css/fonts/lato-normal.woff
 docs/_static/css/fonts/lato-normal.woff2
 docs/_static/js/badge_only.js
 docs/_static/js/html5shiv-printshiv.min.js
 docs/_static/js/html5shiv.min.js
 docs/_static/js/theme.js
 docs/source/ase_interface.rst
+docs/source/asespkcalc.rst
 docs/source/base.rst
 docs/source/calculator.rst
 docs/source/calculators.rst
 docs/source/conf.py
+docs/source/ensemble.rst
 docs/source/geopt.rst
 docs/source/globals.rst
 docs/source/index.rst
 docs/source/interfaces.rst
 docs/source/job.rst
 docs/source/phonon.rst
 docs/source/posinp.rst
```

### Comparing `mlcalcdriver-1.4.0/tests/models/H2O_forces_model` & `mlcalcdriver-1.4.1/tests/models/H2O_forces_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/models/H2O_model` & `mlcalcdriver-1.4.1/tests/models/H2O_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/models/ani1_N2_model` & `mlcalcdriver-1.4.1/tests/models/ani1_N2_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/models/myN2_model` & `mlcalcdriver-1.4.1/tests/models/myN2_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/models/wacsf_model` & `mlcalcdriver-1.4.1/tests/models/wacsf_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/test_angles.py` & `mlcalcdriver-1.4.1/tests/test_angles.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/test_calculators.py` & `mlcalcdriver-1.4.1/tests/test_calculators.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/test_geopt.py` & `mlcalcdriver-1.4.1/tests/test_geopt.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/test_interface.py` & `mlcalcdriver-1.4.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/test_job.py` & `mlcalcdriver-1.4.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/test_phonon.py` & `mlcalcdriver-1.4.1/tests/test_phonon.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/test_posinp.py` & `mlcalcdriver-1.4.1/tests/test_posinp.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.0/tests/test_schnetpack.py` & `mlcalcdriver-1.4.1/tests/test_schnetpack.py`

 * *Files identical despite different names*

