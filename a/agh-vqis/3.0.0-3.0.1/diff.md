# Comparing `tmp/agh_vqis-3.0.0.tar.gz` & `tmp/agh_vqis-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agh_vqis-3.0.0.tar", last modified: Tue Jun 13 13:44:00 2023, max compression
+gzip compressed data, was "agh_vqis-3.0.1.tar", last modified: Fri Jun 16 19:07:33 2023, max compression
```

## Comparing `agh_vqis-3.0.0.tar` & `agh_vqis-3.0.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:44:00.160929 agh_vqis-3.0.0/
--rw-rw-rw-   0        0        0     2826 2023-06-09 20:08:24.000000 agh_vqis-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     7343 2023-06-13 13:44:00.160929 agh_vqis-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6335 2023-06-13 13:29:46.000000 agh_vqis-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 13:43:59.201921 agh_vqis-3.0.0/agh_vqis.egg-info/
--rw-rw-rw-   0        0        0     7343 2023-06-13 13:43:59.000000 agh_vqis-3.0.0/agh_vqis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8077 2023-06-13 13:43:59.000000 agh_vqis-3.0.0/agh_vqis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:43:59.000000 agh_vqis-3.0.0/agh_vqis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2023-06-13 13:43:59.000000 agh_vqis-3.0.0/agh_vqis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 13:43:59.000000 agh_vqis-3.0.0/agh_vqis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-06-09 20:08:24.000000 agh_vqis-3.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-13 13:43:59.139413 agh_vqis-3.0.0/python-cpbd/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:43:59.233167 agh_vqis-3.0.0/python-cpbd/cpbd/
--rw-rw-rw-   0        0        0       49 2023-06-09 20:24:14.000000 agh_vqis-3.0.0/python-cpbd/cpbd/__init__.py
--rw-rw-rw-   0        0        0     7670 2023-06-09 20:24:14.000000 agh_vqis-3.0.0/python-cpbd/cpbd/compute.py
--rw-rw-rw-   0        0        0     1540 2023-06-09 20:24:14.000000 agh_vqis-3.0.0/python-cpbd/cpbd/octave.py
--rw-rw-rw-   0        0        0     1329 2023-06-13 13:44:00.160929 agh_vqis-3.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 13:43:59.139413 agh_vqis-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:43:59.248713 agh_vqis-3.0.0/src/agh_vqis/
--rw-rw-rw-   0        0        0      381 2023-06-09 21:16:32.000000 agh_vqis-3.0.0/src/agh_vqis/__init__.py
--rw-rw-rw-   0        0        0    21918 2023-06-13 13:39:42.000000 agh_vqis-3.0.0/src/agh_vqis/__main__.py
--rw-rw-rw-   0        0        0     1349 2023-06-09 20:08:24.000000 agh_vqis-3.0.0/src/agh_vqis/_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:43:59.248713 agh_vqis-3.0.0/src/agh_vqis/binaries/
--rw-rw-rw-   0        0        0    97508 2023-06-09 20:08:24.000000 agh_vqis-3.0.0/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
--rwxrwxrwx   0        0        0   127167 2023-06-09 20:08:24.000000 agh_vqis-3.0.0/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
--rw-rw-rw-   0        0        0    66424 2023-06-09 20:08:24.000000 agh_vqis-3.0.0/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
-drwxrwxrwx   0        0        0        0 2023-06-13 13:43:59.154966 agh_vqis-3.0.0/src/agh_vqis/models/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:44:00.152976 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/
--rw-rw-rw-   0        0        0    21075 2023-05-23 22:55:31.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    21723 2023-05-23 22:55:33.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    14595 2023-05-23 22:55:36.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    15027 2023-05-23 22:55:38.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    32379 2023-05-23 22:56:00.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    35763 2023-05-23 22:56:02.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    34323 2023-05-23 22:56:04.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    34323 2023-05-23 22:56:06.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    37059 2023-05-23 22:56:08.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    34035 2023-05-23 22:56:10.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    29643 2023-05-23 22:55:40.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
--rw-rw-rw-   0        0        0    33747 2023-05-23 22:55:42.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
--rw-rw-rw-   0        0        0    28059 2023-05-23 22:55:44.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
--rw-rw-rw-   0        0        0    29787 2023-05-23 22:55:45.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
--rw-rw-rw-   0        0        0    33531 2023-05-23 22:55:46.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
--rw-rw-rw-   0        0        0    29355 2023-05-23 22:55:48.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
--rw-rw-rw-   0        0        0    26691 2023-05-23 22:55:50.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
--rw-rw-rw-   0        0        0    31803 2023-05-23 22:55:52.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-05-23 22:55:58.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
--rw-rw-rw-   0        0        0    30291 2023-05-23 22:55:54.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
--rw-rw-rw-   0        0        0    30795 2023-05-23 22:55:56.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
--rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:50.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    26907 2023-05-23 22:56:50.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    38355 2023-05-23 22:56:42.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
--rw-rw-rw-   0        0        0    39075 2023-05-23 22:56:44.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
--rw-rw-rw-   0        0        0    37635 2023-05-23 22:56:46.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
--rw-rw-rw-   0        0        0    37059 2023-05-23 22:56:49.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
--rw-rw-rw-   0        0        0    26979 2023-05-23 22:56:58.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    27339 2023-05-23 22:56:59.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38571 2023-05-23 22:56:51.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
--rw-rw-rw-   0        0        0    39219 2023-05-23 22:56:55.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
--rw-rw-rw-   0        0        0    37923 2023-05-23 22:56:56.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
--rw-rw-rw-   0        0        0    37995 2023-05-23 22:56:57.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
--rw-rw-rw-   0        0        0    27339 2023-05-23 22:57:03.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    27267 2023-05-23 22:57:07.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    38643 2023-05-23 22:57:00.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
--rw-rw-rw-   0        0        0    39363 2023-05-23 22:57:01.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
--rw-rw-rw-   0        0        0    38067 2023-05-23 22:57:01.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
--rw-rw-rw-   0        0        0    38211 2023-05-23 22:57:02.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
--rw-rw-rw-   0        0        0    36915 2023-05-23 22:56:15.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
--rw-rw-rw-   0        0        0    37851 2023-05-23 22:56:16.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
--rw-rw-rw-   0        0        0    37347 2023-05-23 22:56:17.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
--rw-rw-rw-   0        0        0    28779 2023-05-23 22:56:11.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
--rw-rw-rw-   0        0        0    29715 2023-05-23 22:56:13.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
--rw-rw-rw-   0        0        0    30219 2023-05-23 22:56:14.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-05-23 22:56:23.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
--rw-rw-rw-   0        0        0    38283 2023-05-23 22:56:25.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
--rw-rw-rw-   0        0        0    37563 2023-05-23 22:56:26.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
--rw-rw-rw-   0        0        0    27843 2023-05-23 22:56:18.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
--rw-rw-rw-   0        0        0    27267 2023-05-23 22:56:19.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
--rw-rw-rw-   0        0        0    27699 2023-05-23 22:56:20.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
--rw-rw-rw-   0        0        0    37635 2023-05-23 22:56:30.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
--rw-rw-rw-   0        0        0    37275 2023-05-23 22:56:31.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
--rw-rw-rw-   0        0        0    37851 2023-05-23 22:56:32.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
--rw-rw-rw-   0        0        0    29283 2023-05-23 22:56:27.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
--rw-rw-rw-   0        0        0    27483 2023-05-23 22:56:27.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
--rw-rw-rw-   0        0        0    26979 2023-05-23 22:56:28.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
--rw-rw-rw-   0        0        0    37347 2023-05-23 22:56:37.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
--rw-rw-rw-   0        0        0    38139 2023-05-23 22:56:38.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
--rw-rw-rw-   0        0        0    37779 2023-05-23 22:56:40.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
--rw-rw-rw-   0        0        0    29787 2023-05-23 22:56:33.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
--rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:35.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
--rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:35.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
--rw-rw-rw-   0        0        0    17259 2023-05-23 22:57:32.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    17835 2023-05-23 22:57:32.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    27411 2023-05-23 22:57:28.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
--rw-rw-rw-   0        0        0    25179 2023-05-23 22:57:30.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
--rw-rw-rw-   0        0        0    22659 2023-05-23 22:57:31.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
--rw-rw-rw-   0        0        0    17259 2023-05-23 22:57:34.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    17187 2023-05-23 22:57:44.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    25395 2023-05-23 22:57:33.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
--rw-rw-rw-   0        0        0    23955 2023-05-23 22:57:34.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-05-23 22:57:51.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    16827 2023-05-23 22:57:52.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    23667 2023-05-23 22:57:49.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-05-23 22:57:08.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
--rw-rw-rw-   0        0        0    20571 2023-05-23 22:57:09.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
--rw-rw-rw-   0        0        0    22299 2023-05-23 22:57:10.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
--rw-rw-rw-   0        0        0    22155 2023-05-23 22:57:14.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
--rw-rw-rw-   0        0        0    19059 2023-05-23 22:57:12.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
--rw-rw-rw-   0        0        0    18987 2023-05-23 22:57:12.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
--rw-rw-rw-   0        0        0    20571 2023-05-23 22:57:13.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
--rw-rw-rw-   0        0        0    23163 2023-05-23 22:57:20.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-05-23 22:57:21.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
--rw-rw-rw-   0        0        0    22011 2023-05-23 22:57:15.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
--rw-rw-rw-   0        0        0    20283 2023-05-23 22:57:16.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
--rw-rw-rw-   0        0        0    18123 2023-05-23 22:57:17.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
--rw-rw-rw-   0        0        0    22947 2023-05-23 22:57:25.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-05-23 22:57:26.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
--rw-rw-rw-   0        0        0    22587 2023-05-23 22:57:26.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
--rw-rw-rw-   0        0        0    23955 2023-05-23 22:57:22.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
--rw-rw-rw-   0        0        0    21435 2023-05-23 22:57:23.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
--rw-rw-rw-   0        0        0    18699 2023-05-23 22:57:24.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
--rw-rw-rw-   0        0        0     4587 2023-05-23 22:57:59.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
--rw-rw-rw-   0        0        0     5739 2023-05-23 22:57:53.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
--rw-rw-rw-   0        0        0     6459 2023-05-23 22:57:54.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
--rw-rw-rw-   0        0        0     5307 2023-05-23 22:57:55.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
--rw-rw-rw-   0        0        0     5811 2023-05-23 22:57:56.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
--rw-rw-rw-   0        0        0     4947 2023-05-23 22:57:57.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
--rw-rw-rw-   0        0        0     5379 2023-05-23 22:57:58.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
--rw-rw-rw-   0        0        0     5163 2023-05-23 22:57:57.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
--rw-rw-rw-   0        0        0    40443 2023-05-23 22:58:18.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    43467 2023-05-23 22:58:19.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    39435 2023-05-23 22:58:21.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    42171 2023-05-23 22:58:22.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38787 2023-05-23 22:58:23.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    42747 2023-05-23 22:58:00.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
--rw-rw-rw-   0        0        0    39939 2023-05-23 22:58:01.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
--rw-rw-rw-   0        0        0    41235 2023-05-23 22:58:01.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
--rw-rw-rw-   0        0        0    38931 2023-05-23 22:58:02.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
--rw-rw-rw-   0        0        0    40875 2023-05-23 22:58:03.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
--rw-rw-rw-   0        0        0    37923 2023-05-23 22:58:16.000000 agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
-drwxrwxrwx   0        0        0        0 2023-06-13 13:44:00.152976 agh_vqis-3.0.0/src/agh_vqis/models/ugc/
--rw-rw-rw-   0        0        0   594166 2023-06-13 12:09:35.000000 agh_vqis-3.0.0/src/agh_vqis/models/ugc/12k_all_set.json
-drwxrwxrwx   0        0        0        0 2023-06-13 13:44:00.160929 agh_vqis-3.0.0/src/agh_vqis/utils/
--rw-rw-rw-   0        0        0     5470 2023-06-13 13:06:52.000000 agh_vqis-3.0.0/src/agh_vqis/utils/helpers.py
--rw-rw-rw-   0        0        0      754 2023-06-09 21:13:23.000000 agh_vqis-3.0.0/src/agh_vqis/utils/resolution_cast.py
--rw-rw-rw-   0        0        0     5735 2023-06-13 12:52:00.000000 agh_vqis-3.0.0/src/agh_vqis/utils/ugc.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:33.526980 agh_vqis-3.0.1/
+-rw-rw-rw-   0        0        0     2826 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7317 2023-06-16 19:07:33.526980 agh_vqis-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6309 2023-06-16 19:04:34.000000 agh_vqis-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.398168 agh_vqis-3.0.1/agh_vqis.egg-info/
+-rw-rw-rw-   0        0        0     7317 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8077 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.337999 agh_vqis-3.0.1/python-cpbd/
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.413906 agh_vqis-3.0.1/python-cpbd/cpbd/
+-rw-rw-rw-   0        0        0       49 2023-06-09 20:24:14.000000 agh_vqis-3.0.1/python-cpbd/cpbd/__init__.py
+-rw-rw-rw-   0        0        0     7670 2023-06-09 20:24:14.000000 agh_vqis-3.0.1/python-cpbd/cpbd/compute.py
+-rw-rw-rw-   0        0        0     1540 2023-06-09 20:24:14.000000 agh_vqis-3.0.1/python-cpbd/cpbd/octave.py
+-rw-rw-rw-   0        0        0     1329 2023-06-16 19:07:33.540207 agh_vqis-3.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.337999 agh_vqis-3.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.429538 agh_vqis-3.0.1/src/agh_vqis/
+-rw-rw-rw-   0        0        0      381 2023-06-16 19:03:24.000000 agh_vqis-3.0.1/src/agh_vqis/__init__.py
+-rw-rw-rw-   0        0        0    21928 2023-06-16 19:06:30.000000 agh_vqis-3.0.1/src/agh_vqis/__main__.py
+-rw-rw-rw-   0        0        0     1349 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/src/agh_vqis/_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.445290 agh_vqis-3.0.1/src/agh_vqis/binaries/
+-rw-rw-rw-   0        0        0    97508 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
+-rwxrwxrwx   0        0        0   123613 2023-06-16 18:18:43.000000 agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
+-rw-rw-rw-   0        0        0    66424 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.349617 agh_vqis-3.0.1/src/agh_vqis/models/
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:33.486661 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/
+-rw-rw-rw-   0        0        0    21075 2023-05-23 22:55:31.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    21723 2023-05-23 22:55:33.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    14595 2023-05-23 22:55:36.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    15027 2023-05-23 22:55:38.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    32379 2023-05-23 22:56:00.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    35763 2023-05-23 22:56:02.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-05-23 22:56:04.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-05-23 22:56:06.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-05-23 22:56:08.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    34035 2023-05-23 22:56:10.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    29643 2023-05-23 22:55:40.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
+-rw-rw-rw-   0        0        0    33747 2023-05-23 22:55:42.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
+-rw-rw-rw-   0        0        0    28059 2023-05-23 22:55:44.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-05-23 22:55:45.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
+-rw-rw-rw-   0        0        0    33531 2023-05-23 22:55:46.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
+-rw-rw-rw-   0        0        0    29355 2023-05-23 22:55:48.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
+-rw-rw-rw-   0        0        0    26691 2023-05-23 22:55:50.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
+-rw-rw-rw-   0        0        0    31803 2023-05-23 22:55:52.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-05-23 22:55:58.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    30291 2023-05-23 22:55:54.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
+-rw-rw-rw-   0        0        0    30795 2023-05-23 22:55:56.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:50.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    26907 2023-05-23 22:56:50.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    38355 2023-05-23 22:56:42.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
+-rw-rw-rw-   0        0        0    39075 2023-05-23 22:56:44.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-05-23 22:56:46.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-05-23 22:56:49.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-05-23 22:56:58.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-05-23 22:56:59.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38571 2023-05-23 22:56:51.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
+-rw-rw-rw-   0        0        0    39219 2023-05-23 22:56:55.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-05-23 22:56:56.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    37995 2023-05-23 22:56:57.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-05-23 22:57:03.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-05-23 22:57:07.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    38643 2023-05-23 22:57:00.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
+-rw-rw-rw-   0        0        0    39363 2023-05-23 22:57:01.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
+-rw-rw-rw-   0        0        0    38067 2023-05-23 22:57:01.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
+-rw-rw-rw-   0        0        0    38211 2023-05-23 22:57:02.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    36915 2023-05-23 22:56:15.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-05-23 22:56:16.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-05-23 22:56:17.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
+-rw-rw-rw-   0        0        0    28779 2023-05-23 22:56:11.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
+-rw-rw-rw-   0        0        0    29715 2023-05-23 22:56:13.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
+-rw-rw-rw-   0        0        0    30219 2023-05-23 22:56:14.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-05-23 22:56:23.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    38283 2023-05-23 22:56:25.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
+-rw-rw-rw-   0        0        0    37563 2023-05-23 22:56:26.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
+-rw-rw-rw-   0        0        0    27843 2023-05-23 22:56:18.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-05-23 22:56:19.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
+-rw-rw-rw-   0        0        0    27699 2023-05-23 22:56:20.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-05-23 22:56:30.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    37275 2023-05-23 22:56:31.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-05-23 22:56:32.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
+-rw-rw-rw-   0        0        0    29283 2023-05-23 22:56:27.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
+-rw-rw-rw-   0        0        0    27483 2023-05-23 22:56:27.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-05-23 22:56:28.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-05-23 22:56:37.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    38139 2023-05-23 22:56:38.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-05-23 22:56:40.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-05-23 22:56:33.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:35.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:35.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-05-23 22:57:32.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    17835 2023-05-23 22:57:32.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    27411 2023-05-23 22:57:28.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    25179 2023-05-23 22:57:30.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    22659 2023-05-23 22:57:31.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-05-23 22:57:34.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    17187 2023-05-23 22:57:44.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    25395 2023-05-23 22:57:33.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-05-23 22:57:34.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-05-23 22:57:51.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    16827 2023-05-23 22:57:52.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    23667 2023-05-23 22:57:49.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-05-23 22:57:08.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-05-23 22:57:09.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
+-rw-rw-rw-   0        0        0    22299 2023-05-23 22:57:10.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
+-rw-rw-rw-   0        0        0    22155 2023-05-23 22:57:14.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    19059 2023-05-23 22:57:12.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
+-rw-rw-rw-   0        0        0    18987 2023-05-23 22:57:12.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-05-23 22:57:13.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
+-rw-rw-rw-   0        0        0    23163 2023-05-23 22:57:20.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-05-23 22:57:21.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    22011 2023-05-23 22:57:15.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
+-rw-rw-rw-   0        0        0    20283 2023-05-23 22:57:16.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
+-rw-rw-rw-   0        0        0    18123 2023-05-23 22:57:17.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
+-rw-rw-rw-   0        0        0    22947 2023-05-23 22:57:25.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-05-23 22:57:26.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    22587 2023-05-23 22:57:26.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-05-23 22:57:22.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
+-rw-rw-rw-   0        0        0    21435 2023-05-23 22:57:23.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
+-rw-rw-rw-   0        0        0    18699 2023-05-23 22:57:24.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
+-rw-rw-rw-   0        0        0     4587 2023-05-23 22:57:59.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0     5739 2023-05-23 22:57:53.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
+-rw-rw-rw-   0        0        0     6459 2023-05-23 22:57:54.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
+-rw-rw-rw-   0        0        0     5307 2023-05-23 22:57:55.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
+-rw-rw-rw-   0        0        0     5811 2023-05-23 22:57:56.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
+-rw-rw-rw-   0        0        0     4947 2023-05-23 22:57:57.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
+-rw-rw-rw-   0        0        0     5379 2023-05-23 22:57:58.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
+-rw-rw-rw-   0        0        0     5163 2023-05-23 22:57:57.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
+-rw-rw-rw-   0        0        0    40443 2023-05-23 22:58:18.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    43467 2023-05-23 22:58:19.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    39435 2023-05-23 22:58:21.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    42171 2023-05-23 22:58:22.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38787 2023-05-23 22:58:23.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    42747 2023-05-23 22:58:00.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
+-rw-rw-rw-   0        0        0    39939 2023-05-23 22:58:01.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
+-rw-rw-rw-   0        0        0    41235 2023-05-23 22:58:01.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
+-rw-rw-rw-   0        0        0    38931 2023-05-23 22:58:02.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
+-rw-rw-rw-   0        0        0    40875 2023-05-23 22:58:03.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-05-23 22:58:16.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:33.506214 agh_vqis-3.0.1/src/agh_vqis/models/ugc/
+-rw-rw-rw-   0        0        0   594166 2023-06-13 12:09:35.000000 agh_vqis-3.0.1/src/agh_vqis/models/ugc/12k_all_set.json
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:33.526980 agh_vqis-3.0.1/src/agh_vqis/utils/
+-rw-rw-rw-   0        0        0     5470 2023-06-16 19:06:30.000000 agh_vqis-3.0.1/src/agh_vqis/utils/helpers.py
+-rw-rw-rw-   0        0        0      754 2023-06-09 21:13:23.000000 agh_vqis-3.0.1/src/agh_vqis/utils/resolution_cast.py
+-rw-rw-rw-   0        0        0     5735 2023-06-13 12:52:00.000000 agh_vqis-3.0.1/src/agh_vqis/utils/ugc.py
```

### Comparing `agh_vqis-3.0.0/LICENSE` & `agh_vqis-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/PKG-INFO` & `agh_vqis-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agh_vqis
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Python wrapper for 18 image quality indicators.
 Home-page: https://qoe.agh.edu.pl/indicators/
 Author: Jakub Nawała, Filip Korus
 Author-email: jakub.nawala@agh.edu.pl, fkorus@student.agh.edu.pl
 License: EVALUATION LICENSE AGREEMENT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -91,26 +91,26 @@
    Whereas this command will display help:
    ```shell
    $ python3 -m agh_vqis -h
    ```
 6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
 
 
