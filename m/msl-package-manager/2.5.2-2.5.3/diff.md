# Comparing `tmp/msl-package-manager-2.5.2.tar.gz` & `tmp/msl-package-manager-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msl-package-manager-2.5.2.tar", last modified: Mon Nov  8 02:29:34 2021, max compression
+gzip compressed data, was "msl-package-manager-2.5.3.tar", last modified: Fri Jun 16 06:21:20 2023, max compression
```

## Comparing `msl-package-manager-2.5.2.tar` & `msl-package-manager-2.5.3.tar`

### file list

```diff
@@ -1,67 +1,77 @@
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.549534 msl-package-manager-2.5.2/
--rw-rw-rw-   0        0        0       93 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     1131 2021-01-15 01:50:16.000000 msl-package-manager-2.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0       50 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2966 2021-11-08 02:29:34.549534 msl-package-manager-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1681 2021-11-08 01:57:11.000000 msl-package-manager-2.5.2/README.rst
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.479572 msl-package-manager-2.5.2/msl/
--rw-rw-rw-   0        0        0      181 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.479572 msl-package-manager-2.5.2/msl/examples/
--rw-rw-rw-   0        0        0       26 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.479572 msl-package-manager-2.5.2/msl/examples/package_manager/
--rw-rw-rw-   0        0        0        0 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/examples/package_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.499561 msl-package-manager-2.5.2/msl/package_manager/
--rw-rw-rw-   0        0        0      933 2021-11-08 02:25:38.000000 msl-package-manager-2.5.2/msl/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3077 2021-05-21 19:53:26.000000 msl-package-manager-2.5.2/msl/package_manager/authorise.py
--rw-rw-rw-   0        0        0     7256 2021-05-16 03:46:36.000000 msl-package-manager-2.5.2/msl/package_manager/cli.py
--rw-rw-rw-   0        0        0     5049 2021-05-16 03:56:49.000000 msl-package-manager-2.5.2/msl/package_manager/cli_argparse.py
--rw-rw-rw-   0        0        0     2311 2021-05-16 03:53:53.000000 msl-package-manager-2.5.2/msl/package_manager/cli_authorise.py
--rw-rw-rw-   0        0        0     2912 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/cli_create.py
--rw-rw-rw-   0        0        0     1683 2021-05-14 20:00:51.000000 msl-package-manager-2.5.2/msl/package_manager/cli_install.py
--rw-rw-rw-   0        0        0     1729 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/cli_list.py
--rw-rw-rw-   0        0        0     1501 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/cli_uninstall.py
--rw-rw-rw-   0        0        0     2335 2021-08-24 03:24:41.000000 msl-package-manager-2.5.2/msl/package_manager/cli_update.py
--rw-rw-rw-   0        0        0     8440 2021-04-25 06:32:26.000000 msl-package-manager-2.5.2/msl/package_manager/create.py
--rw-rw-rw-   0        0        0     6186 2021-10-17 22:09:48.000000 msl-package-manager-2.5.2/msl/package_manager/install.py
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.509555 msl-package-manager-2.5.2/msl/package_manager/template/
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.519549 msl-package-manager-2.5.2/msl/package_manager/template/${namespace}/
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.519549 msl-package-manager-2.5.2/msl/package_manager/template/${namespace}/${package}/
--rw-rw-rw-   0        0        0      503 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/${namespace}/${package}/__init__.py.template
--rw-rw-rw-   0        0        0      190 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/${namespace}/__init__.py.template
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.519549 msl-package-manager-2.5.2/msl/package_manager/template/${namespace}/examples/
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.519549 msl-package-manager-2.5.2/msl/package_manager/template/${namespace}/examples/${package}/
--rw-rw-rw-   0        0        0        0 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/${namespace}/examples/${package}/__init__.py.template
--rw-rw-rw-   0        0        0       26 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/${namespace}/examples/__init__.py.template
--rw-rw-rw-   0        0        0      697 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/.coveragerc
--rw-rw-rw-   0        0        0      527 2021-01-16 02:39:57.000000 msl-package-manager-2.5.2/msl/package_manager/template/.gitignore
--rw-rw-rw-   0        0        0       62 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/AUTHORS.rst
--rw-rw-rw-   0        0        0       87 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/CHANGES.rst
--rw-rw-rw-   0        0        0     1127 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/MANIFEST.in
--rw-rw-rw-   0        0        0       43 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/README.rst
--rw-rw-rw-   0        0        0    10113 2021-05-14 20:41:39.000000 msl-package-manager-2.5.2/msl/package_manager/template/condatests.py.template
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.529545 msl-package-manager-2.5.2/msl/package_manager/template/docs/
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.529545 msl-package-manager-2.5.2/msl/package_manager/template/docs/_static/
--rw-rw-rw-   0        0        0      110 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/docs/_static/README
--rw-rw-rw-   0        0        0       43 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/docs/authors.rst
--rw-rw-rw-   0        0        0       43 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/docs/changelog.rst
--rw-rw-rw-   0        0        0     6671 2021-04-24 03:07:31.000000 msl-package-manager-2.5.2/msl/package_manager/template/docs/conf.py.template
--rw-rw-rw-   0        0        0      328 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/docs/index.rst
--rw-rw-rw-   0        0        0      101 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/docs/license.rst
--rw-rw-rw-   0        0        0      488 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/setup.cfg
--rw-rw-rw-   0        0        0     6405 2021-05-02 01:55:58.000000 msl-package-manager-2.5.2/msl/package_manager/template/setup.py.template
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.529545 msl-package-manager-2.5.2/msl/package_manager/template/tests/
--rw-rw-rw-   0        0        0      122 2020-07-18 05:05:12.000000 msl-package-manager-2.5.2/msl/package_manager/template/tests/README
--rw-rw-rw-   0        0        0     4554 2021-05-14 20:00:51.000000 msl-package-manager-2.5.2/msl/package_manager/uninstall.py
--rw-rw-rw-   0        0        0    14167 2021-10-13 04:06:29.000000 msl-package-manager-2.5.2/msl/package_manager/update.py
--rw-rw-rw-   0        0        0    34633 2021-10-17 21:43:34.000000 msl-package-manager-2.5.2/msl/package_manager/utils.py
-drwxrwxrwx   0        0        0        0 2021-11-08 02:29:34.539539 msl-package-manager-2.5.2/msl_package_manager.egg-info/
--rw-rw-rw-   0        0        0     2966 2021-11-08 02:29:34.000000 msl-package-manager-2.5.2/msl_package_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1980 2021-11-08 02:29:34.000000 msl-package-manager-2.5.2/msl_package_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-08 02:29:34.000000 msl-package-manager-2.5.2/msl_package_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2021-11-08 02:29:34.000000 msl-package-manager-2.5.2/msl_package_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-11-08 02:29:34.000000 msl-package-manager-2.5.2/msl_package_manager.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       84 2021-11-08 02:29:34.000000 msl-package-manager-2.5.2/msl_package_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2021-11-08 02:29:34.000000 msl-package-manager-2.5.2/msl_package_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      392 2021-11-08 02:29:34.549534 msl-package-manager-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0     7153 2021-10-13 04:56:40.000000 msl-package-manager-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.700039 msl-package-manager-2.5.3/
+-rw-rw-rw-   0        0        0       93 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1131 2023-01-24 03:01:55.000000 msl-package-manager-2.5.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       50 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3035 2023-06-16 06:21:20.700039 msl-package-manager-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1681 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.637774 msl-package-manager-2.5.3/msl/
+-rw-rw-rw-   0        0        0      181 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.637774 msl-package-manager-2.5.3/msl/examples/
+-rw-rw-rw-   0        0        0       26 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.637774 msl-package-manager-2.5.3/msl/examples/package_manager/
+-rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/examples/package_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.653281 msl-package-manager-2.5.3/msl/package_manager/
+-rw-rw-rw-   0        0        0      955 2023-06-16 06:19:21.000000 msl-package-manager-2.5.3/msl/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3115 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/authorise.py
+-rw-rw-rw-   0        0        0     7307 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli.py
+-rw-rw-rw-   0        0        0     5042 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_argparse.py
+-rw-rw-rw-   0        0        0     2449 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_authorise.py
+-rw-rw-rw-   0        0        0     2964 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_create.py
+-rw-rw-rw-   0        0        0     1840 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_install.py
+-rw-rw-rw-   0        0        0     1760 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_list.py
+-rw-rw-rw-   0        0        0     1574 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_uninstall.py
+-rw-rw-rw-   0        0        0     2492 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_update.py
+-rw-rw-rw-   0        0        0     8417 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/create.py
+-rw-rw-rw-   0        0        0     6168 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/install.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/${package}/
+-rw-rw-rw-   0        0        0      503 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/${package}/__init__.py.template
+-rw-rw-rw-   0        0        0      190 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/__init__.py.template
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/examples/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/examples/${package}/
+-rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/examples/${package}/__init__.py.template
+-rw-rw-rw-   0        0        0       26 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/examples/__init__.py.template
+-rw-rw-rw-   0        0        0      697 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/.coveragerc
+-rw-rw-rw-   0        0        0      527 2021-01-20 21:45:34.000000 msl-package-manager-2.5.3/msl/package_manager/template/.gitignore
+-rw-rw-rw-   0        0        0       62 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/AUTHORS.rst
+-rw-rw-rw-   0        0        0      111 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/template/CHANGES.rst
+-rw-rw-rw-   0        0        0     1127 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/MANIFEST.in
+-rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/README.rst
+-rw-rw-rw-   0        0        0    10113 2021-05-16 21:00:34.000000 msl-package-manager-2.5.3/msl/package_manager/template/condatests.py.template
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.684415 msl-package-manager-2.5.3/msl/package_manager/template/docs/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.684415 msl-package-manager-2.5.3/msl/package_manager/template/docs/_static/
+-rw-rw-rw-   0        0        0      110 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/_static/README
+-rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/authors.rst
+-rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/changelog.rst
+-rw-rw-rw-   0        0        0     6671 2022-08-03 04:36:48.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/conf.py.template
+-rw-rw-rw-   0        0        0      328 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/index.rst
+-rw-rw-rw-   0        0        0      101 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/license.rst
+-rw-rw-rw-   0        0        0      488 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/setup.cfg
+-rw-rw-rw-   0        0        0     6504 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/template/setup.py.template
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.684415 msl-package-manager-2.5.3/msl/package_manager/template/tests/
+-rw-rw-rw-   0        0        0      122 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/tests/README
+-rw-rw-rw-   0        0        0     4576 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/uninstall.py
+-rw-rw-rw-   0        0        0    14636 2022-09-13 22:59:17.000000 msl-package-manager-2.5.3/msl/package_manager/update.py
+-rw-rw-rw-   0        0        0    35994 2023-06-16 05:56:00.000000 msl-package-manager-2.5.3/msl/package_manager/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.684415 msl-package-manager-2.5.3/msl_package_manager.egg-info/
+-rw-rw-rw-   0        0        0     3035 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2168 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      138 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      392 2023-06-16 06:21:20.700039 msl-package-manager-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     7303 2023-01-24 03:04:41.000000 msl-package-manager-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.700039 msl-package-manager-2.5.3/tests/
+-rw-rw-rw-   0        0        0    20633 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_cli.py
+-rw-rw-rw-   0        0        0    15288 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_create.py
+-rw-rw-rw-   0        0        0      304 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_github.py
+-rw-rw-rw-   0        0        0     2050 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_install.py
+-rw-rw-rw-   0        0        0     3610 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_issues.py
+-rw-rw-rw-   0        0        0     8258 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_log_output.py
+-rw-rw-rw-   0        0        0      304 2023-06-16 06:03:06.000000 msl-package-manager-2.5.3/tests/test_pypi.py
+-rw-rw-rw-   0        0        0     3739 2023-05-28 20:59:15.000000 msl-package-manager-2.5.3/tests/test_update.py
+-rw-rw-rw-   0        0        0     4873 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_utils.py
```

### Comparing `msl-package-manager-2.5.2/LICENSE.txt` & `msl-package-manager-2.5.3/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017 - 2021, Measurement Standards Laboratory of New Zealand
+Copyright (c) 2017 - 2023, Measurement Standards Laboratory of New Zealand
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `msl-package-manager-2.5.2/PKG-INFO` & `msl-package-manager-2.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msl-package-manager
-Version: 2.5.2
+Version: 2.5.3
 Summary: Install, uninstall, update, list and create MSL packages
 Home-page: https://github.com/MSLNZ/msl-package-manager
 Author: Measurement Standards Laboratory of New Zealand
 Author-email: info@measurement.govt.nz
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -19,18 +19,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: tests
 Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 MSL-Package-Manager
 ===================
 
 |docs| |github tests| |pypi|
@@ -58,25 +60,23 @@
 * colorama_
 
 Documentation
 -------------
 
 The documentation for **MSL Package Manager** can be found here_.
 
-.. |docs| image:: https://readthedocs.org/projects/msl-package-manager/badge/?version=stable
+.. |docs| image:: https://readthedocs.org/projects/msl-package-manager/badge/?version=latest
    :target: https://msl-package-manager.readthedocs.io/en/stable/
    :alt: Documentation Status
    :scale: 100%
 
 .. |github tests| image:: https://github.com/MSLNZ/msl-package-manager/actions/workflows/run-tests.yml/badge.svg
    :target: https://github.com/MSLNZ/msl-package-manager/actions/workflows/run-tests.yml
 
 .. |pypi| image:: https://badge.fury.io/py/msl-package-manager.svg
    :target: https://badge.fury.io/py/msl-package-manager
 
 .. _setuptools: https://pypi.org/project/setuptools/
 .. _colorama: https://pypi.org/project/colorama/
 .. _namespace: https://packaging.python.org/guides/packaging-namespace-packages/
-.. _here: https://msl-package-manager.readthedocs.io/en/latest/
+.. _here: https://msl-package-manager.readthedocs.io/en/stable/
 .. _Measurement Standards Laboratory of New Zealand: https://measurement.govt.nz/
-
-
```

