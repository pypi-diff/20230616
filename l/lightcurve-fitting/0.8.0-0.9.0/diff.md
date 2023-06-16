# Comparing `tmp/lightcurve-fitting-0.8.0.tar.gz` & `tmp/lightcurve-fitting-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcurve-fitting-0.8.0.tar", last modified: Thu Apr 27 23:06:47 2023, max compression
+gzip compressed data, was "lightcurve-fitting-0.9.0.tar", last modified: Fri Jun 16 21:42:29 2023, max compression
```

## Comparing `lightcurve-fitting-0.8.0.tar` & `lightcurve-fitting-0.9.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    35149 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/LICENSE
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      411 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/MANIFEST.in
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1177 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/PKG-INFO
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      650 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/README.md
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.798112 lightcurve-fitting-0.8.0/docs/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      673 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/docs/Makefile
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      797 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/docs/make.bat
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.802112 lightcurve-fitting-0.8.0/docs/source/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1065 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/docs/source/api.rst
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     6603 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/docs/source/conf.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1764 2023-01-27 00:13:14.000000 lightcurve-fitting-0.8.0/docs/source/index.rst
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      382 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/docs/source/installation.rst
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8437 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/docs/source/release-history.rst
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    12589 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/docs/source/usage.rst
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/lightcurve_fitting/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       93 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/__init__.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      497 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/lightcurve_fitting/_version.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    31353 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/bolometric.py
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.802112 lightcurve-fitting-0.8.0/lightcurve_fitting/example/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    41040 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/example/SN2016bkv.txt
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      570 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/ATLAS_cyan.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      570 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/ATLAS_orange.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3760 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.Y.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4565 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.g.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5036 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.i.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5017 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.r.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4937 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.z.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     7261 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GAIA_GAIA0.G.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     9420 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GALEX_GALEX.FUV.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    26420 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GALEX_GALEX.NUV.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    15466 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.H.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8800 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.J.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    17644 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.Ks.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      473 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Cousins.I.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      583 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Cousins.R.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      220 2021-11-29 19:14:50.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Johnson.B.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      260 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Johnson.U.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      300 2021-11-29 19:14:58.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Johnson.V.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     6447 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1000W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4767 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1130W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8458 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1280W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    11362 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1500W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    14404 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1800W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    20246 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F2100W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    20613 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F2550W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4329 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F560W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     6967 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F770W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3256 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F070W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4137 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F090W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5171 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F115W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     7703 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F150W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     9324 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F200W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    13773 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F277W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     7999 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F300M.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     9858 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F335M.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    15841 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F356W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     9708 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F360M.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    17399 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F444W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    22099 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/KAF-1001E.asci
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2990 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/KAF-1001E.csv
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    13083 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Kepler_Kepler.K.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5068 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2295 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1664 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1729 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/QE_E2V_MBBBUV_Broadband.csv
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1780 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.g.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1780 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.i.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1500 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.r.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      940 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.u.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2870 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.z.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3129 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.B.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2247 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.U.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3486 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVM2.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8547 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVW1.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     7623 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVW2.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3066 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.V.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     9139 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/TESS_TESS.Red.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)   276480 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/alpha_lyr_stis_008.fits
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      218 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/json2txt.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    22364 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/orange.asci
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8768 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/orange.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       72 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/pseudobolometric.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       38 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/white.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    21381 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    19574 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/fitting.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    38783 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/lightcurve.py
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/lightcurve_fitting/models/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    10653 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/models/sifto.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    37345 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/models.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      165 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/serif.mplstyle
--rwxrwxr-x   0 griffin   (1002) griffin   (1002)    23773 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/speccal.py
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.802112 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1177 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/PKG-INFO
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3795 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/SOURCES.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)        1 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/dependency_links.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       20 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/entry_points.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       65 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/requires.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       19 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/top_level.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      122 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/requirements.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      200 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/setup.cfg
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2183 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/setup.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    68611 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/versioneer.py
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-06-16 21:42:29.481022 lightcurve-fitting-0.9.0/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    35149 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/LICENSE
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      411 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/MANIFEST.in
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1177 2023-06-16 21:42:29.481022 lightcurve-fitting-0.9.0/PKG-INFO
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      650 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/README.md
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-06-16 21:42:29.473022 lightcurve-fitting-0.9.0/docs/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      673 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/docs/Makefile
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      797 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/docs/make.bat
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-06-16 21:42:29.473022 lightcurve-fitting-0.9.0/docs/source/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1065 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/docs/source/api.rst
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     6603 2023-06-14 18:20:48.000000 lightcurve-fitting-0.9.0/docs/source/conf.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2075 2023-06-16 21:40:39.000000 lightcurve-fitting-0.9.0/docs/source/index.rst
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      382 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/docs/source/installation.rst
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9039 2023-06-16 21:40:39.000000 lightcurve-fitting-0.9.0/docs/source/release-history.rst
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    12859 2023-06-16 21:40:39.000000 lightcurve-fitting-0.9.0/docs/source/usage.rst
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-06-16 21:42:29.481022 lightcurve-fitting-0.9.0/lightcurve_fitting/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       93 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/__init__.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      497 2023-06-16 21:42:29.481022 lightcurve-fitting-0.9.0/lightcurve_fitting/_version.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    31353 2023-04-27 23:03:45.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/bolometric.py
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-06-16 21:42:29.473022 lightcurve-fitting-0.9.0/lightcurve_fitting/example/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    41040 2023-04-27 23:03:45.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/example/SN2016bkv.txt
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-06-16 21:42:29.481022 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      570 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/ATLAS_cyan.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      570 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/ATLAS_orange.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3760 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.Y.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4565 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.g.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     5036 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.i.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     5017 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.r.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4937 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.z.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     7261 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/GAIA_GAIA0.G.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9420 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/GALEX_GALEX.FUV.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    26420 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/GALEX_GALEX.NUV.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    15466 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Gemini_Flamingos2.H.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8800 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Gemini_Flamingos2.J.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    17644 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Gemini_Flamingos2.Ks.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      473 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Generic_Cousins.I.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      583 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Generic_Cousins.R.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      220 2021-11-29 19:14:50.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Generic_Johnson.B.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      260 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Generic_Johnson.U.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      300 2021-11-29 19:14:58.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Generic_Johnson.V.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     6447 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1000W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4767 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1130W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8458 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1280W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    11362 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1500W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    14404 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1800W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    20246 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F2100W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    20613 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F2550W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4329 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F560W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     6967 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F770W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3256 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F070W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4137 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F090W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     5171 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F115W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     7703 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F150W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9324 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F200W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    13773 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F277W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     7999 2023-04-27 23:03:45.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F300M.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9858 2023-04-27 23:03:45.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F335M.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    15841 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F356W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9708 2023-04-27 23:03:45.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F360M.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    17399 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F444W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    22099 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/KAF-1001E.asci
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2990 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/KAF-1001E.csv
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    13083 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Kepler_Kepler.K.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     5068 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2295 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1664 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1729 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/QE_E2V_MBBBUV_Broadband.csv
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1780 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.g.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1780 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.i.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1500 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.r.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      940 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.u.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2870 2022-03-18 17:02:27.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.z.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3129 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.B.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2247 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.U.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3486 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.UVM2.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8547 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.UVW1.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     7623 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.UVW2.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3066 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.V.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9139 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/TESS_TESS.Red.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)   276480 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/alpha_lyr_stis_008.fits
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      218 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/json2txt.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    22364 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/orange.asci
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8768 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/orange.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       72 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/pseudobolometric.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       38 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters/white.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    21405 2023-06-16 21:40:39.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/filters.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    20464 2023-06-16 21:40:39.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/fitting.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    40269 2023-06-16 21:40:39.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/lightcurve.py
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-06-16 21:42:29.481022 lightcurve-fitting-0.9.0/lightcurve_fitting/models/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    10653 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/models/sifto.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    43843 2023-06-16 21:40:39.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/models.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      165 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/serif.mplstyle
+-rwxrwxr-x   0 griffin   (1002) griffin   (1002)    23773 2023-04-27 23:03:45.000000 lightcurve-fitting-0.9.0/lightcurve_fitting/speccal.py
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-06-16 21:42:29.473022 lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1177 2023-06-16 21:42:29.000000 lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/PKG-INFO
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3795 2023-06-16 21:42:29.000000 lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/SOURCES.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)        1 2023-06-16 21:42:29.000000 lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/dependency_links.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       20 2023-06-16 21:42:29.000000 lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/entry_points.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       65 2023-06-16 21:42:29.000000 lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/requires.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       19 2023-06-16 21:42:29.000000 lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/top_level.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      122 2023-04-27 23:03:45.000000 lightcurve-fitting-0.9.0/requirements.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      200 2023-06-16 21:42:29.481022 lightcurve-fitting-0.9.0/setup.cfg
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2183 2022-10-25 19:41:42.000000 lightcurve-fitting-0.9.0/setup.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    68611 2021-09-29 18:54:17.000000 lightcurve-fitting-0.9.0/versioneer.py
```

### Comparing `lightcurve-fitting-0.8.0/LICENSE` & `lightcurve-fitting-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/PKG-INFO` & `lightcurve-fitting-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurve-fitting
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools to fit analytical models to multiband light curves of astronomical transients
 Home-page: https://github.com/griffin-h/lightcurve_fitting
 Author: Griffin Hosseinzadeh
 Author-email: griffin0@arizona.edu
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lightcurve-fitting-0.8.0/README.md` & `lightcurve-fitting-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/docs/Makefile` & `lightcurve-fitting-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/docs/make.bat` & `lightcurve-fitting-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/docs/source/api.rst` & `lightcurve-fitting-0.9.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/docs/source/conf.py` & `lightcurve-fitting-0.9.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'Light Curve Fitting'
-copyright = '2022, Griffin Hosseinzadeh'
+copyright = '2023, Griffin Hosseinzadeh'
 author = 'Griffin Hosseinzadeh'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 import lightcurve_fitting
