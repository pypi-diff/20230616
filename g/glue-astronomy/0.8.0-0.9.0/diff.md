# Comparing `tmp/glue-astronomy-0.8.0.tar.gz` & `tmp/glue-astronomy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-astronomy-0.8.0.tar", last modified: Thu May 11 21:54:47 2023, max compression
+gzip compressed data, was "glue-astronomy-0.9.0.tar", last modified: Thu Jun  1 14:10:43 2023, max compression
```

## Comparing `glue-astronomy-0.8.0.tar` & `glue-astronomy-0.9.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.github/workflows/update-changelog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/data_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/translators.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/spectral_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d_fullstokes.fits
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/test_spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/spectral_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/tests/test_spectral_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/translators/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/nddata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/spectrum1d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/translators/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_nddata.py
--rw-r--r--   0 runner    (1001) docker     (123)    21270 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_spectrum1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.927018 glue-astronomy-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.919018 glue-astronomy-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.919018 glue-astronomy-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-01 14:10:43.927018 glue-astronomy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.919018 glue-astronomy-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/docs/data_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/docs/translators.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/spectral_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d_fullstokes.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/test_spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/spectral_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/tests/test_spectral_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.927018 glue-astronomy-0.9.0/glue_astronomy/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/nddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/spectrum1d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.927018 glue-astronomy-0.9.0/glue_astronomy/translators/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_nddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21571 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_spectrum1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/glue_astronomy/translators/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 14:10:43.000000 glue-astronomy-0.9.0/glue_astronomy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:43.923018 glue-astronomy-0.9.0/glue_astronomy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-01 14:10:43.000000 glue-astronomy-0.9.0/glue_astronomy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-01 14:10:43.000000 glue-astronomy-0.9.0/glue_astronomy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:10:43.000000 glue-astronomy-0.9.0/glue_astronomy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-01 14:10:43.000000 glue-astronomy-0.9.0/glue_astronomy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:10:43.000000 glue-astronomy-0.9.0/glue_astronomy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 14:10:43.000000 glue-astronomy-0.9.0/glue_astronomy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 14:10:43.000000 glue-astronomy-0.9.0/glue_astronomy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-01 14:10:43.927018 glue-astronomy-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-01 14:10:27.000000 glue-astronomy-0.9.0/tox.ini
```

### Comparing `glue-astronomy-0.8.0/.github/workflows/main.yml` & `glue-astronomy-0.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/.github/workflows/update-changelog.yaml` & `glue-astronomy-0.9.0/.github/workflows/update-changelog.yaml`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/.gitignore` & `glue-astronomy-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/CHANGES.md` & `glue-astronomy-0.9.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Full changelog
 
+## v0.8.0 - 2023-05-11
+
+<!-- Release notes generated using configuration in .github/release.yml at main -->
+### What's Changed
+
+#### New Features
+
+- Added translator for `CircleAnnulusPixelRegion` by @pllim in https://github.com/glue-viz/glue-astronomy/pull/90
+
+#### Bug Fixes
+
+- Use `CircularROI.center` to avoid deprecation warnings with glue_core >= 1.10 by @dhomeier in https://github.com/glue-viz/glue-astronomy/pull/91
+
+**Full Changelog**: https://github.com/glue-viz/glue-astronomy/compare/v0.7.0...v0.8.0
+
 ## v0.7.0 - 2023-03-02
 
 <!-- Release notes generated using configuration in .github/release.yml at main -->
 ### What's Changed
 
 #### New Features
```

### Comparing `glue-astronomy-0.8.0/LICENSE` & `glue-astronomy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/PKG-INFO` & `glue-astronomy-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-astronomy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Astronomy-specific plugins for glue
 Home-page: https://github.com/glue-viz/glue-astronomy
 Author: Thomas Robitaille
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_astronomy
 Requires-Python: >=3.8