### Comparing `msl-package-manager-2.5.2/README.rst` & `msl-package-manager-2.5.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 * colorama_
 
 Documentation
 -------------
 
 The documentation for **MSL Package Manager** can be found here_.
 
-.. |docs| image:: https://readthedocs.org/projects/msl-package-manager/badge/?version=stable
+.. |docs| image:: https://readthedocs.org/projects/msl-package-manager/badge/?version=latest
    :target: https://msl-package-manager.readthedocs.io/en/stable/
    :alt: Documentation Status
    :scale: 100%
 
 .. |github tests| image:: https://github.com/MSLNZ/msl-package-manager/actions/workflows/run-tests.yml/badge.svg
    :target: https://github.com/MSLNZ/msl-package-manager/actions/workflows/run-tests.yml
 
 .. |pypi| image:: https://badge.fury.io/py/msl-package-manager.svg
    :target: https://badge.fury.io/py/msl-package-manager
 
 .. _setuptools: https://pypi.org/project/setuptools/
 .. _colorama: https://pypi.org/project/colorama/
 .. _namespace: https://packaging.python.org/guides/packaging-namespace-packages/
-.. _here: https://msl-package-manager.readthedocs.io/en/latest/
+.. _here: https://msl-package-manager.readthedocs.io/en/stable/
 .. _Measurement Standards Laboratory of New Zealand: https://measurement.govt.nz/
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/__init__.py` & `msl-package-manager-2.5.3/msl/package_manager/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,31 +2,27 @@
 Install, uninstall, update, list and create MSL packages.
 
 The following constants are available.
 """
 import re
 from collections import namedtuple
 
+from .authorise import authorise
+from .create import create
+from .install import install
+from .uninstall import uninstall
+from .update import update
+from .utils import github
+from .utils import info
+from .utils import installed
+from .utils import outdated_pypi_packages
+from .utils import pypi
+from .utils import set_log_level
+
 __author__ = 'Measurement Standards Laboratory of New Zealand'
-__copyright__ = '\xa9 2017 - 2021, ' + __author__
-__version__ = '2.5.2'
+__copyright__ = '\xa9 2017 - 2023, ' + __author__
+__version__ = '2.5.3'
 
 _v = re.search(r'(\d+)\.(\d+)\.(\d+)[.-]?(.*)', __version__).groups()
 
 version_info = namedtuple('version_info', 'major minor micro releaselevel')(int(_v[0]), int(_v[1]), int(_v[2]), 'final')
 """:obj:`~collections.namedtuple`: Contains the version information as a (major, minor, micro, releaselevel) tuple."""
-
-_PKG_NAME = 'msl-package-manager'
-
-from .utils import (
-    pypi,
-    github,
-    installed,
-    info,
-    set_log_level,
-    outdated_pypi_packages,
-)
-from .update import update
-from .create import create
-from .install import install
-from .uninstall import uninstall
-from .authorise import authorise
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/authorise.py` & `msl-package-manager-2.5.3/msl/package_manager/authorise.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Create an authorisation file for the GitHub API.
 """
-from .utils import (
-    log,
-    get_username,
-    _get_input,
-    _GITHUB_AUTH_PATH,
-)
+from .utils import _GITHUB_AUTH_PATH
+from .utils import _get_input
+from .utils import get_username
+from .utils import log
 
 WARNING_MESSAGE = """
 Your username and personal access token are saved in plain text in the
 file that is created. You should set the file permissions provided by 
 your operating system to ensure that your GitHub credentials are safe.
 """
 
