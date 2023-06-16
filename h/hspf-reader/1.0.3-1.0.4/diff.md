# Comparing `tmp/hspf_reader-1.0.3.tar.gz` & `tmp/hspf_reader-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspf_reader-1.0.3.tar", last modified: Tue Feb 14 05:49:00 2023, max compression
+gzip compressed data, was "hspf_reader-1.0.4.tar", last modified: Fri Jun 16 20:42:06 2023, max compression
```

## Comparing `hspf_reader-1.0.3.tar` & `hspf_reader-1.0.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.088273 hspf_reader-1.0.3/
--rw-r--r--   0 tim       (1000) tim       (1000)      102 2023-02-12 05:11:04.000000 hspf_reader-1.0.3/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.064273 hspf_reader-1.0.3/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.068273 hspf_reader-1.0.3/.github/workflows/
--rw-r--r--   0 tim       (1000) tim       (1000)      505 2023-02-12 05:11:04.000000 hspf_reader-1.0.3/.github/workflows/clean-workflow-runs.yml
--rw-r--r--   0 tim       (1000) tim       (1000)     2121 2023-02-14 05:45:10.000000 hspf_reader-1.0.3/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      327 2022-08-30 21:28:23.000000 hspf_reader-1.0.3/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2787 2023-02-14 05:41:44.000000 hspf_reader-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)       50 2022-08-30 21:29:29.000000 hspf_reader-1.0.3/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1036 2022-09-27 21:47:42.000000 hspf_reader-1.0.3/BADGES.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      783 2023-02-14 05:42:11.000000 hspf_reader-1.0.3/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3179 2022-08-30 21:29:29.000000 hspf_reader-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1488 2022-08-30 21:29:29.000000 hspf_reader-1.0.3/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      339 2022-09-23 07:37:30.000000 hspf_reader-1.0.3/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     4111 2023-02-14 05:49:00.088273 hspf_reader-1.0.3/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     2616 2022-09-27 21:48:12.000000 hspf_reader-1.0.3/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-02-14 05:42:11.000000 hspf_reader-1.0.3/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.072273 hspf_reader-1.0.3/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-08-30 21:28:21.000000 hspf_reader-1.0.3/docs/Makefile
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.072273 hspf_reader-1.0.3/docs/_function_autosummary/
--rw-rw-r--   0 tim       (1000) tim       (1000)      135 2023-01-14 07:35:12.000000 hspf_reader-1.0.3/docs/_function_autosummary/hspf_reader.hspf_reader.about.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      129 2023-01-14 07:35:12.000000 hspf_reader-1.0.3/docs/_function_autosummary/hspf_reader.hspf_reader.hbn.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      141 2023-01-14 07:35:12.000000 hspf_reader-1.0.3/docs/_function_autosummary/hspf_reader.hspf_reader.plotgen.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      129 2023-01-14 07:35:12.000000 hspf_reader-1.0.3/docs/_function_autosummary/hspf_reader.hspf_reader.wdm.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-11-05 05:41:26.000000 hspf_reader-1.0.3/docs/authors.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      360 2023-01-07 23:58:57.000000 hspf_reader-1.0.3/docs/command_line.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     9668 2023-01-22 03:38:21.000000 hspf_reader-1.0.3/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-11-05 05:41:26.000000 hspf_reader-1.0.3/docs/contributing.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      273 2023-01-02 07:19:03.000000 hspf_reader-1.0.3/docs/function_summary.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-11-05 05:42:41.000000 hspf_reader-1.0.3/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-11-05 05:41:26.000000 hspf_reader-1.0.3/docs/license.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     5104 2022-08-30 21:28:21.000000 hspf_reader-1.0.3/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2022-11-05 05:41:26.000000 hspf_reader-1.0.3/docs/readme.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     2942 2023-02-14 05:42:11.000000 hspf_reader-1.0.3/pyproject.toml
--rw-r--r--   0 tim       (1000) tim       (1000)      261 2022-10-16 16:07:40.000000 hspf_reader-1.0.3/requirements.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-02-14 05:49:00.088273 hspf_reader-1.0.3/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      490 2023-01-22 03:38:21.000000 hspf_reader-1.0.3/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.064273 hspf_reader-1.0.3/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.072273 hspf_reader-1.0.3/src/hspf_reader/
--rw-r--r--   0 tim       (1000) tim       (1000)       67 2023-01-22 03:38:21.000000 hspf_reader-1.0.3/src/hspf_reader/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     9645 2023-02-14 05:41:44.000000 hspf_reader-1.0.3/src/hspf_reader/hspf_reader.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.076273 hspf_reader-1.0.3/src/hspf_reader.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4111 2023-02-14 05:48:59.000000 hspf_reader-1.0.3/src/hspf_reader.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     1280 2023-02-14 05:49:00.000000 hspf_reader-1.0.3/src/hspf_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-02-14 05:48:59.000000 hspf_reader-1.0.3/src/hspf_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       61 2023-02-14 05:48:59.000000 hspf_reader-1.0.3/src/hspf_reader.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      296 2023-02-14 05:48:59.000000 hspf_reader-1.0.3/src/hspf_reader.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       12 2023-02-14 05:48:59.000000 hspf_reader-1.0.3/src/hspf_reader.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 05:49:00.088273 hspf_reader-1.0.3/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:21.000000 hspf_reader-1.0.3/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      482 2023-01-22 03:38:21.000000 hspf_reader-1.0.3/tests/capture.py
--rw-r--r--   0 tim       (1000) tim       (1000)    81920 2022-08-30 21:28:23.000000 hspf_reader-1.0.3/tests/data.wdm
--rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-08-30 21:28:23.000000 hspf_reader-1.0.3/tests/data_6b_np1.hbn
--rw-rw-r--   0 tim       (1000) tim       (1000)    62131 2022-08-31 19:57:44.000000 hspf_reader-1.0.3/tests/data_plotgen.plt
--rw-rw-r--   0 tim       (1000) tim       (1000)   172779 2022-09-27 13:00:11.000000 hspf_reader-1.0.3/tests/data_wdm_1.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   264240 2022-09-27 13:13:16.000000 hspf_reader-1.0.3/tests/data_wdm_2.csv
--rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-09-21 23:17:47.000000 hspf_reader-1.0.3/tests/data_yearly.hbn
--rw-rw-r--   0 tim       (1000) tim       (1000)        0 2022-08-31 21:31:44.000000 hspf_reader-1.0.3/tests/debug_hspf_reader
--rw-r--r--   0 tim       (1000) tim       (1000)    30250 2022-09-21 23:52:50.000000 hspf_reader-1.0.3/tests/sunspot_area.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    15138 2022-09-21 23:53:58.000000 hspf_reader-1.0.3/tests/sunspot_area_with_missing.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     2486 2023-01-22 03:38:21.000000 hspf_reader-1.0.3/tests/test_hbn.py
--rw-r--r--   0 tim       (1000) tim       (1000)    35491 2023-01-22 03:38:21.000000 hspf_reader-1.0.3/tests/test_plotgen.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1239 2023-02-14 05:41:44.000000 hspf_reader-1.0.3/tests/test_wdm.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.849324 hspf_reader-1.0.4/
+-rw-r--r--   0 tim       (1000) tim       (1000)      102 2023-06-16 20:30:10.000000 hspf_reader-1.0.4/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.829324 hspf_reader-1.0.4/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.837324 hspf_reader-1.0.4/.github/workflows/
+-rw-r--r--   0 tim       (1000) tim       (1000)      501 2023-06-16 20:30:10.000000 hspf_reader-1.0.4/.github/workflows/clean-workflow-runs.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)     2121 2023-06-16 20:30:10.000000 hspf_reader-1.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      335 2023-03-05 18:51:19.000000 hspf_reader-1.0.4/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-06-16 20:30:10.000000 hspf_reader-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 tim       (1000) tim       (1000)       50 2022-08-30 21:29:29.000000 hspf_reader-1.0.4/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1036 2022-09-27 21:47:42.000000 hspf_reader-1.0.4/BADGES.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      885 2023-06-16 20:39:46.000000 hspf_reader-1.0.4/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3179 2022-08-30 21:29:29.000000 hspf_reader-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1488 2022-08-30 21:29:29.000000 hspf_reader-1.0.4/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      339 2022-09-23 07:37:30.000000 hspf_reader-1.0.4/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4171 2023-06-16 20:42:06.849324 hspf_reader-1.0.4/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     2676 2023-06-10 05:29:49.000000 hspf_reader-1.0.4/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-06-16 20:39:46.000000 hspf_reader-1.0.4/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.841324 hspf_reader-1.0.4/docs/
+-rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-08-30 21:28:21.000000 hspf_reader-1.0.4/docs/Makefile
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.841324 hspf_reader-1.0.4/docs/_function_autosummary/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      135 2023-06-16 18:22:12.000000 hspf_reader-1.0.4/docs/_function_autosummary/hspf_reader.hspf_reader.about.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      129 2023-06-16 18:22:12.000000 hspf_reader-1.0.4/docs/_function_autosummary/hspf_reader.hspf_reader.hbn.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      141 2023-06-16 18:22:12.000000 hspf_reader-1.0.4/docs/_function_autosummary/hspf_reader.hspf_reader.plotgen.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      129 2023-06-16 18:22:12.000000 hspf_reader-1.0.4/docs/_function_autosummary/hspf_reader.hspf_reader.wdm.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-11-05 05:41:26.000000 hspf_reader-1.0.4/docs/authors.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      360 2023-05-13 04:19:29.000000 hspf_reader-1.0.4/docs/command_line.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     9668 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-11-05 05:41:26.000000 hspf_reader-1.0.4/docs/contributing.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      273 2023-05-13 04:10:12.000000 hspf_reader-1.0.4/docs/function_summary.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-11-05 05:42:41.000000 hspf_reader-1.0.4/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-11-05 05:41:26.000000 hspf_reader-1.0.4/docs/license.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     5104 2022-08-30 21:28:21.000000 hspf_reader-1.0.4/docs/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2022-11-05 05:41:26.000000 hspf_reader-1.0.4/docs/readme.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2942 2023-06-16 20:39:46.000000 hspf_reader-1.0.4/pyproject.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)      261 2022-10-16 16:07:40.000000 hspf_reader-1.0.4/requirements.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-06-16 20:42:06.849324 hspf_reader-1.0.4/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      515 2023-03-01 21:50:42.000000 hspf_reader-1.0.4/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.833324 hspf_reader-1.0.4/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.841324 hspf_reader-1.0.4/src/hspf_reader/
+-rw-r--r--   0 tim       (1000) tim       (1000)       67 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/src/hspf_reader/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10202 2023-06-16 20:29:41.000000 hspf_reader-1.0.4/src/hspf_reader/hspf_reader.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.845324 hspf_reader-1.0.4/src/hspf_reader.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4171 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1280 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       61 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      296 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       12 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.849324 hspf_reader-1.0.4/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      482 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/tests/capture.py
+-rw-r--r--   0 tim       (1000) tim       (1000)    81920 2022-08-30 21:28:23.000000 hspf_reader-1.0.4/tests/data.wdm
+-rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-08-30 21:28:23.000000 hspf_reader-1.0.4/tests/data_6b_np1.hbn
+-rw-rw-r--   0 tim       (1000) tim       (1000)    62131 2022-08-31 19:57:44.000000 hspf_reader-1.0.4/tests/data_plotgen.plt
+-rw-rw-r--   0 tim       (1000) tim       (1000)   172779 2022-09-27 13:00:11.000000 hspf_reader-1.0.4/tests/data_wdm_1.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   264240 2022-09-27 13:13:16.000000 hspf_reader-1.0.4/tests/data_wdm_2.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-09-21 23:17:47.000000 hspf_reader-1.0.4/tests/data_yearly.hbn
+-rw-rw-r--   0 tim       (1000) tim       (1000)        0 2022-08-31 21:31:44.000000 hspf_reader-1.0.4/tests/debug_hspf_reader
+-rw-r--r--   0 tim       (1000) tim       (1000)    30250 2022-09-21 23:52:50.000000 hspf_reader-1.0.4/tests/sunspot_area.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    15138 2022-09-21 23:53:58.000000 hspf_reader-1.0.4/tests/sunspot_area_with_missing.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     2486 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/tests/test_hbn.py
+-rw-r--r--   0 tim       (1000) tim       (1000)    35491 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/tests/test_plotgen.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1239 2023-02-14 05:41:44.000000 hspf_reader-1.0.4/tests/test_wdm.py
```

### Comparing `hspf_reader-1.0.3/.github/workflows/python-package.yml` & `hspf_reader-1.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/.pre-commit-config.yaml` & `hspf_reader-1.0.4/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 ---
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 
-default_language_version:
-    python: python3.8
-
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
       rev: v4.4.0
       hooks:
           - id: check-case-conflict
           - id: check-docstring-first
           - id: check-executables-have-shebangs