-7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
+7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given IQI when applied to the respective frame.
 
 
 8. Cast chosen indicators for different resolutions (**experimental**). For example: to cast Blur to 1440p and Blockiness to 2160p you should pass two additional lines in `options` dictionary like below.
 ```python
-    from agh_vqis import process_single_mm_file, CastIQI, DestResolution
+    from agh_vqis import process_single_mm_file, CastVQI, DestResolution
     from pathlib import Path
     
     if __name__ == '__main__':
         process_single_mm_file(Path('/path/to/single/video.mp4'), options={
-           CastIQI.blur: DestResolution.p1440,
-           CastIQI.blockiness: DestResolution.p2160
+           CastVQI.blur: DestResolution.p1440,
+           CastVQI.blockiness: DestResolution.p2160
         })
    ```
 
    ### Available casts
    ##### Blockiness:
    - 1080p -> 1440p
    - 1080p -> 2160p
```

### Comparing `agh_vqis-3.0.0/README.md` & `agh_vqis-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,26 +67,26 @@
    Whereas this command will display help:
    ```shell
    $ python3 -m agh_vqis -h
    ```
 6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
 
 
-7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
+7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given IQI when applied to the respective frame.
 
 
 8. Cast chosen indicators for different resolutions (**experimental**). For example: to cast Blur to 1440p and Blockiness to 2160p you should pass two additional lines in `options` dictionary like below.
 ```python
-    from agh_vqis import process_single_mm_file, CastIQI, DestResolution
+    from agh_vqis import process_single_mm_file, CastVQI, DestResolution
     from pathlib import Path
     
     if __name__ == '__main__':
         process_single_mm_file(Path('/path/to/single/video.mp4'), options={
-           CastIQI.blur: DestResolution.p1440,
-           CastIQI.blockiness: DestResolution.p2160
+           CastVQI.blur: DestResolution.p1440,
+           CastVQI.blockiness: DestResolution.p2160
         })
    ```
 
    ### Available casts
    ##### Blockiness:
    - 1080p -> 1440p
    - 1080p -> 2160p