@@ -75,12 +73,12 @@
         log.warning('You must enter a username. Did not create the GitHub authorisation file')
         return
 
     if not token:
         log.warning('You must enter a personal access token. Did not create the GitHub authorisation file')
         return
 
-    with open(_GITHUB_AUTH_PATH, 'w') as fp:
+    with open(_GITHUB_AUTH_PATH, mode='wt') as fp:
         fp.write(username + ':' + token)
 
     log.warning(WARNING_MESSAGE)
-    log.info('GitHub credentials were saved to ' + _GITHUB_AUTH_PATH)
+    log.info('GitHub credentials were saved to %s', _GITHUB_AUTH_PATH)
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/cli.py` & `msl-package-manager-2.5.3/msl/package_manager/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Main entry point to either :ref:`install <install-cli>`, :ref:`uninstall <uninstall-cli>`,
 :ref:`update <update-cli>`, :ref:`list <list-cli>` or :ref:`create <create-cli>`
 MSL packages using the command-line interface (CLI).
 """
+import logging
 import os
 import re
-import sys
-import logging
 import subprocess
+import sys
+
 from pkg_resources import parse_version
 
-from . import utils, __version__, _PKG_NAME
+from . import __version__
+from . import utils
+from .utils import _PKG_NAME
 
 PARSER = None
 
 _pip_options_regexg = re.compile(r'\s+(-[a-zA-Z])?,?\s+(--[-\w]+)\s+(<.*>)?\s')
 
 
 def configure_parser():
@@ -86,21 +89,21 @@
             valid_options[long] = value
 
         pip_options_copy = pip_options[:]
         for i, option in enumerate(pip_options_copy):
             if not option.startswith('-'):
                 # make sure the previous item in pip_options accepts a value
                 # if it doesn't then append the option to parsed_args.names
-                # because the name of an msl package got mistakenly added to pip_options
+                # because the name of an MSL package got mistakenly added to pip_options
                 if not valid_options.get(pip_options_copy[i-1]):
                     name = pip_options.pop(pip_options.index(option))
                     parsed_args.names.append(name)
 
             elif option not in valid_options:
-                utils.log.error('No such option for "pip {}": {}'.format(command, option))
+                utils.log.error('No such option for "pip %s": %s', command, option)
                 return False
 
             # if the pip option requires a value then make sure the value did
             # not end up in the parsed_args.names list and the value comes
             # immediately after the appropriate item in the pip_options list
             elif valid_options[option]:
                 arg_index = args.index(option) + 1
@@ -138,15 +141,16 @@
         if parsed_args.cmd in ['install', 'update', 'upgrade']:
             if not pip_options_valid('install'):
                 return
         elif parsed_args.cmd in ['uninstall', 'remove']:
             if not pip_options_valid('uninstall'):
                 return
         else:
-            utils.log.warning('The following options are ignored: ' + ', '.join(p for p in pip_options))
+            utils.log.warning('The following options are ignored: %s',
+                              ' '.join(p for p in pip_options))
 
     parsed_args.pip_options = pip_options
     return parsed_args
 
 
 def _main(*args):
     # parse the input
@@ -169,26 +173,26 @@
     if ret == 'updating_msl_package_manager':
         return
 
     if args.disable_mslpm_version_check:
         return
 
     # check if there is an update for the MSL Package Manager
-    if utils.log.level < logging.WARNING:  # do not log DEBUG messages when checking for the update
-        utils.set_log_level(logging.WARNING)
-
+    # do not log any messages when checking for the update
+    utils.set_log_level(logging.CRITICAL+1)
     pkgs = utils.pypi()
     if not pkgs:
         return
 
     latest = pkgs[_PKG_NAME]['version']
     if parse_version(latest) > parse_version(__version__):
-        utils.log.warning('You are using {0} version {1}, however, version {2} is available.\n'
+        utils.set_log_level(logging.WARNING)
+        utils.log.warning('You are using %s version %s, however, version %s is available.\n'
                           'You should consider updating via the \'msl update package-manager\''
-                          ' command.'.format(_PKG_NAME, __version__, latest))
+                          ' command.', _PKG_NAME, __version__, latest)
 
 
 def main(*args):
     """
     Main entry point to either :ref:`install <install-cli>`, :ref:`uninstall <uninstall-cli>`,
     :ref:`update <update-cli>`, :ref:`list <list-cli>` or :ref:`create <create-cli>`
     MSL packages using the CLI.
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/cli_argparse.py` & `msl-package-manager-2.5.3/msl/package_manager/cli_argparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         """
         args = self.parse_known_args()[0]
         if not args.all and not args.names:
             if not quiet:
                 non_msl_flag = ''
                 if args.cmd in ['update', 'upgrade']:
                     non_msl_flag = ' and/or the --non-msl flag'
-                log.error('You must specify the MSL package name(s) to {} or use '
-                          'the --all flag{}'.format(args.cmd, non_msl_flag))
+                log.error('You must specify the MSL package name(s) to %s or use '
+                          'the --all flag%s', args.cmd, non_msl_flag)
             return False
         return True
 
 
 def add_argument_all(parser):
     """Add an ``--all`` argument to the parser."""
     parser.add_argument(
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/cli_authorise.py` & `msl-package-manager-2.5.3/msl/package_manager/cli_authorise.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 Command line interface for the :ref:`authorise <authorise-cli>` command.
 """
-from .cli_argparse import (
-    add_argument_quiet,
-    add_argument_disable_mslpm_version_check,
-)
-from .authorise import (
-    WARNING_MESSAGE,
-    authorise,
-)
+from .authorise import WARNING_MESSAGE
+from .authorise import authorise
+from .cli_argparse import add_argument_disable_mslpm_version_check
+from .cli_argparse import add_argument_quiet
 
 HELP = 'Enable authorisation to the GitHub API.'
 
 DESCRIPTION = HELP + """
 
 When requesting information about the MSL repositories that are
 available on GitHub there is a limit to how often you can send
@@ -47,20 +43,21 @@
     add_argument_quiet(p)
     add_argument_disable_mslpm_version_check(p)
     p.set_defaults(func=execute)
 
 
 def execute(args, parser):
     """Executes the :ref:`authorise <authorise-cli>` command."""
-    print('To generate a personal access token do the following:')
+    print('For more detailed instructions on how to generate a personal access token see')
+    print('https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token')
+    print()
+    print('To generate a personal access token, perform the following steps:')
     print('  1. Login to your GitHub account')
     print('  2. Go to Settings -> Developer settings -> Personal access tokens')
     print('  3. Click "Generate new token"')
-    print('  4. In the Note field enter a description for the token (e.g., msl-package-manager)')
-    print('  5. Optional: Select the scopes that you want to associate with the token')
-    print('  6. Click "Generate token"')
-    print('  7. Copy the token to your clipboard and paste it in the terminal when asked')
-    print()
-    print('For more detailed instructions see')
-    print('https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token')
+    print('  4. In the "Note" field enter a description for the token (e.g., msl-package-manager)')
+    print('  5. Select the expiration date of your token')
+    print('  6. Optional: Select the scopes that you want to associate with the token')
+    print('  7. Click "Generate token"')
+    print('  8. Copy the token to your clipboard and paste it in the terminal when requested')
     print()
     authorise()
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/cli_create.py` & `msl-package-manager-2.5.3/msl/package_manager/cli_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 Command line interface for the :ref:`create <create-cli>` command.
 """
-from .utils import log
+from .cli_argparse import add_argument_disable_mslpm_version_check
+from .cli_argparse import add_argument_package_names
+from .cli_argparse import add_argument_quiet
+from .cli_argparse import add_argument_yes
 from .create import create
-from .cli_argparse import (
-    add_argument_package_names,
-    add_argument_yes,
-    add_argument_quiet,
-    add_argument_disable_mslpm_version_check,
-)
+from .utils import log
 
 HELP = 'Create a new package.'
 
 DESCRIPTION = HELP + """
 
 To create a new package you must specify the package name,
 and optionally, the name and email address of the author, the
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/cli_list.py` & `msl-package-manager-2.5.3/msl/package_manager/cli_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Command line interface for the :ref:`list <list-cli>` command.
 """
+from .cli_argparse import add_argument_disable_mslpm_version_check
+from .cli_argparse import add_argument_quiet
+from .cli_argparse import add_argument_update_cache
 from .utils import info
-from .cli_argparse import (
-    add_argument_update_cache,
-    add_argument_quiet,
-    add_argument_disable_mslpm_version_check,
-)
 
 HELP = 'Show the information about MSL packages.'
 
 DESCRIPTION = HELP + """
 
 The information can be either for the installed packages,  
 packages that are available as GitHub repositories, or
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/cli_update.py` & `msl-package-manager-2.5.3/msl/package_manager/cli_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 Command line interface for the :ref:`update <update-cli>` command.
 """
