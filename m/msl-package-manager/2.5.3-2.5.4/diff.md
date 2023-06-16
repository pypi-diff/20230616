# Comparing `tmp/msl-package-manager-2.5.3.tar.gz` & `tmp/msl-package-manager-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msl-package-manager-2.5.3.tar", last modified: Fri Jun 16 06:21:20 2023, max compression
+gzip compressed data, was "msl-package-manager-2.5.4.tar", last modified: Fri Jun 16 06:51:29 2023, max compression
```

## Comparing `msl-package-manager-2.5.3.tar` & `msl-package-manager-2.5.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.700039 msl-package-manager-2.5.3/
--rw-rw-rw-   0        0        0       93 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     1131 2023-01-24 03:01:55.000000 msl-package-manager-2.5.3/LICENSE.txt
--rw-rw-rw-   0        0        0       50 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3035 2023-06-16 06:21:20.700039 msl-package-manager-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1681 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.637774 msl-package-manager-2.5.3/msl/
--rw-rw-rw-   0        0        0      181 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.637774 msl-package-manager-2.5.3/msl/examples/
--rw-rw-rw-   0        0        0       26 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.637774 msl-package-manager-2.5.3/msl/examples/package_manager/
--rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/examples/package_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.653281 msl-package-manager-2.5.3/msl/package_manager/
--rw-rw-rw-   0        0        0      955 2023-06-16 06:19:21.000000 msl-package-manager-2.5.3/msl/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3115 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/authorise.py
--rw-rw-rw-   0        0        0     7307 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli.py
--rw-rw-rw-   0        0        0     5042 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_argparse.py
--rw-rw-rw-   0        0        0     2449 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_authorise.py
--rw-rw-rw-   0        0        0     2964 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_create.py
--rw-rw-rw-   0        0        0     1840 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_install.py
--rw-rw-rw-   0        0        0     1760 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_list.py
--rw-rw-rw-   0        0        0     1574 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_uninstall.py
--rw-rw-rw-   0        0        0     2492 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/cli_update.py
--rw-rw-rw-   0        0        0     8417 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/create.py
--rw-rw-rw-   0        0        0     6168 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/install.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/${package}/
--rw-rw-rw-   0        0        0      503 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/${package}/__init__.py.template
--rw-rw-rw-   0        0        0      190 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/__init__.py.template
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/examples/
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.668906 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/examples/${package}/
--rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/examples/${package}/__init__.py.template
--rw-rw-rw-   0        0        0       26 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/${namespace}/examples/__init__.py.template
--rw-rw-rw-   0        0        0      697 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/.coveragerc
--rw-rw-rw-   0        0        0      527 2021-01-20 21:45:34.000000 msl-package-manager-2.5.3/msl/package_manager/template/.gitignore
--rw-rw-rw-   0        0        0       62 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/AUTHORS.rst
--rw-rw-rw-   0        0        0      111 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/template/CHANGES.rst
--rw-rw-rw-   0        0        0     1127 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/MANIFEST.in
--rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/README.rst
--rw-rw-rw-   0        0        0    10113 2021-05-16 21:00:34.000000 msl-package-manager-2.5.3/msl/package_manager/template/condatests.py.template
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.684415 msl-package-manager-2.5.3/msl/package_manager/template/docs/
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.684415 msl-package-manager-2.5.3/msl/package_manager/template/docs/_static/
--rw-rw-rw-   0        0        0      110 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/_static/README
--rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/authors.rst
--rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/changelog.rst
--rw-rw-rw-   0        0        0     6671 2022-08-03 04:36:48.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/conf.py.template
--rw-rw-rw-   0        0        0      328 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/index.rst
--rw-rw-rw-   0        0        0      101 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/docs/license.rst
--rw-rw-rw-   0        0        0      488 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/setup.cfg
--rw-rw-rw-   0        0        0     6504 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/template/setup.py.template
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.684415 msl-package-manager-2.5.3/msl/package_manager/template/tests/
--rw-rw-rw-   0        0        0      122 2020-12-10 23:24:11.000000 msl-package-manager-2.5.3/msl/package_manager/template/tests/README
--rw-rw-rw-   0        0        0     4576 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/msl/package_manager/uninstall.py
--rw-rw-rw-   0        0        0    14636 2022-09-13 22:59:17.000000 msl-package-manager-2.5.3/msl/package_manager/update.py
--rw-rw-rw-   0        0        0    35994 2023-06-16 05:56:00.000000 msl-package-manager-2.5.3/msl/package_manager/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.684415 msl-package-manager-2.5.3/msl_package_manager.egg-info/
--rw-rw-rw-   0        0        0     3035 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2168 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      138 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-16 06:21:20.000000 msl-package-manager-2.5.3/msl_package_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      392 2023-06-16 06:21:20.700039 msl-package-manager-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0     7303 2023-01-24 03:04:41.000000 msl-package-manager-2.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:21:20.700039 msl-package-manager-2.5.3/tests/
--rw-rw-rw-   0        0        0    20633 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_cli.py
--rw-rw-rw-   0        0        0    15288 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_create.py
--rw-rw-rw-   0        0        0      304 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_github.py
--rw-rw-rw-   0        0        0     2050 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_install.py
--rw-rw-rw-   0        0        0     3610 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_issues.py
--rw-rw-rw-   0        0        0     8258 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_log_output.py
--rw-rw-rw-   0        0        0      304 2023-06-16 06:03:06.000000 msl-package-manager-2.5.3/tests/test_pypi.py
--rw-rw-rw-   0        0        0     3739 2023-05-28 20:59:15.000000 msl-package-manager-2.5.3/tests/test_update.py
--rw-rw-rw-   0        0        0     4873 2022-09-11 21:05:22.000000 msl-package-manager-2.5.3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.481466 msl-package-manager-2.5.4/
+-rw-rw-rw-   0        0        0       93 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1131 2023-01-24 03:01:55.000000 msl-package-manager-2.5.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       50 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3035 2023-06-16 06:51:29.481466 msl-package-manager-2.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1681 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.372489 msl-package-manager-2.5.4/msl/
+-rw-rw-rw-   0        0        0      181 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.372489 msl-package-manager-2.5.4/msl/examples/
+-rw-rw-rw-   0        0        0       26 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.372489 msl-package-manager-2.5.4/msl/examples/package_manager/
+-rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/examples/package_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.404599 msl-package-manager-2.5.4/msl/package_manager/
+-rw-rw-rw-   0        0        0      955 2023-06-16 06:43:49.000000 msl-package-manager-2.5.4/msl/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3115 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/authorise.py
+-rw-rw-rw-   0        0        0     7307 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/cli.py
+-rw-rw-rw-   0        0        0     5042 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/cli_argparse.py
+-rw-rw-rw-   0        0        0     2449 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/cli_authorise.py
+-rw-rw-rw-   0        0        0     2964 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/cli_create.py
+-rw-rw-rw-   0        0        0     1840 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/cli_install.py
+-rw-rw-rw-   0        0        0     1760 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/cli_list.py
+-rw-rw-rw-   0        0        0     1574 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/cli_uninstall.py
+-rw-rw-rw-   0        0        0     2492 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/cli_update.py
+-rw-rw-rw-   0        0        0     8417 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/create.py
+-rw-rw-rw-   0        0        0     6168 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/install.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.420238 msl-package-manager-2.5.4/msl/package_manager/template/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.420238 msl-package-manager-2.5.4/msl/package_manager/template/${namespace}/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.420238 msl-package-manager-2.5.4/msl/package_manager/template/${namespace}/${package}/
+-rw-rw-rw-   0        0        0      503 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/${namespace}/${package}/__init__.py.template
+-rw-rw-rw-   0        0        0      190 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/${namespace}/__init__.py.template
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.434477 msl-package-manager-2.5.4/msl/package_manager/template/${namespace}/examples/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.434477 msl-package-manager-2.5.4/msl/package_manager/template/${namespace}/examples/${package}/
+-rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/${namespace}/examples/${package}/__init__.py.template
+-rw-rw-rw-   0        0        0       26 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/${namespace}/examples/__init__.py.template
+-rw-rw-rw-   0        0        0      697 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/.coveragerc
+-rw-rw-rw-   0        0        0      527 2021-01-20 21:45:34.000000 msl-package-manager-2.5.4/msl/package_manager/template/.gitignore
+-rw-rw-rw-   0        0        0       62 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/AUTHORS.rst
+-rw-rw-rw-   0        0        0      111 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/template/CHANGES.rst
+-rw-rw-rw-   0        0        0     1127 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/MANIFEST.in
+-rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/README.rst
+-rw-rw-rw-   0        0        0    10113 2021-05-16 21:00:34.000000 msl-package-manager-2.5.4/msl/package_manager/template/condatests.py.template
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.434477 msl-package-manager-2.5.4/msl/package_manager/template/docs/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.434477 msl-package-manager-2.5.4/msl/package_manager/template/docs/_static/
+-rw-rw-rw-   0        0        0      110 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/docs/_static/README
+-rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/docs/authors.rst
+-rw-rw-rw-   0        0        0       43 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/docs/changelog.rst
+-rw-rw-rw-   0        0        0     6671 2022-08-03 04:36:48.000000 msl-package-manager-2.5.4/msl/package_manager/template/docs/conf.py.template
+-rw-rw-rw-   0        0        0      328 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/docs/index.rst
+-rw-rw-rw-   0        0        0      101 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/docs/license.rst
+-rw-rw-rw-   0        0        0      488 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/setup.cfg
+-rw-rw-rw-   0        0        0     6504 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/template/setup.py.template
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.434477 msl-package-manager-2.5.4/msl/package_manager/template/tests/
+-rw-rw-rw-   0        0        0      122 2020-12-10 23:24:11.000000 msl-package-manager-2.5.4/msl/package_manager/template/tests/README
+-rw-rw-rw-   0        0        0     4576 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/msl/package_manager/uninstall.py
+-rw-rw-rw-   0        0        0    14636 2022-09-13 22:59:17.000000 msl-package-manager-2.5.4/msl/package_manager/update.py
+-rw-rw-rw-   0        0        0    35994 2023-06-16 06:42:12.000000 msl-package-manager-2.5.4/msl/package_manager/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.450103 msl-package-manager-2.5.4/msl_package_manager.egg-info/
+-rw-rw-rw-   0        0        0     3035 2023-06-16 06:51:29.000000 msl-package-manager-2.5.4/msl_package_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2168 2023-06-16 06:51:29.000000 msl-package-manager-2.5.4/msl_package_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:51:29.000000 msl-package-manager-2.5.4/msl_package_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-16 06:51:29.000000 msl-package-manager-2.5.4/msl_package_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-16 06:50:04.000000 msl-package-manager-2.5.4/msl_package_manager.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      138 2023-06-16 06:51:29.000000 msl-package-manager-2.5.4/msl_package_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-16 06:51:29.000000 msl-package-manager-2.5.4/msl_package_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      392 2023-06-16 06:51:29.481466 msl-package-manager-2.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     7303 2023-01-24 03:04:41.000000 msl-package-manager-2.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:51:29.465831 msl-package-manager-2.5.4/tests/
+-rw-rw-rw-   0        0        0    20633 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/tests/test_cli.py
+-rw-rw-rw-   0        0        0    15288 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/tests/test_create.py
+-rw-rw-rw-   0        0        0      304 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/tests/test_github.py
+-rw-rw-rw-   0        0        0     2050 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/tests/test_install.py
+-rw-rw-rw-   0        0        0     3610 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/tests/test_issues.py
+-rw-rw-rw-   0        0        0     8258 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/tests/test_log_output.py
+-rw-rw-rw-   0        0        0      304 2023-06-16 06:03:06.000000 msl-package-manager-2.5.4/tests/test_pypi.py
+-rw-rw-rw-   0        0        0     3739 2023-05-28 20:59:15.000000 msl-package-manager-2.5.4/tests/test_update.py
+-rw-rw-rw-   0        0        0     4873 2022-09-11 21:05:22.000000 msl-package-manager-2.5.4/tests/test_utils.py
```

### Comparing `msl-package-manager-2.5.3/LICENSE.txt` & `msl-package-manager-2.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/PKG-INFO` & `msl-package-manager-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msl-package-manager
-Version: 2.5.3
+Version: 2.5.4
 Summary: Install, uninstall, update, list and create MSL packages
 Home-page: https://github.com/MSLNZ/msl-package-manager
 Author: Measurement Standards Laboratory of New Zealand
 Author-email: info@measurement.govt.nz
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `msl-package-manager-2.5.3/README.rst` & `msl-package-manager-2.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/__init__.py` & `msl-package-manager-2.5.4/msl/package_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 from .utils import installed
 from .utils import outdated_pypi_packages
 from .utils import pypi
 from .utils import set_log_level
 
 __author__ = 'Measurement Standards Laboratory of New Zealand'
 __copyright__ = '\xa9 2017 - 2023, ' + __author__
-__version__ = '2.5.3'
+__version__ = '2.5.4'
 
 _v = re.search(r'(\d+)\.(\d+)\.(\d+)[.-]?(.*)', __version__).groups()
 
 version_info = namedtuple('version_info', 'major minor micro releaselevel')(int(_v[0]), int(_v[1]), int(_v[2]), 'final')
 """:obj:`~collections.namedtuple`: Contains the version information as a (major, minor, micro, releaselevel) tuple."""
```