```

### Comparing `agh_vqis-3.0.0/agh_vqis.egg-info/PKG-INFO` & `agh_vqis-3.0.1/agh_vqis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agh-vqis
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Python wrapper for 18 image quality indicators.
 Home-page: https://qoe.agh.edu.pl/indicators/
 Author: Jakub Nawała, Filip Korus
 Author-email: jakub.nawala@agh.edu.pl, fkorus@student.agh.edu.pl
 License: EVALUATION LICENSE AGREEMENT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -91,26 +91,26 @@
    Whereas this command will display help:
    ```shell
    $ python3 -m agh_vqis -h
    ```
 6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
 
 
-7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
+7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given IQI when applied to the respective frame.
 
 
 8. Cast chosen indicators for different resolutions (**experimental**). For example: to cast Blur to 1440p and Blockiness to 2160p you should pass two additional lines in `options` dictionary like below.
 ```python
-    from agh_vqis import process_single_mm_file, CastIQI, DestResolution
+    from agh_vqis import process_single_mm_file, CastVQI, DestResolution
     from pathlib import Path
     
     if __name__ == '__main__':
         process_single_mm_file(Path('/path/to/single/video.mp4'), options={
-           CastIQI.blur: DestResolution.p1440,
-           CastIQI.blockiness: DestResolution.p2160
+           CastVQI.blur: DestResolution.p1440,
+           CastVQI.blockiness: DestResolution.p2160
         })
    ```
 
    ### Available casts
    ##### Blockiness:
    - 1080p -> 1440p
    - 1080p -> 2160p