+from .cli_argparse import add_argument_all
+from .cli_argparse import add_argument_branch
+from .cli_argparse import add_argument_commit
+from .cli_argparse import add_argument_disable_mslpm_version_check
+from .cli_argparse import add_argument_package_names
+from .cli_argparse import add_argument_quiet
+from .cli_argparse import add_argument_tag
+from .cli_argparse import add_argument_update_cache
+from .cli_argparse import add_argument_yes
 from .update import update
-from .cli_argparse import (
-    add_argument_all,
-    add_argument_branch,
-    add_argument_package_names,
-    add_argument_tag,
-    add_argument_update_cache,
-    add_argument_yes,
-    add_argument_quiet,
-    add_argument_disable_mslpm_version_check,
-    add_argument_commit,
-)
 
 DESCRIPTION = """{} MSL packages.
 
 MSL packages are retrieved from GitHub repositories or from PyPI.
 """
 
 EXAMPLE = """All other optional arguments are passed to "pip install --upgrade".
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/create.py` & `msl-package-manager-2.5.3/msl/package_manager/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,33 +65,33 @@
 
     roots, pkg_names = [], []
     for name in _names:
         if namespace and name.lower().startswith(namespace + '-'):
             name = name[len(namespace)+1:]
 
         if name[0].isdigit():
-            utils.log.warning('A package name cannot start with a number: ignored {!r}'.format(name))
+            utils.log.warning('A package name cannot start with a number: ignored %r', name)
             continue
 
         keep = True
         for c in name:
             if not (c.isalnum() or c == '_' or c == '-'):
                 utils.log.warning('A package name can only contain letters, numbers and underscores: '
-                                  'ignored {!r}'.format(name))
+                                  'ignored %r', name)
                 keep = False
                 break
 
         if keep:
             if namespace:
                 basename = namespace + '-' + name
             else:
                 basename = name
             root = os.path.join(directory, basename)
             if os.path.isdir(root):
-                utils.log.warning('A {!r} folder already exists: ignored "{}"'.format(root, name))
+                utils.log.warning('A %r folder already exists: ignored %r', root, name)
             else:
                 roots.append(root)
                 pkg_names.append(name)
 
     if not pkg_names:
         return
 
@@ -158,15 +158,15 @@
             new_dir = msl_root + root.split(template_dir)[1]
             new_dir = new_dir.replace('${namespace}', aliases['${namespace}'])
             new_dir = new_dir.replace('${package}', aliases['${package}'])
             if not os.path.isdir(new_dir):
                 os.makedirs(new_dir)
 
             for filename in files:
-                with open(os.path.join(root, filename), 'r') as fp:
+                with open(os.path.join(root, filename), mode='rt') as fp:
                     lines = fp.read()
 
                 if not namespace:
                     if filename == '.coveragerc':
                         lines = lines.replace('omit =\n', '')
                         lines = lines.replace('${namespace}/examples/*\n', '')
                     elif filename == 'setup.cfg':
@@ -174,27 +174,27 @@
                     elif filename == 'setup.py.template':
                         lines = lines.replace('${namespace}/${package}', safe_pkg)
                         lines = lines.replace('${namespace}*', safe_pkg)
 
                 for alias in aliases:
                     lines = lines.replace(alias, aliases[alias])
 
-                with open(os.path.join(new_dir, filename.replace('.template', '')), 'w') as fp:
+                with open(os.path.join(new_dir, filename.replace('.template', '')), mode='wt') as fp:
                     fp.write(lines)
 
         if not namespace:
             # create the source folder
             src_dir = os.path.join(msl_root, package.replace('-', '_'))
             os.makedirs(src_dir)
             init = os.path.join(template_dir, '${namespace}', '${package}', '__init__.py.template')
-            with open(init, 'r') as fp:
+            with open(init, mode='rt') as fp:
                 lines = fp.read()
             for alias in aliases:
                 lines = lines.replace(alias, aliases[alias])
-            with open(os.path.join(src_dir, '__init__.py'), 'w') as fp:
+            with open(os.path.join(src_dir, '__init__.py'), mode='wt') as fp:
                 fp.write(lines)
 
         fullname = '{}-{}'.format(namespace, package) if namespace else package
         if os.path.isdir(msl_root):
-            utils.log.info('Created {} in {!r}'.format(fullname, msl_root))
+            utils.log.info('Created %s in %r', fullname, msl_root)
         else:
-            utils.log.error('Error creating {!r}'.format(fullname))
+            utils.log.error('Error creating %r', fullname)
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/install.py` & `msl-package-manager-2.5.3/msl/package_manager/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Install MSL packages.
 """
-import sys
 import subprocess
+import sys
 
 from . import utils
 
 # Fixes issue #8 (repository name != package name)
 # Not sure how to generalize a universal solution since one is free to choose
 # any repository name and package name, therefore this mapping will need to be
 # updated on a case-by-case basis in future releases of msl-package-manager
@@ -117,22 +117,22 @@
     if '--quiet' not in pip_options or '-q' not in pip_options:
         pip_options.extend(['--quiet'] * utils._pip_quiet)
     if '--disable-pip-version-check' not in pip_options:
         pip_options.append('--disable-pip-version-check')
 
     for name, values in packages.items():
         if name in pkgs_pypi and not (branch or commit or tag):
-            utils.log.debug('Installing {!r} from PyPI'.format(name))
+            utils.log.debug('Installing %r from PyPI', name)
             if values['extras_require']:
                 name += values['extras_require']
             if values['version_requested']:
                 name += values['version_requested']
             subprocess.call(exe + pip_options + [name])
         else:
-            utils.log.debug('Installing {!r} from GitHub[{}]'.format(name, github_suffix))
+            utils.log.debug('Installing %r from GitHub[%s]', name, github_suffix)
             if commit or utils.has_git:
                 repo = 'git+https://github.com/MSLNZ/{}.git@{}'.format(name, github_suffix)
             else:
                 repo = 'https://github.com/MSLNZ/{}/archive/{}.{}'.format(name, github_suffix, zip_extn)
 
             egg_name = _egg_name_map.get(name, name)
             repo += '#egg={}'.format(egg_name)
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/template/.coveragerc` & `msl-package-manager-2.5.3/msl/package_manager/template/.coveragerc`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.2/msl/package_manager/template/.gitignore` & `msl-package-manager-2.5.3/msl/package_manager/template/.gitignore`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.2/msl/package_manager/template/LICENSE.txt` & `msl-package-manager-2.5.3/msl/package_manager/template/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.2/msl/package_manager/template/condatests.py.template` & `msl-package-manager-2.5.3/msl/package_manager/template/condatests.py.template`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.2/msl/package_manager/template/docs/conf.py.template` & `msl-package-manager-2.5.3/msl/package_manager/template/docs/conf.py.template`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 release = ${package}.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/template/setup.py.template` & `msl-package-manager-2.5.3/msl/package_manager/template/setup.py.template`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import re
 import sys
 from subprocess import check_output
-from setuptools import (
-    setup,
-    find_packages,
-    Command,
-)
+
+from setuptools import Command
+from setuptools import find_packages
+from setuptools import setup
 
 
 class ApiDocs(Command):
     """
     A custom command that calls sphinx-apidoc
     see: https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html
     """
@@ -148,15 +147,15 @@
 # specify the packages that ${full-name} depends on
 install_requires = []
 
 # specify the packages that are needed for running the tests
 tests_require = ['pytest', 'pytest-cov']
 
 # specify the packages that are needed for building the docs
-docs_require = ['sphinx', 'sphinx_rtd_theme']
+docs_require = ['sphinx', 'sphinx-rtd-theme']
 
 testing = {'test', 'tests'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if testing else []
 
 needs_sphinx = {'doc', 'docs', 'apidoc', 'apidocs'}.intersection(sys.argv)
 sphinx = docs_require + install_requires if needs_sphinx else []
 
@@ -174,15 +173,19 @@
     long_description=read('README.rst'),
     platforms='any',
     license='MIT',
     classifiers=[],  # see https://pypi.python.org/pypi?%3Aaction=list_classifiers
     setup_requires=sphinx + pytest_runner,
     tests_require=tests_require,
     install_requires=install_requires,
-    extras_require={'tests': tests_require, 'docs': docs_require},
+    extras_require={
+        'tests': tests_require,
+        'docs': docs_require,
+        'dev': tests_require + docs_require,
+    },
     cmdclass={'docs': BuildDocs, 'apidocs': ApiDocs},
     packages=find_packages(include=('${namespace}*',)),
     include_package_data=True,  # includes all files specified in MANIFEST.in when building the distribution
 )
 
 if os.path.isfile(init_backup):
     os.remove(init_original)
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/uninstall.py` & `msl-package-manager-2.5.3/msl/package_manager/uninstall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Uninstall MSL packages.
 """
 import os
-import sys
 import subprocess
+import sys
+
 import pkg_resources
 
 from . import utils
 
 
 def uninstall(*names, **kwargs):
     """Uninstall MSL packages.
@@ -70,22 +71,22 @@
                 if len(split) != 2:
                     break
 
                 examples_init_file = os.path.join(dist.module_path, split[0], 'examples', '__init__.py')
                 if not os.path.isfile(examples_init_file):
                     break
 
-                with open(examples_init_file, 'rt') as fp:
+                with open(examples_init_file, mode='rt') as fp:
                     examples_init = fp.readlines()
 
                 init_file = os.path.join(dist.module_path, split[0], '__init__.py')
                 if not os.path.isfile(init_file):
                     break
 
-                with open(init_file, 'rt') as fp:
+                with open(init_file, mode='rt') as fp:
                     init = fp.readlines()
 
                 for line in init:
                     if '__path__' in line and 'pkgutil' in line:
                         return True, os.path.dirname(init_file), init, examples_init
 
         return False, None, None, None
@@ -101,11 +102,11 @@
     if '--yes' not in pip_options or '-y' not in pip_options:
         pip_options.append('--yes')
 
     for pkg in packages:
         is_namespace, path, init, examples_init = check_if_namespace_package(pkg)
         subprocess.call(exe + pip_options + [pkg])
         if is_namespace and os.path.isdir(path):
-            with open(os.path.join(path, '__init__.py'), 'wt') as fp:
+            with open(os.path.join(path, '__init__.py'), mode='wt') as fp:
                 fp.writelines(init)
-            with open(os.path.join(path, 'examples', '__init__.py'), 'wt') as fp:
+            with open(os.path.join(path, 'examples', '__init__.py'), mode='wt') as fp:
                 fp.writelines(examples_init)
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/update.py` & `msl-package-manager-2.5.3/msl/package_manager/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Update MSL packages.
 """
 import os
 import re
-import sys
 import subprocess
-from pkg_resources import parse_version
+import sys
 
 from colorama import Fore
+from pkg_resources import parse_version
 
-from . import utils, _PKG_NAME
+from . import utils
+from .utils import _PKG_NAME
 
 
 def update(*names, **kwargs):
     """Update MSL packages.
 
     MSL packages can be updated from PyPI packages_ (only if a release has been
     uploaded to PyPI) or from GitHub repositories_.
@@ -104,42 +105,46 @@
 
     if not names or all_msl:
         # update all installed MSL packages only if not updating non-MSL packages
         packages = pkgs_installed if (all_msl or not include_non_msl) else {}
     else:
         packages = utils._check_wildcards_and_prefix(names, pkgs_installed)
 
-    w_non_msl = [0, 0]
+    w_non_msl = [0, 0, 0]
     if pkgs_non_msl:
         for name, values in pkgs_non_msl.items():
             w_non_msl = [
                 max(w_non_msl[0], len(name)),
-                max(w_non_msl[1], len(values['installed_version']))
+                max(w_non_msl[1], len(values['installed_version'])),
+                max(w_non_msl[2], len(values['version'])),
             ]
 
-    w = [0, 0]
+    w = [0, 0, 0]
     msl_pkgs_to_update = dict()
     for name, values in packages.items():
 
-        err_msg = 'Cannot update {!r} -- '.format(name)
+        err_msg = 'Cannot update {!r} --'.format(name)
 
         if name not in pkgs_installed:
-            utils.log.error(err_msg + 'The package is not installed')
+            utils.log.error('%s the package is not installed', err_msg)
             continue
 
         installed_version = pkgs_installed[name]['version']
+        if installed_version.endswith('+editable'):
+            utils.log.warning('Skipping %r since it is installed in editable mode', name)
+            continue
 
         # use PyPI to update the package (only if the package is available on PyPI)
         using_pypi = name in pkgs_pypi and not (tag or branch or commit)
         repo_name = pkgs_installed[name]['repo_name']
 
         # an MSL package could have been installed in "editable" mode, i.e., pip install -e .
         # and therefore it might only exist locally until it is pushed to the repository
         repo = pkgs_github.get(repo_name)
-        no_repo_err_msg = err_msg + 'The {!r} repository does not exist'.format(repo_name)
+        no_repo_err_msg = '{} the {!r} repository does not exist'.format(err_msg, repo_name)
 
         extras_require = values['extras_require'] if values.get('extras_require') is not None else ''
 
         if commit is not None:
             if not repo:
                 utils.log.error(no_repo_err_msg)
                 continue
@@ -160,91 +165,99 @@
                     'installed_version': installed_version,
                     'using_pypi': False,
                     'extras_require': extras_require,
                     'version': '[tag:{}]'.format(tag),
                     'repo_name': repo_name,
                 }
             else:
-                utils.log.error(err_msg + 'The {!r} tag does not exist'.format(tag))
+                utils.log.error('%s the %r tag does not exist', err_msg, tag)
                 continue
         elif branch is not None:
             if not repo:
                 utils.log.error(no_repo_err_msg)
                 continue
             if branch in repo['branches']:
                 msl_pkgs_to_update[name] = {
                     'installed_version': installed_version,
                     'using_pypi': False,
                     'extras_require': extras_require,
                     'version': '[branch:{}]'.format(branch),
                     'repo_name': repo_name,
                 }
             else:
-                utils.log.error(err_msg + 'The {!r} branch does not exist'.format(branch))
+                utils.log.error('%s the %r branch does not exist', err_msg, branch)
                 continue
         else:
             if using_pypi:
                 version = pkgs_pypi[name]['version']
             else:
                 if not repo:
                     utils.log.error(no_repo_err_msg)
                     continue
                 version = repo['version']
 
             if not version:
-                # a version number must exist on PyPI, so if this occurs it must be for a github repo
+                # a version number must exist on PyPI,
+                # so if this occurs it must be for a GitHub repo
                 utils.log.error(
-                    err_msg + 'The GitHub repository does not contain a release. Specify a branch, commit or tag'
+                    '%s the GitHub repository does not contain a release '
+                    '(specify a branch, commit or tag)',
+                    err_msg
                 )
                 continue
             elif values.get('version_requested'):
                 # this elif must come before the parse_version check
                 msl_pkgs_to_update[name] = {
                     'installed_version': installed_version,
                     'using_pypi': using_pypi,
                     'extras_require': extras_require,
                     'version': values['version_requested'],
                     'repo_name': repo_name,
                 }
-            elif parse_version(version) > parse_version(installed_version):
+            elif '--force-reinstall' in pip_options or \
+                    parse_version(version) > parse_version(installed_version):
                 msl_pkgs_to_update[name] = {
                     'installed_version': installed_version,
                     'using_pypi': using_pypi,
                     'extras_require': extras_require,
                     'version': version,
                     'repo_name': repo_name,
                 }
             else:
-                utils.log.warning('The {!r} package is already the latest [{}]'.format(name, installed_version))
+                utils.log.warning('The %r package is already the latest [%s]', name, installed_version)
                 continue
 
-        w = [max(w[0], len(name+extras_require)), max(w[1], len(installed_version))]
+        w = [
+            max(w[0], len(name+extras_require)),
+            max(w[1], len(installed_version)),
+            max(w[2], len(msl_pkgs_to_update[name]['version']))
+        ]
 
     msl_pkgs_to_update = utils._sort_packages(msl_pkgs_to_update)
 
     if not msl_pkgs_to_update and not pkgs_non_msl:
-        utils.log.info('{0}No packages to update{0}'.format(Fore.RESET))
+        utils.log.info('%sNo packages to update%s', Fore.RESET, Fore.RESET)
         return
 
     msg = ''
     if msl_pkgs_to_update:
         msg += '\n{}The following MSL packages will be {}UPDATED{}:\n'.format(Fore.RESET, Fore.CYAN, Fore.RESET)
         for pkg, info in msl_pkgs_to_update.items():
             pkg += info['extras_require'] + '  '
             msg += '\n  ' + pkg.ljust(w[0]+2) + info['installed_version'].ljust(w[1]) + \
-                   ' --> ' + info['version'].replace('==', '') + \
+                   ' --> ' + info['version'].replace('==', '').ljust(w[2]) + \
                    '  [{}]'.format('PyPI' if info['using_pypi'] else 'GitHub')
 
     if pkgs_non_msl:
         if msg:
             msg += '\n'
         msg += '\n{}The following non-MSL packages will be {}UPDATED{}:\n'.format(Fore.RESET, Fore.CYAN, Fore.RESET)
         for pkg, info in pkgs_non_msl.items():
-            msg += '\n    ' + pkg.ljust(w_non_msl[0]+2) + info['installed_version'].ljust(w_non_msl[1]) + \
-                   ' --> ' + info['version'] + '  [PyPI]'
+            msg += '\n  ' + pkg.ljust(w_non_msl[0]+2) + info['installed_version'].ljust(w_non_msl[1]) + \
+                   ' --> ' + info['version'].ljust(w_non_msl[2]) + '  [PyPI]'
 
     utils.log.info(msg)
     if not (yes or utils._ask_proceed()):
         return
 
     utils.log.info('')
 
@@ -263,21 +276,21 @@
         pip_options.extend(['--quiet'] * utils._pip_quiet)
     if '--disable-pip-version-check' not in pip_options:
         pip_options.append('--disable-pip-version-check')
 
     # install MSL packages
     for pkg, info in msl_pkgs_to_update.items():
         if info['using_pypi']:
-            utils.log.debug('Updating {!r} from PyPI'.format(pkg))
+            utils.log.debug('Updating %r from PyPI', pkg)
             if info['version'] and info['version'][0] not in '<!=>~':
                 info['version'] = '==' + info['version']
             package = [pkg + info['extras_require'] + info['version']]
             pip_github_options = []
         else:
-            utils.log.debug('Updating {!r} from GitHub[{}]'.format(pkg, github_suffix))
+            utils.log.debug('Updating %r from GitHub[%s]', pkg, github_suffix)
             if commit or utils.has_git:
                 repo = 'git+https://github.com/MSLNZ/{}.git@{}'.format(info['repo_name'], github_suffix)
             else:
                 repo = 'https://github.com/MSLNZ/{}/archive/{}.{}'.format(info['repo_name'], github_suffix, zip_extn)
             repo += '#egg={}'.format(pkg)
             pip_github_options = ['--force-reinstall']
             if info['extras_require']:
@@ -307,12 +320,12 @@
         p = subprocess.Popen(exe + pip_options + packages, stderr=subprocess.PIPE)
         _, err = p.communicate()
         if err:
             message = err.decode().rstrip()
             utils.log.error(message)
             pattern = r'requires (\S+), but you have'
             for requires in re.findall(pattern, message):
-                utils.log.warning('Rolling back to {!r}'.format(requires))
+                utils.log.warning('Rolling back to %r', requires)
                 subprocess.call(exe + pip_options + [requires])
 
     if updating_msl_package_manager:
         return 'updating_msl_package_manager'
```