@@ -22,27 +19,27 @@
           - id: fix-encoding-pragma
             args: [--remove]
           - id: mixed-line-ending
           - id: trailing-whitespace
             exclude: notebooks/tstoolbox_plot_bash.sh
 
     - repo: https://github.com/pappasam/toml-sort
-      rev: v0.22.3
+      rev: v0.23.1
       hooks:
           - id: toml-sort-fix
             args: [--in-place, --spaces-indent-inline-array, '4']
 
     - repo: https://github.com/adrienverge/yamllint.git
-      rev: v1.29.0
+      rev: v1.32.0
       hooks:
           - id: yamllint
             args: [--format, parsable, --strict]
 
     - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
-      rev: 0.2.2
+      rev: 0.2.3
       hooks:
           - id: yamlfmt
 
     - repo: https://github.com/jumanjihouse/pre-commit-hooks
       rev: 3.0.0
       hooks:
           - id: shellcheck
@@ -51,17 +48,18 @@
     - repo: https://github.com/lovesegfault/beautysh
       rev: v6.2.1
       hooks:
           - id: beautysh
             args: [--indent-size, '4']
 
     - repo: https://github.com/psf/black
-      rev: 23.1.0
+      rev: 23.3.0
       hooks:
           - id: black
+          - id: black-jupyter
 
     - repo: https://github.com/pycqa/isort
       rev: 5.12.0
       hooks:
           - id: isort
             name: isort (python)
             args: [--profile, black, --filter-files]
