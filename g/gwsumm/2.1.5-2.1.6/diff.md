# Comparing `tmp/gwsumm-2.1.5.tar.gz` & `tmp/gwsumm-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwsumm-2.1.5.tar", last modified: Mon May 22 17:37:23 2023, max compression
+gzip compressed data, was "gwsumm-2.1.6.tar", last modified: Fri Jun 16 17:19:04 2023, max compression
```

## Comparing `gwsumm-2.1.5.tar` & `gwsumm-2.1.6.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.260926 gwsumm-2.1.5/
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2021-06-17 01:35:02.000000 gwsumm-2.1.5/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)      127 2021-06-17 01:35:02.000000 gwsumm-2.1.5/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     3795 2023-05-22 17:37:23.261059 gwsumm-2.1.5/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2358 2022-11-28 23:58:07.000000 gwsumm-2.1.5/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.262081 gwsumm-2.1.5/gwsumm/
--rw-r--r--   0 egoetz     (501) staff       (20)     1030 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    28540 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      471 2023-05-22 17:37:23.262146 gwsumm-2.1.5/gwsumm/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13749 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/archive.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20413 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10802 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/channels.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14307 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/config.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.225211 gwsumm-2.1.5/gwsumm/data/
--rw-r--r--   0 egoetz     (501) staff       (20)     2098 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/data/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    18673 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/data/coherence.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8781 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/data/mathutils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6643 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/data/range.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16817 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/data/spectral.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32208 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/data/timeseries.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5424 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/data/utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1263 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/globalv.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.227415 gwsumm-2.1.5/gwsumm/html/
--rw-r--r--   0 egoetz     (501) staff       (20)     1268 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/html/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6403 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/html/bootstrap.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8700 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/html/html5.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2539 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/html/static.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.229638 gwsumm-2.1.5/gwsumm/html/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      798 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/html/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4293 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/html/tests/test_bootstrap.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6577 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/html/tests/test_html5.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1947 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/html/tests/test_static.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2116 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/io.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3832 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/mode.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.237162 gwsumm-2.1.5/gwsumm/plot/
--rw-r--r--   0 egoetz     (501) staff       (20)     2776 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    36674 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/plot/builtin.py
--rw-r--r--   0 egoetz     (501) staff       (20)    25918 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.238666 gwsumm-2.1.5/gwsumm/plot/guardian/
--rw-r--r--   0 egoetz     (501) staff       (20)      911 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/guardian/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6353 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/guardian/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7919 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/guardian/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.239504 gwsumm-2.1.5/gwsumm/plot/guardian/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/guardian/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2903 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/guardian/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8243 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/mixins.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7988 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/noisebudget.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12929 2023-05-22 17:37:07.000000 gwsumm-2.1.5/gwsumm/plot/range.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2023 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/registry.py
--rw-r--r--   0 egoetz     (501) staff       (20)    51367 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/segments.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6023 2023-02-24 01:50:34.000000 gwsumm-2.1.5/gwsumm/plot/sei.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.240740 gwsumm-2.1.5/gwsumm/plot/triggers/
--rw-r--r--   0 egoetz     (501) staff       (20)     1014 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/triggers/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9012 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/plot/triggers/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    21913 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/plot/triggers/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.241928 gwsumm-2.1.5/gwsumm/plot/triggers/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/triggers/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3902 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/triggers/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4976 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/plot/utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12263 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/segments.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.243527 gwsumm-2.1.5/gwsumm/state/
--rw-r--r--   0 egoetz     (501) staff       (20)     2023 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/state/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2034 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/state/all.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12603 2023-05-22 17:37:07.000000 gwsumm-2.1.5/gwsumm/state/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3034 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/state/registry.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.254505 gwsumm-2.1.5/gwsumm/tabs/
--rw-r--r--   0 egoetz     (501) staff       (20)     1506 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    29472 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/builtin.py
--rw-r--r--   0 egoetz     (501) staff       (20)    36855 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/tabs/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    39789 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/data.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15759 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/etg.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10248 2021-06-17 16:15:53.000000 gwsumm-2.1.5/gwsumm/tabs/fscan.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10332 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/gracedb.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14122 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/guardian.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9258 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/management.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3611 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/misc.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2107 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/registry.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16837 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tabs/sei.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4984 2022-11-28 23:58:07.000000 gwsumm-2.1.5/gwsumm/tabs/stamp.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.259741 gwsumm-2.1.5/gwsumm/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      790 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1170 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/common.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4780 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_archive.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4855 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4208 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_channels.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8768 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8903 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_data.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1803 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_mode.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10913 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4393 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_tabs.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3782 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15102 2023-03-02 22:42:00.000000 gwsumm-2.1.5/gwsumm/triggers.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1032 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/units.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6446 2021-06-17 01:35:02.000000 gwsumm-2.1.5/gwsumm/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.221042 gwsumm-2.1.5/gwsumm.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     3795 2023-05-22 17:37:23.000000 gwsumm-2.1.5/gwsumm.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2187 2023-05-22 17:37:23.000000 gwsumm-2.1.5/gwsumm.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-05-22 17:37:23.000000 gwsumm-2.1.5/gwsumm.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      204 2023-05-22 17:37:23.000000 gwsumm-2.1.5/gwsumm.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2021-06-17 16:24:33.000000 gwsumm-2.1.5/gwsumm.egg-info/not-zip-safe
--rw-r--r--   0 egoetz     (501) staff       (20)      363 2023-05-22 17:37:23.000000 gwsumm-2.1.5/gwsumm.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        7 2023-05-22 17:37:23.000000 gwsumm-2.1.5/gwsumm.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     2361 2023-05-22 17:37:23.261822 gwsumm-2.1.5/setup.cfg
--rw-r--r--   0 egoetz     (501) staff       (20)     1599 2021-06-17 01:35:02.000000 gwsumm-2.1.5/setup.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-05-22 17:37:23.260563 gwsumm-2.1.5/share/
--rw-r--r--   0 egoetz     (501) staff       (20)     3229 2021-06-17 01:35:02.000000 gwsumm-2.1.5/share/defaults.ini
--rw-r--r--   0 egoetz     (501) staff       (20)      423 2021-06-17 01:35:02.000000 gwsumm-2.1.5/share/matplotlib.ini
--rw-r--r--   0 egoetz     (501) staff       (20)    65747 2021-06-17 01:35:02.000000 gwsumm-2.1.5/versioneer.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.636814 gwsumm-2.1.6/
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2020-04-07 19:56:04.000000 gwsumm-2.1.6/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)      127 2023-03-02 18:03:30.000000 gwsumm-2.1.6/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     3795 2023-06-16 17:19:04.637083 gwsumm-2.1.6/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2358 2022-01-25 22:56:26.000000 gwsumm-2.1.6/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.639792 gwsumm-2.1.6/gwsumm/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1030 2023-03-02 18:03:30.000000 gwsumm-2.1.6/gwsumm/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    28540 2023-06-12 21:59:27.000000 gwsumm-2.1.6/gwsumm/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      471 2023-06-16 17:19:04.639985 gwsumm-2.1.6/gwsumm/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14350 2023-06-16 17:08:27.000000 gwsumm-2.1.6/gwsumm/archive.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20413 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10802 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/channels.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14307 2023-05-22 17:31:39.000000 gwsumm-2.1.6/gwsumm/config.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.609225 gwsumm-2.1.6/gwsumm/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2098 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/data/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    18673 2022-09-15 15:47:20.000000 gwsumm-2.1.6/gwsumm/data/coherence.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8781 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/data/mathutils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6643 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/data/range.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16817 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/data/spectral.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32208 2022-10-03 17:15:55.000000 gwsumm-2.1.6/gwsumm/data/timeseries.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5424 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/data/utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1263 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/globalv.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.610571 gwsumm-2.1.6/gwsumm/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1268 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/html/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6403 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/html/bootstrap.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8700 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/html/html5.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2539 2022-11-24 17:33:11.000000 gwsumm-2.1.6/gwsumm/html/static.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.612455 gwsumm-2.1.6/gwsumm/html/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      798 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/html/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4293 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/html/tests/test_bootstrap.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6577 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/html/tests/test_html5.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1947 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/html/tests/test_static.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2116 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/io.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3832 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/mode.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.616886 gwsumm-2.1.6/gwsumm/plot/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2776 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/plot/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    36674 2023-05-22 17:31:39.000000 gwsumm-2.1.6/gwsumm/plot/builtin.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    25918 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/plot/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.617807 gwsumm-2.1.6/gwsumm/plot/guardian/
+-rw-r--r--   0 egoetz     (501) staff       (20)      911 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/guardian/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6353 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/guardian/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7919 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/guardian/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.618357 gwsumm-2.1.6/gwsumm/plot/guardian/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/guardian/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2903 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/guardian/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8243 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/plot/mixins.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7988 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/plot/noisebudget.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12929 2023-05-22 17:31:47.000000 gwsumm-2.1.6/gwsumm/plot/range.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2023 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/plot/registry.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    51367 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/segments.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6023 2023-03-02 18:03:30.000000 gwsumm-2.1.6/gwsumm/plot/sei.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.619443 gwsumm-2.1.6/gwsumm/plot/triggers/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1014 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/triggers/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9012 2022-12-20 19:28:31.000000 gwsumm-2.1.6/gwsumm/plot/triggers/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    21913 2022-12-20 19:28:31.000000 gwsumm-2.1.6/gwsumm/plot/triggers/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.620133 gwsumm-2.1.6/gwsumm/plot/triggers/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/triggers/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3902 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/plot/triggers/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4976 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/plot/utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12263 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/segments.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.621770 gwsumm-2.1.6/gwsumm/state/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2023 2023-05-22 17:31:39.000000 gwsumm-2.1.6/gwsumm/state/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2034 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/state/all.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12603 2023-05-22 17:31:39.000000 gwsumm-2.1.6/gwsumm/state/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3034 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/state/registry.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.628273 gwsumm-2.1.6/gwsumm/tabs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1506 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/tabs/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    29472 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/tabs/builtin.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    36855 2023-03-02 18:03:30.000000 gwsumm-2.1.6/gwsumm/tabs/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    39789 2023-05-22 17:31:39.000000 gwsumm-2.1.6/gwsumm/tabs/data.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15759 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/tabs/etg.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10248 2022-01-25 22:56:26.000000 gwsumm-2.1.6/gwsumm/tabs/fscan.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10332 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tabs/gracedb.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14122 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/tabs/guardian.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9258 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/tabs/management.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3611 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tabs/misc.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2107 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/tabs/registry.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16837 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/tabs/sei.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4984 2022-09-15 15:47:20.000000 gwsumm-2.1.6/gwsumm/tabs/stamp.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.635324 gwsumm-2.1.6/gwsumm/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      790 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1170 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/common.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4780 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/test_archive.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4855 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4208 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/test_channels.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8768 2023-05-22 17:31:39.000000 gwsumm-2.1.6/gwsumm/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8903 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/test_data.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1803 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/test_mode.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10913 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4393 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/test_tabs.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3782 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15102 2023-03-07 00:53:43.000000 gwsumm-2.1.6/gwsumm/triggers.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1032 2020-04-07 19:56:04.000000 gwsumm-2.1.6/gwsumm/units.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6446 2021-03-09 19:10:52.000000 gwsumm-2.1.6/gwsumm/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.606342 gwsumm-2.1.6/gwsumm.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3795 2023-06-16 17:19:04.000000 gwsumm-2.1.6/gwsumm.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2187 2023-06-16 17:19:04.000000 gwsumm-2.1.6/gwsumm.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-06-16 17:19:04.000000 gwsumm-2.1.6/gwsumm.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      204 2023-06-16 17:19:04.000000 gwsumm-2.1.6/gwsumm.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2022-12-21 02:38:40.000000 gwsumm-2.1.6/gwsumm.egg-info/not-zip-safe
+-rw-r--r--   0 egoetz     (501) staff       (20)      363 2023-06-16 17:19:04.000000 gwsumm-2.1.6/gwsumm.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        7 2023-06-16 17:19:04.000000 gwsumm-2.1.6/gwsumm.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     2361 2023-06-16 17:19:04.639343 gwsumm-2.1.6/setup.cfg
+-rw-r--r--   0 egoetz     (501) staff       (20)     1599 2023-03-02 18:03:30.000000 gwsumm-2.1.6/setup.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-16 17:19:04.636356 gwsumm-2.1.6/share/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3229 2023-03-02 18:03:30.000000 gwsumm-2.1.6/share/defaults.ini
+-rw-r--r--   0 egoetz     (501) staff       (20)      423 2023-03-02 18:03:30.000000 gwsumm-2.1.6/share/matplotlib.ini
+-rw-r--r--   0 egoetz     (501) staff       (20)    65747 2023-03-02 18:03:30.000000 gwsumm-2.1.6/versioneer.py
```

### Comparing `gwsumm-2.1.5/LICENSE` & `gwsumm-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/PKG-INFO` & `gwsumm-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsumm
-Version: 2.1.5
+Version: 2.1.6
 Summary: A python toolbox used by the LIGO Scientific Collaboration for detector characterisation
 Home-page: https://gwsumm.readthedocs.io
 Author: Alex Urban, Duncan Macleod
 Author-email: alexander.urban@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwpy/gwsumm/issues
 Project-URL: Discussion Forum, https://gwdetchar.slack.com