### Comparing `msl-package-manager-2.5.2/msl/package_manager/utils.py` & `msl-package-manager-2.5.3/msl/package_manager/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,43 +2,47 @@
 Functions for the API.
 
 .. _packages: https://pypi.org/search/?q=%22Measurement+Standards+Laboratory+of+New+Zealand%22
 .. _git: https://git-scm.com
 .. _repositories: https://github.com/MSLNZ
 .. _JSON: https://www.json.org/
 """
-import re
-import os
-import sys
-import json
-import time
-import shlex
 import base64
-import struct
+import collections
+import datetime
 import fnmatch
 import getpass
+import json
 import logging
-import textwrap
+import os
 import platform
-import datetime
-import threading
+import re
+import shlex
+import struct
 import subprocess
-import collections
-import pkg_resources
+import sys
+import textwrap
+import threading
+import time
+
 try:
     from importlib import reload
     from urllib.request import urlopen, Request, HTTPError, URLError
 except ImportError:  # then Python 2
     from imp import reload
     from urllib2 import urlopen, Request, HTTPError, URLError
 
-from colorama import Fore, Style, Back, init
-
-from . import _PKG_NAME
+import pkg_resources
+from colorama import Back
+from colorama import Fore
+from colorama import Style
+from colorama import init
+from pkg_resources import packaging
 
+_PKG_NAME = 'msl-package-manager'
 _pip_quiet = 0
 _IS_WINDOWS = sys.platform == 'win32'
 
 _HOME_DIR = os.path.join(os.path.expanduser('~'), '.msl', 'package-manager')
 if not os.path.isdir(_HOME_DIR):
     os.makedirs(_HOME_DIR)
 
@@ -126,88 +130,102 @@
         return packages
 
     def fetch(url_suffix):
         url = 'https://api.github.com' + url_suffix
         try:
             response = urlopen(Request(url, headers=headers))
         except HTTPError as err:
-            if err.code == 401:
-                msg = 'You have provided invalid authorisation information'
+            if err.code == 401 or (err.code == 403 and 'Forbidden' in err.msg):
+                msg = ('You have provided invalid authorisation credentials',)
             elif err.code == 404:
-                # Could get this error if the URL does not exist.
-                # For example, getting .../releases/latest might not exist
-                # if no releases for the repo are available yet.
-                # This not an error type that we care about.
+                # Page not found error.
+                # For example, fetching .../releases/latest might not exist
+                # if no releases for the repo are available yet. This is not
+                # (necessarily) an error; however, if the API routes change
+                # then this error would silently occur but must be fixed.
                 return dict()
             elif err.code == 403:
                 reply = fetch('/rate_limit')
-                if reply['resources']['core']['remaining'] == 0:
-                    reset = int(reply['resources']['core']['reset'])
-                    hms = datetime.datetime.fromtimestamp(reset).strftime('%H:%M:%S')
-                    msg = 'The GitHub API rate limit was exceeded. Retry again at {} or create a file\n' \
-                          'with your GitHub authorisation credentials to increase your rate limit. Run\n' \
-                          '"msl authorise --help" for more details.'.format(hms)
+                core = reply.get('resources', {}).get('core', {})
+                if core.get('remaining') == 0:
+                    reset = core.get('reset', -1)
+                    if reset > 0:
+                        hm = datetime.datetime.fromtimestamp(reset+60).strftime('%I:%M%p')
+                        msg = ('GitHub rate limit exceeded. Not all of the information could be retrieved.\n'
+                               'Retry after %s or create a file with your GitHub authorisation credentials to\n'
+                               'increase your rate limit. Run "msl authorise --help" for more details.', hm)
+                    else:
+                        msg = ("%s (no 'reset' key)", err)
                 else:
-                    msg = 'Unhandled HTTP error 403. The rate_limit was not reached...'
+                    msg = ("%s (no 'remaining' key)", err)
             else:
-                msg = 'Unhandled HTTP error...'
-            log.error('Error requesting {} from GitHub -- {}\n{}'.format(url, err, msg))
-        except URLError as err:
-            log.error('Error requesting {} from GitHub -- {}'.format(url, err))
+                msg = ('Unhandled %s', err)
+            fetch_errors[err.code] = msg
+        except URLError:
+            # Possible reasons for this error are:
+            # 1. Computer has no internet access
+            # 2. GitHub server is offline
+            # 3. The hostname for the GitHub API has changed
+            fetch_errors[0] = ('Cannot access %s', url)
         else:
             return json.loads(response.read().decode('utf-8'))
 
     def fetch_latest_release(repo_name):
         reply = fetch('/repos/MSLNZ/{}/releases/latest'.format(repo_name))
         if reply:
-            val = reply['name'] if reply['name'] else reply['tag_name']
-            val = val.replace('v', '')
+            def verify(ver):
+                # ensure that the version is valid according to PEP 440
+                try:
+                    ver = ver.lstrip('v')
+                    packaging.version.Version(ver)
+                    return ver
+                except packaging.version.InvalidVersion:
+                    return ''
+            version = verify(reply['tag_name']) or verify(reply['name'])
         else:
-            val = ''
-        pkgs[repo_name]['version'] = val
+            version = ''
+        pkgs[repo_name]['version'] = version
 
     def fetch_tags(repo_name):
         reply = fetch('/repos/MSLNZ/{}/tags'.format(repo_name))
         pkgs[repo_name]['tags'] = [tag['name'] for tag in reply] if reply else []
 
     def fetch_branches(repo_name):
         reply = fetch('/repos/MSLNZ/{}/branches'.format(repo_name))
         pkgs[repo_name]['branches'] = [branch['name'] for branch in reply] if reply else []
 
-    def reload_cache():
-        cached_pgks = _inspect_github_pypi('github', False)[0]
-        if cached_pgks:
-            return cached_pgks
-        return dict()
-
-    # check if the user specified their github authorisation credentials
-    #
-    # the os.environ option is used for CI testing and it is not the
-    # recommended way for a user to store their credentials
+    # Check if the user specified their GitHub authorisation credentials.
+    # The os.environ option is used for CI testing, it is not the
+    # recommended way for a user to store their credentials.
     auth = os.environ.get('MSL_PM_GITHUB_AUTH')
     if not auth and os.path.isfile(_GITHUB_AUTH_PATH):
-        with open(_GITHUB_AUTH_PATH, 'rb') as fp:
+        with open(_GITHUB_AUTH_PATH, mode='rb') as fp:
             line = fp.readline().strip()
             auth = base64.b64encode(line).decode('utf-8')
 
     headers = {
         'User-Agent': _PKG_NAME + '/Python',
-        'Accept': 'application/vnd.github.v3+json',
+        'Accept': 'application/vnd.github+json',
     }
     if auth:
         headers['Authorization'] = 'Basic ' + auth
 
     log.debug('Getting the repositories from GitHub')
 
-    # when more than 100 repos exist we'll need to use ?per_page=100&page=2
-    repos = fetch('/orgs/MSLNZ/repos?per_page=100')
+    fetch_errors = {}
+
+    # when more than 100 repos exist we'll need to also fetch "?per_page=100&page=2"
+    repos = fetch('/orgs/MSLNZ/repos?per_page=100&page=1')
     if not repos:
         # even though updating the cache was requested just reload the cached data
-        # because github cannot be connected to right now
-        return reload_cache()
+        # because GitHub cannot be connected to right now
+        for error in fetch_errors.values():
+            log.warning(*error)
+        cache, _ = _inspect_github_pypi('github', False)
+        return cache
 
     pkgs = dict()
     for repo in repos:
         if repo['language'] == 'Python':
             if repo['description'] is None:
                 repo['description'] = ''
             pkgs[repo['name']] = {'description': repo['description']}
@@ -217,16 +235,27 @@
         for fcn in [fetch_latest_release, fetch_tags, fetch_branches]
         for repo_name in pkgs
     ]
     for t in threads:
         t.start()
     for t in threads:
         t.join()
+    for error in fetch_errors.values():
+        log.warning(*error)
+
+    # replace the failed requests with the cached information
+    if fetch_errors and os.path.isfile(path):
+        with open(path, mode='rt') as fp:
+            cached = json.load(fp)
+        for name, value in pkgs.items():
+            for item in ('version', 'tags', 'branches'):
+                if not value[item] and name in cached:
+                    pkgs[name][item] = cached[name][item]
 
-    with open(path, 'w') as fp:
+    with open(path, mode='wt') as fp:
         json.dump(pkgs, fp, indent=2)
 
     return _sort_packages(pkgs)
 
 
 def info(from_github=False, from_pypi=False, update_cache=False, as_json=False):
     """Show information about MSL packages.