@@ -70,33 +68,28 @@
             types: [cython]
             args: [--profile, black, --filter-files]
           - id: isort
             name: isort (pyi)
             types: [pyi]
             args: [--profile, black, --filter-files]
 
-    - repo: https://github.com/dfm/black_nbconvert
-      rev: v0.4.0
-      hooks:
-          - id: black_nbconvert
-
     - repo: https://github.com/asottile/blacken-docs
       rev: 1.13.0
       hooks:
           - id: blacken-docs
 
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.3.1
+      rev: v3.6.0
       hooks:
           - id: pyupgrade
 
     - repo: https://github.com/commitizen-tools/commitizen
-      rev: v2.41.0
+      rev: 3.2.2
       hooks:
           - id: commitizen
             stages: [commit-msg]
 
     - repo: https://github.com/mwouts/jupytext
-      rev: v1.14.4
+      rev: v1.14.6
       hooks:
           - id: jupytext
             args: [--from, ipynb, --to, auto:percent, --sync]
```

### Comparing `hspf_reader-1.0.3/BADGES.rst` & `hspf_reader-1.0.4/BADGES.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/CHANGELOG.md` & `hspf_reader-1.0.4/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v1.0.4 (2023-06-16)
+
+### Fix
+
+- isolated command line functions so not imported by other packages
+
 ## v1.0.3 (2023-02-14)
 
 ### Refactor
 
 - small refactors
 
 ## 1.0.2 (2023-02-04)