```

### Comparing `lightcurve-fitting-0.8.0/docs/source/index.rst` & `lightcurve-fitting-0.9.0/docs/source/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -24,10 +24,13 @@
 References
 ----------
 .. [C08] Conley et al. 2008, ApJ, 681, 482, doi:`10.1086/588518 <https://doi.org/10.1086/588518>`_
 .. [H17] Hosseinzadeh et al. 2017, ApJL, 845, L11, doi:`10.3847/2041-8213/aa8402 <https://doi.org/10.3847/2041-8213/aa8402>`_
 .. [H18] Hosseinzadeh et al. 2018, ApJ, 861, 63, doi:`10.3847/1538-4357/aac5f6 <https://doi.org/10.3847/1538-4357/aac5f6>`_
 .. [H22a] Hosseinzadeh et al. 2022a, ApJL, 933, L45, doi:`10.3847/2041-8213/ac7cef <https://doi.org/10.3847/2041-8213/ac7cef>`_
 .. [H22b] Hosseinzadeh et al. 2022b, ApJ, 935, 31, doi:`10.3847/1538-4357/ac75f0 <https://doi.org/10.3847/1538-4357/ac75f0>`_
+.. [H23a] Hosseinzadeh et al. 2023a, arXiv:`2305.03071 <https://arxiv.org/abs/2305.03071>`_
+.. [H23b] Hosseinzadeh et al. 2023b, arXiv:`2306.06097 <https://arxiv.org/abs/2306.06097>`_
 .. [K10] Kasen 2010, ApJ, 708, 1025, doi:`10.1088/0004-637X/708/2/1025 <https://doi.org/10.1088/0004-637X/708/2/1025>`_
 .. [RW11] Rabinak & Waxman 2011, ApJ, 728, 63, doi:`10.1088/0004-637X/728/1/63 <https://doi.org/10.1088/0004-637X/728/1/63>`_
 .. [SW17] Sapir & Waxman 2017, ApJ, 838, 130, doi:`10.3847/1538-4357/aa64df <https://doi.org/10.3847/1538-4357/aa64df>`_
+.. [MSW23] Morag, Sapir, & Waxman 2023, MNRAS, 522, 2764, doi:`10.1093/mnras/stad899 <https://doi.org/10.1093/mnras/stad899>`_
```

### Comparing `lightcurve-fitting-0.8.0/docs/source/release-history.rst` & `lightcurve-fitting-0.9.0/docs/source/release-history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 ===============
 Release History
 ===============
 
+v0.9.0 (2023-06-16)
+-------------------
+* Add :class:`.ShockCooling4` model from [MSW23]_
+* Add ``filters_to_model`` option to :func:`.lightcurve_corner` and :func:`.lightcurve_model_plot`
+* Propagate ``t0_offset`` option from :func:`.lightcurve_corner` to ``mjd_offset`` option of :func:`.lightcurve_model_plot`
+* Recognize filters RGB, LRGB, and z_s
+* Assume an empty/masked value for filter means "unfiltered"
+* Use colors in marker legend if ``color`` = ``marker`` in :meth:`.LC.plot`
+* Add option to plot phase in hours in :meth:`.LC.plot`
+* Add option to return axes objects in :meth:`.LC.plot`
+
 v0.8.0 (2023-04-27)
 -------------------
 This release includes a major refactor of the :mod:`models` module. Models now require initialization with the :class:`.LC` object to be fit. Updated examples are given in the documentation and the Jupyter notebook. This alleviates the need for model keyword arguments, which are now deprecated. (A warning will be issued if the user tries to supply a ``model_kwargs`` argument.) This also allows for much easier specification of new models by subclassing the existing models.
 
 * Add :class:`.CompanionShocking3` model, which includes viewing angle dependence
 * Added :meth:`.BaseCompanionShocking.t_min` and :meth:`.BaseCompanionShocking.t_max` to indicate when the SiFTO model is computed
 * Require Astropy version 5 (there were already features that required this)
