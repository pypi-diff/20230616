# Comparing `tmp/ShuaiToolBox-1.1.2.7.tar.gz` & `tmp/ShuaiToolBox-1.1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ShuaiToolBox-1.1.2.7.tar", last modified: Thu Jun 15 16:19:30 2023, max compression
+gzip compressed data, was "dist\ShuaiToolBox-1.1.2.8.tar", last modified: Fri Jun 16 03:39:07 2023, max compression
```

## Comparing `ShuaiToolBox-1.1.2.7.tar` & `ShuaiToolBox-1.1.2.8.tar`

### file list

```diff
@@ -1,67 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/
--rw-rw-rw-   0        0        0       36 2023-06-15 16:19:16.000000 ShuaiToolBox-1.1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      223 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/
--rw-rw-rw-   0        0        0   498564 2023-06-15 15:15:41.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/EORmodule.c
--rw-rw-rw-   0        0        0   123392 2023-06-15 15:15:46.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/EORmodule.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   261888 2023-06-15 15:15:41.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/FindContours.c
--rw-rw-rw-   0        0        0    64000 2023-06-15 15:15:47.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/FindContours.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   745738 2023-06-15 15:15:42.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/VideoPro.c
--rw-rw-rw-   0        0        0   180736 2023-06-15 15:15:49.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/VideoPro.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   489730 2023-06-15 15:15:42.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/VideoProList.c
--rw-rw-rw-   0        0        0   123904 2023-06-15 15:15:50.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/VideoProList.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0      207 2023-06-15 16:10:08.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/__init__.py
--rw-rw-rw-   0        0        0   145336 2023-06-15 15:15:42.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/add.c
--rw-rw-rw-   0        0        0    31232 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/add.cp37-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/
-drwxrwxrwx   0        0        0        0 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/
-drwxrwxrwx   0        0        0        0 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/
--rw-rw-rw-   0        0        0      735 2023-06-15 15:15:45.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     2036 2023-06-15 15:15:45.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   818283 2023-06-15 15:15:45.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.obj
--rw-rw-rw-   0        0        0      750 2023-06-15 15:15:47.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     2088 2023-06-15 15:15:47.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   424337 2023-06-15 15:15:47.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.obj
--rw-rw-rw-   0        0        0      730 2023-06-15 15:15:48.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     2016 2023-06-15 15:15:48.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0  1216299 2023-06-15 15:15:48.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.obj
--rw-rw-rw-   0        0        0      750 2023-06-15 15:15:49.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     2088 2023-06-15 15:15:49.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   836913 2023-06-15 15:15:49.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.obj
--rw-rw-rw-   0        0        0      705 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     1928 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   262194 2023-06-15 15:15:50.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.obj
--rw-rw-rw-   0        0        0      735 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     2036 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   339659 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.obj
--rw-rw-rw-   0        0        0      735 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     2036 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   420164 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.obj
--rw-rw-rw-   0        0        0      770 2023-06-15 15:15:52.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     2160 2023-06-15 15:15:52.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   907788 2023-06-15 15:15:52.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.obj
--rw-rw-rw-   0        0        0      735 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     2036 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   400510 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.obj
--rw-rw-rw-   0        0        0      715 2023-06-15 15:15:54.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.cp37-win_amd64.exp
--rw-rw-rw-   0        0        0     1964 2023-06-15 15:15:54.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.cp37-win_amd64.lib
--rw-rw-rw-   0        0        0   219786 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.obj
--rw-rw-rw-   0        0        0   197591 2023-06-15 15:15:42.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/cv_plugin.c
--rw-rw-rw-   0        0        0    44544 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/cv_plugin.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   257468 2023-06-15 15:15:42.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/cv_vdopro.c
--rw-rw-rw-   0        0        0    57856 2023-06-15 15:15:52.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/cv_vdopro.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   545156 2023-06-15 15:15:42.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/opencv_Functions.c
--rw-rw-rw-   0        0        0   132096 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/opencv_Functions.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   252864 2023-06-15 15:15:42.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/py_plugin.c
--rw-rw-rw-   0        0        0    57344 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/py_plugin.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   117874 2023-06-15 15:15:42.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/setup.c
--rw-rw-rw-   0        0        0    22528 2023-06-15 15:15:54.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox/setup.cp37-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox.egg-info/
--rw-rw-rw-   0        0        0      223 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3014 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/ShuaiToolBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 16:19:30.000000 ShuaiToolBox-1.1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      434 2023-06-15 16:19:26.000000 ShuaiToolBox-1.1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:39:07.000000 ShuaiToolBox-1.1.2.8/
+-rw-rw-rw-   0        0        0       36 2023-06-15 16:19:16.000000 ShuaiToolBox-1.1.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      223 2023-06-16 03:39:07.000000 ShuaiToolBox-1.1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 03:39:07.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/
+-rw-rw-rw-   0        0        0   123392 2023-06-16 03:38:05.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/EORmodule.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    64000 2023-06-16 03:38:06.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/FindContours.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   180736 2023-06-16 03:38:07.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/VideoPro.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   123904 2023-06-16 03:38:09.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/VideoProList.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0      236 2023-06-16 03:21:30.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/__init__.py
+-rw-rw-rw-   0        0        0    31232 2023-06-16 03:38:09.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/add.cp37-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-06-16 03:39:07.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/
+drwxrwxrwx   0        0        0        0 2023-06-16 03:39:07.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/
+drwxrwxrwx   0        0        0        0 2023-06-16 03:39:07.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/
+-rw-rw-rw-   0        0        0      735 2023-06-15 15:15:45.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     2036 2023-06-15 15:15:45.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   818283 2023-06-15 15:15:45.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.obj
+-rw-rw-rw-   0        0        0      750 2023-06-15 15:15:47.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     2088 2023-06-15 15:15:47.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   424337 2023-06-15 15:15:47.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.obj
+-rw-rw-rw-   0        0        0      730 2023-06-15 15:15:48.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     2016 2023-06-15 15:15:48.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0  1216299 2023-06-15 15:15:48.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.obj
+-rw-rw-rw-   0        0        0      750 2023-06-15 15:15:49.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     2088 2023-06-15 15:15:49.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   836913 2023-06-15 15:15:49.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.obj
+-rw-rw-rw-   0        0        0      705 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     1928 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   262194 2023-06-15 15:15:50.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.obj
+-rw-rw-rw-   0        0        0      735 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     2036 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   339659 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.obj
+-rw-rw-rw-   0        0        0      735 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     2036 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   420164 2023-06-15 15:15:51.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.obj
+-rw-rw-rw-   0        0        0      770 2023-06-15 15:15:52.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     2160 2023-06-15 15:15:52.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   907788 2023-06-15 15:15:52.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.obj
+-rw-rw-rw-   0        0        0      735 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     2036 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   400510 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.obj
+-rw-rw-rw-   0        0        0      715 2023-06-15 15:15:54.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.cp37-win_amd64.exp
+-rw-rw-rw-   0        0        0     1964 2023-06-15 15:15:54.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.cp37-win_amd64.lib
+-rw-rw-rw-   0        0        0   219786 2023-06-15 15:15:53.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.obj
+-rw-rw-rw-   0        0        0    44544 2023-06-16 03:38:10.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/cv_plugin.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    57856 2023-06-16 03:38:10.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/cv_vdopro.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   131584 2023-06-16 03:38:11.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/opencv_Functions.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    57344 2023-06-16 03:38:12.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/py_plugin.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    22528 2023-06-16 03:38:12.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox/setup.cp37-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-06-16 03:39:07.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-06-16 03:39:06.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2762 2023-06-16 03:39:06.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 03:39:06.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-16 03:39:06.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-16 03:39:06.000000 ShuaiToolBox-1.1.2.8/ShuaiToolBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 03:39:07.000000 ShuaiToolBox-1.1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      434 2023-06-16 03:38:48.000000 ShuaiToolBox-1.1.2.8/setup.py
```

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/FindContours.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoPro.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/VideoProList.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/add.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_plugin.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/cv_vdopro.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/opencv_Functions.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/py_plugin.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.cp37-win_amd64.exp` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.cp37-win_amd64.exp`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.cp37-win_amd64.lib` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.cp37-win_amd64.lib`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.obj` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox/build/temp.win-amd64-3.7/Release/setup.obj`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2.7/ShuaiToolBox.egg-info/SOURCES.txt` & `ShuaiToolBox-1.1.2.8/ShuaiToolBox.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 MANIFEST.in
 README.md
 setup.py
-ShuaiToolBox/EORmodule.c
 ShuaiToolBox/EORmodule.cp37-win_amd64.pyd
-ShuaiToolBox/FindContours.c
 ShuaiToolBox/FindContours.cp37-win_amd64.pyd
-ShuaiToolBox/VideoPro.c
 ShuaiToolBox/VideoPro.cp37-win_amd64.pyd
-ShuaiToolBox/VideoProList.c
 ShuaiToolBox/VideoProList.cp37-win_amd64.pyd
 ShuaiToolBox/__init__.py
-ShuaiToolBox/add.c
 ShuaiToolBox/add.cp37-win_amd64.pyd
-ShuaiToolBox/cv_plugin.c
 ShuaiToolBox/cv_plugin.cp37-win_amd64.pyd
-ShuaiToolBox/cv_vdopro.c
 ShuaiToolBox/cv_vdopro.cp37-win_amd64.pyd
-ShuaiToolBox/opencv_Functions.c
 ShuaiToolBox/opencv_Functions.cp37-win_amd64.pyd
-ShuaiToolBox/py_plugin.c
 ShuaiToolBox/py_plugin.cp37-win_amd64.pyd
-ShuaiToolBox/setup.c
 ShuaiToolBox/setup.cp37-win_amd64.pyd
 ShuaiToolBox.egg-info/PKG-INFO
 ShuaiToolBox.egg-info/SOURCES.txt
 ShuaiToolBox.egg-info/dependency_links.txt
 ShuaiToolBox.egg-info/requires.txt
 ShuaiToolBox.egg-info/top_level.txt
 ShuaiToolBox/build/temp.win-amd64-3.7/Release/EORmodule.cp37-win_amd64.exp
```