```

### Comparing `agh_vqis-3.0.0/agh_vqis.egg-info/SOURCES.txt` & `agh_vqis-3.0.1/agh_vqis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/python-cpbd/cpbd/compute.py` & `agh_vqis-3.0.1/python-cpbd/cpbd/compute.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/python-cpbd/cpbd/octave.py` & `agh_vqis-3.0.1/python-cpbd/cpbd/octave.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/setup.cfg` & `agh_vqis-3.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6768 5f76 7169 730d 0a76 6572   = agh_vqis..ver
-00000020: 7369 6f6e 203d 2033 2e30 2e30 0d0a 6175  sion = 3.0.0..au
+00000020: 7369 6f6e 203d 2033 2e30 2e31 0d0a 6175  sion = 3.0.1..au
 00000030: 7468 6f72 203d 204a 616b 7562 204e 6177  thor = Jakub Naw
 00000040: 61c5 8261 2c20 4669 6c69 7020 4b6f 7275  a..a, Filip Koru
 00000050: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
 00000060: 3d20 6a61 6b75 622e 6e61 7761 6c61 4061  = jakub.nawala@a
 00000070: 6768 2e65 6475 2e70 6c2c 2066 6b6f 7275  gh.edu.pl, fkoru
 00000080: 7340 7374 7564 656e 742e 6167 682e 6564  s@student.agh.ed
 00000090: 752e 706c 0d0a 6465 7363 7269 7074 696f  u.pl..descriptio