```

### Comparing `glue-astronomy-0.8.0/README.rst` & `glue-astronomy-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/RELEASE.rst` & `glue-astronomy-0.9.0/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/docs/Makefile` & `glue-astronomy-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/docs/conf.py` & `glue-astronomy-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/docs/data_loaders.rst` & `glue-astronomy-0.9.0/docs/data_loaders.rst`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/docs/translators.rst` & `glue-astronomy-0.9.0/docs/translators.rst`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/spectral_cube.py` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/spectral_cube.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.fits` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.fits`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.dat` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.dat`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.f0` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.f0`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.dat` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.dat`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.dat` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.dat`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d.fits` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d.fits`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d_fullstokes.fits` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d_fullstokes.fits`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/test_spectral_cube.py` & `glue-astronomy-0.9.0/glue_astronomy/io/spectral_cube/tests/test_spectral_cube.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/spectral_coordinates.py` & `glue-astronomy-0.9.0/glue_astronomy/spectral_coordinates.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/tests/test_spectral_coordinates.py` & `glue-astronomy-0.9.0/glue_astronomy/tests/test_spectral_coordinates.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/nddata.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/nddata.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/regions.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/regions.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from regions import (RectanglePixelRegion, PolygonPixelRegion, CirclePixelRegion,
                      PointPixelRegion, PixCoord, EllipsePixelRegion,
                      AnnulusPixelRegion, CircleAnnulusPixelRegion)
 
 __all__ = ["range_to_rect", "AstropyRegionsHandler"]
 
 GLUE_LT_1_10 = Version(glue_version) < Version('1.10')
+GLUE_LT_1_10_1 = Version(glue_version) < Version('1.10.1.dev')  # remove .dev after it is released
 
 
 def range_to_rect(data, ori, low, high):
     """
     Converts a 1D range on a 2D glue Data set into an astropy regions RectangularPixelRegion.
 
     The region covers the entirety of the data along the axis not specified by the `ori` parameter.
@@ -50,43 +51,69 @@
     ycen = 0.5 * (ymin + ymax)
     width = xmax - xmin
     height = ymax - ymin
     return RectanglePixelRegion(PixCoord(xcen, ycen), width, height)
 
 
 def _is_annulus(subset_state):
+    # There is a new way to make annulus in newer glue.
+    if not GLUE_LT_1_10_1:
+        from glue.core.roi import CircularAnnulusROI
+        res1 = (isinstance(subset_state, RoiSubsetState) and
+                isinstance(subset_state.roi, CircularAnnulusROI))
+    else:
+        res1 = False
+
     # subset_state.state1 = outer circle
     # subset_state.state2 = inner circle
     # subset_state.state2 is inverted, so we need its state1
-    return ((not isinstance(subset_state.state1, InvertState)) and
-            isinstance(subset_state.state1.roi, CircularROI) and
-            isinstance(subset_state.state2, InvertState) and
-            isinstance(subset_state.state2.state1.roi, CircularROI) and
-            (subset_state.state1.roi.xc == subset_state.state2.state1.roi.xc) and
-            (subset_state.state1.roi.yc == subset_state.state2.state1.roi.yc) and
-            (subset_state.state1.roi.radius > subset_state.state2.state1.roi.radius))
+    if not res1:
+        res2 = (hasattr(subset_state, 'state1') and
+                isinstance(subset_state.state1, RoiSubsetState) and
+                isinstance(subset_state.state1.roi, CircularROI) and
+                isinstance(subset_state.state2, InvertState) and
+                isinstance(subset_state.state2.state1, RoiSubsetState) and
+                isinstance(subset_state.state2.state1.roi, CircularROI) and
+                (subset_state.state1.roi.xc == subset_state.state2.state1.roi.xc) and
+                (subset_state.state1.roi.yc == subset_state.state2.state1.roi.yc) and
+                (subset_state.state1.roi.radius > subset_state.state2.state1.roi.radius))
+    else:
+        res2 = False
+
+    return res1 or res2
 
 
 # Put this here because there is nowhere else to put it.
 # https://github.com/glue-viz/glue/issues/2390
 def _annulus_to_subset_state(reg, data):
     """AnnulusPixelRegion to glue subset state."""
     if not isinstance(reg, AnnulusPixelRegion):  # pragma: no cover
         raise ValueError(f"{reg} is not an AnnulusPixelRegion instance")
     # TODO: Add ellipse and rectangle annulus support.
     if not isinstance(reg, CircleAnnulusPixelRegion):  # pragma: no cover
         raise NotImplementedError(f"{reg} not supported")
 
     xcen = reg.center.x
     ycen = reg.center.y
-    state1 = RoiSubsetState(data.pixel_component_ids[1], data.pixel_component_ids[0],
-                            CircularROI(xcen, ycen, reg.outer_radius))
-    state2 = RoiSubsetState(data.pixel_component_ids[1], data.pixel_component_ids[0],
-                            CircularROI(xcen, ycen, reg.inner_radius))
-    return AndState(state1, ~state2)
+
+    # There is a new way to make annulus in newer glue.
+    if not GLUE_LT_1_10_1:
+        from glue.core.roi import CircularAnnulusROI
+        sbst = RoiSubsetState(data.pixel_component_ids[1], data.pixel_component_ids[0],
+                              CircularAnnulusROI(xc=xcen, yc=ycen,
+                                                 inner_radius=reg.inner_radius,
+                                                 outer_radius=reg.outer_radius))
+    else:
+        state1 = RoiSubsetState(data.pixel_component_ids[1], data.pixel_component_ids[0],
+                                CircularROI(xcen, ycen, reg.outer_radius))
+        state2 = RoiSubsetState(data.pixel_component_ids[1], data.pixel_component_ids[0],
+                                CircularROI(xcen, ycen, reg.inner_radius))
+        sbst = AndState(state1, ~state2)
+
+    return sbst
 
 
 @subset_state_translator('astropy-regions')
 class AstropyRegionsHandler:
 
     def to_object(self, subset):
         """
@@ -136,14 +163,26 @@
                 temp_sub.subset_state = RoiSubsetState(x_pix_att, y_pix_att, roi.roi())
                 try:
                     return self.to_object(temp_sub)
                 except NotImplementedError:
                     raise NotImplementedError("ROIs of type {0} are not yet supported"
                                               .format(roi.__class__.__name__))
 
+            # There is a new way to make annulus in newer glue.
+            elif not GLUE_LT_1_10_1:
+                from glue.core.roi import CircularAnnulusROI
+                if isinstance(roi, CircularAnnulusROI):
+                    return CircleAnnulusPixelRegion(
+                        center=PixCoord(x=roi.xc, y=roi.yc),
+                        inner_radius=roi.inner_radius,
+                        outer_radius=roi.outer_radius)
+                else:
+                    raise NotImplementedError("ROIs of type {0} are not yet supported"
+                                              .format(roi.__class__.__name__))
+
             else:
                 raise NotImplementedError("ROIs of type {0} are not yet supported"
                                           .format(roi.__class__.__name__))
 
         elif isinstance(subset_state, RangeSubsetState):
             if subset_state.att == x_pix_att:
                 return range_to_rect(data, 'x', subset_state.lo, subset_state.hi)
```

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/spectral_cube.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/spectral_cube.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/spectrum1d.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/spectrum1d.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_nddata.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_nddata.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_regions.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from glue.core.subset import (RoiSubsetState, RangeSubsetState, OrState,
                               AndState, XorState, MultiOrState, MultiRangeSubsetState)
 
 from glue.viewers.image.pixel_selection_subset_state import PixelSubsetState
 from glue import __version__ as glue_version
 
