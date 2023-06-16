# Comparing `tmp/dissect.thumbcache-1.4.dev2.tar.gz` & `tmp/dissect.thumbcache-1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.thumbcache-1.4.dev2.tar", last modified: Tue May 16 13:27:03 2023, max compression
+gzip compressed data, was "dissect.thumbcache-1.5.dev1.tar", last modified: Fri Jun 16 12:51:14 2023, max compression
```

## Comparing `dissect.thumbcache-1.4.dev2.tar` & `dissect.thumbcache-1.5.dev1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.923299 dissect.thumbcache-1.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-16 13:27:03.919299 dissect.thumbcache-1.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.879299 dissect.thumbcache-1.4.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.883299 dissect.thumbcache-1.4.dev2/dissect/thumbcache/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/c_thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/thumbcache_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.883299 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/extract_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/extract_with_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.883299 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 13:26:50.000000 dissect.thumbcache-1.4.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:27:03.923299 dissect.thumbcache-1.4.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.887299 dissect.thumbcache-1.4.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.879299 dissect.thumbcache-1.4.dev2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.899299 dissect.thumbcache-1.4.dev2/tests/data/windows_10/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_1280.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_1920.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_2560.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_768.db
--rw-r--r--   0 runner    (1001) docker     (123)  3145728 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_custom_stream.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.907299 dissect.thumbcache-1.4.dev2/tests/data/windows_11/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_1280.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_1920.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_2560.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_768.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_custom_stream.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.911299 dissect.thumbcache-1.4.dev2/tests/data/windows_7/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_sr.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.915299 dissect.thumbcache-1.4.dev2/tests/data/windows_81/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_1600.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.919299 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_sr.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.919299 dissect.thumbcache-1.4.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/test_thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/test_thumbcachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.145712 dissect.thumbcache-1.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-16 12:51:14.145712 dissect.thumbcache-1.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.113710 dissect.thumbcache-1.5.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.117711 dissect.thumbcache-1.5.dev1/dissect/thumbcache/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/c_thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/thumbcache_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.117711 dissect.thumbcache-1.5.dev1/dissect/thumbcache/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/tools/extract_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/tools/extract_with_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/dissect/thumbcache/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.117711 dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-16 12:51:13.000000 dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-16 12:51:14.000000 dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:51:13.000000 dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 12:51:13.000000 dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:51:13.000000 dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:51:13.000000 dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-16 12:51:00.000000 dissect.thumbcache-1.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:51:14.145712 dissect.thumbcache-1.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.121711 dissect.thumbcache-1.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.113710 dissect.thumbcache-1.5.dev1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.129711 dissect.thumbcache-1.5.dev1/tests/data/windows_10/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_1280.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_1920.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_2560.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_768.db
+-rw-r--r--   0 runner    (1001) docker     (123)  3145728 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_custom_stream.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.133712 dissect.thumbcache-1.5.dev1/tests/data/windows_11/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_1280.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_1920.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_2560.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_768.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_custom_stream.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.137712 dissect.thumbcache-1.5.dev1/tests/data/windows_7/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_7/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_7/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_7/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_7/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_7/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_7/thumbcache_sr.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.141712 dissect.thumbcache-1.5.dev1/tests/data/windows_81/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_1600.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.145712 dissect.thumbcache-1.5.dev1/tests/data/windows_vista/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_sr.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:14.145712 dissect.thumbcache-1.5.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/test_thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tests/test_thumbcachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:50:53.000000 dissect.thumbcache-1.5.dev1/tox.ini
```

### Comparing `dissect.thumbcache-1.4.dev2/LICENSE` & `dissect.thumbcache-1.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/PKG-INFO` & `dissect.thumbcache-1.5.dev1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: dissect.thumbcache
-Version: 1.4.dev2
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
-Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.thumbcache
 
 A Dissect module implementing parsers for the thumbcache of Windows systems.
 This is commonly used to see which files were opened on a system.
 
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.thumbcache/index.html).
```

### Comparing `dissect.thumbcache-1.4.dev2/README.md` & `dissect.thumbcache-1.5.dev1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: dissect.thumbcache
+Version: 1.5.dev1
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Affero General Public License v3
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
+Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: COPYRIGHT
+
 # dissect.thumbcache
 
 A Dissect module implementing parsers for the thumbcache of Windows systems.
 This is commonly used to see which files were opened on a system.
 
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.thumbcache/index.html).
```

### Comparing `dissect.thumbcache-1.4.dev2/dissect/thumbcache/c_thumbcache.py` & `dissect.thumbcache-1.5.dev1/dissect/thumbcache/c_thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/dissect/thumbcache/index.py` & `dissect.thumbcache-1.5.dev1/dissect/thumbcache/index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/dissect/thumbcache/thumbcache.py` & `dissect.thumbcache-1.5.dev1/dissect/thumbcache/thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/dissect/thumbcache/thumbcache_file.py` & `dissect.thumbcache-1.5.dev1/dissect/thumbcache/thumbcache_file.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/extract_images.py` & `dissect.thumbcache-1.5.dev1/dissect/thumbcache/tools/extract_images.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/extract_with_index.py` & `dissect.thumbcache-1.5.dev1/dissect/thumbcache/tools/extract_with_index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/utils.py` & `dissect.thumbcache-1.5.dev1/dissect/thumbcache/tools/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/PKG-INFO` & `dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 Metadata-Version: 2.1
 Name: dissect.thumbcache
-Version: 1.4.dev2
+Version: 1.5.dev1
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
 Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYRIGHT
 
 # dissect.thumbcache
```

### Comparing `dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/SOURCES.txt` & `dissect.thumbcache-1.5.dev1/dissect.thumbcache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/pyproject.toml` & `dissect.thumbcache-1.5.dev1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,25 @@
 readme = "README.md"
 requires-python = "~=3.9"
 license.text = "Affero General Public License v3"
 authors = [
   {name = "Dissect Team", email = "dissect@fox-it.com"}
 ]
 classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "Environment :: Console",
+  "Intended Audience :: Developers",
+  "Intended Audience :: Information Technology",
+  "License :: OSI Approved",
+  "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
+  "Topic :: Internet :: Log Analysis",
+  "Topic :: Scientific/Engineering :: Information Analysis",
+  "Topic :: Security",
+  "Topic :: Utilities",
 ]
 dependencies = [
     "dissect.cstruct>=3.0.dev,<4.0.dev",
     "dissect.util>=3.0.dev,<4.0.dev",
 ]
 dynamic = ["version"]
```

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_16.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_16.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_256.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_32.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_96.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_96.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_idx.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_10/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_16.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_16.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_256.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_32.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_48.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_48.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_idx.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_11/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_256.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_7/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_idx.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_7/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_256.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_32.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_idx.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_81/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_256.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_32.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_96.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_96.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_idx.db` & `dissect.thumbcache-1.5.dev1/tests/data/windows_vista/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/docs/Makefile` & `dissect.thumbcache-1.5.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/docs/conf.py` & `dissect.thumbcache-1.5.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/test_index.py` & `dissect.thumbcache-1.5.dev1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/test_thumbcache.py` & `dissect.thumbcache-1.5.dev1/tests/test_thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tests/test_thumbcachefile.py` & `dissect.thumbcache-1.5.dev1/tests/test_thumbcachefile.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev2/tox.ini` & `dissect.thumbcache-1.5.dev1/tox.ini`

 * *Files identical despite different names*