### Comparing `msl-package-manager-2.5.3/msl/package_manager/authorise.py` & `msl-package-manager-2.5.4/msl/package_manager/authorise.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/cli.py` & `msl-package-manager-2.5.4/msl/package_manager/cli.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/cli_argparse.py` & `msl-package-manager-2.5.4/msl/package_manager/cli_argparse.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/cli_authorise.py` & `msl-package-manager-2.5.4/msl/package_manager/cli_authorise.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/cli_create.py` & `msl-package-manager-2.5.4/msl/package_manager/cli_create.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/cli_install.py` & `msl-package-manager-2.5.4/msl/package_manager/cli_install.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/cli_list.py` & `msl-package-manager-2.5.4/msl/package_manager/cli_list.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/cli_uninstall.py` & `msl-package-manager-2.5.4/msl/package_manager/cli_uninstall.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/cli_update.py` & `msl-package-manager-2.5.4/msl/package_manager/cli_update.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/create.py` & `msl-package-manager-2.5.4/msl/package_manager/create.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/install.py` & `msl-package-manager-2.5.4/msl/package_manager/install.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/template/.coveragerc` & `msl-package-manager-2.5.4/msl/package_manager/template/.coveragerc`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/template/.gitignore` & `msl-package-manager-2.5.4/msl/package_manager/template/.gitignore`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/template/LICENSE.txt` & `msl-package-manager-2.5.4/msl/package_manager/template/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/template/condatests.py.template` & `msl-package-manager-2.5.4/msl/package_manager/template/condatests.py.template`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/template/docs/conf.py.template` & `msl-package-manager-2.5.4/msl/package_manager/template/docs/conf.py.template`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/template/setup.py.template` & `msl-package-manager-2.5.4/msl/package_manager/template/setup.py.template`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/uninstall.py` & `msl-package-manager-2.5.4/msl/package_manager/uninstall.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/update.py` & `msl-package-manager-2.5.4/msl/package_manager/update.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/msl/package_manager/utils.py` & `msl-package-manager-2.5.4/msl/package_manager/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,15 @@
         except URLError:
             log.error('Cannot access %s', url)
         else:
             return response.read().decode('utf-8')
 
     def use_json_api():
         # use the JSON API as a backup way to get the package information from PyPI