```

### Comparing `hspf_reader-1.0.3/CONTRIBUTING.rst` & `hspf_reader-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/LICENSE.txt` & `hspf_reader-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/PKG-INFO` & `hspf_reader-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspf_reader
-Version: 1.0.3
+Version: 1.0.4
 Summary: Command line script and Python library to read HSPF WDM, binary, and plotgen time series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hspf_reader/docs/index.html#hspf_reader-documentation
 Project-URL: github, https://github.com/timcera/hspf_reader
 Project-URL: bitbucket, https://bitbucket.org/timcera/hspf_reader/src/main/
 Keywords: time-series,hspf,simulation,hydrology,hydrologic,python,cli,command line,script,cli-application
@@ -66,15 +66,25 @@
 
 Use "wdmtoolbox" to create, examine, read, and write to WDM files.
 
 Use "hspfbintoolbox" to catalog and read HSPF binary output files.
 
 Installation
 ------------
-Should be as easy as running ``pip install hspf_reader`` at any command line.
+pip
+~~~
+.. code-block:: bash
+
+    pip install hspf_reader
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge hspf_reader
 
 Usage - Command Line
 --------------------
 Just run 'hspf_reader --help' to get a list of subcommands::
 
 
     usage: hspf_reader [-h]
```

### Comparing `hspf_reader-1.0.3/README.rst` & `hspf_reader-1.0.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,25 @@
 
 Use "wdmtoolbox" to create, examine, read, and write to WDM files.
 
 Use "hspfbintoolbox" to catalog and read HSPF binary output files.
 
 Installation
 ------------
-Should be as easy as running ``pip install hspf_reader`` at any command line.
+pip
+~~~
+.. code-block:: bash
+
+    pip install hspf_reader
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge hspf_reader
 
 Usage - Command Line
 --------------------
 Just run 'hspf_reader --help' to get a list of subcommands::
 
 
     usage: hspf_reader [-h]
```

### Comparing `hspf_reader-1.0.3/docs/Makefile` & `hspf_reader-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/docs/conf.py` & `hspf_reader-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/docs/make.bat` & `hspf_reader-1.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/pyproject.toml` & `hspf_reader-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     ".ipynb_checkpoints/*"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "1.0.3"
+version = "1.0.4"
 version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.jupytext]
 formats = "ipynb,py:percent"
```

### Comparing `hspf_reader-1.0.3/src/hspf_reader/hspf_reader.py` & `hspf_reader-1.0.4/src/hspf_reader/hspf_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,171 @@
 """Collection of functions for reading different time series from HSPF."""
 
 import os.path as _os_path
 import sys as _sys
 import warnings as _warnings
 