```

### Comparing `agh_vqis-3.0.0/src/agh_vqis/__main__.py` & `agh_vqis-3.0.1/src/agh_vqis/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .utils.resolution_cast import *
 
 logger = setup_console_and_file_logger(__name__, log_file_name=f"{__name__}.log", level=logging.INFO)
 
 allowed_mm_file_extensions = ['.jpg', '.jpeg', '.png', '.ts', '.mp4', '.y4m', '.mov', '.avi', '.mkv', '.gif', '.bmp']
 
 
-def _run_agh_viqs(mm_file_path: Path, selected_vqis=32767):
+def _run_agh_vqis(mm_file_path: Path, selected_vqis=32767):
     """
     Runs 15 VQ AGH's Video Quality Indicators (VQIs) on an input video or image (identified by *video_path*) and returns
     Pandas DataFrame with results.
 
     :param mm_file_path: path to a video or image file to process
     :param selected_vqis: a positive 16-bit integer stating which VQIs to run (all are run by default)
     :return: Pandas DataFrame with VQIs results or -1 if an error occurred
@@ -59,15 +59,15 @@
 
     logger.debug(f'{sfs_call_elems[0]} binary file was successfully executed')
 
     vqis_csv_path = Path(random_folder_name, mm_file_path.stem + '.csv')
 
     mv_file(Path('./metricsResultsCSV.csv').resolve(), vqis_csv_path.resolve())
 
-    vqis_res_df = pd.read_csv(vqis_csv_path, sep=r'\s+')
+    vqis_res_df = pd.read_csv(vqis_csv_path.resolve(), sep=r'\s+')
 
     logger.debug('Removing working directory')
     rmdir(random_folder_name)
 
     return vqis_res_df
 
 
@@ -203,15 +203,15 @@
     return [{
         'range_start': int(item['frames_range'].split(', ')[0]) - 1,
         'range_end': int(item['frames_range'].split(', ')[1]) - 1,
         'ugc': item['ugc']
     } for item in shots_data]
 
 
-def get_ugc_iqi(in_path: Path, nb_frames: int, results_vqis: pd.DataFrame):
+def get_ugc_vqi(in_path: Path, nb_frames: int, results_vqis: pd.DataFrame):
     shots = _ugc(in_path, results_vqis)
 
     if shots is None:
         return None
 
     ugc_s = pd.Series(np.zeros(nb_frames))
     for frame in range(nb_frames):
@@ -368,29 +368,29 @@
 
     if not cli:
         selected_vqis = get_selected_vqis(options)
 
     vqis_res_df = None
     if not cli or args.vqis:
         logger.info(f"Running requested AGH VQIs on the input ({str(in_path.resolve())})")
-        vqis_res_df = _run_agh_viqs(in_path, selected_vqis)
+        vqis_res_df = _run_agh_vqis(in_path, selected_vqis)
         if type(vqis_res_df) is not pd.DataFrame:  # Running the VQIs failed
             return -1
 
         if (len(vqis_res_df) != int(nb_frames)) and is_input_video:
             logger.warning(
                 f"For some reason the number of frames read by ffmpeg-python does not match the number of frames read "
                 f"by binary file. You may want to check whether the results are valid.")
             logger.warning(f"This is the difference in the number of frames as indicated by the two methods: "
                            f"{np.abs(len(vqis_res_df) - int(nb_frames))}")
 
     if run_ugc_iqi:
         logger.info(f"Running the UGC IQI on the input ({str(in_path.resolve())})")
 
-        ugc_s = get_ugc_iqi(in_path, int(nb_frames), vqis_res_df)
+        ugc_s = get_ugc_vqi(in_path, int(nb_frames), vqis_res_df)
         if ugc_s is None:
             logger.error(f"Error when running UGC IQI")
         else:
             ugc_s.name = "UGC"
             results.update({Results.UGC: ugc_s})
 
     if vqis_res_df is not None:
@@ -400,15 +400,15 @@
 
     # options = options | {CastIQI.blur: DestResolution.p360}
     # options = options | {CastIQI.interlace: DestResolution.p1080}
 
     if not cli or True:
         res_df = results[Results.VQIS]
 
-        for cast_iqi in [CastIQI.blockiness, CastIQI.interlace, CastIQI.blur, CastIQI.noise, CastIQI.contrast, CastIQI.exposure]:
+        for cast_iqi in [CastVQI.blockiness, CastVQI.interlace, CastVQI.blur, CastVQI.noise, CastVQI.contrast, CastVQI.exposure]:
             if cast_iqi not in options:
                 continue
 
             cast_iqi_name = cast_iqi.split('_')[-1]
 
             dst_resolution = options[cast_iqi]
             if is_model_available(cast_iqi_name, in_mm_file_h, dst_resolution):
```

### Comparing `agh_vqis-3.0.0/src/agh_vqis/_logger.py` & `agh_vqis-3.0.1/src/agh_vqis/_logger.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt` & `agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/binaries/agh_vqis_binary_x86_mt` & `agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_x86_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb` & `agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/models/ugc/12k_all_set.json` & `agh_vqis-3.0.1/src/agh_vqis/models/ugc/12k_all_set.json`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/utils/helpers.py` & `agh_vqis-3.0.1/src/agh_vqis/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     slice = 'slice'
     flickering = 'flickering'
     colourfulness = 'colourfulness'
     blur_amount = 'blur_amount'
     ugc = 'ugc'
 
 
-class CastIQI:
+class CastVQI:
     blockiness = 'cast_Blockiness'
     blur = 'cast_Blur'
     contrast = 'cast_Contrast'
     exposure = 'cast_Exposure(bri)'
     interlace = 'cast_Interlace'
     noise = 'cast_Noise'
```

### Comparing `agh_vqis-3.0.0/src/agh_vqis/utils/resolution_cast.py` & `agh_vqis-3.0.1/src/agh_vqis/utils/resolution_cast.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.0/src/agh_vqis/utils/ugc.py` & `agh_vqis-3.0.1/src/agh_vqis/utils/ugc.py`

 * *Files identical despite different names*