-        projects = ('msl-package-manager', 'msl-network', 'msl-loadlib', 'msl-io' 
+        projects = ('msl-package-manager', 'msl-network', 'msl-loadlib', 'msl-io',
                     'GTC', 'Quantity-Value')
         for project in projects:
             response = request('/pypi/{}/json'.format(project))
             if response:
                 _info = json.loads(response).get('info')
                 if _info:
                     pkgs[project] = {
```

### Comparing `msl-package-manager-2.5.3/msl_package_manager.egg-info/PKG-INFO` & `msl-package-manager-2.5.4/msl_package_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msl-package-manager
-Version: 2.5.3
+Version: 2.5.4
 Summary: Install, uninstall, update, list and create MSL packages
 Home-page: https://github.com/MSLNZ/msl-package-manager
 Author: Measurement Standards Laboratory of New Zealand
 Author-email: info@measurement.govt.nz
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `msl-package-manager-2.5.3/msl_package_manager.egg-info/SOURCES.txt` & `msl-package-manager-2.5.4/msl_package_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/setup.py` & `msl-package-manager-2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/tests/test_cli.py` & `msl-package-manager-2.5.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/tests/test_create.py` & `msl-package-manager-2.5.4/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/tests/test_install.py` & `msl-package-manager-2.5.4/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/tests/test_issues.py` & `msl-package-manager-2.5.4/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/tests/test_log_output.py` & `msl-package-manager-2.5.4/tests/test_log_output.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/tests/test_update.py` & `msl-package-manager-2.5.4/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `msl-package-manager-2.5.3/tests/test_utils.py` & `msl-package-manager-2.5.4/tests/test_utils.py`

 * *Files identical despite different names*