-import cltoolbox
 import pandas as pd
-from cltoolbox.rst_text_formatter import RSTHelpFormatter
 from toolbox_utils import tsutils
 from toolbox_utils.readers.hbn import hbn_extract as _hbn
 from toolbox_utils.readers.plotgen import plotgen_extract as _plotgen
 from toolbox_utils.readers.wdm import wdm_extract as _wdm
 
 _warnings.filterwarnings("ignore")
 
 
-@cltoolbox.command()
-def about():
-    """Display version number and system information."""
-    tsutils.about(__name__)
+@tsutils.doc(tsutils.docstrings)
+def hbn(hbnpath, interval, *labels, **kwds):
+    r"""Prints out data to the screen from a HSPF binary output file.
+
+    Parameters
+    ----------
+    hbnpath : str
+        The HSPF binary output file.  This file must have been created from
+        a completed model run.
+
+    interval : str
+        One of 'yearly', 'monthly', 'daily', or 'bivl'.  The 'bivl' option
+        is a sub-daily interval defined in the UCI file.  Typically 'bivl'
+        is used for hourly output, but can be set to any value that evenly
+        divides into a day and needs to match the BIVL setting in the model
+        run.
+
+    labels : str
+        The remaining arguments uniquely identify a time-series in the
+        binary file.  The format is
+        'OPERATIONTYPE,ID,VARIABLEGROUP,VARIABLE'.
+
+        For example: 'PERLND,101,PWATER,UZS IMPLND,101,IWATER,RETS'
+
+        Leaving a section without an entry will wild card that
+        specification.  To get all the PWATER variables for PERLND 101 the
+        label would use::
+
+            PERLND,101,PWATER,
+
+        To get TAET for all PERLNDs::
 
+            PERLND,,,TAET
 
-@cltoolbox.command("plotgen", formatter_class=RSTHelpFormatter)
-def _plotgen_cli(start_date=None, end_date=None, *plotgen_args):
+        Note that there are spaces ONLY between label specifications not
+        within the labels themselves.
+
+        +-----------------------+-------------------------------+
+        | OPERATIONTYPE         | VARIABLEGROUP                 |
+        +=======================+===============================+
+        | PERLND                | ATEMP, SNOW, PWATER, SEDMNT,  |
+        |                       | PSTEMP, PWTGAS, PQUAL,        |
+        |                       | MSTLAY, PEST, NITR, PHOS,     |
+        |                       | TRACER                        |
+        +-----------------------+-------------------------------+
+        | IMPLND                | ATEMP, SNOW, IWATER, SOLIDS,  |
+        |                       | IWTGAS, IQUAL                 |
+        +-----------------------+-------------------------------+
+        | RCHRES                | HYDR, CONS, HTRCH, SEDTRN,    |
+        |                       | GQUAL, OXRX, NUTRX, PLANK,    |
+        |                       | PHCARB, INFLOW, OFLOW, ROFLOW |
+        +-----------------------+-------------------------------+
+        | BMPRAC                | Not used Have to leave        |
+        |                       | VARIABLEGROUP as a wild card. |
+        |                       | For example,                  |
+        |                       | 'BMPRAC,875,,RMVOL'           |
+        +-----------------------+-------------------------------+
+
+        The Time Series Catalog in the HSPF Manual lists all of the
+        variables in each of these VARIABLEGROUPs.  For BMPRAC, all of the
+        variables in all Groups in the Catalog are available in the unnamed
+        (blank) Group.
+
+        ID is the operation type identification number specified in the UCI
+        file.
+
+        Here, the user can specify:
+
+        - a single ID number to match (1-999)
+        - no entry, matching all ID's in the hbn file
+        - a range, specified as any combination of integers and
+          groups of integers marked as "start:end", with multiple
+          allowed sub-ranges separated by the "+" sign.
+
+        +------------------+-------------------------+
+        | Example Label ID | Expands to:             |
+        +==================+=========================+
+        | 1:10             | 1,2,3,4,5,6,7,8,9,10    |
+        +------------------+-------------------------+
+        | 11:14+19:22      | 11,12,13,14,19,20,21,22 |
+        +------------------+-------------------------+
+        | 3:5+7            | 3,4,5,7                 |
+        +------------------+-------------------------+
+
+    ${start_date}
+
+    ${end_date}
+
+    sort_columns:
+        [optional, default is False]
+
+        If set to False will maintain the columns order of the labels.  If
+        set to True will sort all columns by their columns names.
+    """
+    try:
+        start_date = kwds.pop("start_date")
+    except KeyError:
+        start_date = None
+    try:
+        end_date = kwds.pop("end_date")
+    except KeyError:
+        end_date = None
+    try:
+        sort_columns = kwds.pop("sort_columns")
+    except KeyError:
+        sort_columns = False
+    if len(kwds) > 0:
+        raise ValueError(
+            tsutils.error_wrapper(
+                f"""
+                The only allowed keywords are start_date and end_date.  You
+                have given {kwds}.
+                """
+            )
+        )
+
+    labels = tsutils.make_list(labels)
+
+    result = pd.DataFrame()
+    for lab in [labels]:
+        nts = _hbn(hbnpath, interval, lab, sort_columns=sort_columns)
+        result = result.join(nts, how="outer")
+    result = tsutils.common_kwds(result, start_date=start_date, end_date=end_date)
+    return tsutils.asbestfreq(result)
+
+
+@tsutils.doc(tsutils.docstrings)
+def plotgen(*plotgen_args, **kwds):
     """Print out plotgen data to the screen with ISO-8601 dates.
 
     Parameters
     ----------
-    *plotgen_args : str
+    plotgen_args : str
         Path and plotgen file name
         followed by space separated list of
         fields. For example::
 
             'file.plt 234 345 456'
 
             OR
-            `file.plt` can be space separated sets of 'plotgetpath,field'.
+            `file.plt` can be space separated sets of 'plotgenpath,field'.
 
             'file.plt,FIELD1 file2.plt,FIELD2 file.plt,FIELD3'
 
     ${start_date}
 
     ${end_date}
 
     """