@@ -263,15 +292,18 @@
         typ, pkgs = 'PyPI Package', pypi(update_cache=update_cache)
         if not pkgs:
             return
     else:
         typ, pkgs = 'Package', installed()
 
     if as_json:
-        log.info(Fore.RESET)
+        if not (from_github or from_pypi):
+            for name, value in pkgs.items():
+                pkgs[name]['requires'] = [str(r) for r in value['requires']]
+        log.debug(Fore.RESET)
         log.info(json.dumps(pkgs, indent=2))
         return
 
     # determine the maximum width of each column
     header = ['MSL ' + typ, 'Version', 'Description']
     w = [len(h) for h in header]
     for p in pkgs:
@@ -313,25 +345,25 @@
     """Get the information about the MSL packages that are installed.
 
     Returns
     -------
     :class:`dict`
         The information about the MSL packages that are installed.
     """
-    log.debug('Getting the packages from {}'.format(os.path.dirname(sys.executable)))
+    log.debug('Getting the packages from %s', os.path.dirname(sys.executable))
 
     gh = github(update_cache=False)
 
     # refresh the working_set
     reload(pkg_resources)
 
     pkgs = {}
     for dist in pkg_resources.working_set:
         repo_name = None
-        if dist.project_name in gh:  # the installed name might be different than the repo name
+        if dist.project_name in gh:  # the installed name might be different from the repo name
             repo_name = dist.project_name
 
         description = ''
         requires = []
         if dist.has_metadata(dist.PKG_INFO):
             for line in dist.get_metadata_lines(dist.PKG_INFO):
                 if line.startswith('Summary:'):
@@ -376,15 +408,15 @@
         The information about the PyPI packages that are outdated.
     """
     pkgs_to_update = dict()
     log.debug('Checking PyPI for all non-MSL packages that are outdated')
     try:
         output = subprocess.check_output([sys.executable, '-m', 'pip', 'list', '--outdated'])
     except subprocess.CalledProcessError as e:
-        log.error('ERROR: processing "pip list --outdated" raised -> {}'.format(e))
+        log.error('ERROR: processing "pip list --outdated" raised -> %s', e)
         return pkgs_to_update
 
     lines = output.decode().splitlines()
     if not lines:
         return pkgs_to_update
 
     header = [item.lower() for item in lines[0].split()]
@@ -460,58 +492,59 @@
         The information about the MSL packages_ that are available on PyPI.
     """
     packages, path = _inspect_github_pypi('pypi', update_cache)
     if packages:
         return packages
 
     def request(endpoint):
-        # send a request to the PyPI endpoint
+        url = 'https://pypi.org' + endpoint
         try:
-            reply = urlopen(Request('https://pypi.org' + endpoint, headers=headers))
-        except URLError as err:
-            log.error('Error requesting {!r} -- {}'.format(endpoint, err))
+            response = urlopen(Request(url, headers=headers))
+        except URLError:
+            log.error('Cannot access %s', url)
         else:
-            return reply.read().decode('utf-8')
+            return response.read().decode('utf-8')
 
     def use_json_api():
         # use the JSON API as a backup way to get the package information from PyPI
-        projects = ('msl-package-manager', 'msl-network', 'msl-loadlib', 'GTC', 'Quantity-Value')
+        projects = ('msl-package-manager', 'msl-network', 'msl-loadlib', 'msl-io' 
+                    'GTC', 'Quantity-Value')
         for project in projects:
-            reply = request('/pypi/{}/json'.format(project))
-            if reply:
-                info = json.loads(reply).get('info')
-                if info:
+            response = request('/pypi/{}/json'.format(project))
+            if response:
+                _info = json.loads(response).get('info')
+                if _info:
                     pkgs[project] = {
-                        'version': info.get('version', 'UNKNOWN'),
-                        'description': info.get('summary', 'UNKNOWN')
+                        'version': _info.get('version', 'UNKNOWN'),
+                        'description': _info.get('summary', 'UNKNOWN')
                     }
 
     pkgs = dict()
     log.debug('Getting the packages from PyPI')
     headers = {'User-Agent': _PKG_NAME + '/Python'}
 
     # use the /search endpoint before the /json endpoint since searching does not
     # depend on knowing in advance what MSL packages are available on PyPI
     reply = request('/search/?q=%22Measurement+Standards+Laboratory+of+New+Zealand%22&o=')
     if reply:
         items = re.findall(
             r'<span class="package-snippet__name">(?P<name>.+)</span>\s+'
             r'<span class="package-snippet__version">(?P<version>.+)</span>\s+'
-            r'<span class="package-snippet__released">.+\s+(?P<released>.+)\s+.+\s+.+\s+'
+            r'<span class="package-snippet__created">.+\s+(?P<created>.+)\s+.+\s+.+\s+'
             r'<p class="package-snippet__description">(?P<description>.+)</p>',
             reply,
         )
         for item in items:
-            name, version, released, description = item
+            name, version, created, description = item
             pkgs[name] = {
                 'version': version,
                 'description': description,
             }
         if not pkgs:
-            log.critical('PyPI regex pattern is invalid for the /search endpoint')
+            log.warning('The regex pattern is invalid for the /search route, using /json instead')
             use_json_api()
     else:
         use_json_api()
 
     if not pkgs:
         return _inspect_github_pypi('pypi', False)[0]
 
@@ -547,30 +580,30 @@
     """Ask whether to proceed with the command.
 
     Returns
     -------
     :class:`bool`
         Whether to proceed.
     """
-    ask = '\nProceed ([y]/n)? '
+    ask = '\nProceed (Y/n)? '
     response = _get_input(ask).lower()
     while True:
         if response.startswith('y') or not response:
             return True
         elif response.startswith('n'):
             return False
         else:
             log.info('Invalid response')
             response = _get_input(ask).lower()
 
 
 def _check_kwargs(kwargs, allowed):
     for item in kwargs:
         if item not in allowed:
-            log.warning('Invalid kwarg {!r}'.format(item))
+            log.warning('Invalid kwarg %r', item)
 
 
 def _check_wildcards_and_prefix(names, pkgs):
     """Check if a Unix shell-style wildcard was used or if the package
     name starts with the msl- prefix.
 
     Parameters
@@ -589,26 +622,26 @@
     pkgs_map = dict((p.lower(), p) for p in pkgs)
     for name in names:
         found = re.search(_package_name_regex, name.lower())
         if not found:
             continue
         result = found.groupdict()
         if not result['package_name']:
-            log.error('Invalid package name {!r}'.format(name))
+            log.error('Invalid package name %r', name)
             continue
         found_it = False
         for prefix in ['', 'msl-']:
             for match in fnmatch.filter(pkgs_map, prefix+result['package_name']):
                 found_it = True
                 _packages[pkgs_map[match]] = {
                     'extras_require': result['extras_require'],
                     'version_requested': result['version_requested']
                 }
         if not found_it:
-            log.warning('No MSL packages match {!r}'.format(name))
+            log.warning('No MSL packages match %r', name)
     return _packages
 
 
 def _create_install_list(names, branch, commit, tag, update_cache):
     """Create a list of package names to ``install`` that are GitHub repositories_.
 
     Parameters