```

### Comparing `lightcurve-fitting-0.8.0/docs/source/usage.rst` & `lightcurve-fitting-0.9.0/docs/source/usage.rst`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 The following column names are used by the package, although the light curve can have extra columns
 [alternative column names are given in square brackets]:
 
  * MJD (required): modified Julian date of the observation [mjd, JD, jd (JD/jd are converted)]
  * mag (required): magnitude of the observation [Magnitude, Mag, ab_mag, PSFmag, MAG, omag, magnitude, apparent_mag]
  * dmag (required): uncertainty on the magnitude [Magnitude_Error, magerr, MagErr, mag_err, e_mag, Error, err, PSFerr,
-   MAGERR, e_omag, e_magnitude, apparent_mag_err, Mag_Err, emag]
+   MAGERR, e_omag, e_magnitude, apparent_mag_err, Mag_Err, emag, error]
  * filter (required): name of the filter [filter, filt Filter, band, FLT, Band] (see :ref:`Filters` below)
  * nondet: True if the magnitude is an upper limit, False otherwise [Is_Limit, UL, l_omag, upper_limit, upperlimit]
  * flux: the spectral flux density (:math:`F_ν`, arbitrary units) of the observation [FLUXCAL]
  * dflux: uncertainty on the flux [FLUXCALERR]
  * phase: time since a reference date (e.g., peak or explosion) in rest-frame days [Phase, PHASE]
  * absmag: absolute magnitude of the observation
  * lum: the spectral luminosity density (:math:`L_ν`, in watts/hertz) of the observation
@@ -137,26 +137,30 @@
     \sigma_{i,\mathrm{eff}} = \sqrt{ \sigma_i^2 + \left( \sigma * \bar{\sigma} \right)^2 }
 
 For bolometric light curve fitting, you can also set a maximum for this intrinsic scatter using the ``sigma_max`` keyword (default: 10). (For model fitting, you can set a maximum using the ``priors`` keyword.)
 
 Model Fitting
 -------------
 The :mod:`.models` and :mod:`.fitting` submodules allow you to fit analytical models to the observed data.
-Right now, there are two classes of models: :class:`.BaseCompanionShocking`, which is the SiFTO Type Ia supernova template [C08]_ plus a shock component from [K10]_, and :class:`.BaseShockCooling`, which is the [SW17]_ model for shock cooling in a core-collapse supernova.
+Right now, there are three classes of models: :class:`.BaseCompanionShocking`, which is the SiFTO Type Ia supernova template [C08]_ plus a shock component from [K10]_; :class:`.BaseShockCooling`, which is the [SW17]_ model for shock cooling in a core-collapse supernova; and :class:`.ShockCooling4`, which is the updated shock cooling model of [MSW23]_.
 The variations on these classes are as follows:
 
  * :class:`.CompanionShocking` uses factors on the r and i SiFTO models and a factor on the U shock component.
    This was used in my paper on SN 2017cbv [H17]_.
  * :class:`.CompanionShocking2` uses time offsets for the U and i SiFTO models.
    This was used in my paper on SN 2021aefx [H22a]_.
  * :class:`.CompanionShocking3` is the same as :class:`.CompanionShocking2` but includes viewing angle dependence.
+   This was used in my paper on SN 2023bee [H23a]_.
  * :class:`.ShockCooling` is formulated in terms of physical parameters :math:`v_s, M_\mathrm{env}, f_ρ M, R`.
  * :class:`.ShockCooling2` is formulated in terms of scaling parameters :math:`T_1, L_1, t_\mathrm{tr}`.
    This was used in my paper on SN 2016bkv [H18]_.
- * :class:`.ShockCooling3` is the same as :class:`.ShockCooling` but with :math:`d_L` and :math:`E(B-V)` as free parameters. (Therefore it fits the flux instead of the luminosity.) This was used in my paper on SN 2021yja [H22b]_.
+ * :class:`.ShockCooling3` is the same as :class:`.ShockCooling` but with :math:`d_L` and :math:`E(B-V)` as free parameters. (Therefore it fits the flux instead of the luminosity.)
+   This was used in my paper on SN 2021yja [H22b]_.
+ * :class:`.ShockCooling4` is the updated shock cooling model of [MSW23]_.
+   This was used in my paper on SN 2023ixf [H23b]_.
 
 **Note on the shock cooling models:**
 There are degeneracies between many of the physical parameters that make them difficult to fit independently.
 This led us to fit develop the :data:`.ShockCooling2` model just to see if the model could fit the data at all.
 Since it did not fit well, we concluded that the physical parameters we could have obtained by fitting the :data:`.ShockCooling` model were irrelevant.
 However, in order to measure, for example, the progenitor radius, one must use the :data:`.ShockCooling` model.
```

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/bolometric.py` & `lightcurve-fitting-0.9.0/lightcurve_fitting/bolometric.py`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/example/SN2016bkv.txt` & `lightcurve-fitting-0.9.0/lightcurve_fitting/example/SN2016bkv.txt`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/ATLAS_cyan.txt` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/ATLAS_cyan.txt`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/ATLAS_orange.txt` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/ATLAS_orange.txt`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.Y.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.Y.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.g.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.g.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.i.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.i.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.r.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.r.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.z.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/CTIO_DECam.z.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GAIA_GAIA0.G.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/GAIA_GAIA0.G.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GALEX_GALEX.FUV.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/GALEX_GALEX.FUV.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GALEX_GALEX.NUV.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/GALEX_GALEX.NUV.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.H.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Gemini_Flamingos2.H.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.J.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Gemini_Flamingos2.J.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.Ks.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Gemini_Flamingos2.Ks.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Cousins.R.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Generic_Cousins.R.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1000W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1000W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1130W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1130W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1280W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1280W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1500W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1500W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1800W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F1800W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F2100W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F2100W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F2550W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F2550W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F560W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F560W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F770W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_MIRI.F770W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F070W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F070W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F090W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F090W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F115W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F115W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F150W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F150W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F200W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F200W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F277W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F277W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F300M.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F300M.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F335M.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F335M.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F356W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F356W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F360M.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F360M.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F444W.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/JWST_NIRCam.F444W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/KAF-1001E.asci` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/KAF-1001E.asci`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/KAF-1001E.csv` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/KAF-1001E.csv`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Kepler_Kepler.K.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Kepler_Kepler.K.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/QE_E2V_MBBBUV_Broadband.csv` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/QE_E2V_MBBBUV_Broadband.csv`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.g.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.g.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.i.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.i.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.r.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.r.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.u.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.u.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.z.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/SLOAN_SDSS.z.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.B.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.B.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.U.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.U.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVM2.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.UVM2.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVW1.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.UVW1.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVW2.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.UVW2.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.V.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/Swift_UVOT.V.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/TESS_TESS.Red.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/TESS_TESS.Red.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/alpha_lyr_stis_008.fits` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/alpha_lyr_stis_008.fits`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/orange.asci` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/orange.asci`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/orange.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters/orange.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/filters.py` & `lightcurve-fitting-0.9.0/lightcurve_fitting/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,29 +380,29 @@
     Filter(['g', "g'", 'gp', 'gprime', 'F475W'], '#00CCFF', 1, 'Gunn', filename='SLOAN_SDSS.g.dat', angstrom=True),
     Filter('g-DECam', '#00CCFF', 1, 'DECam', filename='CTIO_DECam.g.dat', angstrom=True),
     Filter(['c', 'cyan'], 'c', 1, 'ATLAS', filename='ATLAS_cyan.txt'),
     Filter('V', '#79FF00', 1, 'Johnson', 3.636e-23, filename='Generic_Johnson.V.dat', angstrom=True, mec='k', textcolor='#46CC00'),
     Filter(['V_S', 'v', 'vs'], '#00FF30', 1, 'Swift', 3.664e-23, filename='Swift_UVOT.V.dat', angstrom=True),
     Filter('Itagaki', 'w', 0, 'Itagaki', filename='KAF-1001E.asci', linecolor='k', italics=False),
     Filter('white', 'w', 0, 'MOSFiT', filename='white.txt', linecolor='k', italics=False),