-    return tsutils.printiso(
-        plotgen(*plotgen_args, start_date=start_date, end_date=end_date)
-    )
-
-
-@tsutils.copy_doc(_plotgen_cli)
-def plotgen(*plotgenpath, **kwds):
-    """Read plotgen file and return a pandas DataFrame."""
 
     try:
         start_date = kwds.pop("start_date")
     except KeyError:
         start_date = None
     try:
         end_date = kwds.pop("end_date")
@@ -67,15 +177,15 @@
                 f"""
                 The only allowed keywords are start_date and end_date.  You
                 have given {kwds}.
                 """
             )
         )
 
-    labels = tsutils.normalize_command_line_args(plotgenpath)
+    labels = tsutils.normalize_command_line_args(plotgen_args)
 
     result = pd.DataFrame()
     cnt = 0
     for lab in labels:
         pltpath, *fields = lab
         if fields:
             for field in fields:
@@ -88,21 +198,21 @@
                 result = result.join(nts, how="outer")
         else:
             result = _plotgen(pltpath)
         result = tsutils.common_kwds(result, start_date=start_date, end_date=end_date)
     return tsutils.asbestfreq(result)
 
 
-@cltoolbox.command("wdm", formatter_class=RSTHelpFormatter)
-def _wdm_cli(start_date=None, end_date=None, *wdmpath):
+@tsutils.doc(tsutils.docstrings)
+def wdm(*wdmpath, **kwds):
     """Print out DSN data to the screen with ISO-8601 dates.
 
     Parameters
     ----------
-    *wdmpath : str
+    wdmpath : str
         Path and WDM file name
         followed by space separated list of
         DSNs. For example::
 
             'file.wdm 234 345 456'
 
             OR
@@ -111,20 +221,14 @@
             'file.wdm,101 file2.wdm,104 file.wdm,227'
 
     ${start_date}
 
     ${end_date}
 
     """
-    return tsutils.printiso(wdm(*wdmpath, start_date=start_date, end_date=end_date))
-
-
-@tsutils.copy_doc(_wdm_cli)
-def wdm(*wdmpath, **kwds):
-    """Read WDM file and return a pandas DataFrame."""
 
     try:
         start_date = kwds.pop("start_date")
     except KeyError:
         start_date = None
     try:
         end_date = kwds.pop("end_date")
@@ -154,156 +258,61 @@
                 col_name = f"{nts.columns[0]}_{cnt}"
             nts.columns = [col_name]
             result = result.join(nts, how="outer")
     result = tsutils.common_kwds(result, start_date=start_date, end_date=end_date)
     return tsutils.asbestfreq(result)
 
 