@@ -639,27 +672,27 @@
 
     if not names:  # e.g., the --all flag
         packages = dict((pkg, {'extras_require': None, 'version_requested': None})
                         for pkg in pkgs_github if pkg != _PKG_NAME and pkg.startswith('msl-'))
     else:
         packages = _check_wildcards_and_prefix(names, pkgs_github)
 
-    # the name of an installed package can be different than the repo name
+    # the name of an installed package can be different from the repo name
     repo_names = [p['repo_name'] for p in pkgs_installed.values()]
 
     pkgs = {}
     for name, value in packages.items():
         if name in pkgs_installed or name in repo_names:
-            log.warning('The {!r} package is already installed -- use the update command'.format(name))
+            log.warning('The %r package is already installed -- use the update command', name)
         elif name not in pkgs_github:
-            log.error('Cannot install {!r} -- the package does not exist'.format(name))
+            log.error('Cannot install %r -- the package does not exist', name)
         elif branch is not None and branch not in pkgs_github[name]['branches']:
-            log.error('Cannot install {!r} -- a {!r} branch does not exist'.format(name, branch))
+            log.error('Cannot install %r -- a %r branch does not exist', name, branch)
         elif tag is not None and tag not in pkgs_github[name]['tags']:
-            log.error('Cannot install {!r} -- a {!r} tag does not exist'.format(name, tag))
+            log.error('Cannot install %r -- a %r tag does not exist', name, tag)
         else:
             pkgs[name] = pkgs_github[name]
             pkgs[name]['version_requested'] = value['version_requested']
             pkgs[name]['extras_require'] = value['extras_require']
     return pkgs
 
 
@@ -683,18 +716,18 @@
         names = [pkg for pkg in pkgs_installed if pkg != _PKG_NAME]
     else:
         names = _check_wildcards_and_prefix(names, pkgs_installed)
 
     pkgs = {}
     for name in names:
         if name == _PKG_NAME:
-            log.warning('The MSL Package Manager cannot uninstall itself. '
-                        'Use "pip uninstall {}"'.format(_PKG_NAME))
+            log.warning('The MSL Package Manager cannot uninstall itself, '
+                        'run "pip uninstall %s"', _PKG_NAME)
         elif name not in pkgs_installed:
-            log.error('Cannot uninstall {!r}: The package is not installed.'.format(name))
+            log.error('Cannot uninstall %r -- the package is not installed.', name)
         else:
             pkgs[name] = pkgs_installed[name]
     return pkgs
 
 
 def _get_input(msg):
     """Get input from the user.
@@ -774,23 +807,23 @@
     else:
         assert False, '{!r} != github or pypi'.format(where)
 
     path = os.path.join(_HOME_DIR, where+'.json')
 
     cached_pgks = None
     if os.path.isfile(path):
-        with open(path, 'r') as f:
+        with open(path, mode='rt') as f:
             cached_pgks = _sort_packages(json.load(f))
 
     one_day = 60 * 60 * 24
     if (not update_cache) and (cached_pgks is not None) and (time.time() < os.path.getmtime(path) + one_day):
         # The installed() function also calls github() so this log message could be displayed twice.
         # Avoid seeing the following log message when the installed() function was previously called.
         if where == 'pypi' or not _ColourStreamHandler.previous_message.endswith(os.path.dirname(sys.executable)):
-            log.debug('Loaded the cached information about the ' + suffix)
+            log.debug('Loaded the cached information about the %s', suffix)
         return _sort_packages(cached_pgks), path
 
     return dict(), path
 
 
 def _log_install_uninstall_message(packages, action, branch=None, commit=None, tag=None, pkgs_pypi=None):
     """Print the ``install`` or ``uninstall`` summary for what is going to happen.
@@ -908,16 +941,17 @@
 def _get_terminal_size():
     """
     Taken from https://gist.github.com/jtriley/1108174
 
     getTerminalSize()
      - get width and height of console
      - works on linux,os x,windows,cygwin(windows)
+
      originally retrieved from:
-     http://stackoverflow.com/questions/566746/how-to-get-console-window-width-in-python
+     https://stackoverflow.com/questions/566746/how-to-get-console-window-width-in-python
     """
     current_os = platform.system()
     tuple_xy = None
     if current_os == 'Windows':
         tuple_xy = _get_terminal_size_windows()
         if tuple_xy is None:
             tuple_xy = _get_terminal_size_tput()
@@ -944,16 +978,15 @@
              maxx, maxy) = struct.unpack("hhhhHhhhhhh", csbi.raw)
             return right - left, bottom - top
     except:
         pass
 
 
 def _get_terminal_size_tput():
-    # get terminal width
-    # src: http://stackoverflow.com/questions/263890/how-do-i-find-the-width-height-of-a-terminal-window
+    # https://stackoverflow.com/questions/263890/how-do-i-find-the-width-height-of-a-terminal-window
     try:
         cols = int(subprocess.check_call(shlex.split('tput cols')))
         rows = int(subprocess.check_call(shlex.split('tput lines')))
         return cols, rows
     except:
         pass
```

### Comparing `msl-package-manager-2.5.2/msl_package_manager.egg-info/PKG-INFO` & `msl-package-manager-2.5.3/msl_package_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msl-package-manager
-Version: 2.5.2
+Version: 2.5.3
 Summary: Install, uninstall, update, list and create MSL packages
 Home-page: https://github.com/MSLNZ/msl-package-manager
 Author: Measurement Standards Laboratory of New Zealand
 Author-email: info@measurement.govt.nz
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -19,18 +19,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: tests
 Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 MSL-Package-Manager
 ===================
 
 |docs| |github tests| |pypi|
@@ -58,25 +60,23 @@
 * colorama_
 
 Documentation
 -------------
 
 The documentation for **MSL Package Manager** can be found here_.
 
-.. |docs| image:: https://readthedocs.org/projects/msl-package-manager/badge/?version=stable
+.. |docs| image:: https://readthedocs.org/projects/msl-package-manager/badge/?version=latest
    :target: https://msl-package-manager.readthedocs.io/en/stable/
    :alt: Documentation Status
    :scale: 100%
 
 .. |github tests| image:: https://github.com/MSLNZ/msl-package-manager/actions/workflows/run-tests.yml/badge.svg
    :target: https://github.com/MSLNZ/msl-package-manager/actions/workflows/run-tests.yml
 
 .. |pypi| image:: https://badge.fury.io/py/msl-package-manager.svg
    :target: https://badge.fury.io/py/msl-package-manager
 
 .. _setuptools: https://pypi.org/project/setuptools/
 .. _colorama: https://pypi.org/project/colorama/
 .. _namespace: https://packaging.python.org/guides/packaging-namespace-packages/
-.. _here: https://msl-package-manager.readthedocs.io/en/latest/
+.. _here: https://msl-package-manager.readthedocs.io/en/stable/
 .. _Measurement Standards Laboratory of New Zealand: https://measurement.govt.nz/
-
-
```

### Comparing `msl-package-manager-2.5.2/setup.py` & `msl-package-manager-2.5.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import re
 import sys
 from subprocess import check_output
-from setuptools import (
-    setup,
-    find_packages,
-    Command,
-)
+
+from setuptools import Command
+from setuptools import find_packages
+from setuptools import setup
 
 
 class ApiDocs(Command):
     """
     A custom command that calls sphinx-apidoc
     see: https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html
     """
@@ -146,15 +145,15 @@
 
 
 install_requires = ['setuptools', 'colorama']
 tests_require = [
     'pytest>=4.4',  # >=4.4 to support the "-p conftest" option
     'pytest-cov',
 ]
-docs_require = ['sphinx', 'sphinx_rtd_theme']
+docs_require = ['sphinx', 'sphinx-rtd-theme']
 
 testing = {'test', 'tests'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if testing else []
 
 needs_sphinx = {'doc', 'docs', 'apidoc', 'apidocs'}.intersection(sys.argv)
 sphinx = docs_require + install_requires if needs_sphinx else []
 
@@ -185,21 +184,26 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
     ],
     setup_requires=sphinx + pytest_runner,
     tests_require=tests_require,
     install_requires=install_requires,
-    extras_require={'tests': tests_require, 'docs': docs_require},
+    extras_require={
+        'tests': tests_require,
+        'docs': docs_require,
+        'dev': tests_require + docs_require,
+    },
     cmdclass={'docs': BuildDocs, 'apidocs': ApiDocs},
     entry_points={
         'console_scripts': [
             'msl = msl.package_manager.cli:main',
         ],
     },
     packages=find_packages(include=('msl*',)),
```