```

### Comparing `gwsumm-2.1.5/README.rst` & `gwsumm-2.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/__init__.py` & `gwsumm-2.1.6/gwsumm/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/__main__.py` & `gwsumm-2.1.6/gwsumm/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/archive.py` & `gwsumm-2.1.6/gwsumm/archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,27 @@
             raise
         warnings.warn(f"failed to read {sourcefile} [{exc}], removing...")
         os.remove(sourcefile)
         return
 
     with File(sourcefile, 'r') as h5file:
 
+        # Make sure that each part of the archive file is not corrupted by
+        # trying to read the data. If any part is broken, delete the file and
+        # return without loading anything into the gwsumm.globalv variables
+        try:
+            # simple lambda function here to do nothing but visit each item
+            h5file.visititems(lambda name, obj: None)
+        except RuntimeError as exc:
+            if not rm_source_on_fail:
+                raise
+            warnings.warn(f"failed to read {sourcefile} [{exc}], removing...")
+            os.remove(sourcefile)
+            return
+
         # -- channels ---------------------------
 
         try:
             ctable = Table.read(h5file['channels'])
         except KeyError:  # no channels table written
             pass
         else:
```

### Comparing `gwsumm-2.1.5/gwsumm/batch.py` & `gwsumm-2.1.6/gwsumm/batch.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/channels.py` & `gwsumm-2.1.6/gwsumm/channels.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/config.py` & `gwsumm-2.1.6/gwsumm/config.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/data/__init__.py` & `gwsumm-2.1.6/gwsumm/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/data/coherence.py` & `gwsumm-2.1.6/gwsumm/data/coherence.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/data/mathutils.py` & `gwsumm-2.1.6/gwsumm/data/mathutils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/data/range.py` & `gwsumm-2.1.6/gwsumm/data/range.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/data/spectral.py` & `gwsumm-2.1.6/gwsumm/data/spectral.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/data/timeseries.py` & `gwsumm-2.1.6/gwsumm/data/timeseries.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/data/utils.py` & `gwsumm-2.1.6/gwsumm/data/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/globalv.py` & `gwsumm-2.1.6/gwsumm/globalv.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/html/__init__.py` & `gwsumm-2.1.6/gwsumm/html/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/html/bootstrap.py` & `gwsumm-2.1.6/gwsumm/html/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/html/html5.py` & `gwsumm-2.1.6/gwsumm/html/html5.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/html/static.py` & `gwsumm-2.1.6/gwsumm/html/static.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/html/tests/__init__.py` & `gwsumm-2.1.6/gwsumm/html/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/html/tests/test_bootstrap.py` & `gwsumm-2.1.6/gwsumm/html/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/html/tests/test_html5.py` & `gwsumm-2.1.6/gwsumm/html/tests/test_html5.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/html/tests/test_static.py` & `gwsumm-2.1.6/gwsumm/html/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/io.py` & `gwsumm-2.1.6/gwsumm/io.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/mode.py` & `gwsumm-2.1.6/gwsumm/mode.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/__init__.py` & `gwsumm-2.1.6/gwsumm/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/builtin.py` & `gwsumm-2.1.6/gwsumm/plot/builtin.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/core.py` & `gwsumm-2.1.6/gwsumm/plot/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/guardian/__init__.py` & `gwsumm-2.1.6/gwsumm/plot/guardian/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/guardian/__main__.py` & `gwsumm-2.1.6/gwsumm/plot/guardian/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/guardian/core.py` & `gwsumm-2.1.6/gwsumm/plot/guardian/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/guardian/tests/__init__.py` & `gwsumm-2.1.6/gwsumm/plot/guardian/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/guardian/tests/test_main.py` & `gwsumm-2.1.6/gwsumm/plot/guardian/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/mixins.py` & `gwsumm-2.1.6/gwsumm/plot/mixins.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/noisebudget.py` & `gwsumm-2.1.6/gwsumm/plot/noisebudget.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/range.py` & `gwsumm-2.1.6/gwsumm/plot/range.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/registry.py` & `gwsumm-2.1.6/gwsumm/plot/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/segments.py` & `gwsumm-2.1.6/gwsumm/plot/segments.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/sei.py` & `gwsumm-2.1.6/gwsumm/plot/sei.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/triggers/__init__.py` & `gwsumm-2.1.6/gwsumm/plot/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/triggers/__main__.py` & `gwsumm-2.1.6/gwsumm/plot/triggers/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/triggers/core.py` & `gwsumm-2.1.6/gwsumm/plot/triggers/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/triggers/tests/__init__.py` & `gwsumm-2.1.6/gwsumm/plot/triggers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/triggers/tests/test_main.py` & `gwsumm-2.1.6/gwsumm/plot/triggers/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/plot/utils.py` & `gwsumm-2.1.6/gwsumm/plot/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/segments.py` & `gwsumm-2.1.6/gwsumm/segments.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/state/__init__.py` & `gwsumm-2.1.6/gwsumm/state/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/state/all.py` & `gwsumm-2.1.6/gwsumm/state/all.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/state/core.py` & `gwsumm-2.1.6/gwsumm/state/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/state/registry.py` & `gwsumm-2.1.6/gwsumm/state/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/__init__.py` & `gwsumm-2.1.6/gwsumm/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/builtin.py` & `gwsumm-2.1.6/gwsumm/tabs/builtin.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/core.py` & `gwsumm-2.1.6/gwsumm/tabs/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/data.py` & `gwsumm-2.1.6/gwsumm/tabs/data.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/etg.py` & `gwsumm-2.1.6/gwsumm/tabs/etg.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/fscan.py` & `gwsumm-2.1.6/gwsumm/tabs/fscan.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/gracedb.py` & `gwsumm-2.1.6/gwsumm/tabs/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/guardian.py` & `gwsumm-2.1.6/gwsumm/tabs/guardian.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/management.py` & `gwsumm-2.1.6/gwsumm/tabs/management.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/misc.py` & `gwsumm-2.1.6/gwsumm/tabs/misc.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/registry.py` & `gwsumm-2.1.6/gwsumm/tabs/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/sei.py` & `gwsumm-2.1.6/gwsumm/tabs/sei.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tabs/stamp.py` & `gwsumm-2.1.6/gwsumm/tabs/stamp.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/__init__.py` & `gwsumm-2.1.6/gwsumm/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/common.py` & `gwsumm-2.1.6/gwsumm/tests/common.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_archive.py` & `gwsumm-2.1.6/gwsumm/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_batch.py` & `gwsumm-2.1.6/gwsumm/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_channels.py` & `gwsumm-2.1.6/gwsumm/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_config.py` & `gwsumm-2.1.6/gwsumm/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_data.py` & `gwsumm-2.1.6/gwsumm/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_mode.py` & `gwsumm-2.1.6/gwsumm/tests/test_mode.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_plot.py` & `gwsumm-2.1.6/gwsumm/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_tabs.py` & `gwsumm-2.1.6/gwsumm/tests/test_tabs.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/tests/test_utils.py` & `gwsumm-2.1.6/gwsumm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/triggers.py` & `gwsumm-2.1.6/gwsumm/triggers.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/units.py` & `gwsumm-2.1.6/gwsumm/units.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm/utils.py` & `gwsumm-2.1.6/gwsumm/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/gwsumm.egg-info/PKG-INFO` & `gwsumm-2.1.6/gwsumm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsumm
-Version: 2.1.5
+Version: 2.1.6
 Summary: A python toolbox used by the LIGO Scientific Collaboration for detector characterisation
 Home-page: https://gwsumm.readthedocs.io
 Author: Alex Urban, Duncan Macleod
 Author-email: alexander.urban@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwpy/gwsumm/issues
 Project-URL: Discussion Forum, https://gwdetchar.slack.com
```

### Comparing `gwsumm-2.1.5/gwsumm.egg-info/SOURCES.txt` & `gwsumm-2.1.6/gwsumm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/setup.cfg` & `gwsumm-2.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/setup.py` & `gwsumm-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/share/defaults.ini` & `gwsumm-2.1.6/share/defaults.ini`

 * *Files identical despite different names*

### Comparing `gwsumm-2.1.5/versioneer.py` & `gwsumm-2.1.6/versioneer.py`

 * *Files identical despite different names*