-@cltoolbox.command("hbn", formatter_class=RSTHelpFormatter)
-def _hbn_cli(
-    hbnfilename, interval, start_date=None, end_date=None, sort_columns=False, *labels
-):
-    r"""Prints out data to the screen from a HSPF binary output file.
-
-    Parameters
-    ----------
-    hbnfilename : str
-        The HSPF binary output file.  This file must have been created from
-        a completed model run.
-
-    interval : str
-        One of 'yearly', 'monthly', 'daily', or 'bivl'.  The 'bivl' option is
-        a sub-daily interval defined in the UCI file.  Typically 'bivl' is used
-        for hourly output, but can be set to any value that evenly divides into
-        a day.
-
-    *labels : str
-        The remaining arguments uniquely identify a time-series in the
-        binary file.  The format is 'OPERATIONTYPE,ID,VARIABLEGROUP,VARIABLE'.
-
-        For example: 'PERLND,101,PWATER,UZS IMPLND,101,IWATER,RETS'
-
-        Leaving a section without an entry will wild card that
-        specification.  To get all the PWATER variables for PERLND 101 the
-        label would read:
-
-        'PERLND,101,PWATER,'
-
-        To get TAET for all PERLNDs:
-
-        'PERLND,,,TAET'
-
-        Note that there are spaces ONLY between label specifications not within
-        the labels themselves.
-
-        OPERATIONTYE can be PERLND, IMPLND, RCHRES, and BMPRAC.
-
-        ID is the operation type identification number specified in the UCI
-        file. These numbers must be in the range 1-999.
-
-        Here, the user can specify
-
-            - a single ID number to match
-            - no entry, matching any operation ID number
-            - a range, specified as any combination of simple integers and
-              groups of integers marked as "start:end", with multiple allowed
-              sub-ranges separated by the "+" sign.
-
-        Examples:
-
-            +-----------------------+-------------------------------+
-            | Label ID              | Expands to:                   |
-            +=======================+===============================+
-            | 1:10                  | 1,2,3,4,5,6,7,8,9,10          |
-            +-----------------------+-------------------------------+
-            | 101:119+221:239       | 101,102..119,221,221,...239   |
-            +-----------------------+-------------------------------+
-            | 3:5+7                 | 3,4,5,7                       |
-            +-----------------------+-------------------------------+
-
-        VARIABLEGROUP depends on OPERATIONTYPE where::
-
-            if OPERATIONTYPE is PERLND then VARIABLEGROUP can be one of
-                'ATEMP', 'SNOW', 'PWATER', 'SEDMNT', 'PSTEMP', 'PWTGAS',
-                'PQUAL', 'MSTLAY', 'PEST', 'NITR', 'PHOS', 'TRACER'
-
-            if OPERATIONTYPE is IMPLND then VARIABLEGROUP can be one of
-                'ATEMP', 'SNOW', 'IWATER', 'SOLIDS', 'IWTGAS', 'IQUAL'
-
-            if OPERATIONTYPE is RCHRES then VARIABLEGROUP can be one of
-                'HYDR', 'CONS', 'HTRCH', 'SEDTRN', 'GQUAL', 'OXRX', 'NUTRX',
-                'PLANK', 'PHCARB', 'INFLOW', 'OFLOW', 'ROFLOW'
-
-            if OPERATIONTYPE is BMPRAC then VARIABLEGROUP is not used and you
-            have to leave VARIABLEGROUP as a wild card.  For example,
-            'BMPRAC,875,,RMVOL'.
-
-        The Time Series Catalog in the HSPF Manual lists all of the variables
-        in each of these VARIABLEGROUPs.  For BMPRAC, all of the variables in
-        all Groups in the Catalog are available in the unnamed (blank) Group.
-
-    ${start_date}
-
-    ${end_date}
-
-    sort_columns:
-        [optional, default is False]
-
-        If set to False will maintain the columns order of the labels.  If set
-        to True will sort all columns by their columns names."""
-    tsutils.printiso(
-        hbn(
-            hbnfilename,
-            interval,
-            *labels,
-            start_date=start_date,
-            end_date=end_date,
-            sort_columns=sort_columns,
-        )
-    )
-
+def main():
+    """Set debug, register *_cli functions, and run cltoolbox.main function."""
+    import cltoolbox
+    from cltoolbox.rst_text_formatter import RSTHelpFormatter
 
-@tsutils.copy_doc(_hbn_cli)
-def hbn(hbnpath, interval, *labels, **kwds):
-    """Read hbn file and return a pandas DataFrame."""
+    if not _os_path.exists("debug_hspf_reader"):
+        _sys.tracebacklimit = 0
 