-from glue_astronomy.translators.regions import _annulus_to_subset_state
+from glue_astronomy.translators.regions import _annulus_to_subset_state, GLUE_LT_1_10_1
 
 
 class TestAstropyRegions:
 
     def setup_method(self, method):
         self.data = Data(flux=np.ones((128, 256)))  # ny, nx
         self.dc = DataCollection([self.data])
@@ -307,14 +307,21 @@
         assert not reg.contains(PixCoord(5.1, 6.1))
         assert not reg.contains(PixCoord(11, 12))
 
     def test_circular_annulus(self):
         reg_orig = CircleAnnulusPixelRegion(
             center=PixCoord(x=50, y=25), inner_radius=7, outer_radius=13)
         subset_state = _annulus_to_subset_state(reg_orig, self.data)
+
+        # There is a new way to make annulus in newer glue.
+        if not GLUE_LT_1_10_1:
+            from glue.core.roi import CircularAnnulusROI
+            assert (isinstance(subset_state, RoiSubsetState) and
+                    isinstance(subset_state.roi, CircularAnnulusROI))
+
         self.dc.new_subset_group(subset_state=subset_state, label='annulus_1')
         reg = self.data.get_selection_definition(subset_id='annulus_1', format='astropy-regions')
 
         # Would round-trip if translator worked correctly.
         assert isinstance(reg, CircleAnnulusPixelRegion)
         assert reg.center.x == reg_orig.center.x
         assert reg.center.y == reg_orig.center.y
```

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_spectral_cube.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_spectral_cube.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_spectrum1d.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_spectrum1d.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_trace.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy/translators/trace.py` & `glue-astronomy-0.9.0/glue_astronomy/translators/trace.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/glue_astronomy.egg-info/PKG-INFO` & `glue-astronomy-0.9.0/glue_astronomy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-astronomy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Astronomy-specific plugins for glue
 Home-page: https://github.com/glue-viz/glue-astronomy
 Author: Thomas Robitaille
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_astronomy
 Requires-Python: >=3.8
```

### Comparing `glue-astronomy-0.8.0/glue_astronomy.egg-info/SOURCES.txt` & `glue-astronomy-0.9.0/glue_astronomy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/setup.cfg` & `glue-astronomy-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.8.0/tox.ini` & `glue-astronomy-0.9.0/tox.ini`

 * *Files identical despite different names*