-    Filter(['unfilt.', '0', 'C', 'clear', 'pseudobolometric', 'griz'], 'w', 0, 'MOSFiT',
+    Filter(['unfilt.', '0', 'C', 'clear', 'pseudobolometric', 'griz', 'RGB', 'LGRB'], 'w', 0, 'MOSFiT',
            filename='pseudobolometric.txt', linecolor='k', italics=False),
     Filter('G', 'w', 0, 'Gaia', filename='GAIA_GAIA0.G.dat', angstrom=True, linecolor='k'),
     Filter('Kepler', 'r', 0, 'Kepler', filename='Kepler_Kepler.K.dat', angstrom=True, italics=False),
     Filter('TESS', 'r', 0, 'TESS', filename='TESS_TESS.Red.dat', angstrom=True, italics=False),
     Filter(['DLT40', 'Open', 'Clear'], 'w', 0, 'DLT40', filename='QE_E2V_MBBBUV_Broadband.csv', linecolor='k', italics=False),
     Filter('w', 'w', 0, 'Gunn', filename='PAN-STARRS_PS1.w.dat', angstrom=True, linecolor='k'),
     Filter(['o', 'orange'], 'orange', 0, 'ATLAS', filename='ATLAS_orange.txt'),
     Filter(['r', "r'", 'rp', 'rprime', 'F625W'], '#FF7D00', 0, 'Gunn', filename='SLOAN_SDSS.r.dat', angstrom=True),
     Filter('r-DECam', '#FF7D00', 0, 'DECam', filename='CTIO_DECam.r.dat', angstrom=True),
     Filter(['R', 'Rc', 'R_s'], '#FF7000', 0, 'Johnson', 3.064e-23, filename='Generic_Cousins.R.dat', mec='k', angstrom=True),  # '#CC5900'
     Filter(['i', "i'", 'ip', 'iprime', 'F775W'], '#90002C', -1, 'Gunn', filename='SLOAN_SDSS.i.dat', angstrom=True),
     Filter('i-DECam', '#90002C', -1, 'DECam', filename='CTIO_DECam.i.dat', angstrom=True),
     Filter(['I', 'Ic'], '#66000B', -1, 'Johnson', 2.416e-23, filename='Generic_Cousins.I.dat', mec='k', angstrom=True),  # brightened from '#1C0003'
-    Filter('zs', '#000000', -2, 'Gunn', filename='PAN-STARRS_PS1.z.dat', angstrom=True),
+    Filter(['z_s', 'zs'], '#000000', -2, 'Gunn', filename='PAN-STARRS_PS1.z.dat', angstrom=True),
     Filter(['z', "z'", 'zp', 'zprime'], '#000000', -2, 'Gunn', filename='SLOAN_SDSS.z.dat', angstrom=True),
     Filter('z-DECam', '#000000', -2, 'DECam', filename='CTIO_DECam.z.dat', angstrom=True),
     Filter('y', 'y', -3, 'Gunn', filename='PAN-STARRS_PS1.y.dat', angstrom=True),
     Filter('y-DECam', 'y', -3, 'DECam', filename='CTIO_DECam.Y.dat', angstrom=True),
     Filter('J', '#444444', -2, 'UKIRT', 1.589e-23, filename='Gemini_Flamingos2.J.dat', angstrom=True),
     Filter('H', '#888888', -3, 'UKIRT', 1.021e-23, filename='Gemini_Flamingos2.H.dat', angstrom=True),
     Filter(['K', 'Ks'], '#CCCCCC', -4, 'UKIRT', 0.640e-23, filename='Gemini_Flamingos2.Ks.dat', angstrom=True),
```

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/fitting.py` & `lightcurve-fitting-0.9.0/lightcurve_fitting/fitting.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,15 +167,16 @@
 
     return sampler
 
 
 def lightcurve_corner(lc, model, sampler_flatchain, model_kwargs=None,
                       num_models_to_plot=100, lcaxis_posn=(0.7, 0.55, 0.2, 0.4),
                       filter_spacing=1., tmin=None, tmax=None, t0_offset=None, save_plot_as='', ycol=None,
-                      textsize='medium', param_textsize='large', use_sigma=False, xscale='linear'):
+                      textsize='medium', param_textsize='large', use_sigma=False, xscale='linear',
+                      filters_to_model=None):
     """
     Plot the posterior distributions in a corner (pair) plot, with an inset showing the observed and model light curves.
 
     Parameters
     ----------
     lc : lightcurve_fitting.lightcurve.LC
         Table of broadband photometry including columns "MJD", "mag", "dmag", "filter"
@@ -192,28 +193,30 @@
     filter_spacing : float, optional
         Spacing between filters in the light curve inset, in units determined by the order of magnitude of the
         luminosities. Default: 1.
     tmin, tmax : float, optional
         Starting and ending times for which to plot the models in the light curve inset. Default: determined by the
         time range of the observed light curve.
     t0_offset : float, optional
-        Reference time for the explosion time in the corner plot. Default: the earliest explosion time in
-        `sampler_flatchain`, rounded down.
+        Reference time for the explosion time in the corner plot and the horizontal axis of the light curve inset.
+         Default: the earliest explosion time in `sampler_flatchain`, rounded down.
     save_plot_as : str, optional
         Filename to which to save the resulting plot
     ycol : str, optional
         Quantity to plot on the light curve inset. Choices: "lum", "flux", or "absmag". Default: model.output_quantity
     textsize : str, optional
         Font size for the x- and y-axis labels, as well as the tick labels. Default: 'medium'
     param_textsize : str, optional
         Font size for the parameter text. Default: 'large'
     use_sigma : bool, optional
         If True, treat the last parameter as an intrinsic scatter parameter that does not get passed to the model
     xscale : str, optional
         Scale for the x-axis of the model plot. Choices: "linear" (default) or "log".
+    filters_to_model : list, set, optional
+        (Unique) list of filters for which to calculate the model light curves. Default: all filters in `lc`.
 
     Returns
     -------
     fig : matplotlib.pyplot.Figure
         Figure object containing the plot
     corner_ax : array-like
         Array of matplotlib.pyplot.Axes objects corresponding to the corner plot
@@ -221,27 +224,29 @@
         Axes object for the light curve inset
     """
     if model_kwargs is not None:
         raise Exception(MODEL_KWARGS_WARNING)
     if ycol is None:
         ycol = model.output_quantity
     plt.style.use(resource_filename('lightcurve_fitting', 'serif.mplstyle'))
+    if use_sigma and model.input_names[-1] != '\\sigma':
+        model.input_names.append('\\sigma')
+        model.units.append(u.dimensionless_unscaled)
 
     sampler_flatchain_corner = sampler_flatchain.copy()
     axis_labels_corner = model.axis_labels
     for var in ['t_0', 't_\\mathrm{max}']:
         if var in model.input_names:
             i_t0 = model.input_names.index(var)
             if t0_offset is None:
-                mjd_offset = np.floor(sampler_flatchain_corner[:, i_t0].min())
-            else:
-                mjd_offset = t0_offset
-            if mjd_offset != 0.:
-                sampler_flatchain_corner[:, i_t0] -= mjd_offset
-                axis_labels_corner[i_t0] = f'${var} - {mjd_offset:.0f}$ (d)'
+                t0_offset = np.floor(sampler_flatchain_corner[:, i_t0].min())
+            if t0_offset != 0.:
+                sampler_flatchain_corner[:, i_t0] -= t0_offset
+                t0_offset_formatted = '{:f}'.format(t0_offset).rstrip('0').rstrip('.')
+                axis_labels_corner[i_t0] = f'${var} - {t0_offset_formatted}$ (d)'
 
     fig = corner.corner(sampler_flatchain_corner, labels=axis_labels_corner, label_kwargs={'size': textsize})
     corner_axes = np.array(fig.get_axes()).reshape(sampler_flatchain.shape[-1], sampler_flatchain.shape[-1])
     for i in range(sampler_flatchain.shape[-1]):
         corner_axes[i, 0].tick_params(labelsize=textsize)
         corner_axes[-1, i].tick_params(labelsize=textsize)
 
@@ -250,28 +255,28 @@
         ax.spines['left'].set_visible(False)
         ax.spines['right'].set_visible(False)
         ax.xaxis.set_ticks_position('bottom')
         ax.yaxis.set_ticks_position('none')
 
     ax = fig.add_axes(lcaxis_posn)
     lightcurve_model_plot(lc, model, sampler_flatchain, model_kwargs, num_models_to_plot, filter_spacing,
-                          tmin, tmax, ycol, textsize, ax, use_sigma=use_sigma, xscale=xscale)
+                          tmin, tmax, ycol, textsize, ax, t0_offset, use_sigma, xscale, filters_to_model)
 
     paramtexts = format_credible_interval(sampler_flatchain, varnames=model.input_names, units=model.units)
     fig.text(0.45, 0.95, '\n'.join(paramtexts), va='top', ha='center', fontdict={'size': param_textsize})
     if save_plot_as:
         fig.savefig(save_plot_as)
         print('saving figure as ' + save_plot_as)
 
     return fig, corner_axes, ax
 
 
 def lightcurve_model_plot(lc, model, sampler_flatchain, model_kwargs=None, num_models_to_plot=100, filter_spacing=1.,
                           tmin=None, tmax=None, ycol=None, textsize='medium', ax=None, mjd_offset=None, use_sigma=False,
-                          xscale='linear'):
+                          xscale='linear', filters_to_model=None):
     """
     Plot the observed and model light curves.
 
     Parameters
     ----------
     lc : lightcurve_fitting.lightcurve.LC
         Table of broadband photometry including columns "MJD", "mag", "dmag", "filter"
@@ -298,31 +303,39 @@
     mjd_offset : float, optional
         Reference time on the horizontal axis of the light curve inset. Default: determined by the starting time of
         the model light curve.
     use_sigma : bool, optional
         If True, treat the last parameter as an intrinsic scatter parameter that does not get passed to the model
     xscale : str, optional
         Scale for the x-axis. Choices: "linear" (default) or "log".
+    filters_to_model : list, set, optional
+        (Unique) list of filters for which to calculate the model light curves. Default: all filters in `lc`.
     """
     if model_kwargs is not None:
         raise Exception(MODEL_KWARGS_WARNING)
     if ycol is None:
         ycol = model.output_quantity
     if ax is None:
         ax = plt.axes()
+    if use_sigma and model.input_names[-1] != '\\sigma':
+        model.input_names.append('\\sigma')
+        model.units.append(u.dimensionless_unscaled)
 
     choices = np.random.choice(sampler_flatchain.shape[0], num_models_to_plot)
     ps = sampler_flatchain[choices].T
 
     if tmin is None:
         tmin = np.min(lc['MJD'])
     if tmax is None:
         tmax = np.max(lc['MJD'])
     xfit = np.geomspace(tmin, tmax, 1000) if xscale == 'log' else np.linspace(tmin, tmax, 1000)
-    ufilts = np.unique(lc['filter'])
+    if filters_to_model is None:
+        ufilts = np.unique(lc['filter'])
+    else:
+        ufilts = np.array([filtdict[f] for f in filters_to_model])
     if use_sigma:
         y_fit = model(xfit, ufilts, *ps[:-1])
     else:
         y_fit = model(xfit, ufilts, *ps)
 
     # for CompanionShocking, add SiFTO model as dashed lines
     if isinstance(model, CompanionShocking):
```

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/lightcurve.py` & `lightcurve-fitting-0.9.0/lightcurve_fitting/lightcurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from matplotlib.path import Path
 from astropy.table import Table, vstack, MaskedColumn
 from astropy.cosmology import Planck18
 from .filters import filtdict
 import itertools
 from matplotlib.markers import MarkerStyle
 from matplotlib.patches import Patch
+from functools import partial
 try:
     from config import markers
 except ModuleNotFoundError:
     markers = {}
 
 
 class Arrow(Path):
@@ -39,15 +40,15 @@
 column_names = {
     'Filter': ['filter', 'filt', 'Filter', 'band', 'FLT', 'Band'],
     'Telescope': ['telescope', 'Telescope', 'Tel', 'tel+inst'],
     'Source': ['source', 'Source'],
     'Apparent Magnitude': ['mag', 'Magnitude', 'Mag', 'ab_mag', 'PSFmag', 'MAG', 'omag', 'magnitude', 'apparent_mag'],
     'Apparent Magnitude Uncertainty': [
         'dmag', 'Magnitude_Error', 'magerr', 'MagErr', 'mag_err', 'e_mag', 'Error', 'err', 'PSFerr', 'MAGERR', 'e_omag',
-        'e_magnitude', 'apparent_mag_err', 'Mag_Err', 'emag',
+        'e_magnitude', 'apparent_mag_err', 'Mag_Err', 'emag', 'error',
     ],
     'MJD': ['MJD', 'mjd'],
     'JD': ['JD', 'jd'],
     'Phase (rest days)': ['phase', 'Phase', 'PHASE'],
     'Flux $F_ν$ (W m$^{-2}$ Hz$^{-1}$)': ['flux', 'FLUXCAL'],
     'Flux Uncertainty': ['dflux', 'FLUXCALERR'],
     'Nondetection': ['nondet', 'Is_Limit', 'UL', 'l_omag', 'upper_limit', 'upperlimit'],
@@ -75,14 +76,15 @@
         Table.__init__(self, *args, **kwargs)
         self.normalize_column_names()
         if 'filter' in self.colnames and self['filter'].dtype != object:
             self.filters_to_objects()
         self.nondetSigmas = 3.
         self.groupby = {'filter', 'source'}
         self.markers = markers.copy()
+        self.colors = {}
 
     def where(self, **kwargs):
         """
         Select the subset of a light curve matching some criteria, given as keyword arguments, e.g., ``colname=value``.
 
         The keyword ``colname`` can be any of the following:
           * a column in the table, in which case rows must match ``value`` in that column
@@ -151,15 +153,15 @@
             nondet = (self['nondet'] == 'True') | (self['nondet'] == 'T') | (self['nondet'] == '>')
             self.replace_column('nondet', nondet)
 
     def filters_to_objects(self):
         """
         Parse the ``'filter'`` column into :class:`filters.Filter` objects
         """
-        filters = np.array([filtdict['?'] if np.ma.is_masked(f) or str(f) not in filtdict else filtdict[str(f)]
+        filters = np.array([filtdict['0'] if np.ma.is_masked(f) else filtdict.get(str(f), filtdict['?'])
                             for f in self['filter']])
         is_swift = np.zeros(len(self), bool)
         if 'telescope' in self.colnames:
             is_swift |= self['telescope'] == 'Swift'
             is_swift |= self['telescope'] == 'UVOT'
             is_swift |= self['telescope'] == 'Swift/UVOT'
             is_swift |= self['telescope'] == 'Swift+UVOT'
@@ -403,15 +405,15 @@
             if 'dphase0' in self.colnames:
                 self['dphase0'] *= 24.
             if 'dphase1' in self.colnames:
                 self['dphase1'] *= 24.
 
     def plot(self, xcol='phase', ycol='absmag', offset_factor=1., color='filter', marker=None, use_lines=False,
              normalize=False, fillmark=True, mjd_axis=True, appmag_axis=True, loc_mark=None, loc_filt=None, ncol_mark=1,
-             lgd_filters=None, tight_layout=True, **kwargs):
+             lgd_filters=None, tight_layout=True, phase_hours=False, return_axes=False, **kwargs):
         """
         Plot the light curve, with nondetections marked with a downward-pointing arrow
 
         Parameters
         ----------
         xcol : str, optional
             Column to plot on the horizontal axis. Default: ``'phase'``
@@ -442,17 +444,28 @@
             Number of columns in the marker legend. Default: 1.
         lgd_filters : list, array-like, optional
             Customize the arrangement of filters in the legend by providing a list of filters for each column. ``None``
             can be used to leave a blank space in the column. Only filters given here will be used. The default
             arrangement shows all filters arranged by ``.system`` (columns) and ``.offset`` (rows).
         tight_layout : bool, optional
             Adjust the figure margins to look beautiful. Default: True.
+        phase_hours : bool, optional
+            Plot the phase in units of rest-frame hours instead of rest-frame days. Default: False.
+        return_axes : bool, optional
+            Return the newly created axes if ``mjd_axis=True`` or ``appmag_axis=True``. Default: False.
         kwargs
             Keyword arguments matching column names in the light curve are used to specify a subset of points to plot.
             Additional keyword arguments passed to :func:`matplotlib.pyplot.plot`.
+
+        Returns
+        -------
+        top : matplotlib.pyplot.Axes, optional
+            The upper x-axis, if ``mjd_axis=True`` and ``return_axes=True``. Otherwise, None.
+        right : matplotlib.pyplot.Axes, optional
+            The right y-axis, if ``appmag_axis=True`` and ``return_axes=True``. Otherwise, None.
         """
         if xcol.startswith('filter'):
             unit = xcol.split(':')[-1] if ':' in xcol else None
             xcol = 'wl_eff'
             self[xcol] = [f.wl_eff.to(unit) if unit else f.wl_eff for f in self['filter']]
         xchoices = ['phase', 'MJD']
         while xcol not in self.keys():
@@ -497,16 +510,20 @@
             filt = g['filter'][0]
             if color == 'filter':
                 col = filt.color
                 mec = filt.mec
             elif color == 'name' and 'plotcolor' in self.meta:
                 col = self.meta['plotcolor']
                 mec = col if col not in ['w', '#FFFFFF'] else 'k'
+            elif g[color][0] in self.colors:
+                col = self.colors[g[color][0]]
+                mec = col if col not in ['w', '#FFFFFF'] else 'k'
             else:
                 col = mec = next(itercolors)
+            self.colors[g[color][0]] = col
             mfc = col if fillmark else 'none'
             if marker == 'name' and 'marker' in self.meta:
                 mark = self.meta['marker']
             elif marker in plottable.keys():
                 if g[marker][0] not in self.markers:
                     for nextmarker in othermarkers:
                         if nextmarker not in usedmarkers:
@@ -566,47 +583,60 @@
         # format axes
         ymin, ymax = plt.ylim()
         if 'mag' in ycol and ymax > ymin:
             plt.ylim(ymax, ymin)
         lgd_title = None
         for axlabel, keys in column_names.items():
             if xcol in keys:
+                if xcol == 'phase' and phase_hours:
+                    axlabel = axlabel.replace('days', 'hours')
                 plt.xlabel(axlabel)
             elif ycol in keys:
                 plt.ylabel(axlabel)
             elif marker in keys:
                 lgd_title = axlabel
 
         # add auxiliary axes
         mjd_axis = mjd_axis and xcol == 'phase' and 'redshift' in self.meta and 'refmjd' in self.meta
         appmag_axis = appmag_axis and ycol == 'absmag' and 'dm' in self.meta
         if mjd_axis or appmag_axis:
-            top, right = aux_axes(self._phase2mjd if mjd_axis else None, self._abs2app if appmag_axis else None)
+            xfunc = partial(self._phase2mjd, hours=phase_hours)
+            top, right = aux_axes(xfunc if mjd_axis else None, self._abs2app if appmag_axis else None)
             if mjd_axis:
                 top.xaxis.get_major_formatter().set_useOffset(False)
                 top.set_xlabel('MJD')
             if appmag_axis:
                 right.set_ylabel('Apparent Magnitude')
 
         # add legends
             if marker in self.colnames:
-                labels = sorted(set(self[marker]))
-                lines = [plt.Line2D([], [], mec='k', mfc='none', ms=ms, marker=self.markers[label], linestyle='none')
-                         for label in labels]
+                labels = sorted(set(self[marker]), key=lambda s: s.lower())
+                lines = []
+                for label in labels:
+                    if marker == color:
+                        mec = mfc = self.colors[label]
+                    else:
+                        mec = 'k'
+                        mfc = 'none'
+                    line = plt.Line2D([], [], mec=mec, mfc=mfc, ms=ms, marker=self.markers[label], linestyle='none')
+                    lines.append(line)
                 custom_legend(top, lines, labels, ncol=ncol_mark, loc=loc_mark, title=lgd_title, frameon=True)
 
             if color == 'filter':
                 if lgd_filters is None:
                     lgd_filters = set(self['filter'])
                 lines, labels, ncol = filter_legend(lgd_filters, offset_factor)
                 custom_legend(right, lines, labels, loc=loc_filt, ncol=ncol, title='Filter', frameon=True)
 
         if tight_layout:
             plt.tight_layout()
 
+        if return_axes and (mjd_axis or appmag_axis):
+            return top, right
+
     def _phase2mjd(self, phase, hours=False):
         return phase * (1. + self.meta['redshift']) / (24. if hours else 1.) + self.meta['refmjd']
 
     def _abs2app(self, absmag):
         return absmag + self.meta['dm']  # extinction-corrected apparent magnitude
 
     @classmethod
@@ -736,15 +766,15 @@
     ncol : int
         Number of columns needed for the filter legend
     """
     lines = []
     labels = []
     if isinstance(filts, set):
         filts = filtsetup(filts)
-    elif isinstance(filts[0], str):
+    elif isinstance(filts[0], str) or (isinstance(filts[0], list) and isinstance(filts[0][0], str)):
         filts = np.vectorize(filtdict.get)(filts)
     for filt in filts.flatten():
         if filt is None:
             labels.append('')
             lines.append(Patch(color='none', ec='none'))
         else:
             col = filt.color
```

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/models/sifto.dat` & `lightcurve-fitting-0.9.0/lightcurve_fitting/models/sifto.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/models.py` & `lightcurve-fitting-0.9.0/lightcurve_fitting/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,14 +76,17 @@
         if redshift:
             self.z = redshift
         elif lc is not None and 'redshift' in lc.meta:
             self.z = lc.meta['redshift']
         else:
             self.z = 0.
 
+    def __repr__(self):
+        return f'<{self.__class__.__name__}: z={self.z:.3f}>'
+
     def __call__(self, *args, **kwargs):
         return self.evaluate(*args, **kwargs)
 
     @abstractmethod
     def evaluate(self, *args, **kwargs):
         return NotImplemented
 
@@ -192,26 +195,26 @@
         if n == 1.5:
             self.n = 1.5
             self.A = 0.94
             self.a = 1.67
             self.alpha = 0.8
             self.epsilon_1 = 0.027
             self.epsilon_2 = 0.086
-            self.L_0 = 2.0e42
-            self.T_0 = 1.61
+            self.L_0 = 2.0e42  # erg / s
+            self.T_0 = 1.61  # eV
             self.Tph_to_Tcol = 1.1
         elif n == 3.:
             self.n = 3.
             self.A = 0.79
             self.a = 4.57
             self.alpha = 0.73
             self.epsilon_1 = 0.016
             self.epsilon_2 = 0.175
-            self.L_0 = 2.1e42
-            self.T_0 = 1.69
+            self.L_0 = 2.1e42  # erg / s
+            self.T_0 = 1.69  # eV
             self.Tph_to_Tcol = 1.0
         else:
             raise ValueError('n can only be 1.5 or 3')
 
         self.epsilon_T = 2 * self.epsilon_1 - 0.5
         self.epsilon_L = -2 * self.epsilon_2
 
@@ -497,14 +500,167 @@
         return super().t_min([p[0], p[1], p[2], p[3], p[6] if len(p) > 6 else 0.], kappa=kappa)
 
     @staticmethod
     def t_max(p, kappa=1.):
         return super().t_max([p[0], p[1], p[2], p[3], p[6] if len(p) > 6 else 0.], kappa=kappa)
 
 
+class ShockCooling4(Model):
+    """
+    The shock cooling model of Morag, Sapir, & Waxman (https://doi.org/10.1093/mnras/stad899).
+
+    :math:`L(\\tilde{t}) = L_\\mathrm{br}\\left\{\\tilde{t}^{-4/3} + 0.9\\exp\\left[-\\left(\\frac{2.0t}{t_\\mathrm{tr}}\\right)^{0.5}\\right] \\tilde{t}^{-0.17}\\right\}` (Eq. A1)
+
+    :math:`T_\\mathrm{col}(\\tilde{t}) = T_\\mathrm{col,br} \\min(0.97\\tilde{t}^{-1/3}, \\tilde{t}^{-0.45})` (Eq. A2)
+
+    :math:`\\tilde{t} \\equiv \\frac{t}{t_\\mathrm{br}}`, where :math:`t_\\mathrm{br} = (0.86\\,\\mathrm{h}) R^{1.26} v_\\mathrm{s*}^{-1.13} (f_\\rho M \\kappa)^{-0.13}` (Eq. A5)
+
+    :math:`L_\\mathrm{br} = (3.69 \\times 10^{42}\\,\\mathrm{erg}\\,\\mathrm{s}^{-1}) R^{0.78} v_\\mathrm{s*}^{2.11} (f_\\rho M)^{0.11} \\kappa^{-0.89}` (Eq. A6)
+
+    :math:`T_\\mathrm{col,br} = (8.19\\,\\mathrm{eV}) R^{-0.32} v_\\mathrm{s*}^{0.58} (f_\\rho M)^{0.03} \\kappa^{-0.22}` (Eq. A7)
+
+    :math:`t_\\mathrm{tr} = (19.5\\,\\mathrm{d}) \\sqrt{\\frac{\\kappa M}{v_\\mathrm{s*}}}` (Eq. A9)
+
+    Parameters
+    ----------
+    lc : lightcurve_fitting.lightcurve.LC, optional
+        The light curve to which the model will be fit. Only used to get the redshift if `redshift` is not given.
+    redshift : float, optional
+        The redshift between blackbody source and the observed filters. Default: 0.
+
+    Attributes
+    ----------
+    z : float
+        The redshift between blackbody source and the observed filters
+    n : float
+        The polytropic index of the progenitor
+    A : float
+        Coefficient on the luminosity suppression factor (Eq. A1)
+    a : float
+        Coefficient on the transparency timescale (Eq. A1)
+    alpha : float
+        Exponent on the transparency timescale (Eq. A1)
+    L_br_0 : float
+        Coefficient on the luminosity expression in erg/s (Eq. A6)
+    T_col_br_0 : float
+        Coefficient on the temperature expression in eV (Eq. A7)
+    t_min_0 : float
+        Coefficient on the minimum validity time in days (Eq. A3)
+    t_br_0 : float
+        Coefficient on the :math:`\\tilde{t}` timescale in days (Eq. A5)
+    t_07eV_0 : float
+        Coefficient on the time at which the ejecta reach 0.7 eV in days (Eq. A8)
+    t_tr_0 : float
+        Coefficient on the transparency timescale in days (Eq. A9)
+    """
+    input_names = [
+        'v_\\mathrm{s*}',
+        'M_\\mathrm{env}',
+        'f_\\rho M',
+        'R',
+        't_0',
+    ]
+    units = [
+        10. ** 8.5 * u.cm / u.s,
+        u.Msun,
+        u.Msun,
+        1e13 * u.cm,
+        u.d,
+    ]
+
+    def __init__(self, lc=None, redshift=0.):
+        super().__init__(lc, redshift=redshift)
+
+        self.A = 0.9
+        self.a = 2.
+        self.alpha = 0.5
+        self.L_br_0 = 3.69e42  # erg / s
+        self.T_col_br_0 = 8.19  # eV
+        self.t_min_0 = 0.012  # d (17 min)
+        self.t_br_0 = 0.036  # d (0.86 h)
+        self.t_07eV_0 = 6.86  # d
+        self.t_tr_0 = 19.5  # d
+
+    def temperature_radius(self, t_in, v_s, M_env, f_rho_M, R, t_exp=0., kappa=1.):
+        t_br = self.t_br_0 * R ** 1.26 * v_s ** -1.13 * f_rho_M ** -0.13  # Eq. A5
+        L_br = self.L_br_0 * R ** 0.78 * v_s ** 2.11 * f_rho_M ** 0.11 * kappa ** -0.89  # Eq. A6
+        T_col_br = self.T_col_br_0 * R ** -0.32 * v_s ** 0.58 ** f_rho_M ** 0.03 * kappa ** -0.22  # Eq. A7
+        t_tr = self.t_tr_0 * np.sqrt(kappa * M_env / v_s)  # Eq. A9
+
+        t = np.reshape(t_in, (-1, 1)) - t_exp
+        ttilde = t / t_br
+        L = L_br * (power(ttilde, -4. / 3.)
+                    + self.A * np.exp(-power(self.a * t / t_tr, self.alpha)) * power(ttilde, -0.17))  # Eq. A1
+        T_col = T_col_br * np.minimum(0.97 * power(ttilde, -1. / 3.), power(ttilde, -0.45))  # Eq. A2
+
+        T_K = np.squeeze(T_col) / k_B
+        R_bb = c3 * np.squeeze(L) ** 0.5 * power(T_K, -2.)
+        return T_K, R_bb
+
+    def evaluate(self, t_in, f, v_s, M_env, f_rho_M, R, t_exp=0., kappa=1.):
+        """
+        Evaluate this model at a range of times and filters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        v_s : float, array-like
+            The shock speed in :math:`10^{8.5}` cm/s
+        M_env : float, array-like
+            The envelope mass in solar masses
+        f_rho_M : float, array-like
+            The product :math:`f_ρ M`, where ":math:`f_ρ` is a numerical factor of order unity that depends on the inner
+            envelope structure" and :math:`M` is the ejecta mass in solar masses
+        R : float, array-like
+            The progenitor radius in :math:`10^{13}` cm
+        t_exp : float, array-like, optional
+            The explosion epoch. Default: 0.
+        kappa : float, array-like, optional
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g). Default: 1.
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+        T_K, R_bb = self.temperature_radius(t_in, v_s, M_env, f_rho_M, R, t_exp, kappa)
+        lum_blackbody = blackbody_to_filters(f, T_K, R_bb, self.z)
+        lum_suppressed = blackbody_to_filters(f, 0.74 * T_K, 0.74 ** -2. * R_bb, self.z)
+        lum = np.minimum(lum_blackbody, lum_suppressed)  # Eq. A4
+        return lum
+
+    def t_min(self, p, kappa=1.):
+        """
+        The minimum time at which the model is valid
+
+        :math:`t_\\mathrm{min} = (17\\,\\mathrm{min}) R + t_\\mathrm{exp}` (Eq. A3)
+        """
+        R = p[3]
+        t_exp = p[4] if len(p) > 4 else 0.
+        return self.t_min_0 * R + t_exp  # Eq. A3
+
+    def t_max(self, p, kappa=1.):
+        """
+        The maximum time at which the model is valid
+
+        :math:`t_\\mathrm{max} = \\min(t_\\mathrm{0.7\\,eV}, 0.5 t_\\mathrm{tr})` (Eq. A3)
+
+        :math:`t_\\mathrm{0.7\\,eV} = (6.86\\,\\mathrm{d}) R^{0.56} v_\\mathrm{s*}^{0.16} \\kappa^{-0.61} (f_\\rho M)^{-0.06}` (Eq. A8)
+
+        :math:`t_\\mathrm{tr} = (19.5\\,\\mathrm{d}) \\sqrt{\\frac{\\kappa M}{v_\\mathrm{s*}}}` (Eq. A9)
+        """
+        v_s, M_env, f_rho_M, R, t_exp, *_ = p
+        t_07eV = self.t_07eV_0 * R ** 0.56 * v_s ** 0.16 * kappa ** -0.61 * f_rho_M ** -0.06  # Eq. A8
+        t_tr = self.t_tr_0 ** np.sqrt(kappa * M_env / v_s)  # Eq. A9
+        return np.minimum(t_07eV, t_tr / self.a) + t_exp  # Eq. A3
+
+
 sifto_filename = resource_filename('lightcurve_fitting', 'models/sifto.dat')
 sifto = Table.read(sifto_filename, format='ascii')[3:]  # the first three points are ~0
 M_chandra = u.def_unit('M_chandra', 1.4 * u.Msun, format={'latex': 'M_\\mathrm{Ch}'})
 
 
 class BaseCompanionShocking(Model):
     """
```

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting/speccal.py` & `lightcurve-fitting-0.9.0/lightcurve_fitting/speccal.py`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/PKG-INFO` & `lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurve-fitting
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools to fit analytical models to multiband light curves of astronomical transients
 Home-page: https://github.com/griffin-h/lightcurve_fitting
 Author: Griffin Hosseinzadeh
 Author-email: griffin0@arizona.edu
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/SOURCES.txt` & `lightcurve-fitting-0.9.0/lightcurve_fitting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/setup.py` & `lightcurve-fitting-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.8.0/versioneer.py` & `lightcurve-fitting-0.9.0/versioneer.py`

 * *Files identical despite different names*