-    try:
-        start_date = kwds.pop("start_date")
-    except KeyError:
-        start_date = None
-    try:
-        end_date = kwds.pop("end_date")
-    except KeyError:
-        end_date = None
-    try:
-        sort_columns = kwds.pop("sort_columns")
-    except KeyError:
-        sort_columns = False
-    if len(kwds) > 0:
-        raise ValueError(
-            tsutils.error_wrapper(
-                f"""
-                The only allowed keywords are start_date and end_date.  You
-                have given {kwds}.
-                """
+    @cltoolbox.command("hbn", formatter_class=RSTHelpFormatter)
+    @tsutils.copy_doc(hbn)
+    def _hbn_cli(
+        hbnpath,
+        interval,
+        start_date=None,
+        end_date=None,
+        sort_columns=False,
+        *labels,
+    ):
+        """docstring replaced by tsutils.copy_doc"""
+        tsutils.printiso(
+            hbn(
+                hbnpath,
+                interval,
+                *labels,
+                start_date=start_date,
+                end_date=end_date,
+                sort_columns=sort_columns,
             )
         )
 
-    labels = tsutils.make_list(labels)
-
-    result = pd.DataFrame()
-    for lab in [labels]:
-        nts = _hbn(hbnpath, interval, lab, sort_columns=sort_columns)
-        result = result.join(nts, how="outer")
-    result = tsutils.common_kwds(result, start_date=start_date, end_date=end_date)
-    return tsutils.asbestfreq(result)
+    @cltoolbox.command("plotgen", formatter_class=RSTHelpFormatter)
+    @tsutils.copy_doc(plotgen)
+    def _plotgen_cli(start_date=None, end_date=None, *plotgen_args):
+        """docstring replaced by tsutils.copy_doc"""
+        tsutils.printiso(
+            plotgen(*plotgen_args, start_date=start_date, end_date=end_date)
+        )
 
+    @cltoolbox.command("wdm", formatter_class=RSTHelpFormatter)
+    @tsutils.copy_doc(wdm)
+    def _wdm_cli(start_date=None, end_date=None, *wdmpath):
+        """docstring replaced by tsutils.copy_doc"""
+        tsutils.printiso(wdm(*wdmpath, start_date=start_date, end_date=end_date))
+
+    @cltoolbox.command()
+    def about():
+        """Display version number and system information."""
+        tsutils.about(__name__)
 
-def main():
-    """Set debug and run cltoolbox.main function."""
-    if not _os_path.exists("debug_hspf_reader"):
-        _sys.tracebacklimit = 0
     cltoolbox.main()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hspf_reader-1.0.3/src/hspf_reader.egg-info/PKG-INFO` & `hspf_reader-1.0.4/src/hspf_reader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspf-reader
-Version: 1.0.3
+Version: 1.0.4
 Summary: Command line script and Python library to read HSPF WDM, binary, and plotgen time series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hspf_reader/docs/index.html#hspf_reader-documentation
 Project-URL: github, https://github.com/timcera/hspf_reader
 Project-URL: bitbucket, https://bitbucket.org/timcera/hspf_reader/src/main/
 Keywords: time-series,hspf,simulation,hydrology,hydrologic,python,cli,command line,script,cli-application
@@ -66,15 +66,25 @@
 
 Use "wdmtoolbox" to create, examine, read, and write to WDM files.
 
 Use "hspfbintoolbox" to catalog and read HSPF binary output files.
 
 Installation
 ------------
-Should be as easy as running ``pip install hspf_reader`` at any command line.
+pip
+~~~
+.. code-block:: bash
+
+    pip install hspf_reader
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge hspf_reader
 
 Usage - Command Line
 --------------------
 Just run 'hspf_reader --help' to get a list of subcommands::
 
 
     usage: hspf_reader [-h]
```

### Comparing `hspf_reader-1.0.3/src/hspf_reader.egg-info/SOURCES.txt` & `hspf_reader-1.0.4/src/hspf_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/data.wdm` & `hspf_reader-1.0.4/tests/data.wdm`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/data_6b_np1.hbn` & `hspf_reader-1.0.4/tests/data_6b_np1.hbn`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/data_plotgen.plt` & `hspf_reader-1.0.4/tests/data_plotgen.plt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/data_wdm_1.csv` & `hspf_reader-1.0.4/tests/data_wdm_1.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/data_wdm_2.csv` & `hspf_reader-1.0.4/tests/data_wdm_2.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/data_yearly.hbn` & `hspf_reader-1.0.4/tests/data_yearly.hbn`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/sunspot_area.csv` & `hspf_reader-1.0.4/tests/sunspot_area.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/sunspot_area_with_missing.csv` & `hspf_reader-1.0.4/tests/sunspot_area_with_missing.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/test_hbn.py` & `hspf_reader-1.0.4/tests/test_hbn.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/test_plotgen.py` & `hspf_reader-1.0.4/tests/test_plotgen.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.3/tests/test_wdm.py` & `hspf_reader-1.0.4/tests/test_wdm.py`

 * *Files identical despite different names*

