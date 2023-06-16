# Comparing `tmp/scikit-base-0.4.5.tar.gz` & `tmp/scikit-base-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-base-0.4.5.tar", last modified: Sun May 14 14:08:20 2023, max compression
+gzip compressed data, was "scikit-base-0.4.6.tar", last modified: Fri Jun 16 01:48:18 2023, max compression
```

## Comparing `scikit-base-0.4.5.tar` & `scikit-base-0.4.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.770985 scikit-base-0.4.5/
--rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     6614 2023-05-14 14:08:20.770985 scikit-base-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2023-05-14 13:54:44.000000 scikit-base-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:19.927915 scikit-base-0.4.5/docs/
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.162083 scikit-base-0.4.5/docs/source/
--rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.5/docs/source/conf.py
--rw-rw-rw-   0        0        0     3468 2023-05-14 14:07:55.000000 scikit-base-0.4.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.189737 scikit-base-0.4.5/scikit_base.egg-info/
--rw-rw-rw-   0        0        0     6614 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1937 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      517 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.5/scikit_base.egg-info/zip-safe
--rw-rw-rw-   0        0        0      368 2023-05-14 14:08:20.775527 scikit-base-0.4.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.215207 scikit-base-0.4.5/skbase/
--rw-rw-rw-   0        0        0      468 2023-04-25 09:18:44.000000 scikit-base-0.4.5/skbase/__init__.py
--rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.5/skbase/_exceptions.py
--rw-rw-rw-   0        0        0     1112 2023-05-13 18:22:14.000000 scikit-base-0.4.5/skbase/_nopytest_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.230969 scikit-base-0.4.5/skbase/base/
--rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/base/__init__.py
--rw-rw-rw-   0        0        0    44796 2023-05-13 18:22:14.000000 scikit-base-0.4.5/skbase/base/_base.py
--rw-rw-rw-   0        0        0    36497 2023-04-26 13:58:57.000000 scikit-base-0.4.5/skbase/base/_meta.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.283991 scikit-base-0.4.5/skbase/base/_pretty_printing/
--rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/base/_pretty_printing/__init__.py
--rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 scikit-base-0.4.5/skbase/base/_pretty_printing/_object_html_repr.py
--rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.5/skbase/base/_pretty_printing/_pprint.py
--rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/base/_tagmanager.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.308561 scikit-base-0.4.5/skbase/lookup/
--rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.5/skbase/lookup/__init__.py
--rw-rw-rw-   0        0        0    39934 2023-05-11 20:27:18.000000 scikit-base-0.4.5/skbase/lookup/_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.365675 scikit-base-0.4.5/skbase/lookup/tests/
--rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/lookup/tests/__init__.py
--rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 scikit-base-0.4.5/skbase/lookup/tests/test_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.386607 scikit-base-0.4.5/skbase/testing/
--rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.5/skbase/testing/__init__.py
--rw-rw-rw-   0        0        0    37298 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/testing/test_all_objects.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.441619 scikit-base-0.4.5/skbase/testing/utils/
--rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/testing/utils/__init__.py
--rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/testing/utils/_conditional_fixtures.py
--rw-rw-rw-   0        0        0      484 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/testing/utils/_dependencies.py
--rw-rw-rw-   0        0        0      350 2023-05-13 23:40:38.000000 scikit-base-0.4.5/skbase/testing/utils/deep_equals.py
--rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.5/skbase/testing/utils/inspect.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.462284 scikit-base-0.4.5/skbase/testing/utils/tests/
--rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.5/skbase/testing/utils/tests/__init__.py
--rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.5/skbase/testing/utils/tests/test_check_dependencies.py
--rw-rw-rw-   0        0        0     1771 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/testing/utils/tests/test_deep_equals.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.521731 scikit-base-0.4.5/skbase/tests/
--rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.5/skbase/tests/__init__.py
--rw-rw-rw-   0        0        0     8671 2023-05-13 23:40:38.000000 scikit-base-0.4.5/skbase/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.549208 scikit-base-0.4.5/skbase/tests/mock_package/
--rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/tests/mock_package/__init__.py
--rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/tests/mock_package/test_mock_package.py
--rw-rw-rw-   0        0        0    43013 2023-05-13 18:22:14.000000 scikit-base-0.4.5/skbase/tests/test_base.py
--rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/tests/test_baseestimator.py
--rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/tests/test_exceptions.py
--rw-rw-rw-   0        0        0     4567 2023-05-11 20:27:18.000000 scikit-base-0.4.5/skbase/tests/test_meta.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.597140 scikit-base-0.4.5/skbase/utils/
--rw-rw-rw-   0        0        0      654 2023-05-13 23:40:38.000000 scikit-base-0.4.5/skbase/utils/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/_check.py
--rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/_iter.py
--rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/_nested_iter.py
--rw-rw-rw-   0        0        0     3225 2023-05-04 17:40:43.000000 scikit-base-0.4.5/skbase/utils/_utils.py
--rw-rw-rw-   0        0        0    11657 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/utils/deep_equals.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.628352 scikit-base-0.4.5/skbase/utils/dependencies/
--rw-rw-rw-   0        0        0      363 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/utils/dependencies/__init__.py
--rw-rw-rw-   0        0        0    10612 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/utils/dependencies/_dependencies.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.707152 scikit-base-0.4.5/skbase/utils/tests/
--rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/tests/__init__.py
--rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/tests/test_check.py
--rw-rw-rw-   0        0        0     5045 2023-05-04 17:40:43.000000 scikit-base-0.4.5/skbase/utils/tests/test_iter.py
--rw-rw-rw-   0        0        0     2314 2023-05-04 17:40:43.000000 scikit-base-0.4.5/skbase/utils/tests/test_nested_iter.py
--rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.743759 scikit-base-0.4.5/skbase/validate/
--rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/validate/__init__.py
--rw-rw-rw-   0        0        0    15180 2023-05-11 20:27:18.000000 scikit-base-0.4.5/skbase/validate/_named_objects.py
--rw-rw-rw-   0        0        0    12466 2023-05-11 20:51:59.000000 scikit-base-0.4.5/skbase/validate/_types.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.769985 scikit-base-0.4.5/skbase/validate/tests/
--rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/validate/tests/__init__.py
--rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/validate/tests/test_iterable_named_objects.py
--rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/validate/tests/test_type_validations.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:18.171089 scikit-base-0.4.6/
+-rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0     6811 2023-06-16 01:48:18.172109 scikit-base-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3506 2023-06-16 01:46:32.000000 scikit-base-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.174351 scikit-base-0.4.6/docs/
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.526451 scikit-base-0.4.6/docs/source/
+-rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3431 2023-06-16 01:48:06.000000 scikit-base-0.4.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.629004 scikit-base-0.4.6/scikit_base.egg-info/
+-rw-rw-rw-   0        0        0     6811 2023-06-16 01:48:17.000000 scikit-base-0.4.6/scikit_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1937 2023-06-16 01:48:17.000000 scikit-base-0.4.6/scikit_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 01:48:17.000000 scikit-base-0.4.6/scikit_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      517 2023-06-16 01:48:17.000000 scikit-base-0.4.6/scikit_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2023-06-16 01:48:17.000000 scikit-base-0.4.6/scikit_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.6/scikit_base.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      368 2023-06-16 01:48:18.182122 scikit-base-0.4.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.650801 scikit-base-0.4.6/skbase/
+-rw-rw-rw-   0        0        0      468 2023-06-16 01:37:08.000000 scikit-base-0.4.6/skbase/__init__.py
+-rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.6/skbase/_exceptions.py
+-rw-rw-rw-   0        0        0     1112 2023-05-13 18:22:14.000000 scikit-base-0.4.6/skbase/_nopytest_tests.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.711124 scikit-base-0.4.6/skbase/base/
+-rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/base/__init__.py
+-rw-rw-rw-   0        0        0    47999 2023-06-16 01:37:17.000000 scikit-base-0.4.6/skbase/base/_base.py
+-rw-rw-rw-   0        0        0    36497 2023-06-11 22:51:35.000000 scikit-base-0.4.6/skbase/base/_meta.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.739362 scikit-base-0.4.6/skbase/base/_pretty_printing/
+-rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/base/_pretty_printing/__init__.py
+-rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 scikit-base-0.4.6/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.6/skbase/base/_pretty_printing/_pprint.py
+-rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/base/_tagmanager.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.751278 scikit-base-0.4.6/skbase/lookup/
+-rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.6/skbase/lookup/__init__.py
+-rw-rw-rw-   0        0        0    40149 2023-06-16 01:37:08.000000 scikit-base-0.4.6/skbase/lookup/_lookup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.759331 scikit-base-0.4.6/skbase/lookup/tests/
+-rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.6/skbase/lookup/tests/__init__.py
+-rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 scikit-base-0.4.6/skbase/lookup/tests/test_lookup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.775746 scikit-base-0.4.6/skbase/testing/
+-rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.6/skbase/testing/__init__.py
+-rw-rw-rw-   0        0        0    37298 2023-05-13 18:22:13.000000 scikit-base-0.4.6/skbase/testing/test_all_objects.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.859972 scikit-base-0.4.6/skbase/testing/utils/
+-rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.6/skbase/testing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/testing/utils/_conditional_fixtures.py
+-rw-rw-rw-   0        0        0      484 2023-05-13 18:22:13.000000 scikit-base-0.4.6/skbase/testing/utils/_dependencies.py
+-rw-rw-rw-   0        0        0      350 2023-05-13 23:40:38.000000 scikit-base-0.4.6/skbase/testing/utils/deep_equals.py
+-rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.6/skbase/testing/utils/inspect.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.891067 scikit-base-0.4.6/skbase/testing/utils/tests/
+-rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.6/skbase/testing/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.6/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-rw-rw-   0        0        0     1771 2023-05-13 18:22:13.000000 scikit-base-0.4.6/skbase/testing/utils/tests/test_deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.946518 scikit-base-0.4.6/skbase/tests/
+-rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.6/skbase/tests/__init__.py
+-rw-rw-rw-   0        0        0     8671 2023-05-13 23:40:38.000000 scikit-base-0.4.6/skbase/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:17.980529 scikit-base-0.4.6/skbase/tests/mock_package/
+-rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.6/skbase/tests/mock_package/__init__.py
+-rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.6/skbase/tests/mock_package/test_mock_package.py
+-rw-rw-rw-   0        0        0    43784 2023-06-16 01:37:17.000000 scikit-base-0.4.6/skbase/tests/test_base.py
+-rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/tests/test_baseestimator.py
+-rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.6/skbase/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     4567 2023-05-11 20:27:18.000000 scikit-base-0.4.6/skbase/tests/test_meta.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:18.057389 scikit-base-0.4.6/skbase/utils/
+-rw-rw-rw-   0        0        0      654 2023-05-13 23:40:38.000000 scikit-base-0.4.6/skbase/utils/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/utils/_check.py
+-rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/utils/_iter.py
+-rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/utils/_nested_iter.py
+-rw-rw-rw-   0        0        0     3225 2023-05-04 17:40:43.000000 scikit-base-0.4.6/skbase/utils/_utils.py
+-rw-rw-rw-   0        0        0    11657 2023-05-13 18:22:13.000000 scikit-base-0.4.6/skbase/utils/deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:18.081392 scikit-base-0.4.6/skbase/utils/dependencies/
+-rw-rw-rw-   0        0        0      363 2023-05-13 18:22:13.000000 scikit-base-0.4.6/skbase/utils/dependencies/__init__.py
+-rw-rw-rw-   0        0        0    10612 2023-05-13 18:22:13.000000 scikit-base-0.4.6/skbase/utils/dependencies/_dependencies.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:18.130066 scikit-base-0.4.6/skbase/utils/tests/
+-rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/utils/tests/test_check.py
+-rw-rw-rw-   0        0        0     5045 2023-05-04 17:40:43.000000 scikit-base-0.4.6/skbase/utils/tests/test_iter.py
+-rw-rw-rw-   0        0        0     2314 2023-05-04 17:40:43.000000 scikit-base-0.4.6/skbase/utils/tests/test_nested_iter.py
+-rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/utils/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:18.164109 scikit-base-0.4.6/skbase/validate/
+-rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/validate/__init__.py
+-rw-rw-rw-   0        0        0    15180 2023-05-11 20:27:18.000000 scikit-base-0.4.6/skbase/validate/_named_objects.py
+-rw-rw-rw-   0        0        0    12466 2023-05-11 20:51:59.000000 scikit-base-0.4.6/skbase/validate/_types.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:48:18.170075 scikit-base-0.4.6/skbase/validate/tests/
+-rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/validate/tests/__init__.py
+-rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/validate/tests/test_iterable_named_objects.py
+-rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.6/skbase/validate/tests/test_type_validations.py
```

### Comparing `scikit-base-0.4.5/LICENSE` & `scikit-base-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/PKG-INFO` & `scikit-base-0.4.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,414 +1,426 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2073 6369  : 2.1..Name: sci
 00000020: 6b69 742d 6261 7365 0d0a 5665 7273 696f  kit-base..Versio
-00000030: 6e3a 2030 2e34 2e35 0d0a 5375 6d6d 6172  n: 0.4.5..Summar
+00000030: 6e3a 2030 2e34 2e36 0d0a 5375 6d6d 6172  n: 0.4.6..Summar
 00000040: 793a 2042 6173 6520 636c 6173 7365 7320  y: Base classes 
 00000050: 666f 7220 736b 6c65 6172 6e2d 6c69 6b65  for sklearn-like
 00000060: 2070 6172 616d 6574 7269 6320 6f62 6a65   parametric obje
-00000070: 6374 730d 0a41 7574 686f 723a 2046 7261  cts..Author: Fra
-00000080: 6e7a 204b 6972 c3a1 6c79 2c20 4d61 726b  nz Kir..ly, Mark
-00000090: 7573 204c c3b6 6e69 6e67 2c20 5279 616e  us L..ning, Ryan
-000000a0: 204b 7568 6e73 0d0a 4d61 696e 7461 696e   Kuhns..Maintain
-000000b0: 6572 2d65 6d61 696c 3a20 4672 616e 7a20  er-email: Franz 
-000000c0: 4b69 7261 6c79 203c 662e 6b69 7261 6c79  Kiraly <f.kiraly
-000000d0: 4075 636c 2e61 632e 756b 3e2c 2052 7961  @ucl.ac.uk>, Rya
-000000e0: 6e20 4b75 686e 7320 3c72 6b2e 736b 6261  n Kuhns <rk.skba
-000000f0: 7365 4067 6d61 696c 2e63 6f6d 3e0d 0a4c  se@gmail.com>..L
-00000100: 6963 656e 7365 3a20 4253 4420 332d 436c  icense: BSD 3-Cl
-00000110: 6175 7365 204c 6963 656e 7365 0d0a 2020  ause License..  
-00000120: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000130: 436f 7079 7269 6768 7420 2863 2920 3230  Copyright (c) 20
-00000140: 3232 2c20 736b 6261 7365 2044 6576 656c  22, skbase Devel
-00000150: 6f70 6572 730d 0a20 2020 2020 2020 2041  opers..        A
-00000160: 6c6c 2072 6967 6874 7320 7265 7365 7276  ll rights reserv
-00000170: 6564 2e0d 0a20 2020 2020 2020 200d 0a20  ed...        .. 
-00000180: 2020 2020 2020 2052 6564 6973 7472 6962         Redistrib
-00000190: 7574 696f 6e20 616e 6420 7573 6520 696e  ution and use in
-000001a0: 2073 6f75 7263 6520 616e 6420 6269 6e61   source and bina
-000001b0: 7279 2066 6f72 6d73 2c20 7769 7468 206f  ry forms, with o
-000001c0: 7220 7769 7468 6f75 740d 0a20 2020 2020  r without..     
-000001d0: 2020 206d 6f64 6966 6963 6174 696f 6e2c     modification,
-000001e0: 2061 7265 2070 6572 6d69 7474 6564 2070   are permitted p
-000001f0: 726f 7669 6465 6420 7468 6174 2074 6865  rovided that the
-00000200: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6469   following condi
-00000210: 7469 6f6e 7320 6172 6520 6d65 743a 0d0a  tions are met:..
-00000220: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000230: 2020 312e 2052 6564 6973 7472 6962 7574    1. Redistribut
-00000240: 696f 6e73 206f 6620 736f 7572 6365 2063  ions of source c
-00000250: 6f64 6520 6d75 7374 2072 6574 6169 6e20  ode must retain 
-00000260: 7468 6520 6162 6f76 6520 636f 7079 7269  the above copyri
-00000270: 6768 7420 6e6f 7469 6365 2c20 7468 6973  ght notice, this
-00000280: 0d0a 2020 2020 2020 2020 2020 206c 6973  ..           lis
-00000290: 7420 6f66 2063 6f6e 6469 7469 6f6e 7320  t of conditions 
-000002a0: 616e 6420 7468 6520 666f 6c6c 6f77 696e  and the followin
-000002b0: 6720 6469 7363 6c61 696d 6572 2e0d 0a20  g disclaimer... 
-000002c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000002d0: 2032 2e20 5265 6469 7374 7269 6275 7469   2. Redistributi
-000002e0: 6f6e 7320 696e 2062 696e 6172 7920 666f  ons in binary fo
-000002f0: 726d 206d 7573 7420 7265 7072 6f64 7563  rm must reproduc
-00000300: 6520 7468 6520 6162 6f76 6520 636f 7079  e the above copy
-00000310: 7269 6768 7420 6e6f 7469 6365 2c0d 0a20  right notice,.. 
-00000320: 2020 2020 2020 2020 2020 7468 6973 206c            this l
-00000330: 6973 7420 6f66 2063 6f6e 6469 7469 6f6e  ist of condition
-00000340: 7320 616e 6420 7468 6520 666f 6c6c 6f77  s and the follow
-00000350: 696e 6720 6469 7363 6c61 696d 6572 2069  ing disclaimer i
-00000360: 6e20 7468 6520 646f 6375 6d65 6e74 6174  n the documentat
-00000370: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00000380: 616e 642f 6f72 206f 7468 6572 206d 6174  and/or other mat
-00000390: 6572 6961 6c73 2070 726f 7669 6465 6420  erials provided 
-000003a0: 7769 7468 2074 6865 2064 6973 7472 6962  with the distrib
-000003b0: 7574 696f 6e2e 0d0a 2020 2020 2020 2020  ution...        
-000003c0: 0d0a 2020 2020 2020 2020 332e 204e 6569  ..        3. Nei
-000003d0: 7468 6572 2074 6865 206e 616d 6520 6f66  ther the name of
-000003e0: 2074 6865 2063 6f70 7972 6967 6874 2068   the copyright h
-000003f0: 6f6c 6465 7220 6e6f 7220 7468 6520 6e61  older nor the na
-00000400: 6d65 7320 6f66 2069 7473 0d0a 2020 2020  mes of its..    
-00000410: 2020 2020 2020 2063 6f6e 7472 6962 7574         contribut
-00000420: 6f72 7320 6d61 7920 6265 2075 7365 6420  ors may be used 
-00000430: 746f 2065 6e64 6f72 7365 206f 7220 7072  to endorse or pr
-00000440: 6f6d 6f74 6520 7072 6f64 7563 7473 2064  omote products d
-00000450: 6572 6976 6564 2066 726f 6d0d 0a20 2020  erived from..   
-00000460: 2020 2020 2020 2020 7468 6973 2073 6f66          this sof
-00000470: 7477 6172 6520 7769 7468 6f75 7420 7370  tware without sp
-00000480: 6563 6966 6963 2070 7269 6f72 2077 7269  ecific prior wri
-00000490: 7474 656e 2070 6572 6d69 7373 696f 6e2e  tten permission.
-000004a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000004b0: 2020 2020 5448 4953 2053 4f46 5457 4152      THIS SOFTWAR
-000004c0: 4520 4953 2050 524f 5649 4445 4420 4259  E IS PROVIDED BY
-000004d0: 2054 4845 2043 4f50 5952 4947 4854 2048   THE COPYRIGHT H
-000004e0: 4f4c 4445 5253 2041 4e44 2043 4f4e 5452  OLDERS AND CONTR
-000004f0: 4942 5554 4f52 5320 2241 5320 4953 220d  IBUTORS "AS IS".
-00000500: 0a20 2020 2020 2020 2041 4e44 2041 4e59  .        AND ANY
-00000510: 2045 5850 5245 5353 204f 5220 494d 504c   EXPRESS OR IMPL
-00000520: 4945 4420 5741 5252 414e 5449 4553 2c20  IED WARRANTIES, 
-00000530: 494e 434c 5544 494e 472c 2042 5554 204e  INCLUDING, BUT N
-00000540: 4f54 204c 494d 4954 4544 2054 4f2c 2054  OT LIMITED TO, T
-00000550: 4845 0d0a 2020 2020 2020 2020 494d 504c  HE..        IMPL
-00000560: 4945 4420 5741 5252 414e 5449 4553 204f  IED WARRANTIES O
-00000570: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
-00000580: 5920 414e 4420 4649 544e 4553 5320 464f  Y AND FITNESS FO
-00000590: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
-000005a0: 5552 504f 5345 2041 5245 0d0a 2020 2020  URPOSE ARE..    
-000005b0: 2020 2020 4449 5343 4c41 494d 4544 2e20      DISCLAIMED. 
-000005c0: 494e 204e 4f20 4556 454e 5420 5348 414c  IN NO EVENT SHAL
-000005d0: 4c20 5448 4520 434f 5059 5249 4748 5420  L THE COPYRIGHT 
-000005e0: 484f 4c44 4552 204f 5220 434f 4e54 5249  HOLDER OR CONTRI
-000005f0: 4255 544f 5253 2042 4520 4c49 4142 4c45  BUTORS BE LIABLE
-00000600: 0d0a 2020 2020 2020 2020 464f 5220 414e  ..        FOR AN
-00000610: 5920 4449 5245 4354 2c20 494e 4449 5245  Y DIRECT, INDIRE
-00000620: 4354 2c20 494e 4349 4445 4e54 414c 2c20  CT, INCIDENTAL, 
-00000630: 5350 4543 4941 4c2c 2045 5845 4d50 4c41  SPECIAL, EXEMPLA
-00000640: 5259 2c20 4f52 2043 4f4e 5345 5155 454e  RY, OR CONSEQUEN
-00000650: 5449 414c 0d0a 2020 2020 2020 2020 4441  TIAL..        DA
-00000660: 4d41 4745 5320 2849 4e43 4c55 4449 4e47  MAGES (INCLUDING
-00000670: 2c20 4255 5420 4e4f 5420 4c49 4d49 5445  , BUT NOT LIMITE
-00000680: 4420 544f 2c20 5052 4f43 5552 454d 454e  D TO, PROCUREMEN
-00000690: 5420 4f46 2053 5542 5354 4954 5554 4520  T OF SUBSTITUTE 
-000006a0: 474f 4f44 5320 4f52 0d0a 2020 2020 2020  GOODS OR..      
-000006b0: 2020 5345 5256 4943 4553 3b20 4c4f 5353    SERVICES; LOSS
-000006c0: 204f 4620 5553 452c 2044 4154 412c 204f   OF USE, DATA, O
-000006d0: 5220 5052 4f46 4954 533b 204f 5220 4255  R PROFITS; OR BU
-000006e0: 5349 4e45 5353 2049 4e54 4552 5255 5054  SINESS INTERRUPT
-000006f0: 494f 4e29 2048 4f57 4556 4552 0d0a 2020  ION) HOWEVER..  
-00000700: 2020 2020 2020 4341 5553 4544 2041 4e44        CAUSED AND
-00000710: 204f 4e20 414e 5920 5448 454f 5259 204f   ON ANY THEORY O
-00000720: 4620 4c49 4142 494c 4954 592c 2057 4845  F LIABILITY, WHE
-00000730: 5448 4552 2049 4e20 434f 4e54 5241 4354  THER IN CONTRACT
-00000740: 2c20 5354 5249 4354 204c 4941 4249 4c49  , STRICT LIABILI
-00000750: 5459 2c0d 0a20 2020 2020 2020 204f 5220  TY,..        OR 
-00000760: 544f 5254 2028 494e 434c 5544 494e 4720  TORT (INCLUDING 
-00000770: 4e45 474c 4947 454e 4345 204f 5220 4f54  NEGLIGENCE OR OT
-00000780: 4845 5257 4953 4529 2041 5249 5349 4e47  HERWISE) ARISING
-00000790: 2049 4e20 414e 5920 5741 5920 4f55 5420   IN ANY WAY OUT 
-000007a0: 4f46 2054 4845 2055 5345 0d0a 2020 2020  OF THE USE..    
-000007b0: 2020 2020 4f46 2054 4849 5320 534f 4654      OF THIS SOFT
-000007c0: 5741 5245 2c20 4556 454e 2049 4620 4144  WARE, EVEN IF AD
-000007d0: 5649 5345 4420 4f46 2054 4845 2050 4f53  VISED OF THE POS
-000007e0: 5349 4249 4c49 5459 204f 4620 5355 4348  SIBILITY OF SUCH
-000007f0: 2044 414d 4147 452e 0d0a 2020 2020 2020   DAMAGE...      
-00000800: 2020 0d0a 5072 6f6a 6563 742d 5552 4c3a    ..Project-URL:
-00000810: 2068 6f6d 6570 6167 652c 2068 7474 7073   homepage, https
-00000820: 3a2f 2f67 6974 6875 622e 636f 6d2f 736b  ://github.com/sk
-00000830: 7469 6d65 2f73 6b62 6173 650d 0a50 726f  time/skbase..Pro
-00000840: 6a65 6374 2d55 524c 3a20 7265 706f 7369  ject-URL: reposi
-00000850: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
-00000860: 7468 7562 2e63 6f6d 2f73 6b74 696d 652f  thub.com/sktime/
-00000870: 736b 6261 7365 0d0a 5072 6f6a 6563 742d  skbase..Project-
-00000880: 5552 4c3a 2064 6f63 756d 656e 7461 7469  URL: documentati
-00000890: 6f6e 2c20 6874 7470 733a 2f2f 6769 7468  on, https://gith
-000008a0: 7562 2e63 6f6d 2f73 6b74 696d 652f 736b  ub.com/sktime/sk
-000008b0: 6261 7365 0d0a 5072 6f6a 6563 742d 5552  base..Project-UR
-000008c0: 4c3a 2064 6f77 6e6c 6f61 642c 2068 7474  L: download, htt
-000008d0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000008e0: 6f6a 6563 742f 736b 6261 7365 2f23 6669  oject/skbase/#fi
-000008f0: 6c65 730d 0a4b 6579 776f 7264 733a 2064  les..Keywords: d
-00000900: 6174 612d 7363 6965 6e63 652c 6d61 6368  ata-science,mach
-00000910: 696e 652d 6c65 6172 6e69 6e67 2c73 6369  ine-learning,sci
-00000920: 6b69 742d 6c65 6172 6e0d 0a43 6c61 7373  kit-learn..Class
-00000930: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-00000940: 4175 6469 656e 6365 203a 3a20 5363 6965  Audience :: Scie
-00000950: 6e63 652f 5265 7365 6172 6368 0d0a 436c  nce/Research..Cl
-00000960: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
-00000970: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-00000980: 6576 656c 6f70 6572 730d 0a43 6c61 7373  evelopers..Class
-00000990: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-000009a0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000009b0: 3a20 4253 4420 4c69 6365 6e73 650d 0a43  : BSD License..C
-000009c0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000009d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000009e0: 3a3a 2050 7974 686f 6e0d 0a43 6c61 7373  :: Python..Class
-000009f0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
-00000a00: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
-00000a10: 6d65 6e74 0d0a 436c 6173 7369 6669 6572  ment..Classifier
-00000a20: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
-00000a30: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-00000a40: 670d 0a43 6c61 7373 6966 6965 723a 204f  g..Classifier: O
-00000a50: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000a60: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
-00000a70: 5769 6e64 6f77 730d 0a43 6c61 7373 6966  Windows..Classif
-00000a80: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000a90: 7973 7465 6d20 3a3a 2050 4f53 4958 0d0a  ystem :: POSIX..
-00000aa0: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000ab0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000ac0: 556e 6978 0d0a 436c 6173 7369 6669 6572  Unix..Classifier
-00000ad0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-00000ae0: 656d 203a 3a20 4d61 634f 530d 0a43 6c61  em :: MacOS..Cla
-00000af0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000b00: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000b10: 2050 7974 686f 6e20 3a3a 2033 2e37 0d0a   Python :: 3.7..
-00000b20: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000b30: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000b40: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000b50: 380d 0a43 6c61 7373 6966 6965 723a 2050  8..Classifier: P
-00000b60: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000b70: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000b80: 2033 2e39 0d0a 436c 6173 7369 6669 6572   3.9..Classifier
-00000b90: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000ba0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000bb0: 203a 3a20 332e 3130 0d0a 436c 6173 7369   :: 3.10..Classi
-00000bc0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000bd0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000be0: 7468 6f6e 203a 3a20 332e 3131 0d0a 5265  thon :: 3.11..Re
-00000bf0: 7175 6972 6573 2d50 7974 686f 6e3a 203c  quires-Python: <
-00000c00: 332e 3132 2c3e 3d33 2e37 0d0a 4465 7363  3.12,>=3.7..Desc
-00000c10: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000c20: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000c30: 6f77 6e0d 0a50 726f 7669 6465 732d 4578  own..Provides-Ex
-00000c40: 7472 613a 2061 6c6c 5f65 7874 7261 730d  tra: all_extras.
-00000c50: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000c60: 2064 6576 0d0a 5072 6f76 6964 6573 2d45   dev..Provides-E
-00000c70: 7874 7261 3a20 6c69 6e74 6572 730d 0a50  xtra: linters..P
-00000c80: 726f 7669 6465 732d 4578 7472 613a 2062  rovides-Extra: b
-00000c90: 696e 6465 720d 0a50 726f 7669 6465 732d  inder..Provides-
-00000ca0: 4578 7472 613a 2064 6f63 730d 0a50 726f  Extra: docs..Pro
-00000cb0: 7669 6465 732d 4578 7472 613a 2074 6573  vides-Extra: tes
-00000cc0: 740d 0a4c 6963 656e 7365 2d46 696c 653a  t..License-File:
-00000cd0: 204c 4943 454e 5345 0d0a 0d0a 0d0a 2320   LICENSE......# 
-00000ce0: 5765 6c63 6f6d 6520 746f 2073 6b62 6173  Welcome to skbas
-00000cf0: 650d 0a0d 0a3e 2041 2062 6173 6520 636c  e....> A base cl
-00000d00: 6173 7320 666f 7220 7363 696b 6974 2d6c  ass for scikit-l
-00000d10: 6561 726e 2d6c 696b 6520 616e 6420 736b  earn-like and sk
-00000d20: 7469 6d65 2d6c 696b 6520 7061 7261 6d65  time-like parame
-00000d30: 7472 6963 206f 626a 6563 7473 0d0a 0d0a  tric objects....
-00000d40: 6073 6b62 6173 6560 2070 726f 7669 6465  `skbase` provide
-00000d50: 7320 6261 7365 2063 6c61 7373 6573 2066  s base classes f
-00000d60: 6f72 2063 7265 6174 696e 6720 7363 696b  or creating scik
-00000d70: 6974 2d6c 6561 726e 2d6c 696b 6520 7061  it-learn-like pa
-00000d80: 7261 6d65 7472 6963 206f 626a 6563 7473  rametric objects
-00000d90: 2c0d 0a61 6c6f 6e67 2077 6974 6820 746f  ,..along with to
-00000da0: 6f6c 7320 746f 206d 616b 6520 6974 2065  ols to make it e
-00000db0: 6173 6965 7220 746f 2062 7569 6c64 2079  asier to build y
-00000dc0: 6f75 7220 6f77 6e20 7061 636b 6167 6573  our own packages
-00000dd0: 2074 6861 7420 666f 6c6c 6f77 2074 6865   that follow the
-00000de0: 7365 0d0a 6465 7369 676e 2070 6174 7465  se..design patte
-00000df0: 726e 732e 0d0a 0d0a 3a72 6f63 6b65 743a  rns.....:rocket:
-00000e00: 2056 6572 7369 6f6e 2030 2e34 2e35 2069   Version 0.4.5 i
-00000e10: 7320 6e6f 7720 6176 6169 6c61 626c 652e  s now available.
-00000e20: 2043 6865 636b 6f75 7420 6f75 720d 0a5b   Checkout our..[
-00000e30: 7265 6c65 6173 6520 6e6f 7465 735d 2868  release notes](h
-00000e40: 7474 7073 3a2f 2f73 6b62 6173 652e 7265  ttps://skbase.re
-00000e50: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000e60: 6c61 7465 7374 2f63 6861 6e67 656c 6f67  latest/changelog
-00000e70: 2e68 746d 6c29 2e0d 0a0d 0a7c 204f 7665  .html).....| Ove
-00000e80: 7276 6965 7720 7c20 7c0d 0a7c 2d2d 2d7c  rview | |..|---|
-00000e90: 2d2d 2d7c 0d0a 7c20 2a2a 4349 2f43 442a  ---|..| **CI/CD*
-00000ea0: 2a20 7c20 5b21 5b54 6573 7473 5d28 6874  * | [![Tests](ht
-00000eb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ec0: 2f73 6b74 696d 652f 736b 6261 7365 2f61  /sktime/skbase/a
-00000ed0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-00000ee0: 2f74 6573 742e 796d 6c2f 6261 6467 652e  /test.yml/badge.
-00000ef0: 7376 673f 6272 616e 6368 3d6d 6169 6e29  svg?branch=main)
-00000f00: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000f10: 2e63 6f6d 2f73 6b74 696d 652f 736b 6261  .com/sktime/skba
-00000f20: 7365 2f61 6374 696f 6e73 2f77 6f72 6b66  se/actions/workf
-00000f30: 6c6f 7773 2f74 6573 742e 796d 6c29 205b  lows/test.yml) [
-00000f40: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
-00000f50: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000f60: 2f73 6b74 696d 652f 736b 6261 7365 2f62  /sktime/skbase/b
-00000f70: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
-00000f80: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
-00000f90: 3d32 4a34 3234 4e4c 4f38 3229 5d28 6874  =2J424NLO82)](ht
-00000fa0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000fb0: 2f67 682f 736b 7469 6d65 2f73 6b62 6173  /gh/sktime/skbas
-00000fc0: 6529 205b 215b 446f 6375 6d65 6e74 6174  e) [![Documentat
-00000fd0: 696f 6e20 5374 6174 7573 5d28 6874 7470  ion Status](http
-00000fe0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
-00000ff0: 6f72 672f 7072 6f6a 6563 7473 2f73 6b62  org/projects/skb
-00001000: 6173 652f 6261 6467 652f 3f76 6572 7369  ase/badge/?versi
-00001010: 6f6e 3d6c 6174 6573 7429 5d28 6874 7470  on=latest)](http
-00001020: 733a 2f2f 736b 6261 7365 2e72 6561 6474  s://skbase.readt
-00001030: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00001040: 6573 742f 3f62 6164 6765 3d6c 6174 6573  est/?badge=lates
-00001050: 7429 205b 215b 7072 652d 636f 6d6d 6974  t) [![pre-commit
-00001060: 2e63 6920 7374 6174 7573 5d28 6874 7470  .ci status](http
-00001070: 733a 2f2f 7265 7375 6c74 732e 7072 652d  s://results.pre-
-00001080: 636f 6d6d 6974 2e63 692f 6261 6467 652f  commit.ci/badge/
-00001090: 6769 7468 7562 2f73 6b74 696d 652f 736b  github/sktime/sk
-000010a0: 6261 7365 2f6d 6169 6e2e 7376 6729 5d28  base/main.svg)](
-000010b0: 6874 7470 733a 2f2f 7265 7375 6c74 732e  https://results.
-000010c0: 7072 652d 636f 6d6d 6974 2e63 692f 6c61  pre-commit.ci/la
-000010d0: 7465 7374 2f67 6974 6875 622f 736b 7469  test/github/skti
-000010e0: 6d65 2f73 6b62 6173 652f 6d61 696e 2920  me/skbase/main) 
-000010f0: 7c0d 0a7c 202a 2a43 6f64 652a 2a20 7c20  |..| **Code** | 
-00001100: 205b 215b 2170 7970 695d 2868 7474 7073   [![!pypi](https
-00001110: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001120: 6f2f 7079 7069 2f76 2f73 6369 6b69 742d  o/pypi/v/scikit-
-00001130: 6261 7365 3f63 6f6c 6f72 3d6f 7261 6e67  base?color=orang
-00001140: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
-00001150: 2e6f 7267 2f70 726f 6a65 6374 2f73 6b62  .org/project/skb
-00001160: 6173 652f 2920 205b 215b 2170 7974 686f  ase/)  [![!pytho
-00001170: 6e2d 7665 7273 696f 6e73 5d28 6874 7470  n-versions](http
-00001180: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00001190: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
-000011a0: 6e73 2f73 6369 6b69 742d 6261 7365 295d  ns/scikit-base)]
-000011b0: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
-000011c0: 686f 6e2e 6f72 672f 2920 5b21 5b21 626c  hon.org/) [![!bl
-000011d0: 6163 6b5d 2868 7474 7073 3a2f 2f69 6d67  ack](https://img
-000011e0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000011f0: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
-00001200: 6c61 636b 2d30 3030 3030 302e 7376 6729  lack-000000.svg)
-00001210: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001220: 2e63 6f6d 2f70 7366 2f62 6c61 636b 2920  .com/psf/black) 
-00001230: 5b21 5b73 6563 7572 6974 793a 2062 616e  [![security: ban
-00001240: 6469 745d 2868 7474 7073 3a2f 2f69 6d67  dit](https://img
-00001250: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00001260: 652f 7365 6375 7269 7479 2d62 616e 6469  e/security-bandi
-00001270: 742d 7965 6c6c 6f77 2e73 7667 295d 2868  t-yellow.svg)](h
-00001280: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001290: 6d2f 5079 4351 412f 6261 6e64 6974 2920  m/PyCQA/bandit) 
-000012a0: 7c0d 0a7c 202a 2a44 6f77 6e6c 6f61 6473  |..| **Downloads
-000012b0: 2a2a 7c20 5b21 5b44 6f77 6e6c 6f61 6473  **| [![Downloads
-000012c0: 5d28 6874 7470 733a 2f2f 7374 6174 6963  ](https://static
-000012d0: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
-000012e0: 6e61 6c69 7a65 642d 6261 6467 652f 7363  nalized-badge/sc
-000012f0: 696b 6974 2d62 6173 653f 7065 7269 6f64  ikit-base?period
-00001300: 3d77 6565 6b26 756e 6974 733d 696e 7465  =week&units=inte
-00001310: 726e 6174 696f 6e61 6c5f 7379 7374 656d  rnational_system
-00001320: 266c 6566 745f 636f 6c6f 723d 6772 6579  &left_color=grey
-00001330: 2672 6967 6874 5f63 6f6c 6f72 3d62 6c75  &right_color=blu
-00001340: 6526 6c65 6674 5f74 6578 743d 7765 656b  e&left_text=week
-00001350: 6c79 2532 3028 7079 7069 2929 5d28 6874  ly%20(pypi))](ht
-00001360: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
-00001370: 7072 6f6a 6563 742f 7363 696b 6974 2d62  project/scikit-b
-00001380: 6173 6529 205b 215b 446f 776e 6c6f 6164  ase) [![Download
-00001390: 735d 2868 7474 7073 3a2f 2f73 7461 7469  s](https://stati
-000013a0: 632e 7065 7079 2e74 6563 682f 7065 7273  c.pepy.tech/pers
-000013b0: 6f6e 616c 697a 6564 2d62 6164 6765 2f73  onalized-badge/s
-000013c0: 6369 6b69 742d 6261 7365 3f70 6572 696f  cikit-base?perio
-000013d0: 643d 6d6f 6e74 6826 756e 6974 733d 696e  d=month&units=in
-000013e0: 7465 726e 6174 696f 6e61 6c5f 7379 7374  ternational_syst
-000013f0: 656d 266c 6566 745f 636f 6c6f 723d 6772  em&left_color=gr
-00001400: 6579 2672 6967 6874 5f63 6f6c 6f72 3d62  ey&right_color=b
-00001410: 6c75 6526 6c65 6674 5f74 6578 743d 6d6f  lue&left_text=mo
-00001420: 6e74 686c 7925 3230 2870 7970 6929 295d  nthly%20(pypi))]
-00001430: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-00001440: 6368 2f70 726f 6a65 6374 2f73 6369 6b69  ch/project/sciki
-00001450: 742d 6261 7365 2920 5b21 5b44 6f77 6e6c  t-base) [![Downl
-00001460: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
-00001470: 6174 6963 2e70 6570 792e 7465 6368 2f70  atic.pepy.tech/p
-00001480: 6572 736f 6e61 6c69 7a65 642d 6261 6467  ersonalized-badg
-00001490: 652f 7363 696b 6974 2d62 6173 653f 7065  e/scikit-base?pe
-000014a0: 7269 6f64 3d74 6f74 616c 2675 6e69 7473  riod=total&units
-000014b0: 3d69 6e74 6572 6e61 7469 6f6e 616c 5f73  =international_s
-000014c0: 7973 7465 6d26 6c65 6674 5f63 6f6c 6f72  ystem&left_color
-000014d0: 3d67 7265 7926 7269 6768 745f 636f 6c6f  =grey&right_colo
-000014e0: 723d 626c 7565 266c 6566 745f 7465 7874  r=blue&left_text
-000014f0: 3d63 756d 756c 6174 6976 6525 3230 2870  =cumulative%20(p
-00001500: 7970 6929 295d 2868 7474 7073 3a2f 2f70  ypi))](https://p
-00001510: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
-00001520: 2f73 6369 6b69 742d 6261 7365 2920 7c0d  /scikit-base) |.
-00001530: 0a0d 0a3c 212d 2d20 414c 4c2d 434f 4e54  ...<!-- ALL-CONT
-00001540: 5249 4255 544f 5253 2d42 4144 4745 3a53  RIBUTORS-BADGE:S
-00001550: 5441 5254 202d 2044 6f20 6e6f 7420 7265  TART - Do not re
-00001560: 6d6f 7665 206f 7220 6d6f 6469 6679 2074  move or modify t
-00001570: 6869 7320 7365 6374 696f 6e20 2d2d 3e0d  his section -->.
-00001580: 0a5b 215b 416c 6c20 436f 6e74 7269 6275  .[![All Contribu
-00001590: 746f 7273 5d28 6874 7470 733a 2f2f 696d  tors](https://im
-000015a0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000015b0: 6765 2f61 6c6c 5f63 6f6e 7472 6962 7574  ge/all_contribut
-000015c0: 6f72 732d 3133 2d6f 7261 6e67 652e 7376  ors-13-orange.sv
-000015d0: 673f 7374 796c 653d 666c 6174 2d73 7175  g?style=flat-squ
-000015e0: 6172 6529 5d28 2363 6f6e 7472 6962 7574  are)](#contribut
-000015f0: 6f72 7329 0d0a 3c21 2d2d 2041 4c4c 2d43  ors)..<!-- ALL-C
-00001600: 4f4e 5452 4942 5554 4f52 532d 4241 4447  ONTRIBUTORS-BADG
-00001610: 453a 454e 4420 2d2d 3e0d 0a0d 0a23 2320  E:END -->....## 
-00001620: 446f 6375 6d65 6e74 6174 696f 6e0d 0a0d  Documentation...
-00001630: 0a54 6f20 6c65 6172 6e20 6d6f 7265 2061  .To learn more a
-00001640: 626f 7574 2074 6865 2070 6163 6b61 6765  bout the package
-00001650: 2063 6865 636b 6f75 7420 6f75 7220 5b64   checkout our [d
-00001660: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00001670: 7470 733a 2f2f 736b 6261 7365 2e72 6561  tps://skbase.rea
-00001680: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00001690: 6174 6573 742f 292e 0d0a 0d0a 2323 203a  atest/).....## :
-000016a0: 686f 7572 676c 6173 735f 666c 6f77 696e  hourglass_flowin
-000016b0: 675f 7361 6e64 3a20 496e 7374 616c 6c20  g_sand: Install 
-000016c0: 736b 6261 7365 0d0a 466f 7220 7472 6f75  skbase..For trou
-000016d0: 626c 6520 7368 6f6f 7469 6e67 206f 7220  ble shooting or 
-000016e0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-000016f0: 2c20 7365 6520 6f75 720d 0a5b 6465 7461  , see our..[deta
-00001700: 696c 6564 2069 6e73 7461 6c6c 6174 696f  iled installatio
-00001710: 6e20 696e 7374 7275 6374 696f 6e73 5d28  n instructions](
-00001720: 6874 7470 733a 2f2f 736b 6261 7365 2e72  https://skbase.r
-00001730: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00001740: 2f6c 6174 6573 742f 7573 6572 5f64 6f63  /latest/user_doc
-00001750: 756d 656e 7461 7469 6f6e 2f69 6e73 7461  umentation/insta
-00001760: 6c6c 6174 696f 6e2e 6874 6d6c 292e 0d0a  llation.html)...
-00001770: 0d0a 2d20 2a2a 4f70 6572 6174 696e 6720  ..- **Operating 
-00001780: 7379 7374 656d 2a2a 3a20 6d61 634f 5320  system**: macOS 
-00001790: 5820 c2b7 204c 696e 7578 20c2 b720 5769  X .. Linux .. Wi
-000017a0: 6e64 6f77 7320 382e 3120 6f72 2068 6967  ndows 8.1 or hig
-000017b0: 6865 720d 0a2d 202a 2a50 7974 686f 6e20  her..- **Python 
-000017c0: 7665 7273 696f 6e2a 2a3a 2050 7974 686f  version**: Pytho
-000017d0: 6e20 332e 372c 2033 2e38 2c20 332e 392c  n 3.7, 3.8, 3.9,
-000017e0: 2033 2e31 3020 616e 6420 332e 3131 0d0a   3.10 and 3.11..
-000017f0: 2d20 2a2a 5061 636b 6167 6520 6d61 6e61  - **Package mana
-00001800: 6765 7273 2a2a 3a20 5b70 6970 5d0d 0a0d  gers**: [pip]...
-00001810: 0a5b 7069 705d 3a20 6874 7470 733a 2f2f  .[pip]: https://
-00001820: 7069 702e 7079 7061 2e69 6f2f 656e 2f73  pip.pypa.io/en/s
-00001830: 7461 626c 652f 0d0a 0d0a 2323 2320 7069  table/....### pi
-00001840: 700d 0a73 6b62 6173 6520 7265 6c65 6173  p..skbase releas
-00001850: 6573 2061 7265 2061 7661 696c 6162 6c65  es are available
-00001860: 2061 7320 736f 7572 6365 2070 6163 6b61   as source packa
-00001870: 6765 7320 616e 6420 6269 6e61 7279 2077  ges and binary w
-00001880: 6865 656c 7320 7669 6120 5079 5049 0d0a  heels via PyPI..
-00001890: 616e 6420 6361 6e20 6265 2069 6e73 7461  and can be insta
-000018a0: 6c6c 6564 2075 7369 6e67 2070 6970 2e20  lled using pip. 
-000018b0: 4368 6563 6b6f 7574 2074 6865 2066 756c  Checkout the ful
-000018c0: 6c20 6c69 7374 206f 6620 7072 652d 636f  l list of pre-co
-000018d0: 6d70 696c 6564 205b 7768 6565 6c73 206f  mpiled [wheels o
-000018e0: 6e20 5079 5069 5d28 6874 7470 733a 2f2f  n PyPi](https://
-000018f0: 7079 7069 2e6f 7267 2f73 696d 706c 652f  pypi.org/simple/
-00001900: 736b 6261 7365 2f29 2e0d 0a0d 0a54 6f20  skbase/).....To 
-00001910: 696e 7374 616c 6c20 7468 6520 636f 7265  install the core
-00001920: 2070 6163 6b61 6765 2075 7365 3a0d 0a0d   package use:...
-00001930: 0a60 6060 6261 7368 0d0a 7069 7020 696e  .```bash..pip in
-00001940: 7374 616c 6c20 7363 696b 6974 2d62 6173  stall scikit-bas
-00001950: 650d 0a60 6060 0d0a 0d0a 6f72 2c20 6966  e..```....or, if
-00001960: 2079 6f75 2077 616e 7420 746f 2069 6e73   you want to ins
-00001970: 7461 6c6c 2077 6974 6820 7468 6520 6d61  tall with the ma
-00001980: 7869 6d75 6d20 7365 7420 6f66 2064 6570  ximum set of dep
-00001990: 656e 6465 6e63 6965 732c 2075 7365 3a0d  endencies, use:.
-000019a0: 0a0d 0a60 6060 6261 7368 0d0a 7069 7020  ...```bash..pip 
-000019b0: 696e 7374 616c 6c20 7363 696b 6974 2d62  install scikit-b
-000019c0: 6173 655b 616c 6c5f 6578 7472 6173 5d0d  ase[all_extras].
-000019d0: 0a60 6060 0d0a                           .```..
+00000070: 6374 730d 0a41 7574 686f 722d 656d 6169  cts..Author-emai
+00000080: 6c3a 2073 6b74 696d 6520 6465 7665 6c6f  l: sktime develo
+00000090: 7065 7273 203c 736b 7469 6d65 2e74 6f6f  pers <sktime.too
+000000a0: 6c62 6f78 4067 6d61 696c 2e63 6f6d 3e0d  lbox@gmail.com>.
+000000b0: 0a4d 6169 6e74 6169 6e65 723a 2046 7261  .Maintainer: Fra
+000000c0: 6e7a 204b 6972 c3a1 6c79 0d0a 4d61 696e  nz Kir..ly..Main
+000000d0: 7461 696e 6572 2d65 6d61 696c 3a20 736b  tainer-email: sk
+000000e0: 7469 6d65 2064 6576 656c 6f70 6572 7320  time developers 
+000000f0: 3c73 6b74 696d 652e 746f 6f6c 626f 7840  <sktime.toolbox@
+00000100: 676d 6169 6c2e 636f 6d3e 0d0a 4c69 6365  gmail.com>..Lice
+00000110: 6e73 653a 2042 5344 2033 2d43 6c61 7573  nse: BSD 3-Claus
+00000120: 6520 4c69 6365 6e73 650d 0a20 2020 2020  e License..     
+00000130: 2020 200d 0a20 2020 2020 2020 2043 6f70     ..        Cop
+00000140: 7972 6967 6874 2028 6329 2032 3032 322c  yright (c) 2022,
+00000150: 2073 6b62 6173 6520 4465 7665 6c6f 7065   skbase Develope
+00000160: 7273 0d0a 2020 2020 2020 2020 416c 6c20  rs..        All 
+00000170: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
+00000180: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00000190: 2020 2020 5265 6469 7374 7269 6275 7469      Redistributi
+000001a0: 6f6e 2061 6e64 2075 7365 2069 6e20 736f  on and use in so
+000001b0: 7572 6365 2061 6e64 2062 696e 6172 7920  urce and binary 
+000001c0: 666f 726d 732c 2077 6974 6820 6f72 2077  forms, with or w
+000001d0: 6974 686f 7574 0d0a 2020 2020 2020 2020  ithout..        
+000001e0: 6d6f 6469 6669 6361 7469 6f6e 2c20 6172  modification, ar
+000001f0: 6520 7065 726d 6974 7465 6420 7072 6f76  e permitted prov
+00000200: 6964 6564 2074 6861 7420 7468 6520 666f  ided that the fo
+00000210: 6c6c 6f77 696e 6720 636f 6e64 6974 696f  llowing conditio
+00000220: 6e73 2061 7265 206d 6574 3a0d 0a20 2020  ns are met:..   
+00000230: 2020 2020 200d 0a20 2020 2020 2020 2031       ..        1
+00000240: 2e20 5265 6469 7374 7269 6275 7469 6f6e  . Redistribution
+00000250: 7320 6f66 2073 6f75 7263 6520 636f 6465  s of source code
+00000260: 206d 7573 7420 7265 7461 696e 2074 6865   must retain the
+00000270: 2061 626f 7665 2063 6f70 7972 6967 6874   above copyright
+00000280: 206e 6f74 6963 652c 2074 6869 730d 0a20   notice, this.. 
+00000290: 2020 2020 2020 2020 2020 6c69 7374 206f            list o
+000002a0: 6620 636f 6e64 6974 696f 6e73 2061 6e64  f conditions and
+000002b0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
+000002c0: 6973 636c 6169 6d65 722e 0d0a 2020 2020  isclaimer...    
+000002d0: 2020 2020 0d0a 2020 2020 2020 2020 322e      ..        2.
+000002e0: 2052 6564 6973 7472 6962 7574 696f 6e73   Redistributions
+000002f0: 2069 6e20 6269 6e61 7279 2066 6f72 6d20   in binary form 
+00000300: 6d75 7374 2072 6570 726f 6475 6365 2074  must reproduce t
+00000310: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
+00000320: 6874 206e 6f74 6963 652c 0d0a 2020 2020  ht notice,..    
+00000330: 2020 2020 2020 2074 6869 7320 6c69 7374         this list
+00000340: 206f 6620 636f 6e64 6974 696f 6e73 2061   of conditions a
+00000350: 6e64 2074 6865 2066 6f6c 6c6f 7769 6e67  nd the following
+00000360: 2064 6973 636c 6169 6d65 7220 696e 2074   disclaimer in t
+00000370: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00000380: 0d0a 2020 2020 2020 2020 2020 2061 6e64  ..           and
+00000390: 2f6f 7220 6f74 6865 7220 6d61 7465 7269  /or other materi
+000003a0: 616c 7320 7072 6f76 6964 6564 2077 6974  als provided wit
+000003b0: 6820 7468 6520 6469 7374 7269 6275 7469  h the distributi
+000003c0: 6f6e 2e0d 0a20 2020 2020 2020 200d 0a20  on...        .. 
+000003d0: 2020 2020 2020 2033 2e20 4e65 6974 6865         3. Neithe
+000003e0: 7220 7468 6520 6e61 6d65 206f 6620 7468  r the name of th
+000003f0: 6520 636f 7079 7269 6768 7420 686f 6c64  e copyright hold
+00000400: 6572 206e 6f72 2074 6865 206e 616d 6573  er nor the names
+00000410: 206f 6620 6974 730d 0a20 2020 2020 2020   of its..       
+00000420: 2020 2020 636f 6e74 7269 6275 746f 7273      contributors
+00000430: 206d 6179 2062 6520 7573 6564 2074 6f20   may be used to 
+00000440: 656e 646f 7273 6520 6f72 2070 726f 6d6f  endorse or promo
+00000450: 7465 2070 726f 6475 6374 7320 6465 7269  te products deri
+00000460: 7665 6420 6672 6f6d 0d0a 2020 2020 2020  ved from..      
+00000470: 2020 2020 2074 6869 7320 736f 6674 7761       this softwa
+00000480: 7265 2077 6974 686f 7574 2073 7065 6369  re without speci
+00000490: 6669 6320 7072 696f 7220 7772 6974 7465  fic prior writte
+000004a0: 6e20 7065 726d 6973 7369 6f6e 2e0d 0a20  n permission... 
+000004b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000004c0: 2054 4849 5320 534f 4654 5741 5245 2049   THIS SOFTWARE I
+000004d0: 5320 5052 4f56 4944 4544 2042 5920 5448  S PROVIDED BY TH
+000004e0: 4520 434f 5059 5249 4748 5420 484f 4c44  E COPYRIGHT HOLD
+000004f0: 4552 5320 414e 4420 434f 4e54 5249 4255  ERS AND CONTRIBU
+00000500: 544f 5253 2022 4153 2049 5322 0d0a 2020  TORS "AS IS"..  
+00000510: 2020 2020 2020 414e 4420 414e 5920 4558        AND ANY EX
+00000520: 5052 4553 5320 4f52 2049 4d50 4c49 4544  PRESS OR IMPLIED
+00000530: 2057 4152 5241 4e54 4945 532c 2049 4e43   WARRANTIES, INC
+00000540: 4c55 4449 4e47 2c20 4255 5420 4e4f 5420  LUDING, BUT NOT 
+00000550: 4c49 4d49 5445 4420 544f 2c20 5448 450d  LIMITED TO, THE.
+00000560: 0a20 2020 2020 2020 2049 4d50 4c49 4544  .        IMPLIED
+00000570: 2057 4152 5241 4e54 4945 5320 4f46 204d   WARRANTIES OF M
+00000580: 4552 4348 414e 5441 4249 4c49 5459 2041  ERCHANTABILITY A
+00000590: 4e44 2046 4954 4e45 5353 2046 4f52 2041  ND FITNESS FOR A
+000005a0: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
+000005b0: 4f53 4520 4152 450d 0a20 2020 2020 2020  OSE ARE..       
+000005c0: 2044 4953 434c 4149 4d45 442e 2049 4e20   DISCLAIMED. IN 
+000005d0: 4e4f 2045 5645 4e54 2053 4841 4c4c 2054  NO EVENT SHALL T
+000005e0: 4845 2043 4f50 5952 4947 4854 2048 4f4c  HE COPYRIGHT HOL
+000005f0: 4445 5220 4f52 2043 4f4e 5452 4942 5554  DER OR CONTRIBUT
+00000600: 4f52 5320 4245 204c 4941 424c 450d 0a20  ORS BE LIABLE.. 
+00000610: 2020 2020 2020 2046 4f52 2041 4e59 2044         FOR ANY D
+00000620: 4952 4543 542c 2049 4e44 4952 4543 542c  IRECT, INDIRECT,
+00000630: 2049 4e43 4944 454e 5441 4c2c 2053 5045   INCIDENTAL, SPE
+00000640: 4349 414c 2c20 4558 454d 504c 4152 592c  CIAL, EXEMPLARY,
+00000650: 204f 5220 434f 4e53 4551 5545 4e54 4941   OR CONSEQUENTIA
+00000660: 4c0d 0a20 2020 2020 2020 2044 414d 4147  L..        DAMAG
+00000670: 4553 2028 494e 434c 5544 494e 472c 2042  ES (INCLUDING, B
+00000680: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
+00000690: 4f2c 2050 524f 4355 5245 4d45 4e54 204f  O, PROCUREMENT O
+000006a0: 4620 5355 4253 5449 5455 5445 2047 4f4f  F SUBSTITUTE GOO
+000006b0: 4453 204f 520d 0a20 2020 2020 2020 2053  DS OR..        S
+000006c0: 4552 5649 4345 533b 204c 4f53 5320 4f46  ERVICES; LOSS OF
+000006d0: 2055 5345 2c20 4441 5441 2c20 4f52 2050   USE, DATA, OR P
+000006e0: 524f 4649 5453 3b20 4f52 2042 5553 494e  ROFITS; OR BUSIN
+000006f0: 4553 5320 494e 5445 5252 5550 5449 4f4e  ESS INTERRUPTION
+00000700: 2920 484f 5745 5645 520d 0a20 2020 2020  ) HOWEVER..     
+00000710: 2020 2043 4155 5345 4420 414e 4420 4f4e     CAUSED AND ON
+00000720: 2041 4e59 2054 4845 4f52 5920 4f46 204c   ANY THEORY OF L
+00000730: 4941 4249 4c49 5459 2c20 5748 4554 4845  IABILITY, WHETHE
+00000740: 5220 494e 2043 4f4e 5452 4143 542c 2053  R IN CONTRACT, S
+00000750: 5452 4943 5420 4c49 4142 494c 4954 592c  TRICT LIABILITY,
+00000760: 0d0a 2020 2020 2020 2020 4f52 2054 4f52  ..        OR TOR
+00000770: 5420 2849 4e43 4c55 4449 4e47 204e 4547  T (INCLUDING NEG
+00000780: 4c49 4745 4e43 4520 4f52 204f 5448 4552  LIGENCE OR OTHER
+00000790: 5749 5345 2920 4152 4953 494e 4720 494e  WISE) ARISING IN
+000007a0: 2041 4e59 2057 4159 204f 5554 204f 4620   ANY WAY OUT OF 
+000007b0: 5448 4520 5553 450d 0a20 2020 2020 2020  THE USE..       
+000007c0: 204f 4620 5448 4953 2053 4f46 5457 4152   OF THIS SOFTWAR
+000007d0: 452c 2045 5645 4e20 4946 2041 4456 4953  E, EVEN IF ADVIS
+000007e0: 4544 204f 4620 5448 4520 504f 5353 4942  ED OF THE POSSIB
+000007f0: 494c 4954 5920 4f46 2053 5543 4820 4441  ILITY OF SUCH DA
+00000800: 4d41 4745 2e0d 0a20 2020 2020 2020 200d  MAGE...        .
+00000810: 0a50 726f 6a65 6374 2d55 524c 3a20 686f  .Project-URL: ho
+00000820: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
+00000830: 6769 7468 7562 2e63 6f6d 2f73 6b74 696d  github.com/sktim
+00000840: 652f 736b 6261 7365 0d0a 5072 6f6a 6563  e/skbase..Projec
+00000850: 742d 5552 4c3a 2072 6570 6f73 6974 6f72  t-URL: repositor
+00000860: 792c 2068 7474 7073 3a2f 2f67 6974 6875  y, https://githu
+00000870: 622e 636f 6d2f 736b 7469 6d65 2f73 6b62  b.com/sktime/skb
+00000880: 6173 650d 0a50 726f 6a65 6374 2d55 524c  ase..Project-URL
+00000890: 3a20 646f 6375 6d65 6e74 6174 696f 6e2c  : documentation,
+000008a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000008b0: 636f 6d2f 736b 7469 6d65 2f73 6b62 6173  com/sktime/skbas
+000008c0: 650d 0a50 726f 6a65 6374 2d55 524c 3a20  e..Project-URL: 
+000008d0: 646f 776e 6c6f 6164 2c20 6874 7470 733a  download, https:
+000008e0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+000008f0: 6374 2f73 6b62 6173 652f 2366 696c 6573  ct/skbase/#files
+00000900: 0d0a 4b65 7977 6f72 6473 3a20 6461 7461  ..Keywords: data
+00000910: 2d73 6369 656e 6365 2c6d 6163 6869 6e65  -science,machine
+00000920: 2d6c 6561 726e 696e 672c 7363 696b 6974  -learning,scikit
+00000930: 2d6c 6561 726e 0d0a 436c 6173 7369 6669  -learn..Classifi
+00000940: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+00000950: 6965 6e63 6520 3a3a 2053 6369 656e 6365  ience :: Science
+00000960: 2f52 6573 6561 7263 680d 0a43 6c61 7373  /Research..Class
+00000970: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
+00000980: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000990: 6c6f 7065 7273 0d0a 436c 6173 7369 6669  lopers..Classifi
+000009a0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+000009b0: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
+000009c0: 5344 204c 6963 656e 7365 0d0a 436c 6173  SD License..Clas
+000009d0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000009e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000009f0: 5079 7468 6f6e 0d0a 436c 6173 7369 6669  Python..Classifi
+00000a00: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
+00000a10: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
+00000a20: 740d 0a43 6c61 7373 6966 6965 723a 2054  t..Classifier: T
+00000a30: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+00000a40: 6963 2f45 6e67 696e 6565 7269 6e67 0d0a  ic/Engineering..
+00000a50: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+00000a60: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000a70: 4d69 6372 6f73 6f66 7420 3a3a 2057 696e  Microsoft :: Win
+00000a80: 646f 7773 0d0a 436c 6173 7369 6669 6572  dows..Classifier
+00000a90: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000aa0: 656d 203a 3a20 504f 5349 580d 0a43 6c61  em :: POSIX..Cla
+00000ab0: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
+00000ac0: 6e67 2053 7973 7465 6d20 3a3a 2055 6e69  ng System :: Uni
+00000ad0: 780d 0a43 6c61 7373 6966 6965 723a 204f  x..Classifier: O
+00000ae0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000af0: 3a3a 204d 6163 4f53 0d0a 436c 6173 7369  :: MacOS..Classi
+00000b00: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000b10: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000b20: 7468 6f6e 203a 3a20 332e 370d 0a43 6c61  thon :: 3.7..Cla
+00000b30: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000b40: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000b50: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
+00000b60: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000b70: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000b80: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000b90: 390d 0a43 6c61 7373 6966 6965 723a 2050  9..Classifier: P
+00000ba0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000bb0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000bc0: 2033 2e31 300d 0a43 6c61 7373 6966 6965   3.10..Classifie
+00000bd0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000be0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000bf0: 6e20 3a3a 2033 2e31 310d 0a52 6571 7569  n :: 3.11..Requi
+00000c00: 7265 732d 5079 7468 6f6e 3a20 3c33 2e31  res-Python: <3.1
+00000c10: 322c 3e3d 332e 370d 0a44 6573 6372 6970  2,>=3.7..Descrip
+00000c20: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000c30: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000c40: 0d0a 5072 6f76 6964 6573 2d45 7874 7261  ..Provides-Extra
+00000c50: 3a20 616c 6c5f 6578 7472 6173 0d0a 5072  : all_extras..Pr
+00000c60: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
+00000c70: 760d 0a50 726f 7669 6465 732d 4578 7472  v..Provides-Extr
+00000c80: 613a 206c 696e 7465 7273 0d0a 5072 6f76  a: linters..Prov
+00000c90: 6964 6573 2d45 7874 7261 3a20 6269 6e64  ides-Extra: bind
+00000ca0: 6572 0d0a 5072 6f76 6964 6573 2d45 7874  er..Provides-Ext
+00000cb0: 7261 3a20 646f 6373 0d0a 5072 6f76 6964  ra: docs..Provid
+00000cc0: 6573 2d45 7874 7261 3a20 7465 7374 0d0a  es-Extra: test..
+00000cd0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000ce0: 4345 4e53 450d 0a0d 0a3c 6120 6872 6566  CENSE....<a href
+00000cf0: 3d22 6874 7470 733a 2f2f 736b 6261 7365  ="https://skbase
+00000d00: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000d10: 656e 2f6c 6174 6573 742f 223e 3c69 6d67  en/latest/"><img
+00000d20: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000d30: 7468 7562 2e63 6f6d 2f73 6b74 696d 652f  thub.com/sktime/
+00000d40: 736b 6261 7365 2f62 6c6f 622f 6d61 696e  skbase/blob/main
+00000d50: 2f64 6f63 732f 736f 7572 6365 2f69 6d61  /docs/source/ima
+00000d60: 6765 732f 736b 6261 7365 2d6c 6f67 6f2d  ges/skbase-logo-
+00000d70: 7769 7468 2d6e 616d 652e 706e 6722 2077  with-name.png" w
+00000d80: 6964 7468 3d22 3137 3522 2061 6c69 676e  idth="175" align
+00000d90: 3d22 7269 6768 7422 202f 3e3c 2f61 3e0d  ="right" /></a>.
+00000da0: 0a0d 0a23 2057 656c 636f 6d65 2074 6f20  ...# Welcome to 
+00000db0: 736b 6261 7365 0d0a 0d0a 3e20 4120 6261  skbase....> A ba
+00000dc0: 7365 2063 6c61 7373 2066 6f72 2073 6369  se class for sci
+00000dd0: 6b69 742d 6c65 6172 6e2d 6c69 6b65 2061  kit-learn-like a
+00000de0: 6e64 2073 6b74 696d 652d 6c69 6b65 2070  nd sktime-like p
+00000df0: 6172 616d 6574 7269 6320 6f62 6a65 6374  arametric object
+00000e00: 730d 0a0d 0a60 736b 6261 7365 6020 7072  s....`skbase` pr
+00000e10: 6f76 6964 6573 2062 6173 6520 636c 6173  ovides base clas
+00000e20: 7365 7320 666f 7220 6372 6561 7469 6e67  ses for creating
+00000e30: 2073 6369 6b69 742d 6c65 6172 6e2d 6c69   scikit-learn-li
+00000e40: 6b65 2070 6172 616d 6574 7269 6320 6f62  ke parametric ob
+00000e50: 6a65 6374 732c 0d0a 616c 6f6e 6720 7769  jects,..along wi
+00000e60: 7468 2074 6f6f 6c73 2074 6f20 6d61 6b65  th tools to make
+00000e70: 2069 7420 6561 7369 6572 2074 6f20 6275   it easier to bu
+00000e80: 696c 6420 796f 7572 206f 776e 2070 6163  ild your own pac
+00000e90: 6b61 6765 7320 7468 6174 2066 6f6c 6c6f  kages that follo
+00000ea0: 7720 7468 6573 650d 0a64 6573 6967 6e20  w these..design 
+00000eb0: 7061 7474 6572 6e73 2e0d 0a0d 0a3a 726f  patterns.....:ro
+00000ec0: 636b 6574 3a20 5665 7273 696f 6e20 302e  cket: Version 0.
+00000ed0: 342e 3620 6973 206e 6f77 2061 7661 696c  4.6 is now avail
+00000ee0: 6162 6c65 2e20 4368 6563 6b6f 7574 206f  able. Checkout o
+00000ef0: 7572 0d0a 5b72 656c 6561 7365 206e 6f74  ur..[release not
+00000f00: 6573 5d28 6874 7470 733a 2f2f 736b 6261  es](https://skba
+00000f10: 7365 2e72 6561 6474 6865 646f 6373 2e69  se.readthedocs.i
+00000f20: 6f2f 656e 2f6c 6174 6573 742f 6368 616e  o/en/latest/chan
+00000f30: 6765 6c6f 672e 6874 6d6c 292e 0d0a 0d0a  gelog.html).....
+00000f40: 7c20 4f76 6572 7669 6577 207c 207c 0d0a  | Overview | |..
+00000f50: 7c2d 2d2d 7c2d 2d2d 7c0d 0a7c 202a 2a43  |---|---|..| **C
+00000f60: 492f 4344 2a2a 207c 205b 215b 5465 7374  I/CD** | [![Test
+00000f70: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000f80: 622e 636f 6d2f 736b 7469 6d65 2f73 6b62  b.com/sktime/skb
+00000f90: 6173 652f 6163 7469 6f6e 732f 776f 726b  ase/actions/work
+00000fa0: 666c 6f77 732f 7465 7374 2e79 6d6c 2f62  flows/test.yml/b
+00000fb0: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
+00000fc0: 6d61 696e 295d 2868 7474 7073 3a2f 2f67  main)](https://g
+00000fd0: 6974 6875 622e 636f 6d2f 736b 7469 6d65  ithub.com/sktime
+00000fe0: 2f73 6b62 6173 652f 6163 7469 6f6e 732f  /skbase/actions/
+00000ff0: 776f 726b 666c 6f77 732f 7465 7374 2e79  workflows/test.y
+00001000: 6d6c 2920 5b21 5b63 6f64 6563 6f76 5d28  ml) [![codecov](
+00001010: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00001020: 696f 2f67 682f 736b 7469 6d65 2f73 6b62  io/gh/sktime/skb
+00001030: 6173 652f 6272 616e 6368 2f6d 6169 6e2f  ase/branch/main/
+00001040: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00001050: 746f 6b65 6e3d 324a 3432 344e 4c4f 3832  token=2J424NLO82
+00001060: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00001070: 6f76 2e69 6f2f 6768 2f73 6b74 696d 652f  ov.io/gh/sktime/
+00001080: 736b 6261 7365 2920 5b21 5b44 6f63 756d  skbase) [![Docum
+00001090: 656e 7461 7469 6f6e 2053 7461 7475 735d  entation Status]
+000010a0: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
+000010b0: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
+000010c0: 732f 736b 6261 7365 2f62 6164 6765 2f3f  s/skbase/badge/?
+000010d0: 7665 7273 696f 6e3d 6c61 7465 7374 295d  version=latest)]
+000010e0: 2868 7474 7073 3a2f 2f73 6b62 6173 652e  (https://skbase.
+000010f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00001100: 6e2f 6c61 7465 7374 2f3f 6261 6467 653d  n/latest/?badge=
+00001110: 6c61 7465 7374 2920 5b21 5b70 7265 2d63  latest) [![pre-c
+00001120: 6f6d 6d69 742e 6369 2073 7461 7475 735d  ommit.ci status]
+00001130: 2868 7474 7073 3a2f 2f72 6573 756c 7473  (https://results
+00001140: 2e70 7265 2d63 6f6d 6d69 742e 6369 2f62  .pre-commit.ci/b
+00001150: 6164 6765 2f67 6974 6875 622f 736b 7469  adge/github/skti
+00001160: 6d65 2f73 6b62 6173 652f 6d61 696e 2e73  me/skbase/main.s
+00001170: 7667 295d 2868 7474 7073 3a2f 2f72 6573  vg)](https://res
+00001180: 756c 7473 2e70 7265 2d63 6f6d 6d69 742e  ults.pre-commit.
+00001190: 6369 2f6c 6174 6573 742f 6769 7468 7562  ci/latest/github
+000011a0: 2f73 6b74 696d 652f 736b 6261 7365 2f6d  /sktime/skbase/m
+000011b0: 6169 6e29 207c 0d0a 7c20 2a2a 436f 6465  ain) |..| **Code
+000011c0: 2a2a 207c 2020 5b21 5b21 7079 7069 5d28  ** |  [![!pypi](
+000011d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000011e0: 6c64 732e 696f 2f70 7970 692f 762f 7363  lds.io/pypi/v/sc
+000011f0: 696b 6974 2d62 6173 653f 636f 6c6f 723d  ikit-base?color=
+00001200: 6f72 616e 6765 295d 2868 7474 7073 3a2f  orange)](https:/
+00001210: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00001220: 742f 736b 6261 7365 2f29 2020 5b21 5b21  t/skbase/)  [![!
+00001230: 7079 7468 6f6e 2d76 6572 7369 6f6e 735d  python-versions]
+00001240: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00001250: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+00001260: 6572 7369 6f6e 732f 7363 696b 6974 2d62  ersions/scikit-b
+00001270: 6173 6529 5d28 6874 7470 733a 2f2f 7777  ase)](https://ww
+00001280: 772e 7079 7468 6f6e 2e6f 7267 2f29 205b  w.python.org/) [
+00001290: 215b 2162 6c61 636b 5d28 6874 7470 733a  ![!black](https:
+000012a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000012b0: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
+000012c0: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
+000012d0: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+000012e0: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
+000012f0: 6163 6b29 205b 215b 7365 6375 7269 7479  ack) [![security
+00001300: 3a20 6261 6e64 6974 5d28 6874 7470 733a  : bandit](https:
+00001310: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001320: 2f62 6164 6765 2f73 6563 7572 6974 792d  /badge/security-
+00001330: 6261 6e64 6974 2d79 656c 6c6f 772e 7376  bandit-yellow.sv
+00001340: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00001350: 7562 2e63 6f6d 2f50 7943 5141 2f62 616e  ub.com/PyCQA/ban
+00001360: 6469 7429 207c 0d0a 7c20 2a2a 446f 776e  dit) |..| **Down
+00001370: 6c6f 6164 732a 2a7c 205b 215b 446f 776e  loads**| [![Down
+00001380: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
+00001390: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
+000013a0: 7065 7273 6f6e 616c 697a 6564 2d62 6164  personalized-bad
+000013b0: 6765 2f73 6369 6b69 742d 6261 7365 3f70  ge/scikit-base?p
+000013c0: 6572 696f 643d 7765 656b 2675 6e69 7473  eriod=week&units
+000013d0: 3d69 6e74 6572 6e61 7469 6f6e 616c 5f73  =international_s
+000013e0: 7973 7465 6d26 6c65 6674 5f63 6f6c 6f72  ystem&left_color
+000013f0: 3d67 7265 7926 7269 6768 745f 636f 6c6f  =grey&right_colo
+00001400: 723d 626c 7565 266c 6566 745f 7465 7874  r=blue&left_text
+00001410: 3d77 6565 6b6c 7925 3230 2870 7970 6929  =weekly%20(pypi)
+00001420: 295d 2868 7474 7073 3a2f 2f70 6570 792e  )](https://pepy.
+00001430: 7465 6368 2f70 726f 6a65 6374 2f73 6369  tech/project/sci
+00001440: 6b69 742d 6261 7365 2920 5b21 5b44 6f77  kit-base) [![Dow
+00001450: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
+00001460: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
+00001470: 2f70 6572 736f 6e61 6c69 7a65 642d 6261  /personalized-ba
+00001480: 6467 652f 7363 696b 6974 2d62 6173 653f  dge/scikit-base?
+00001490: 7065 7269 6f64 3d6d 6f6e 7468 2675 6e69  period=month&uni
+000014a0: 7473 3d69 6e74 6572 6e61 7469 6f6e 616c  ts=international
+000014b0: 5f73 7973 7465 6d26 6c65 6674 5f63 6f6c  _system&left_col
+000014c0: 6f72 3d67 7265 7926 7269 6768 745f 636f  or=grey&right_co
+000014d0: 6c6f 723d 626c 7565 266c 6566 745f 7465  lor=blue&left_te
+000014e0: 7874 3d6d 6f6e 7468 6c79 2532 3028 7079  xt=monthly%20(py
+000014f0: 7069 2929 5d28 6874 7470 733a 2f2f 7065  pi))](https://pe
+00001500: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
+00001510: 7363 696b 6974 2d62 6173 6529 205b 215b  scikit-base) [![
+00001520: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
+00001530: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
+00001540: 6563 682f 7065 7273 6f6e 616c 697a 6564  ech/personalized
+00001550: 2d62 6164 6765 2f73 6369 6b69 742d 6261  -badge/scikit-ba
+00001560: 7365 3f70 6572 696f 643d 746f 7461 6c26  se?period=total&
+00001570: 756e 6974 733d 696e 7465 726e 6174 696f  units=internatio
+00001580: 6e61 6c5f 7379 7374 656d 266c 6566 745f  nal_system&left_
+00001590: 636f 6c6f 723d 6772 6579 2672 6967 6874  color=grey&right
+000015a0: 5f63 6f6c 6f72 3d62 6c75 6526 6c65 6674  _color=blue&left
+000015b0: 5f74 6578 743d 6375 6d75 6c61 7469 7665  _text=cumulative
+000015c0: 2532 3028 7079 7069 2929 5d28 6874 7470  %20(pypi))](http
+000015d0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+000015e0: 6f6a 6563 742f 7363 696b 6974 2d62 6173  oject/scikit-bas
+000015f0: 6529 207c 0d0a 0d0a 3c21 2d2d 2041 4c4c  e) |....<!-- ALL
+00001600: 2d43 4f4e 5452 4942 5554 4f52 532d 4241  -CONTRIBUTORS-BA
+00001610: 4447 453a 5354 4152 5420 2d20 446f 206e  DGE:START - Do n
+00001620: 6f74 2072 656d 6f76 6520 6f72 206d 6f64  ot remove or mod
+00001630: 6966 7920 7468 6973 2073 6563 7469 6f6e  ify this section
+00001640: 202d 2d3e 0d0a 5b21 5b41 6c6c 2043 6f6e   -->..[![All Con
+00001650: 7472 6962 7574 6f72 735d 2868 7474 7073  tributors](https
+00001660: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001670: 6f2f 6261 6467 652f 616c 6c5f 636f 6e74  o/badge/all_cont
+00001680: 7269 6275 746f 7273 2d31 332d 6f72 616e  ributors-13-oran
+00001690: 6765 2e73 7667 3f73 7479 6c65 3d66 6c61  ge.svg?style=fla
+000016a0: 742d 7371 7561 7265 295d 2823 636f 6e74  t-square)](#cont
+000016b0: 7269 6275 746f 7273 290d 0a3c 212d 2d20  ributors)..<!-- 
+000016c0: 414c 4c2d 434f 4e54 5249 4255 544f 5253  ALL-CONTRIBUTORS
+000016d0: 2d42 4144 4745 3a45 4e44 202d 2d3e 0d0a  -BADGE:END -->..
+000016e0: 0d0a 2323 2044 6f63 756d 656e 7461 7469  ..## Documentati
+000016f0: 6f6e 0d0a 0d0a 546f 206c 6561 726e 206d  on....To learn m
+00001700: 6f72 6520 6162 6f75 7420 7468 6520 7061  ore about the pa
+00001710: 636b 6167 6520 6368 6563 6b6f 7574 206f  ckage checkout o
+00001720: 7572 205b 646f 6375 6d65 6e74 6174 696f  ur [documentatio
+00001730: 6e5d 2868 7474 7073 3a2f 2f73 6b62 6173  n](https://skbas
+00001740: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00001750: 2f65 6e2f 6c61 7465 7374 2f29 2e0d 0a0d  /en/latest/)....
+00001760: 0a23 2320 3a68 6f75 7267 6c61 7373 5f66  .## :hourglass_f
+00001770: 6c6f 7769 6e67 5f73 616e 643a 2049 6e73  lowing_sand: Ins
+00001780: 7461 6c6c 2073 6b62 6173 650d 0a46 6f72  tall skbase..For
+00001790: 2074 726f 7562 6c65 2073 686f 6f74 696e   trouble shootin
+000017a0: 6720 6f72 206d 6f72 6520 696e 666f 726d  g or more inform
+000017b0: 6174 696f 6e2c 2073 6565 206f 7572 0d0a  ation, see our..
+000017c0: 5b64 6574 6169 6c65 6420 696e 7374 616c  [detailed instal
+000017d0: 6c61 7469 6f6e 2069 6e73 7472 7563 7469  lation instructi
+000017e0: 6f6e 735d 2868 7474 7073 3a2f 2f73 6b62  ons](https://skb
+000017f0: 6173 652e 7265 6164 7468 6564 6f63 732e  ase.readthedocs.
+00001800: 696f 2f65 6e2f 6c61 7465 7374 2f75 7365  io/en/latest/use
+00001810: 725f 646f 6375 6d65 6e74 6174 696f 6e2f  r_documentation/
+00001820: 696e 7374 616c 6c61 7469 6f6e 2e68 746d  installation.htm
+00001830: 6c29 2e0d 0a0d 0a2d 202a 2a4f 7065 7261  l).....- **Opera
+00001840: 7469 6e67 2073 7973 7465 6d2a 2a3a 206d  ting system**: m
+00001850: 6163 4f53 2058 20c2 b720 4c69 6e75 7820  acOS X .. Linux 
+00001860: c2b7 2057 696e 646f 7773 2038 2e31 206f  .. Windows 8.1 o
+00001870: 7220 6869 6768 6572 0d0a 2d20 2a2a 5079  r higher..- **Py
+00001880: 7468 6f6e 2076 6572 7369 6f6e 2a2a 3a20  thon version**: 
+00001890: 5079 7468 6f6e 2033 2e37 2c20 332e 382c  Python 3.7, 3.8,
+000018a0: 2033 2e39 2c20 332e 3130 2061 6e64 2033   3.9, 3.10 and 3
+000018b0: 2e31 310d 0a2d 202a 2a50 6163 6b61 6765  .11..- **Package
+000018c0: 206d 616e 6167 6572 732a 2a3a 205b 7069   managers**: [pi
+000018d0: 705d 0d0a 0d0a 5b70 6970 5d3a 2068 7474  p]....[pip]: htt
+000018e0: 7073 3a2f 2f70 6970 2e70 7970 612e 696f  ps://pip.pypa.io
+000018f0: 2f65 6e2f 7374 6162 6c65 2f0d 0a0d 0a23  /en/stable/....#
+00001900: 2323 2070 6970 0d0a 736b 6261 7365 2072  ## pip..skbase r
+00001910: 656c 6561 7365 7320 6172 6520 6176 6169  eleases are avai
+00001920: 6c61 626c 6520 6173 2073 6f75 7263 6520  lable as source 
+00001930: 7061 636b 6167 6573 2061 6e64 2062 696e  packages and bin
+00001940: 6172 7920 7768 6565 6c73 2076 6961 2050  ary wheels via P
+00001950: 7950 490d 0a61 6e64 2063 616e 2062 6520  yPI..and can be 
+00001960: 696e 7374 616c 6c65 6420 7573 696e 6720  installed using 
+00001970: 7069 702e 2043 6865 636b 6f75 7420 7468  pip. Checkout th
+00001980: 6520 6675 6c6c 206c 6973 7420 6f66 2070  e full list of p
+00001990: 7265 2d63 6f6d 7069 6c65 6420 5b77 6865  re-compiled [whe
+000019a0: 656c 7320 6f6e 2050 7950 695d 2868 7474  els on PyPi](htt
+000019b0: 7073 3a2f 2f70 7970 692e 6f72 672f 7369  ps://pypi.org/si
+000019c0: 6d70 6c65 2f73 6b62 6173 652f 292e 0d0a  mple/skbase/)...
+000019d0: 0d0a 546f 2069 6e73 7461 6c6c 2074 6865  ..To install the
+000019e0: 2063 6f72 6520 7061 636b 6167 6520 7573   core package us
+000019f0: 653a 0d0a 0d0a 6060 6062 6173 680d 0a70  e:....```bash..p
+00001a00: 6970 2069 6e73 7461 6c6c 2073 6369 6b69  ip install sciki
+00001a10: 742d 6261 7365 0d0a 6060 600d 0a0d 0a6f  t-base..```....o
+00001a20: 722c 2069 6620 796f 7520 7761 6e74 2074  r, if you want t
+00001a30: 6f20 696e 7374 616c 6c20 7769 7468 2074  o install with t
+00001a40: 6865 206d 6178 696d 756d 2073 6574 206f  he maximum set o
+00001a50: 6620 6465 7065 6e64 656e 6369 6573 2c20  f dependencies, 
+00001a60: 7573 653a 0d0a 0d0a 6060 6062 6173 680d  use:....```bash.
+00001a70: 0a70 6970 2069 6e73 7461 6c6c 2073 6369  .pip install sci
+00001a80: 6b69 742d 6261 7365 5b61 6c6c 5f65 7874  kit-base[all_ext
+00001a90: 7261 735d 0d0a 6060 600d 0a              ras]..```..
```

### Comparing `scikit-base-0.4.5/README.md` & `scikit-base-0.4.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,208 +1,220 @@
-00000000: 0d0a 2320 5765 6c63 6f6d 6520 746f 2073  ..# Welcome to s
-00000010: 6b62 6173 650d 0a0d 0a3e 2041 2062 6173  kbase....> A bas
-00000020: 6520 636c 6173 7320 666f 7220 7363 696b  e class for scik
-00000030: 6974 2d6c 6561 726e 2d6c 696b 6520 616e  it-learn-like an
-00000040: 6420 736b 7469 6d65 2d6c 696b 6520 7061  d sktime-like pa
-00000050: 7261 6d65 7472 6963 206f 626a 6563 7473  rametric objects
-00000060: 0d0a 0d0a 6073 6b62 6173 6560 2070 726f  ....`skbase` pro
-00000070: 7669 6465 7320 6261 7365 2063 6c61 7373  vides base class
-00000080: 6573 2066 6f72 2063 7265 6174 696e 6720  es for creating 
-00000090: 7363 696b 6974 2d6c 6561 726e 2d6c 696b  scikit-learn-lik
-000000a0: 6520 7061 7261 6d65 7472 6963 206f 626a  e parametric obj
-000000b0: 6563 7473 2c0d 0a61 6c6f 6e67 2077 6974  ects,..along wit
-000000c0: 6820 746f 6f6c 7320 746f 206d 616b 6520  h tools to make 
-000000d0: 6974 2065 6173 6965 7220 746f 2062 7569  it easier to bui
-000000e0: 6c64 2079 6f75 7220 6f77 6e20 7061 636b  ld your own pack
-000000f0: 6167 6573 2074 6861 7420 666f 6c6c 6f77  ages that follow
-00000100: 2074 6865 7365 0d0a 6465 7369 676e 2070   these..design p
-00000110: 6174 7465 726e 732e 0d0a 0d0a 3a72 6f63  atterns.....:roc
-00000120: 6b65 743a 2056 6572 7369 6f6e 2030 2e34  ket: Version 0.4
-00000130: 2e35 2069 7320 6e6f 7720 6176 6169 6c61  .5 is now availa
-00000140: 626c 652e 2043 6865 636b 6f75 7420 6f75  ble. Checkout ou
-00000150: 720d 0a5b 7265 6c65 6173 6520 6e6f 7465  r..[release note
-00000160: 735d 2868 7474 7073 3a2f 2f73 6b62 6173  s](https://skbas
-00000170: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00000180: 2f65 6e2f 6c61 7465 7374 2f63 6861 6e67  /en/latest/chang
-00000190: 656c 6f67 2e68 746d 6c29 2e0d 0a0d 0a7c  elog.html).....|
-000001a0: 204f 7665 7276 6965 7720 7c20 7c0d 0a7c   Overview | |..|
-000001b0: 2d2d 2d7c 2d2d 2d7c 0d0a 7c20 2a2a 4349  ---|---|..| **CI
-000001c0: 2f43 442a 2a20 7c20 5b21 5b54 6573 7473  /CD** | [![Tests
-000001d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000001e0: 2e63 6f6d 2f73 6b74 696d 652f 736b 6261  .com/sktime/skba
-000001f0: 7365 2f61 6374 696f 6e73 2f77 6f72 6b66  se/actions/workf
-00000200: 6c6f 7773 2f74 6573 742e 796d 6c2f 6261  lows/test.yml/ba
-00000210: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-00000220: 6169 6e29 5d28 6874 7470 733a 2f2f 6769  ain)](https://gi
-00000230: 7468 7562 2e63 6f6d 2f73 6b74 696d 652f  thub.com/sktime/
-00000240: 736b 6261 7365 2f61 6374 696f 6e73 2f77  skbase/actions/w
-00000250: 6f72 6b66 6c6f 7773 2f74 6573 742e 796d  orkflows/test.ym
-00000260: 6c29 205b 215b 636f 6465 636f 765d 2868  l) [![codecov](h
-00000270: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-00000280: 6f2f 6768 2f73 6b74 696d 652f 736b 6261  o/gh/sktime/skba
-00000290: 7365 2f62 7261 6e63 682f 6d61 696e 2f67  se/branch/main/g
-000002a0: 7261 7068 2f62 6164 6765 2e73 7667 3f74  raph/badge.svg?t
-000002b0: 6f6b 656e 3d32 4a34 3234 4e4c 4f38 3229  oken=2J424NLO82)
-000002c0: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
-000002d0: 762e 696f 2f67 682f 736b 7469 6d65 2f73  v.io/gh/sktime/s
-000002e0: 6b62 6173 6529 205b 215b 446f 6375 6d65  kbase) [![Docume
-000002f0: 6e74 6174 696f 6e20 5374 6174 7573 5d28  ntation Status](
-00000300: 6874 7470 733a 2f2f 7265 6164 7468 6564  https://readthed
-00000310: 6f63 732e 6f72 672f 7072 6f6a 6563 7473  ocs.org/projects
-00000320: 2f73 6b62 6173 652f 6261 6467 652f 3f76  /skbase/badge/?v
-00000330: 6572 7369 6f6e 3d6c 6174 6573 7429 5d28  ersion=latest)](
-00000340: 6874 7470 733a 2f2f 736b 6261 7365 2e72  https://skbase.r
-00000350: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000360: 2f6c 6174 6573 742f 3f62 6164 6765 3d6c  /latest/?badge=l
-00000370: 6174 6573 7429 205b 215b 7072 652d 636f  atest) [![pre-co
-00000380: 6d6d 6974 2e63 6920 7374 6174 7573 5d28  mmit.ci status](
-00000390: 6874 7470 733a 2f2f 7265 7375 6c74 732e  https://results.
-000003a0: 7072 652d 636f 6d6d 6974 2e63 692f 6261  pre-commit.ci/ba
-000003b0: 6467 652f 6769 7468 7562 2f73 6b74 696d  dge/github/sktim
-000003c0: 652f 736b 6261 7365 2f6d 6169 6e2e 7376  e/skbase/main.sv
-000003d0: 6729 5d28 6874 7470 733a 2f2f 7265 7375  g)](https://resu
-000003e0: 6c74 732e 7072 652d 636f 6d6d 6974 2e63  lts.pre-commit.c
-000003f0: 692f 6c61 7465 7374 2f67 6974 6875 622f  i/latest/github/
-00000400: 736b 7469 6d65 2f73 6b62 6173 652f 6d61  sktime/skbase/ma
-00000410: 696e 2920 7c0d 0a7c 202a 2a43 6f64 652a  in) |..| **Code*
-00000420: 2a20 7c20 205b 215b 2170 7970 695d 2868  * |  [![!pypi](h
-00000430: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000440: 6473 2e69 6f2f 7079 7069 2f76 2f73 6369  ds.io/pypi/v/sci
-00000450: 6b69 742d 6261 7365 3f63 6f6c 6f72 3d6f  kit-base?color=o
-00000460: 7261 6e67 6529 5d28 6874 7470 733a 2f2f  range)](https://
-00000470: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000480: 2f73 6b62 6173 652f 2920 205b 215b 2170  /skbase/)  [![!p
-00000490: 7974 686f 6e2d 7665 7273 696f 6e73 5d28  ython-versions](
-000004a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000004b0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
-000004c0: 7273 696f 6e73 2f73 6369 6b69 742d 6261  rsions/scikit-ba
-000004d0: 7365 295d 2868 7474 7073 3a2f 2f77 7777  se)](https://www
-000004e0: 2e70 7974 686f 6e2e 6f72 672f 2920 5b21  .python.org/) [!
-000004f0: 5b21 626c 6163 6b5d 2868 7474 7073 3a2f  [!black](https:/
-00000500: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000510: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
-00000520: 6c65 2d62 6c61 636b 2d30 3030 3030 302e  le-black-000000.
-00000530: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
-00000540: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
-00000550: 636b 2920 5b21 5b73 6563 7572 6974 793a  ck) [![security:
-00000560: 2062 616e 6469 745d 2868 7474 7073 3a2f   bandit](https:/
-00000570: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000580: 6261 6467 652f 7365 6375 7269 7479 2d62  badge/security-b
-00000590: 616e 6469 742d 7965 6c6c 6f77 2e73 7667  andit-yellow.svg
-000005a0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-000005b0: 622e 636f 6d2f 5079 4351 412f 6261 6e64  b.com/PyCQA/band
-000005c0: 6974 2920 7c0d 0a7c 202a 2a44 6f77 6e6c  it) |..| **Downl
-000005d0: 6f61 6473 2a2a 7c20 5b21 5b44 6f77 6e6c  oads**| [![Downl
-000005e0: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
-000005f0: 6174 6963 2e70 6570 792e 7465 6368 2f70  atic.pepy.tech/p
-00000600: 6572 736f 6e61 6c69 7a65 642d 6261 6467  ersonalized-badg
-00000610: 652f 7363 696b 6974 2d62 6173 653f 7065  e/scikit-base?pe
-00000620: 7269 6f64 3d77 6565 6b26 756e 6974 733d  riod=week&units=
-00000630: 696e 7465 726e 6174 696f 6e61 6c5f 7379  international_sy
-00000640: 7374 656d 266c 6566 745f 636f 6c6f 723d  stem&left_color=
-00000650: 6772 6579 2672 6967 6874 5f63 6f6c 6f72  grey&right_color
-00000660: 3d62 6c75 6526 6c65 6674 5f74 6578 743d  =blue&left_text=
-00000670: 7765 656b 6c79 2532 3028 7079 7069 2929  weekly%20(pypi))
-00000680: 5d28 6874 7470 733a 2f2f 7065 7079 2e74  ](https://pepy.t
-00000690: 6563 682f 7072 6f6a 6563 742f 7363 696b  ech/project/scik
-000006a0: 6974 2d62 6173 6529 205b 215b 446f 776e  it-base) [![Down
-000006b0: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
-000006c0: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
-000006d0: 7065 7273 6f6e 616c 697a 6564 2d62 6164  personalized-bad
-000006e0: 6765 2f73 6369 6b69 742d 6261 7365 3f70  ge/scikit-base?p
-000006f0: 6572 696f 643d 6d6f 6e74 6826 756e 6974  eriod=month&unit
-00000700: 733d 696e 7465 726e 6174 696f 6e61 6c5f  s=international_
-00000710: 7379 7374 656d 266c 6566 745f 636f 6c6f  system&left_colo
-00000720: 723d 6772 6579 2672 6967 6874 5f63 6f6c  r=grey&right_col
-00000730: 6f72 3d62 6c75 6526 6c65 6674 5f74 6578  or=blue&left_tex
-00000740: 743d 6d6f 6e74 686c 7925 3230 2870 7970  t=monthly%20(pyp
-00000750: 6929 295d 2868 7474 7073 3a2f 2f70 6570  i))](https://pep
-00000760: 792e 7465 6368 2f70 726f 6a65 6374 2f73  y.tech/project/s
-00000770: 6369 6b69 742d 6261 7365 2920 5b21 5b44  cikit-base) [![D
-00000780: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
-00000790: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
-000007a0: 6368 2f70 6572 736f 6e61 6c69 7a65 642d  ch/personalized-
-000007b0: 6261 6467 652f 7363 696b 6974 2d62 6173  badge/scikit-bas
-000007c0: 653f 7065 7269 6f64 3d74 6f74 616c 2675  e?period=total&u
-000007d0: 6e69 7473 3d69 6e74 6572 6e61 7469 6f6e  nits=internation
-000007e0: 616c 5f73 7973 7465 6d26 6c65 6674 5f63  al_system&left_c
-000007f0: 6f6c 6f72 3d67 7265 7926 7269 6768 745f  olor=grey&right_
-00000800: 636f 6c6f 723d 626c 7565 266c 6566 745f  color=blue&left_
-00000810: 7465 7874 3d63 756d 756c 6174 6976 6525  text=cumulative%
-00000820: 3230 2870 7970 6929 295d 2868 7474 7073  20(pypi))](https
-00000830: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
-00000840: 6a65 6374 2f73 6369 6b69 742d 6261 7365  ject/scikit-base
-00000850: 2920 7c0d 0a0d 0a3c 212d 2d20 414c 4c2d  ) |....<!-- ALL-
-00000860: 434f 4e54 5249 4255 544f 5253 2d42 4144  CONTRIBUTORS-BAD
-00000870: 4745 3a53 5441 5254 202d 2044 6f20 6e6f  GE:START - Do no
-00000880: 7420 7265 6d6f 7665 206f 7220 6d6f 6469  t remove or modi
-00000890: 6679 2074 6869 7320 7365 6374 696f 6e20  fy this section 
-000008a0: 2d2d 3e0d 0a5b 215b 416c 6c20 436f 6e74  -->..[![All Cont
-000008b0: 7269 6275 746f 7273 5d28 6874 7470 733a  ributors](https:
-000008c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000008d0: 2f62 6164 6765 2f61 6c6c 5f63 6f6e 7472  /badge/all_contr
-000008e0: 6962 7574 6f72 732d 3133 2d6f 7261 6e67  ibutors-13-orang
-000008f0: 652e 7376 673f 7374 796c 653d 666c 6174  e.svg?style=flat
-00000900: 2d73 7175 6172 6529 5d28 2363 6f6e 7472  -square)](#contr
-00000910: 6962 7574 6f72 7329 0d0a 3c21 2d2d 2041  ibutors)..<!-- A
-00000920: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
-00000930: 4241 4447 453a 454e 4420 2d2d 3e0d 0a0d  BADGE:END -->...
-00000940: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
-00000950: 6e0d 0a0d 0a54 6f20 6c65 6172 6e20 6d6f  n....To learn mo
-00000960: 7265 2061 626f 7574 2074 6865 2070 6163  re about the pac
-00000970: 6b61 6765 2063 6865 636b 6f75 7420 6f75  kage checkout ou
-00000980: 7220 5b64 6f63 756d 656e 7461 7469 6f6e  r [documentation
-00000990: 5d28 6874 7470 733a 2f2f 736b 6261 7365  ](https://skbase
-000009a0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000009b0: 656e 2f6c 6174 6573 742f 292e 0d0a 0d0a  en/latest/).....
-000009c0: 2323 203a 686f 7572 676c 6173 735f 666c  ## :hourglass_fl
-000009d0: 6f77 696e 675f 7361 6e64 3a20 496e 7374  owing_sand: Inst
-000009e0: 616c 6c20 736b 6261 7365 0d0a 466f 7220  all skbase..For 
-000009f0: 7472 6f75 626c 6520 7368 6f6f 7469 6e67  trouble shooting
-00000a00: 206f 7220 6d6f 7265 2069 6e66 6f72 6d61   or more informa
-00000a10: 7469 6f6e 2c20 7365 6520 6f75 720d 0a5b  tion, see our..[
-00000a20: 6465 7461 696c 6564 2069 6e73 7461 6c6c  detailed install
-00000a30: 6174 696f 6e20 696e 7374 7275 6374 696f  ation instructio
-00000a40: 6e73 5d28 6874 7470 733a 2f2f 736b 6261  ns](https://skba
-00000a50: 7365 2e72 6561 6474 6865 646f 6373 2e69  se.readthedocs.i
-00000a60: 6f2f 656e 2f6c 6174 6573 742f 7573 6572  o/en/latest/user
-00000a70: 5f64 6f63 756d 656e 7461 7469 6f6e 2f69  _documentation/i
-00000a80: 6e73 7461 6c6c 6174 696f 6e2e 6874 6d6c  nstallation.html
-00000a90: 292e 0d0a 0d0a 2d20 2a2a 4f70 6572 6174  ).....- **Operat
-00000aa0: 696e 6720 7379 7374 656d 2a2a 3a20 6d61  ing system**: ma
-00000ab0: 634f 5320 5820 c2b7 204c 696e 7578 20c2  cOS X .. Linux .
-00000ac0: b720 5769 6e64 6f77 7320 382e 3120 6f72  . Windows 8.1 or
-00000ad0: 2068 6967 6865 720d 0a2d 202a 2a50 7974   higher..- **Pyt
-00000ae0: 686f 6e20 7665 7273 696f 6e2a 2a3a 2050  hon version**: P
-00000af0: 7974 686f 6e20 332e 372c 2033 2e38 2c20  ython 3.7, 3.8, 
-00000b00: 332e 392c 2033 2e31 3020 616e 6420 332e  3.9, 3.10 and 3.
-00000b10: 3131 0d0a 2d20 2a2a 5061 636b 6167 6520  11..- **Package 
-00000b20: 6d61 6e61 6765 7273 2a2a 3a20 5b70 6970  managers**: [pip
-00000b30: 5d0d 0a0d 0a5b 7069 705d 3a20 6874 7470  ]....[pip]: http
-00000b40: 733a 2f2f 7069 702e 7079 7061 2e69 6f2f  s://pip.pypa.io/
-00000b50: 656e 2f73 7461 626c 652f 0d0a 0d0a 2323  en/stable/....##
-00000b60: 2320 7069 700d 0a73 6b62 6173 6520 7265  # pip..skbase re
-00000b70: 6c65 6173 6573 2061 7265 2061 7661 696c  leases are avail
-00000b80: 6162 6c65 2061 7320 736f 7572 6365 2070  able as source p
-00000b90: 6163 6b61 6765 7320 616e 6420 6269 6e61  ackages and bina
-00000ba0: 7279 2077 6865 656c 7320 7669 6120 5079  ry wheels via Py
-00000bb0: 5049 0d0a 616e 6420 6361 6e20 6265 2069  PI..and can be i
-00000bc0: 6e73 7461 6c6c 6564 2075 7369 6e67 2070  nstalled using p
-00000bd0: 6970 2e20 4368 6563 6b6f 7574 2074 6865  ip. Checkout the
-00000be0: 2066 756c 6c20 6c69 7374 206f 6620 7072   full list of pr
-00000bf0: 652d 636f 6d70 696c 6564 205b 7768 6565  e-compiled [whee
-00000c00: 6c73 206f 6e20 5079 5069 5d28 6874 7470  ls on PyPi](http
-00000c10: 733a 2f2f 7079 7069 2e6f 7267 2f73 696d  s://pypi.org/sim
-00000c20: 706c 652f 736b 6261 7365 2f29 2e0d 0a0d  ple/skbase/)....
-00000c30: 0a54 6f20 696e 7374 616c 6c20 7468 6520  .To install the 
-00000c40: 636f 7265 2070 6163 6b61 6765 2075 7365  core package use
-00000c50: 3a0d 0a0d 0a60 6060 6261 7368 0d0a 7069  :....```bash..pi
-00000c60: 7020 696e 7374 616c 6c20 7363 696b 6974  p install scikit
-00000c70: 2d62 6173 650d 0a60 6060 0d0a 0d0a 6f72  -base..```....or
-00000c80: 2c20 6966 2079 6f75 2077 616e 7420 746f  , if you want to
-00000c90: 2069 6e73 7461 6c6c 2077 6974 6820 7468   install with th
-00000ca0: 6520 6d61 7869 6d75 6d20 7365 7420 6f66  e maximum set of
-00000cb0: 2064 6570 656e 6465 6e63 6965 732c 2075   dependencies, u
-00000cc0: 7365 3a0d 0a0d 0a60 6060 6261 7368 0d0a  se:....```bash..
-00000cd0: 7069 7020 696e 7374 616c 6c20 7363 696b  pip install scik
-00000ce0: 6974 2d62 6173 655b 616c 6c5f 6578 7472  it-base[all_extr
-00000cf0: 6173 5d0d 0a60 6060 0d0a                 as]..```..
+00000000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000010: 2f73 6b62 6173 652e 7265 6164 7468 6564  /skbase.readthed
+00000020: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000030: 2f22 3e3c 696d 6720 7372 633d 2268 7474  /"><img src="htt
+00000040: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000050: 736b 7469 6d65 2f73 6b62 6173 652f 626c  sktime/skbase/bl
+00000060: 6f62 2f6d 6169 6e2f 646f 6373 2f73 6f75  ob/main/docs/sou
+00000070: 7263 652f 696d 6167 6573 2f73 6b62 6173  rce/images/skbas
+00000080: 652d 6c6f 676f 2d77 6974 682d 6e61 6d65  e-logo-with-name
+00000090: 2e70 6e67 2220 7769 6474 683d 2231 3735  .png" width="175
+000000a0: 2220 616c 6967 6e3d 2272 6967 6874 2220  " align="right" 
+000000b0: 2f3e 3c2f 613e 0d0a 0d0a 2320 5765 6c63  /></a>....# Welc
+000000c0: 6f6d 6520 746f 2073 6b62 6173 650d 0a0d  ome to skbase...
+000000d0: 0a3e 2041 2062 6173 6520 636c 6173 7320  .> A base class 
+000000e0: 666f 7220 7363 696b 6974 2d6c 6561 726e  for scikit-learn
+000000f0: 2d6c 696b 6520 616e 6420 736b 7469 6d65  -like and sktime
+00000100: 2d6c 696b 6520 7061 7261 6d65 7472 6963  -like parametric
+00000110: 206f 626a 6563 7473 0d0a 0d0a 6073 6b62   objects....`skb
+00000120: 6173 6560 2070 726f 7669 6465 7320 6261  ase` provides ba
+00000130: 7365 2063 6c61 7373 6573 2066 6f72 2063  se classes for c
+00000140: 7265 6174 696e 6720 7363 696b 6974 2d6c  reating scikit-l
+00000150: 6561 726e 2d6c 696b 6520 7061 7261 6d65  earn-like parame
+00000160: 7472 6963 206f 626a 6563 7473 2c0d 0a61  tric objects,..a
+00000170: 6c6f 6e67 2077 6974 6820 746f 6f6c 7320  long with tools 
+00000180: 746f 206d 616b 6520 6974 2065 6173 6965  to make it easie
+00000190: 7220 746f 2062 7569 6c64 2079 6f75 7220  r to build your 
+000001a0: 6f77 6e20 7061 636b 6167 6573 2074 6861  own packages tha
+000001b0: 7420 666f 6c6c 6f77 2074 6865 7365 0d0a  t follow these..
+000001c0: 6465 7369 676e 2070 6174 7465 726e 732e  design patterns.
+000001d0: 0d0a 0d0a 3a72 6f63 6b65 743a 2056 6572  ....:rocket: Ver
+000001e0: 7369 6f6e 2030 2e34 2e36 2069 7320 6e6f  sion 0.4.6 is no
+000001f0: 7720 6176 6169 6c61 626c 652e 2043 6865  w available. Che
+00000200: 636b 6f75 7420 6f75 720d 0a5b 7265 6c65  ckout our..[rele
+00000210: 6173 6520 6e6f 7465 735d 2868 7474 7073  ase notes](https
+00000220: 3a2f 2f73 6b62 6173 652e 7265 6164 7468  ://skbase.readth
+00000230: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00000240: 7374 2f63 6861 6e67 656c 6f67 2e68 746d  st/changelog.htm
+00000250: 6c29 2e0d 0a0d 0a7c 204f 7665 7276 6965  l).....| Overvie
+00000260: 7720 7c20 7c0d 0a7c 2d2d 2d7c 2d2d 2d7c  w | |..|---|---|
+00000270: 0d0a 7c20 2a2a 4349 2f43 442a 2a20 7c20  ..| **CI/CD** | 
+00000280: 5b21 5b54 6573 7473 5d28 6874 7470 733a  [![Tests](https:
+00000290: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6b74  //github.com/skt
+000002a0: 696d 652f 736b 6261 7365 2f61 6374 696f  ime/skbase/actio
+000002b0: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
+000002c0: 742e 796d 6c2f 6261 6467 652e 7376 673f  t.yml/badge.svg?
+000002d0: 6272 616e 6368 3d6d 6169 6e29 5d28 6874  branch=main)](ht
+000002e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000002f0: 2f73 6b74 696d 652f 736b 6261 7365 2f61  /sktime/skbase/a
+00000300: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000310: 2f74 6573 742e 796d 6c29 205b 215b 636f  /test.yml) [![co
+00000320: 6465 636f 765d 2868 7474 7073 3a2f 2f63  decov](https://c
+00000330: 6f64 6563 6f76 2e69 6f2f 6768 2f73 6b74  odecov.io/gh/skt
+00000340: 696d 652f 736b 6261 7365 2f62 7261 6e63  ime/skbase/branc
+00000350: 682f 6d61 696e 2f67 7261 7068 2f62 6164  h/main/graph/bad
+00000360: 6765 2e73 7667 3f74 6f6b 656e 3d32 4a34  ge.svg?token=2J4
+00000370: 3234 4e4c 4f38 3229 5d28 6874 7470 733a  24NLO82)](https:
+00000380: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
+00000390: 736b 7469 6d65 2f73 6b62 6173 6529 205b  sktime/skbase) [
+000003a0: 215b 446f 6375 6d65 6e74 6174 696f 6e20  ![Documentation 
+000003b0: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
+000003c0: 7265 6164 7468 6564 6f63 732e 6f72 672f  readthedocs.org/
+000003d0: 7072 6f6a 6563 7473 2f73 6b62 6173 652f  projects/skbase/
+000003e0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+000003f0: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
+00000400: 736b 6261 7365 2e72 6561 6474 6865 646f  skbase.readthedo
+00000410: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000420: 3f62 6164 6765 3d6c 6174 6573 7429 205b  ?badge=latest) [
+00000430: 215b 7072 652d 636f 6d6d 6974 2e63 6920  ![pre-commit.ci 
+00000440: 7374 6174 7573 5d28 6874 7470 733a 2f2f  status](https://
+00000450: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
+00000460: 6974 2e63 692f 6261 6467 652f 6769 7468  it.ci/badge/gith
+00000470: 7562 2f73 6b74 696d 652f 736b 6261 7365  ub/sktime/skbase
+00000480: 2f6d 6169 6e2e 7376 6729 5d28 6874 7470  /main.svg)](http
+00000490: 733a 2f2f 7265 7375 6c74 732e 7072 652d  s://results.pre-
+000004a0: 636f 6d6d 6974 2e63 692f 6c61 7465 7374  commit.ci/latest
+000004b0: 2f67 6974 6875 622f 736b 7469 6d65 2f73  /github/sktime/s
+000004c0: 6b62 6173 652f 6d61 696e 2920 7c0d 0a7c  kbase/main) |..|
+000004d0: 202a 2a43 6f64 652a 2a20 7c20 205b 215b   **Code** |  [![
+000004e0: 2170 7970 695d 2868 7474 7073 3a2f 2f69  !pypi](https://i
+000004f0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000500: 7069 2f76 2f73 6369 6b69 742d 6261 7365  pi/v/scikit-base
+00000510: 3f63 6f6c 6f72 3d6f 7261 6e67 6529 5d28  ?color=orange)](
+00000520: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000530: 2f70 726f 6a65 6374 2f73 6b62 6173 652f  /project/skbase/
+00000540: 2920 205b 215b 2170 7974 686f 6e2d 7665  )  [![!python-ve
+00000550: 7273 696f 6e73 5d28 6874 7470 733a 2f2f  rsions](https://
+00000560: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000570: 7970 692f 7079 7665 7273 696f 6e73 2f73  ypi/pyversions/s
+00000580: 6369 6b69 742d 6261 7365 295d 2868 7474  cikit-base)](htt
+00000590: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+000005a0: 6f72 672f 2920 5b21 5b21 626c 6163 6b5d  org/) [![!black]
+000005b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000005c0: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
+000005d0: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
+000005e0: 2d30 3030 3030 302e 7376 6729 5d28 6874  -000000.svg)](ht
+000005f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000600: 2f70 7366 2f62 6c61 636b 2920 5b21 5b73  /psf/black) [![s
+00000610: 6563 7572 6974 793a 2062 616e 6469 745d  ecurity: bandit]
+00000620: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000630: 656c 6473 2e69 6f2f 6261 6467 652f 7365  elds.io/badge/se
+00000640: 6375 7269 7479 2d62 616e 6469 742d 7965  curity-bandit-ye
+00000650: 6c6c 6f77 2e73 7667 295d 2868 7474 7073  llow.svg)](https
+00000660: 3a2f 2f67 6974 6875 622e 636f 6d2f 5079  ://github.com/Py
+00000670: 4351 412f 6261 6e64 6974 2920 7c0d 0a7c  CQA/bandit) |..|
+00000680: 202a 2a44 6f77 6e6c 6f61 6473 2a2a 7c20   **Downloads**| 
+00000690: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
+000006a0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
+000006b0: 792e 7465 6368 2f70 6572 736f 6e61 6c69  y.tech/personali
+000006c0: 7a65 642d 6261 6467 652f 7363 696b 6974  zed-badge/scikit
+000006d0: 2d62 6173 653f 7065 7269 6f64 3d77 6565  -base?period=wee
+000006e0: 6b26 756e 6974 733d 696e 7465 726e 6174  k&units=internat
+000006f0: 696f 6e61 6c5f 7379 7374 656d 266c 6566  ional_system&lef
+00000700: 745f 636f 6c6f 723d 6772 6579 2672 6967  t_color=grey&rig
+00000710: 6874 5f63 6f6c 6f72 3d62 6c75 6526 6c65  ht_color=blue&le
+00000720: 6674 5f74 6578 743d 7765 656b 6c79 2532  ft_text=weekly%2
+00000730: 3028 7079 7069 2929 5d28 6874 7470 733a  0(pypi))](https:
+00000740: 2f2f 7065 7079 2e74 6563 682f 7072 6f6a  //pepy.tech/proj
+00000750: 6563 742f 7363 696b 6974 2d62 6173 6529  ect/scikit-base)
+00000760: 205b 215b 446f 776e 6c6f 6164 735d 2868   [![Downloads](h
+00000770: 7474 7073 3a2f 2f73 7461 7469 632e 7065  ttps://static.pe
+00000780: 7079 2e74 6563 682f 7065 7273 6f6e 616c  py.tech/personal
+00000790: 697a 6564 2d62 6164 6765 2f73 6369 6b69  ized-badge/sciki
+000007a0: 742d 6261 7365 3f70 6572 696f 643d 6d6f  t-base?period=mo
+000007b0: 6e74 6826 756e 6974 733d 696e 7465 726e  nth&units=intern
+000007c0: 6174 696f 6e61 6c5f 7379 7374 656d 266c  ational_system&l
+000007d0: 6566 745f 636f 6c6f 723d 6772 6579 2672  eft_color=grey&r
+000007e0: 6967 6874 5f63 6f6c 6f72 3d62 6c75 6526  ight_color=blue&
+000007f0: 6c65 6674 5f74 6578 743d 6d6f 6e74 686c  left_text=monthl
+00000800: 7925 3230 2870 7970 6929 295d 2868 7474  y%20(pypi))](htt
+00000810: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00000820: 726f 6a65 6374 2f73 6369 6b69 742d 6261  roject/scikit-ba
+00000830: 7365 2920 5b21 5b44 6f77 6e6c 6f61 6473  se) [![Downloads
+00000840: 5d28 6874 7470 733a 2f2f 7374 6174 6963  ](https://static
+00000850: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
+00000860: 6e61 6c69 7a65 642d 6261 6467 652f 7363  nalized-badge/sc
+00000870: 696b 6974 2d62 6173 653f 7065 7269 6f64  ikit-base?period
+00000880: 3d74 6f74 616c 2675 6e69 7473 3d69 6e74  =total&units=int
+00000890: 6572 6e61 7469 6f6e 616c 5f73 7973 7465  ernational_syste
+000008a0: 6d26 6c65 6674 5f63 6f6c 6f72 3d67 7265  m&left_color=gre
+000008b0: 7926 7269 6768 745f 636f 6c6f 723d 626c  y&right_color=bl
+000008c0: 7565 266c 6566 745f 7465 7874 3d63 756d  ue&left_text=cum
+000008d0: 756c 6174 6976 6525 3230 2870 7970 6929  ulative%20(pypi)
+000008e0: 295d 2868 7474 7073 3a2f 2f70 6570 792e  )](https://pepy.
+000008f0: 7465 6368 2f70 726f 6a65 6374 2f73 6369  tech/project/sci
+00000900: 6b69 742d 6261 7365 2920 7c0d 0a0d 0a3c  kit-base) |....<
+00000910: 212d 2d20 414c 4c2d 434f 4e54 5249 4255  !-- ALL-CONTRIBU
+00000920: 544f 5253 2d42 4144 4745 3a53 5441 5254  TORS-BADGE:START
+00000930: 202d 2044 6f20 6e6f 7420 7265 6d6f 7665   - Do not remove
+00000940: 206f 7220 6d6f 6469 6679 2074 6869 7320   or modify this 
+00000950: 7365 6374 696f 6e20 2d2d 3e0d 0a5b 215b  section -->..[![
+00000960: 416c 6c20 436f 6e74 7269 6275 746f 7273  All Contributors
+00000970: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000980: 6965 6c64 732e 696f 2f62 6164 6765 2f61  ields.io/badge/a
+00000990: 6c6c 5f63 6f6e 7472 6962 7574 6f72 732d  ll_contributors-
+000009a0: 3133 2d6f 7261 6e67 652e 7376 673f 7374  13-orange.svg?st
+000009b0: 796c 653d 666c 6174 2d73 7175 6172 6529  yle=flat-square)
+000009c0: 5d28 2363 6f6e 7472 6962 7574 6f72 7329  ](#contributors)
+000009d0: 0d0a 3c21 2d2d 2041 4c4c 2d43 4f4e 5452  ..<!-- ALL-CONTR
+000009e0: 4942 5554 4f52 532d 4241 4447 453a 454e  IBUTORS-BADGE:EN
+000009f0: 4420 2d2d 3e0d 0a0d 0a23 2320 446f 6375  D -->....## Docu
+00000a00: 6d65 6e74 6174 696f 6e0d 0a0d 0a54 6f20  mentation....To 
+00000a10: 6c65 6172 6e20 6d6f 7265 2061 626f 7574  learn more about
+00000a20: 2074 6865 2070 6163 6b61 6765 2063 6865   the package che
+00000a30: 636b 6f75 7420 6f75 7220 5b64 6f63 756d  ckout our [docum
+00000a40: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+00000a50: 2f2f 736b 6261 7365 2e72 6561 6474 6865  //skbase.readthe
+00000a60: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00000a70: 742f 292e 0d0a 0d0a 2323 203a 686f 7572  t/).....## :hour
+00000a80: 676c 6173 735f 666c 6f77 696e 675f 7361  glass_flowing_sa
+00000a90: 6e64 3a20 496e 7374 616c 6c20 736b 6261  nd: Install skba
+00000aa0: 7365 0d0a 466f 7220 7472 6f75 626c 6520  se..For trouble 
+00000ab0: 7368 6f6f 7469 6e67 206f 7220 6d6f 7265  shooting or more
+00000ac0: 2069 6e66 6f72 6d61 7469 6f6e 2c20 7365   information, se
+00000ad0: 6520 6f75 720d 0a5b 6465 7461 696c 6564  e our..[detailed
+00000ae0: 2069 6e73 7461 6c6c 6174 696f 6e20 696e   installation in
+00000af0: 7374 7275 6374 696f 6e73 5d28 6874 7470  structions](http
+00000b00: 733a 2f2f 736b 6261 7365 2e72 6561 6474  s://skbase.readt
+00000b10: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000b20: 6573 742f 7573 6572 5f64 6f63 756d 656e  est/user_documen
+00000b30: 7461 7469 6f6e 2f69 6e73 7461 6c6c 6174  tation/installat
+00000b40: 696f 6e2e 6874 6d6c 292e 0d0a 0d0a 2d20  ion.html).....- 
+00000b50: 2a2a 4f70 6572 6174 696e 6720 7379 7374  **Operating syst
+00000b60: 656d 2a2a 3a20 6d61 634f 5320 5820 c2b7  em**: macOS X ..
+00000b70: 204c 696e 7578 20c2 b720 5769 6e64 6f77   Linux .. Window
+00000b80: 7320 382e 3120 6f72 2068 6967 6865 720d  s 8.1 or higher.
+00000b90: 0a2d 202a 2a50 7974 686f 6e20 7665 7273  .- **Python vers
+00000ba0: 696f 6e2a 2a3a 2050 7974 686f 6e20 332e  ion**: Python 3.
+00000bb0: 372c 2033 2e38 2c20 332e 392c 2033 2e31  7, 3.8, 3.9, 3.1
+00000bc0: 3020 616e 6420 332e 3131 0d0a 2d20 2a2a  0 and 3.11..- **
+00000bd0: 5061 636b 6167 6520 6d61 6e61 6765 7273  Package managers
+00000be0: 2a2a 3a20 5b70 6970 5d0d 0a0d 0a5b 7069  **: [pip]....[pi
+00000bf0: 705d 3a20 6874 7470 733a 2f2f 7069 702e  p]: https://pip.
+00000c00: 7079 7061 2e69 6f2f 656e 2f73 7461 626c  pypa.io/en/stabl
+00000c10: 652f 0d0a 0d0a 2323 2320 7069 700d 0a73  e/....### pip..s
+00000c20: 6b62 6173 6520 7265 6c65 6173 6573 2061  kbase releases a
+00000c30: 7265 2061 7661 696c 6162 6c65 2061 7320  re available as 
+00000c40: 736f 7572 6365 2070 6163 6b61 6765 7320  source packages 
+00000c50: 616e 6420 6269 6e61 7279 2077 6865 656c  and binary wheel
+00000c60: 7320 7669 6120 5079 5049 0d0a 616e 6420  s via PyPI..and 
+00000c70: 6361 6e20 6265 2069 6e73 7461 6c6c 6564  can be installed
+00000c80: 2075 7369 6e67 2070 6970 2e20 4368 6563   using pip. Chec
+00000c90: 6b6f 7574 2074 6865 2066 756c 6c20 6c69  kout the full li
+00000ca0: 7374 206f 6620 7072 652d 636f 6d70 696c  st of pre-compil
+00000cb0: 6564 205b 7768 6565 6c73 206f 6e20 5079  ed [wheels on Py
+00000cc0: 5069 5d28 6874 7470 733a 2f2f 7079 7069  Pi](https://pypi
+00000cd0: 2e6f 7267 2f73 696d 706c 652f 736b 6261  .org/simple/skba
+00000ce0: 7365 2f29 2e0d 0a0d 0a54 6f20 696e 7374  se/).....To inst
+00000cf0: 616c 6c20 7468 6520 636f 7265 2070 6163  all the core pac
+00000d00: 6b61 6765 2075 7365 3a0d 0a0d 0a60 6060  kage use:....```
+00000d10: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
+00000d20: 6c20 7363 696b 6974 2d62 6173 650d 0a60  l scikit-base..`
+00000d30: 6060 0d0a 0d0a 6f72 2c20 6966 2079 6f75  ``....or, if you
+00000d40: 2077 616e 7420 746f 2069 6e73 7461 6c6c   want to install
+00000d50: 2077 6974 6820 7468 6520 6d61 7869 6d75   with the maximu
+00000d60: 6d20 7365 7420 6f66 2064 6570 656e 6465  m set of depende
+00000d70: 6e63 6965 732c 2075 7365 3a0d 0a0d 0a60  ncies, use:....`
+00000d80: 6060 6261 7368 0d0a 7069 7020 696e 7374  ``bash..pip inst
+00000d90: 616c 6c20 7363 696b 6974 2d62 6173 655b  all scikit-base[
+00000da0: 616c 6c5f 6578 7472 6173 5d0d 0a60 6060  all_extras]..```
+00000db0: 0d0a                                     ..
```

### Comparing `scikit-base-0.4.5/docs/source/conf.py` & `scikit-base-0.4.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/pyproject.toml` & `scikit-base-0.4.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 [project]
 name = "scikit-base"
-version = "0.4.5"
+version = "0.4.6"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
-    {name = "Franz Király"},
-    {name = "Markus Löning"},
-    {name = "Ryan Kuhns"},
+    {name = "sktime developers", email = "sktime.toolbox@gmail.com"},
 ]
 maintainers = [
-    {name = "Franz Kiraly", email = "f.kiraly@ucl.ac.uk"},
-    {name = "Ryan Kuhns", email = "rk.skbase@gmail.com"},
+    {name = "sktime developers", email = "sktime.toolbox@gmail.com"},
+    {name = "Franz Király"},
 ]
 readme = "README.md"
 keywords = [
     "data-science",
     "machine-learning",
     "scikit-learn",
 ]
```

### Comparing `scikit-base-0.4.5/scikit_base.egg-info/PKG-INFO` & `scikit-base-0.4.6/scikit_base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,414 +1,426 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2073 6369  : 2.1..Name: sci
 00000020: 6b69 742d 6261 7365 0d0a 5665 7273 696f  kit-base..Versio
-00000030: 6e3a 2030 2e34 2e35 0d0a 5375 6d6d 6172  n: 0.4.5..Summar
+00000030: 6e3a 2030 2e34 2e36 0d0a 5375 6d6d 6172  n: 0.4.6..Summar
 00000040: 793a 2042 6173 6520 636c 6173 7365 7320  y: Base classes 
 00000050: 666f 7220 736b 6c65 6172 6e2d 6c69 6b65  for sklearn-like
 00000060: 2070 6172 616d 6574 7269 6320 6f62 6a65   parametric obje
-00000070: 6374 730d 0a41 7574 686f 723a 2046 7261  cts..Author: Fra
-00000080: 6e7a 204b 6972 c3a1 6c79 2c20 4d61 726b  nz Kir..ly, Mark
-00000090: 7573 204c c3b6 6e69 6e67 2c20 5279 616e  us L..ning, Ryan
-000000a0: 204b 7568 6e73 0d0a 4d61 696e 7461 696e   Kuhns..Maintain
-000000b0: 6572 2d65 6d61 696c 3a20 4672 616e 7a20  er-email: Franz 
-000000c0: 4b69 7261 6c79 203c 662e 6b69 7261 6c79  Kiraly <f.kiraly
-000000d0: 4075 636c 2e61 632e 756b 3e2c 2052 7961  @ucl.ac.uk>, Rya
-000000e0: 6e20 4b75 686e 7320 3c72 6b2e 736b 6261  n Kuhns <rk.skba
-000000f0: 7365 4067 6d61 696c 2e63 6f6d 3e0d 0a4c  se@gmail.com>..L
-00000100: 6963 656e 7365 3a20 4253 4420 332d 436c  icense: BSD 3-Cl
-00000110: 6175 7365 204c 6963 656e 7365 0d0a 2020  ause License..  
-00000120: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000130: 436f 7079 7269 6768 7420 2863 2920 3230  Copyright (c) 20
-00000140: 3232 2c20 736b 6261 7365 2044 6576 656c  22, skbase Devel
-00000150: 6f70 6572 730d 0a20 2020 2020 2020 2041  opers..        A
-00000160: 6c6c 2072 6967 6874 7320 7265 7365 7276  ll rights reserv
-00000170: 6564 2e0d 0a20 2020 2020 2020 200d 0a20  ed...        .. 
-00000180: 2020 2020 2020 2052 6564 6973 7472 6962         Redistrib
-00000190: 7574 696f 6e20 616e 6420 7573 6520 696e  ution and use in
-000001a0: 2073 6f75 7263 6520 616e 6420 6269 6e61   source and bina
-000001b0: 7279 2066 6f72 6d73 2c20 7769 7468 206f  ry forms, with o
-000001c0: 7220 7769 7468 6f75 740d 0a20 2020 2020  r without..     
-000001d0: 2020 206d 6f64 6966 6963 6174 696f 6e2c     modification,
-000001e0: 2061 7265 2070 6572 6d69 7474 6564 2070   are permitted p
-000001f0: 726f 7669 6465 6420 7468 6174 2074 6865  rovided that the
-00000200: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6469   following condi
-00000210: 7469 6f6e 7320 6172 6520 6d65 743a 0d0a  tions are met:..
-00000220: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000230: 2020 312e 2052 6564 6973 7472 6962 7574    1. Redistribut
-00000240: 696f 6e73 206f 6620 736f 7572 6365 2063  ions of source c
-00000250: 6f64 6520 6d75 7374 2072 6574 6169 6e20  ode must retain 
-00000260: 7468 6520 6162 6f76 6520 636f 7079 7269  the above copyri
-00000270: 6768 7420 6e6f 7469 6365 2c20 7468 6973  ght notice, this
-00000280: 0d0a 2020 2020 2020 2020 2020 206c 6973  ..           lis
-00000290: 7420 6f66 2063 6f6e 6469 7469 6f6e 7320  t of conditions 
-000002a0: 616e 6420 7468 6520 666f 6c6c 6f77 696e  and the followin
-000002b0: 6720 6469 7363 6c61 696d 6572 2e0d 0a20  g disclaimer... 
-000002c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000002d0: 2032 2e20 5265 6469 7374 7269 6275 7469   2. Redistributi
-000002e0: 6f6e 7320 696e 2062 696e 6172 7920 666f  ons in binary fo
-000002f0: 726d 206d 7573 7420 7265 7072 6f64 7563  rm must reproduc
-00000300: 6520 7468 6520 6162 6f76 6520 636f 7079  e the above copy
-00000310: 7269 6768 7420 6e6f 7469 6365 2c0d 0a20  right notice,.. 
-00000320: 2020 2020 2020 2020 2020 7468 6973 206c            this l
-00000330: 6973 7420 6f66 2063 6f6e 6469 7469 6f6e  ist of condition
-00000340: 7320 616e 6420 7468 6520 666f 6c6c 6f77  s and the follow
-00000350: 696e 6720 6469 7363 6c61 696d 6572 2069  ing disclaimer i
-00000360: 6e20 7468 6520 646f 6375 6d65 6e74 6174  n the documentat
-00000370: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00000380: 616e 642f 6f72 206f 7468 6572 206d 6174  and/or other mat
-00000390: 6572 6961 6c73 2070 726f 7669 6465 6420  erials provided 
-000003a0: 7769 7468 2074 6865 2064 6973 7472 6962  with the distrib
-000003b0: 7574 696f 6e2e 0d0a 2020 2020 2020 2020  ution...        
-000003c0: 0d0a 2020 2020 2020 2020 332e 204e 6569  ..        3. Nei
-000003d0: 7468 6572 2074 6865 206e 616d 6520 6f66  ther the name of
-000003e0: 2074 6865 2063 6f70 7972 6967 6874 2068   the copyright h
-000003f0: 6f6c 6465 7220 6e6f 7220 7468 6520 6e61  older nor the na
-00000400: 6d65 7320 6f66 2069 7473 0d0a 2020 2020  mes of its..    
-00000410: 2020 2020 2020 2063 6f6e 7472 6962 7574         contribut
-00000420: 6f72 7320 6d61 7920 6265 2075 7365 6420  ors may be used 
-00000430: 746f 2065 6e64 6f72 7365 206f 7220 7072  to endorse or pr
-00000440: 6f6d 6f74 6520 7072 6f64 7563 7473 2064  omote products d
-00000450: 6572 6976 6564 2066 726f 6d0d 0a20 2020  erived from..   
-00000460: 2020 2020 2020 2020 7468 6973 2073 6f66          this sof
-00000470: 7477 6172 6520 7769 7468 6f75 7420 7370  tware without sp
-00000480: 6563 6966 6963 2070 7269 6f72 2077 7269  ecific prior wri
-00000490: 7474 656e 2070 6572 6d69 7373 696f 6e2e  tten permission.
-000004a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000004b0: 2020 2020 5448 4953 2053 4f46 5457 4152      THIS SOFTWAR
-000004c0: 4520 4953 2050 524f 5649 4445 4420 4259  E IS PROVIDED BY
-000004d0: 2054 4845 2043 4f50 5952 4947 4854 2048   THE COPYRIGHT H
-000004e0: 4f4c 4445 5253 2041 4e44 2043 4f4e 5452  OLDERS AND CONTR
-000004f0: 4942 5554 4f52 5320 2241 5320 4953 220d  IBUTORS "AS IS".
-00000500: 0a20 2020 2020 2020 2041 4e44 2041 4e59  .        AND ANY
-00000510: 2045 5850 5245 5353 204f 5220 494d 504c   EXPRESS OR IMPL
-00000520: 4945 4420 5741 5252 414e 5449 4553 2c20  IED WARRANTIES, 
-00000530: 494e 434c 5544 494e 472c 2042 5554 204e  INCLUDING, BUT N
-00000540: 4f54 204c 494d 4954 4544 2054 4f2c 2054  OT LIMITED TO, T
-00000550: 4845 0d0a 2020 2020 2020 2020 494d 504c  HE..        IMPL
-00000560: 4945 4420 5741 5252 414e 5449 4553 204f  IED WARRANTIES O
-00000570: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
-00000580: 5920 414e 4420 4649 544e 4553 5320 464f  Y AND FITNESS FO
-00000590: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
-000005a0: 5552 504f 5345 2041 5245 0d0a 2020 2020  URPOSE ARE..    
-000005b0: 2020 2020 4449 5343 4c41 494d 4544 2e20      DISCLAIMED. 
-000005c0: 494e 204e 4f20 4556 454e 5420 5348 414c  IN NO EVENT SHAL
-000005d0: 4c20 5448 4520 434f 5059 5249 4748 5420  L THE COPYRIGHT 
-000005e0: 484f 4c44 4552 204f 5220 434f 4e54 5249  HOLDER OR CONTRI
-000005f0: 4255 544f 5253 2042 4520 4c49 4142 4c45  BUTORS BE LIABLE
-00000600: 0d0a 2020 2020 2020 2020 464f 5220 414e  ..        FOR AN
-00000610: 5920 4449 5245 4354 2c20 494e 4449 5245  Y DIRECT, INDIRE
-00000620: 4354 2c20 494e 4349 4445 4e54 414c 2c20  CT, INCIDENTAL, 
-00000630: 5350 4543 4941 4c2c 2045 5845 4d50 4c41  SPECIAL, EXEMPLA
-00000640: 5259 2c20 4f52 2043 4f4e 5345 5155 454e  RY, OR CONSEQUEN
-00000650: 5449 414c 0d0a 2020 2020 2020 2020 4441  TIAL..        DA
-00000660: 4d41 4745 5320 2849 4e43 4c55 4449 4e47  MAGES (INCLUDING
-00000670: 2c20 4255 5420 4e4f 5420 4c49 4d49 5445  , BUT NOT LIMITE
-00000680: 4420 544f 2c20 5052 4f43 5552 454d 454e  D TO, PROCUREMEN
-00000690: 5420 4f46 2053 5542 5354 4954 5554 4520  T OF SUBSTITUTE 
-000006a0: 474f 4f44 5320 4f52 0d0a 2020 2020 2020  GOODS OR..      
-000006b0: 2020 5345 5256 4943 4553 3b20 4c4f 5353    SERVICES; LOSS
-000006c0: 204f 4620 5553 452c 2044 4154 412c 204f   OF USE, DATA, O
-000006d0: 5220 5052 4f46 4954 533b 204f 5220 4255  R PROFITS; OR BU
-000006e0: 5349 4e45 5353 2049 4e54 4552 5255 5054  SINESS INTERRUPT
-000006f0: 494f 4e29 2048 4f57 4556 4552 0d0a 2020  ION) HOWEVER..  
-00000700: 2020 2020 2020 4341 5553 4544 2041 4e44        CAUSED AND
-00000710: 204f 4e20 414e 5920 5448 454f 5259 204f   ON ANY THEORY O
-00000720: 4620 4c49 4142 494c 4954 592c 2057 4845  F LIABILITY, WHE
-00000730: 5448 4552 2049 4e20 434f 4e54 5241 4354  THER IN CONTRACT
-00000740: 2c20 5354 5249 4354 204c 4941 4249 4c49  , STRICT LIABILI
-00000750: 5459 2c0d 0a20 2020 2020 2020 204f 5220  TY,..        OR 
-00000760: 544f 5254 2028 494e 434c 5544 494e 4720  TORT (INCLUDING 
-00000770: 4e45 474c 4947 454e 4345 204f 5220 4f54  NEGLIGENCE OR OT
-00000780: 4845 5257 4953 4529 2041 5249 5349 4e47  HERWISE) ARISING
-00000790: 2049 4e20 414e 5920 5741 5920 4f55 5420   IN ANY WAY OUT 
-000007a0: 4f46 2054 4845 2055 5345 0d0a 2020 2020  OF THE USE..    
-000007b0: 2020 2020 4f46 2054 4849 5320 534f 4654      OF THIS SOFT
-000007c0: 5741 5245 2c20 4556 454e 2049 4620 4144  WARE, EVEN IF AD
-000007d0: 5649 5345 4420 4f46 2054 4845 2050 4f53  VISED OF THE POS
-000007e0: 5349 4249 4c49 5459 204f 4620 5355 4348  SIBILITY OF SUCH
-000007f0: 2044 414d 4147 452e 0d0a 2020 2020 2020   DAMAGE...      
-00000800: 2020 0d0a 5072 6f6a 6563 742d 5552 4c3a    ..Project-URL:
-00000810: 2068 6f6d 6570 6167 652c 2068 7474 7073   homepage, https
-00000820: 3a2f 2f67 6974 6875 622e 636f 6d2f 736b  ://github.com/sk
-00000830: 7469 6d65 2f73 6b62 6173 650d 0a50 726f  time/skbase..Pro
-00000840: 6a65 6374 2d55 524c 3a20 7265 706f 7369  ject-URL: reposi
-00000850: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
-00000860: 7468 7562 2e63 6f6d 2f73 6b74 696d 652f  thub.com/sktime/
-00000870: 736b 6261 7365 0d0a 5072 6f6a 6563 742d  skbase..Project-
-00000880: 5552 4c3a 2064 6f63 756d 656e 7461 7469  URL: documentati
-00000890: 6f6e 2c20 6874 7470 733a 2f2f 6769 7468  on, https://gith
-000008a0: 7562 2e63 6f6d 2f73 6b74 696d 652f 736b  ub.com/sktime/sk
-000008b0: 6261 7365 0d0a 5072 6f6a 6563 742d 5552  base..Project-UR
-000008c0: 4c3a 2064 6f77 6e6c 6f61 642c 2068 7474  L: download, htt
-000008d0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000008e0: 6f6a 6563 742f 736b 6261 7365 2f23 6669  oject/skbase/#fi
-000008f0: 6c65 730d 0a4b 6579 776f 7264 733a 2064  les..Keywords: d
-00000900: 6174 612d 7363 6965 6e63 652c 6d61 6368  ata-science,mach
-00000910: 696e 652d 6c65 6172 6e69 6e67 2c73 6369  ine-learning,sci
-00000920: 6b69 742d 6c65 6172 6e0d 0a43 6c61 7373  kit-learn..Class
-00000930: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-00000940: 4175 6469 656e 6365 203a 3a20 5363 6965  Audience :: Scie
-00000950: 6e63 652f 5265 7365 6172 6368 0d0a 436c  nce/Research..Cl
-00000960: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
-00000970: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-00000980: 6576 656c 6f70 6572 730d 0a43 6c61 7373  evelopers..Class
-00000990: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-000009a0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000009b0: 3a20 4253 4420 4c69 6365 6e73 650d 0a43  : BSD License..C
-000009c0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000009d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000009e0: 3a3a 2050 7974 686f 6e0d 0a43 6c61 7373  :: Python..Class
-000009f0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
-00000a00: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
-00000a10: 6d65 6e74 0d0a 436c 6173 7369 6669 6572  ment..Classifier
-00000a20: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
-00000a30: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-00000a40: 670d 0a43 6c61 7373 6966 6965 723a 204f  g..Classifier: O
-00000a50: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000a60: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
-00000a70: 5769 6e64 6f77 730d 0a43 6c61 7373 6966  Windows..Classif
-00000a80: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000a90: 7973 7465 6d20 3a3a 2050 4f53 4958 0d0a  ystem :: POSIX..
-00000aa0: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000ab0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000ac0: 556e 6978 0d0a 436c 6173 7369 6669 6572  Unix..Classifier
-00000ad0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-00000ae0: 656d 203a 3a20 4d61 634f 530d 0a43 6c61  em :: MacOS..Cla
-00000af0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000b00: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000b10: 2050 7974 686f 6e20 3a3a 2033 2e37 0d0a   Python :: 3.7..
-00000b20: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000b30: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000b40: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000b50: 380d 0a43 6c61 7373 6966 6965 723a 2050  8..Classifier: P
-00000b60: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000b70: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000b80: 2033 2e39 0d0a 436c 6173 7369 6669 6572   3.9..Classifier
-00000b90: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000ba0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000bb0: 203a 3a20 332e 3130 0d0a 436c 6173 7369   :: 3.10..Classi
-00000bc0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000bd0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000be0: 7468 6f6e 203a 3a20 332e 3131 0d0a 5265  thon :: 3.11..Re
-00000bf0: 7175 6972 6573 2d50 7974 686f 6e3a 203c  quires-Python: <
-00000c00: 332e 3132 2c3e 3d33 2e37 0d0a 4465 7363  3.12,>=3.7..Desc
-00000c10: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000c20: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000c30: 6f77 6e0d 0a50 726f 7669 6465 732d 4578  own..Provides-Ex
-00000c40: 7472 613a 2061 6c6c 5f65 7874 7261 730d  tra: all_extras.
-00000c50: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000c60: 2064 6576 0d0a 5072 6f76 6964 6573 2d45   dev..Provides-E
-00000c70: 7874 7261 3a20 6c69 6e74 6572 730d 0a50  xtra: linters..P
-00000c80: 726f 7669 6465 732d 4578 7472 613a 2062  rovides-Extra: b
-00000c90: 696e 6465 720d 0a50 726f 7669 6465 732d  inder..Provides-
-00000ca0: 4578 7472 613a 2064 6f63 730d 0a50 726f  Extra: docs..Pro
-00000cb0: 7669 6465 732d 4578 7472 613a 2074 6573  vides-Extra: tes
-00000cc0: 740d 0a4c 6963 656e 7365 2d46 696c 653a  t..License-File:
-00000cd0: 204c 4943 454e 5345 0d0a 0d0a 0d0a 2320   LICENSE......# 
-00000ce0: 5765 6c63 6f6d 6520 746f 2073 6b62 6173  Welcome to skbas
-00000cf0: 650d 0a0d 0a3e 2041 2062 6173 6520 636c  e....> A base cl
-00000d00: 6173 7320 666f 7220 7363 696b 6974 2d6c  ass for scikit-l
-00000d10: 6561 726e 2d6c 696b 6520 616e 6420 736b  earn-like and sk
-00000d20: 7469 6d65 2d6c 696b 6520 7061 7261 6d65  time-like parame
-00000d30: 7472 6963 206f 626a 6563 7473 0d0a 0d0a  tric objects....
-00000d40: 6073 6b62 6173 6560 2070 726f 7669 6465  `skbase` provide
-00000d50: 7320 6261 7365 2063 6c61 7373 6573 2066  s base classes f
-00000d60: 6f72 2063 7265 6174 696e 6720 7363 696b  or creating scik
-00000d70: 6974 2d6c 6561 726e 2d6c 696b 6520 7061  it-learn-like pa
-00000d80: 7261 6d65 7472 6963 206f 626a 6563 7473  rametric objects
-00000d90: 2c0d 0a61 6c6f 6e67 2077 6974 6820 746f  ,..along with to
-00000da0: 6f6c 7320 746f 206d 616b 6520 6974 2065  ols to make it e
-00000db0: 6173 6965 7220 746f 2062 7569 6c64 2079  asier to build y
-00000dc0: 6f75 7220 6f77 6e20 7061 636b 6167 6573  our own packages
-00000dd0: 2074 6861 7420 666f 6c6c 6f77 2074 6865   that follow the
-00000de0: 7365 0d0a 6465 7369 676e 2070 6174 7465  se..design patte
-00000df0: 726e 732e 0d0a 0d0a 3a72 6f63 6b65 743a  rns.....:rocket:
-00000e00: 2056 6572 7369 6f6e 2030 2e34 2e35 2069   Version 0.4.5 i
-00000e10: 7320 6e6f 7720 6176 6169 6c61 626c 652e  s now available.
-00000e20: 2043 6865 636b 6f75 7420 6f75 720d 0a5b   Checkout our..[
-00000e30: 7265 6c65 6173 6520 6e6f 7465 735d 2868  release notes](h
-00000e40: 7474 7073 3a2f 2f73 6b62 6173 652e 7265  ttps://skbase.re
-00000e50: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000e60: 6c61 7465 7374 2f63 6861 6e67 656c 6f67  latest/changelog
-00000e70: 2e68 746d 6c29 2e0d 0a0d 0a7c 204f 7665  .html).....| Ove
-00000e80: 7276 6965 7720 7c20 7c0d 0a7c 2d2d 2d7c  rview | |..|---|
-00000e90: 2d2d 2d7c 0d0a 7c20 2a2a 4349 2f43 442a  ---|..| **CI/CD*
-00000ea0: 2a20 7c20 5b21 5b54 6573 7473 5d28 6874  * | [![Tests](ht
-00000eb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ec0: 2f73 6b74 696d 652f 736b 6261 7365 2f61  /sktime/skbase/a
-00000ed0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-00000ee0: 2f74 6573 742e 796d 6c2f 6261 6467 652e  /test.yml/badge.
-00000ef0: 7376 673f 6272 616e 6368 3d6d 6169 6e29  svg?branch=main)
-00000f00: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000f10: 2e63 6f6d 2f73 6b74 696d 652f 736b 6261  .com/sktime/skba
-00000f20: 7365 2f61 6374 696f 6e73 2f77 6f72 6b66  se/actions/workf
-00000f30: 6c6f 7773 2f74 6573 742e 796d 6c29 205b  lows/test.yml) [
-00000f40: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
-00000f50: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000f60: 2f73 6b74 696d 652f 736b 6261 7365 2f62  /sktime/skbase/b
-00000f70: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
-00000f80: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
-00000f90: 3d32 4a34 3234 4e4c 4f38 3229 5d28 6874  =2J424NLO82)](ht
-00000fa0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000fb0: 2f67 682f 736b 7469 6d65 2f73 6b62 6173  /gh/sktime/skbas
-00000fc0: 6529 205b 215b 446f 6375 6d65 6e74 6174  e) [![Documentat
-00000fd0: 696f 6e20 5374 6174 7573 5d28 6874 7470  ion Status](http
-00000fe0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
-00000ff0: 6f72 672f 7072 6f6a 6563 7473 2f73 6b62  org/projects/skb
-00001000: 6173 652f 6261 6467 652f 3f76 6572 7369  ase/badge/?versi
-00001010: 6f6e 3d6c 6174 6573 7429 5d28 6874 7470  on=latest)](http
-00001020: 733a 2f2f 736b 6261 7365 2e72 6561 6474  s://skbase.readt
-00001030: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00001040: 6573 742f 3f62 6164 6765 3d6c 6174 6573  est/?badge=lates
-00001050: 7429 205b 215b 7072 652d 636f 6d6d 6974  t) [![pre-commit
-00001060: 2e63 6920 7374 6174 7573 5d28 6874 7470  .ci status](http
-00001070: 733a 2f2f 7265 7375 6c74 732e 7072 652d  s://results.pre-
-00001080: 636f 6d6d 6974 2e63 692f 6261 6467 652f  commit.ci/badge/
-00001090: 6769 7468 7562 2f73 6b74 696d 652f 736b  github/sktime/sk
-000010a0: 6261 7365 2f6d 6169 6e2e 7376 6729 5d28  base/main.svg)](
-000010b0: 6874 7470 733a 2f2f 7265 7375 6c74 732e  https://results.
-000010c0: 7072 652d 636f 6d6d 6974 2e63 692f 6c61  pre-commit.ci/la
-000010d0: 7465 7374 2f67 6974 6875 622f 736b 7469  test/github/skti
-000010e0: 6d65 2f73 6b62 6173 652f 6d61 696e 2920  me/skbase/main) 
-000010f0: 7c0d 0a7c 202a 2a43 6f64 652a 2a20 7c20  |..| **Code** | 
-00001100: 205b 215b 2170 7970 695d 2868 7474 7073   [![!pypi](https
-00001110: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001120: 6f2f 7079 7069 2f76 2f73 6369 6b69 742d  o/pypi/v/scikit-
-00001130: 6261 7365 3f63 6f6c 6f72 3d6f 7261 6e67  base?color=orang
-00001140: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
-00001150: 2e6f 7267 2f70 726f 6a65 6374 2f73 6b62  .org/project/skb
-00001160: 6173 652f 2920 205b 215b 2170 7974 686f  ase/)  [![!pytho
-00001170: 6e2d 7665 7273 696f 6e73 5d28 6874 7470  n-versions](http
-00001180: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00001190: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
-000011a0: 6e73 2f73 6369 6b69 742d 6261 7365 295d  ns/scikit-base)]
-000011b0: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
-000011c0: 686f 6e2e 6f72 672f 2920 5b21 5b21 626c  hon.org/) [![!bl
-000011d0: 6163 6b5d 2868 7474 7073 3a2f 2f69 6d67  ack](https://img
-000011e0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000011f0: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
-00001200: 6c61 636b 2d30 3030 3030 302e 7376 6729  lack-000000.svg)
-00001210: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001220: 2e63 6f6d 2f70 7366 2f62 6c61 636b 2920  .com/psf/black) 
-00001230: 5b21 5b73 6563 7572 6974 793a 2062 616e  [![security: ban
-00001240: 6469 745d 2868 7474 7073 3a2f 2f69 6d67  dit](https://img
-00001250: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00001260: 652f 7365 6375 7269 7479 2d62 616e 6469  e/security-bandi
-00001270: 742d 7965 6c6c 6f77 2e73 7667 295d 2868  t-yellow.svg)](h
-00001280: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001290: 6d2f 5079 4351 412f 6261 6e64 6974 2920  m/PyCQA/bandit) 
-000012a0: 7c0d 0a7c 202a 2a44 6f77 6e6c 6f61 6473  |..| **Downloads
-000012b0: 2a2a 7c20 5b21 5b44 6f77 6e6c 6f61 6473  **| [![Downloads
-000012c0: 5d28 6874 7470 733a 2f2f 7374 6174 6963  ](https://static
-000012d0: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
-000012e0: 6e61 6c69 7a65 642d 6261 6467 652f 7363  nalized-badge/sc
-000012f0: 696b 6974 2d62 6173 653f 7065 7269 6f64  ikit-base?period
-00001300: 3d77 6565 6b26 756e 6974 733d 696e 7465  =week&units=inte
-00001310: 726e 6174 696f 6e61 6c5f 7379 7374 656d  rnational_system
-00001320: 266c 6566 745f 636f 6c6f 723d 6772 6579  &left_color=grey
-00001330: 2672 6967 6874 5f63 6f6c 6f72 3d62 6c75  &right_color=blu
-00001340: 6526 6c65 6674 5f74 6578 743d 7765 656b  e&left_text=week
-00001350: 6c79 2532 3028 7079 7069 2929 5d28 6874  ly%20(pypi))](ht
-00001360: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
-00001370: 7072 6f6a 6563 742f 7363 696b 6974 2d62  project/scikit-b
-00001380: 6173 6529 205b 215b 446f 776e 6c6f 6164  ase) [![Download
-00001390: 735d 2868 7474 7073 3a2f 2f73 7461 7469  s](https://stati
-000013a0: 632e 7065 7079 2e74 6563 682f 7065 7273  c.pepy.tech/pers
-000013b0: 6f6e 616c 697a 6564 2d62 6164 6765 2f73  onalized-badge/s
-000013c0: 6369 6b69 742d 6261 7365 3f70 6572 696f  cikit-base?perio
-000013d0: 643d 6d6f 6e74 6826 756e 6974 733d 696e  d=month&units=in
-000013e0: 7465 726e 6174 696f 6e61 6c5f 7379 7374  ternational_syst
-000013f0: 656d 266c 6566 745f 636f 6c6f 723d 6772  em&left_color=gr
-00001400: 6579 2672 6967 6874 5f63 6f6c 6f72 3d62  ey&right_color=b
-00001410: 6c75 6526 6c65 6674 5f74 6578 743d 6d6f  lue&left_text=mo
-00001420: 6e74 686c 7925 3230 2870 7970 6929 295d  nthly%20(pypi))]
-00001430: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-00001440: 6368 2f70 726f 6a65 6374 2f73 6369 6b69  ch/project/sciki
-00001450: 742d 6261 7365 2920 5b21 5b44 6f77 6e6c  t-base) [![Downl
-00001460: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
-00001470: 6174 6963 2e70 6570 792e 7465 6368 2f70  atic.pepy.tech/p
-00001480: 6572 736f 6e61 6c69 7a65 642d 6261 6467  ersonalized-badg
-00001490: 652f 7363 696b 6974 2d62 6173 653f 7065  e/scikit-base?pe
-000014a0: 7269 6f64 3d74 6f74 616c 2675 6e69 7473  riod=total&units
-000014b0: 3d69 6e74 6572 6e61 7469 6f6e 616c 5f73  =international_s
-000014c0: 7973 7465 6d26 6c65 6674 5f63 6f6c 6f72  ystem&left_color
-000014d0: 3d67 7265 7926 7269 6768 745f 636f 6c6f  =grey&right_colo
-000014e0: 723d 626c 7565 266c 6566 745f 7465 7874  r=blue&left_text
-000014f0: 3d63 756d 756c 6174 6976 6525 3230 2870  =cumulative%20(p
-00001500: 7970 6929 295d 2868 7474 7073 3a2f 2f70  ypi))](https://p
-00001510: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
-00001520: 2f73 6369 6b69 742d 6261 7365 2920 7c0d  /scikit-base) |.
-00001530: 0a0d 0a3c 212d 2d20 414c 4c2d 434f 4e54  ...<!-- ALL-CONT
-00001540: 5249 4255 544f 5253 2d42 4144 4745 3a53  RIBUTORS-BADGE:S
-00001550: 5441 5254 202d 2044 6f20 6e6f 7420 7265  TART - Do not re
-00001560: 6d6f 7665 206f 7220 6d6f 6469 6679 2074  move or modify t
-00001570: 6869 7320 7365 6374 696f 6e20 2d2d 3e0d  his section -->.
-00001580: 0a5b 215b 416c 6c20 436f 6e74 7269 6275  .[![All Contribu
-00001590: 746f 7273 5d28 6874 7470 733a 2f2f 696d  tors](https://im
-000015a0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000015b0: 6765 2f61 6c6c 5f63 6f6e 7472 6962 7574  ge/all_contribut
-000015c0: 6f72 732d 3133 2d6f 7261 6e67 652e 7376  ors-13-orange.sv
-000015d0: 673f 7374 796c 653d 666c 6174 2d73 7175  g?style=flat-squ
-000015e0: 6172 6529 5d28 2363 6f6e 7472 6962 7574  are)](#contribut
-000015f0: 6f72 7329 0d0a 3c21 2d2d 2041 4c4c 2d43  ors)..<!-- ALL-C
-00001600: 4f4e 5452 4942 5554 4f52 532d 4241 4447  ONTRIBUTORS-BADG
-00001610: 453a 454e 4420 2d2d 3e0d 0a0d 0a23 2320  E:END -->....## 
-00001620: 446f 6375 6d65 6e74 6174 696f 6e0d 0a0d  Documentation...
-00001630: 0a54 6f20 6c65 6172 6e20 6d6f 7265 2061  .To learn more a
-00001640: 626f 7574 2074 6865 2070 6163 6b61 6765  bout the package
-00001650: 2063 6865 636b 6f75 7420 6f75 7220 5b64   checkout our [d
-00001660: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00001670: 7470 733a 2f2f 736b 6261 7365 2e72 6561  tps://skbase.rea
-00001680: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00001690: 6174 6573 742f 292e 0d0a 0d0a 2323 203a  atest/).....## :
-000016a0: 686f 7572 676c 6173 735f 666c 6f77 696e  hourglass_flowin
-000016b0: 675f 7361 6e64 3a20 496e 7374 616c 6c20  g_sand: Install 
-000016c0: 736b 6261 7365 0d0a 466f 7220 7472 6f75  skbase..For trou
-000016d0: 626c 6520 7368 6f6f 7469 6e67 206f 7220  ble shooting or 
-000016e0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-000016f0: 2c20 7365 6520 6f75 720d 0a5b 6465 7461  , see our..[deta
-00001700: 696c 6564 2069 6e73 7461 6c6c 6174 696f  iled installatio
-00001710: 6e20 696e 7374 7275 6374 696f 6e73 5d28  n instructions](
-00001720: 6874 7470 733a 2f2f 736b 6261 7365 2e72  https://skbase.r
-00001730: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00001740: 2f6c 6174 6573 742f 7573 6572 5f64 6f63  /latest/user_doc
-00001750: 756d 656e 7461 7469 6f6e 2f69 6e73 7461  umentation/insta
-00001760: 6c6c 6174 696f 6e2e 6874 6d6c 292e 0d0a  llation.html)...
-00001770: 0d0a 2d20 2a2a 4f70 6572 6174 696e 6720  ..- **Operating 
-00001780: 7379 7374 656d 2a2a 3a20 6d61 634f 5320  system**: macOS 
-00001790: 5820 c2b7 204c 696e 7578 20c2 b720 5769  X .. Linux .. Wi
-000017a0: 6e64 6f77 7320 382e 3120 6f72 2068 6967  ndows 8.1 or hig
-000017b0: 6865 720d 0a2d 202a 2a50 7974 686f 6e20  her..- **Python 
-000017c0: 7665 7273 696f 6e2a 2a3a 2050 7974 686f  version**: Pytho
-000017d0: 6e20 332e 372c 2033 2e38 2c20 332e 392c  n 3.7, 3.8, 3.9,
-000017e0: 2033 2e31 3020 616e 6420 332e 3131 0d0a   3.10 and 3.11..
-000017f0: 2d20 2a2a 5061 636b 6167 6520 6d61 6e61  - **Package mana
-00001800: 6765 7273 2a2a 3a20 5b70 6970 5d0d 0a0d  gers**: [pip]...
-00001810: 0a5b 7069 705d 3a20 6874 7470 733a 2f2f  .[pip]: https://
-00001820: 7069 702e 7079 7061 2e69 6f2f 656e 2f73  pip.pypa.io/en/s
-00001830: 7461 626c 652f 0d0a 0d0a 2323 2320 7069  table/....### pi
-00001840: 700d 0a73 6b62 6173 6520 7265 6c65 6173  p..skbase releas
-00001850: 6573 2061 7265 2061 7661 696c 6162 6c65  es are available
-00001860: 2061 7320 736f 7572 6365 2070 6163 6b61   as source packa
-00001870: 6765 7320 616e 6420 6269 6e61 7279 2077  ges and binary w
-00001880: 6865 656c 7320 7669 6120 5079 5049 0d0a  heels via PyPI..
-00001890: 616e 6420 6361 6e20 6265 2069 6e73 7461  and can be insta
-000018a0: 6c6c 6564 2075 7369 6e67 2070 6970 2e20  lled using pip. 
-000018b0: 4368 6563 6b6f 7574 2074 6865 2066 756c  Checkout the ful
-000018c0: 6c20 6c69 7374 206f 6620 7072 652d 636f  l list of pre-co
-000018d0: 6d70 696c 6564 205b 7768 6565 6c73 206f  mpiled [wheels o
-000018e0: 6e20 5079 5069 5d28 6874 7470 733a 2f2f  n PyPi](https://
-000018f0: 7079 7069 2e6f 7267 2f73 696d 706c 652f  pypi.org/simple/
-00001900: 736b 6261 7365 2f29 2e0d 0a0d 0a54 6f20  skbase/).....To 
-00001910: 696e 7374 616c 6c20 7468 6520 636f 7265  install the core
-00001920: 2070 6163 6b61 6765 2075 7365 3a0d 0a0d   package use:...
-00001930: 0a60 6060 6261 7368 0d0a 7069 7020 696e  .```bash..pip in
-00001940: 7374 616c 6c20 7363 696b 6974 2d62 6173  stall scikit-bas
-00001950: 650d 0a60 6060 0d0a 0d0a 6f72 2c20 6966  e..```....or, if
-00001960: 2079 6f75 2077 616e 7420 746f 2069 6e73   you want to ins
-00001970: 7461 6c6c 2077 6974 6820 7468 6520 6d61  tall with the ma
-00001980: 7869 6d75 6d20 7365 7420 6f66 2064 6570  ximum set of dep
-00001990: 656e 6465 6e63 6965 732c 2075 7365 3a0d  endencies, use:.
-000019a0: 0a0d 0a60 6060 6261 7368 0d0a 7069 7020  ...```bash..pip 
-000019b0: 696e 7374 616c 6c20 7363 696b 6974 2d62  install scikit-b
-000019c0: 6173 655b 616c 6c5f 6578 7472 6173 5d0d  ase[all_extras].
-000019d0: 0a60 6060 0d0a                           .```..
+00000070: 6374 730d 0a41 7574 686f 722d 656d 6169  cts..Author-emai
+00000080: 6c3a 2073 6b74 696d 6520 6465 7665 6c6f  l: sktime develo
+00000090: 7065 7273 203c 736b 7469 6d65 2e74 6f6f  pers <sktime.too
+000000a0: 6c62 6f78 4067 6d61 696c 2e63 6f6d 3e0d  lbox@gmail.com>.
+000000b0: 0a4d 6169 6e74 6169 6e65 723a 2046 7261  .Maintainer: Fra
+000000c0: 6e7a 204b 6972 c3a1 6c79 0d0a 4d61 696e  nz Kir..ly..Main
+000000d0: 7461 696e 6572 2d65 6d61 696c 3a20 736b  tainer-email: sk
+000000e0: 7469 6d65 2064 6576 656c 6f70 6572 7320  time developers 
+000000f0: 3c73 6b74 696d 652e 746f 6f6c 626f 7840  <sktime.toolbox@
+00000100: 676d 6169 6c2e 636f 6d3e 0d0a 4c69 6365  gmail.com>..Lice
+00000110: 6e73 653a 2042 5344 2033 2d43 6c61 7573  nse: BSD 3-Claus
+00000120: 6520 4c69 6365 6e73 650d 0a20 2020 2020  e License..     
+00000130: 2020 200d 0a20 2020 2020 2020 2043 6f70     ..        Cop
+00000140: 7972 6967 6874 2028 6329 2032 3032 322c  yright (c) 2022,
+00000150: 2073 6b62 6173 6520 4465 7665 6c6f 7065   skbase Develope
+00000160: 7273 0d0a 2020 2020 2020 2020 416c 6c20  rs..        All 
+00000170: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
+00000180: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00000190: 2020 2020 5265 6469 7374 7269 6275 7469      Redistributi
+000001a0: 6f6e 2061 6e64 2075 7365 2069 6e20 736f  on and use in so
+000001b0: 7572 6365 2061 6e64 2062 696e 6172 7920  urce and binary 
+000001c0: 666f 726d 732c 2077 6974 6820 6f72 2077  forms, with or w
+000001d0: 6974 686f 7574 0d0a 2020 2020 2020 2020  ithout..        
+000001e0: 6d6f 6469 6669 6361 7469 6f6e 2c20 6172  modification, ar
+000001f0: 6520 7065 726d 6974 7465 6420 7072 6f76  e permitted prov
+00000200: 6964 6564 2074 6861 7420 7468 6520 666f  ided that the fo
+00000210: 6c6c 6f77 696e 6720 636f 6e64 6974 696f  llowing conditio
+00000220: 6e73 2061 7265 206d 6574 3a0d 0a20 2020  ns are met:..   
+00000230: 2020 2020 200d 0a20 2020 2020 2020 2031       ..        1
+00000240: 2e20 5265 6469 7374 7269 6275 7469 6f6e  . Redistribution
+00000250: 7320 6f66 2073 6f75 7263 6520 636f 6465  s of source code
+00000260: 206d 7573 7420 7265 7461 696e 2074 6865   must retain the
+00000270: 2061 626f 7665 2063 6f70 7972 6967 6874   above copyright
+00000280: 206e 6f74 6963 652c 2074 6869 730d 0a20   notice, this.. 
+00000290: 2020 2020 2020 2020 2020 6c69 7374 206f            list o
+000002a0: 6620 636f 6e64 6974 696f 6e73 2061 6e64  f conditions and
+000002b0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
+000002c0: 6973 636c 6169 6d65 722e 0d0a 2020 2020  isclaimer...    
+000002d0: 2020 2020 0d0a 2020 2020 2020 2020 322e      ..        2.
+000002e0: 2052 6564 6973 7472 6962 7574 696f 6e73   Redistributions
+000002f0: 2069 6e20 6269 6e61 7279 2066 6f72 6d20   in binary form 
+00000300: 6d75 7374 2072 6570 726f 6475 6365 2074  must reproduce t
+00000310: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
+00000320: 6874 206e 6f74 6963 652c 0d0a 2020 2020  ht notice,..    
+00000330: 2020 2020 2020 2074 6869 7320 6c69 7374         this list
+00000340: 206f 6620 636f 6e64 6974 696f 6e73 2061   of conditions a
+00000350: 6e64 2074 6865 2066 6f6c 6c6f 7769 6e67  nd the following
+00000360: 2064 6973 636c 6169 6d65 7220 696e 2074   disclaimer in t
+00000370: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00000380: 0d0a 2020 2020 2020 2020 2020 2061 6e64  ..           and
+00000390: 2f6f 7220 6f74 6865 7220 6d61 7465 7269  /or other materi
+000003a0: 616c 7320 7072 6f76 6964 6564 2077 6974  als provided wit
+000003b0: 6820 7468 6520 6469 7374 7269 6275 7469  h the distributi
+000003c0: 6f6e 2e0d 0a20 2020 2020 2020 200d 0a20  on...        .. 
+000003d0: 2020 2020 2020 2033 2e20 4e65 6974 6865         3. Neithe
+000003e0: 7220 7468 6520 6e61 6d65 206f 6620 7468  r the name of th
+000003f0: 6520 636f 7079 7269 6768 7420 686f 6c64  e copyright hold
+00000400: 6572 206e 6f72 2074 6865 206e 616d 6573  er nor the names
+00000410: 206f 6620 6974 730d 0a20 2020 2020 2020   of its..       
+00000420: 2020 2020 636f 6e74 7269 6275 746f 7273      contributors
+00000430: 206d 6179 2062 6520 7573 6564 2074 6f20   may be used to 
+00000440: 656e 646f 7273 6520 6f72 2070 726f 6d6f  endorse or promo
+00000450: 7465 2070 726f 6475 6374 7320 6465 7269  te products deri
+00000460: 7665 6420 6672 6f6d 0d0a 2020 2020 2020  ved from..      
+00000470: 2020 2020 2074 6869 7320 736f 6674 7761       this softwa
+00000480: 7265 2077 6974 686f 7574 2073 7065 6369  re without speci
+00000490: 6669 6320 7072 696f 7220 7772 6974 7465  fic prior writte
+000004a0: 6e20 7065 726d 6973 7369 6f6e 2e0d 0a20  n permission... 
+000004b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000004c0: 2054 4849 5320 534f 4654 5741 5245 2049   THIS SOFTWARE I
+000004d0: 5320 5052 4f56 4944 4544 2042 5920 5448  S PROVIDED BY TH
+000004e0: 4520 434f 5059 5249 4748 5420 484f 4c44  E COPYRIGHT HOLD
+000004f0: 4552 5320 414e 4420 434f 4e54 5249 4255  ERS AND CONTRIBU
+00000500: 544f 5253 2022 4153 2049 5322 0d0a 2020  TORS "AS IS"..  
+00000510: 2020 2020 2020 414e 4420 414e 5920 4558        AND ANY EX
+00000520: 5052 4553 5320 4f52 2049 4d50 4c49 4544  PRESS OR IMPLIED
+00000530: 2057 4152 5241 4e54 4945 532c 2049 4e43   WARRANTIES, INC
+00000540: 4c55 4449 4e47 2c20 4255 5420 4e4f 5420  LUDING, BUT NOT 
+00000550: 4c49 4d49 5445 4420 544f 2c20 5448 450d  LIMITED TO, THE.
+00000560: 0a20 2020 2020 2020 2049 4d50 4c49 4544  .        IMPLIED
+00000570: 2057 4152 5241 4e54 4945 5320 4f46 204d   WARRANTIES OF M
+00000580: 4552 4348 414e 5441 4249 4c49 5459 2041  ERCHANTABILITY A
+00000590: 4e44 2046 4954 4e45 5353 2046 4f52 2041  ND FITNESS FOR A
+000005a0: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
+000005b0: 4f53 4520 4152 450d 0a20 2020 2020 2020  OSE ARE..       
+000005c0: 2044 4953 434c 4149 4d45 442e 2049 4e20   DISCLAIMED. IN 
+000005d0: 4e4f 2045 5645 4e54 2053 4841 4c4c 2054  NO EVENT SHALL T
+000005e0: 4845 2043 4f50 5952 4947 4854 2048 4f4c  HE COPYRIGHT HOL
+000005f0: 4445 5220 4f52 2043 4f4e 5452 4942 5554  DER OR CONTRIBUT
+00000600: 4f52 5320 4245 204c 4941 424c 450d 0a20  ORS BE LIABLE.. 
+00000610: 2020 2020 2020 2046 4f52 2041 4e59 2044         FOR ANY D
+00000620: 4952 4543 542c 2049 4e44 4952 4543 542c  IRECT, INDIRECT,
+00000630: 2049 4e43 4944 454e 5441 4c2c 2053 5045   INCIDENTAL, SPE
+00000640: 4349 414c 2c20 4558 454d 504c 4152 592c  CIAL, EXEMPLARY,
+00000650: 204f 5220 434f 4e53 4551 5545 4e54 4941   OR CONSEQUENTIA
+00000660: 4c0d 0a20 2020 2020 2020 2044 414d 4147  L..        DAMAG
+00000670: 4553 2028 494e 434c 5544 494e 472c 2042  ES (INCLUDING, B
+00000680: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
+00000690: 4f2c 2050 524f 4355 5245 4d45 4e54 204f  O, PROCUREMENT O
+000006a0: 4620 5355 4253 5449 5455 5445 2047 4f4f  F SUBSTITUTE GOO
+000006b0: 4453 204f 520d 0a20 2020 2020 2020 2053  DS OR..        S
+000006c0: 4552 5649 4345 533b 204c 4f53 5320 4f46  ERVICES; LOSS OF
+000006d0: 2055 5345 2c20 4441 5441 2c20 4f52 2050   USE, DATA, OR P
+000006e0: 524f 4649 5453 3b20 4f52 2042 5553 494e  ROFITS; OR BUSIN
+000006f0: 4553 5320 494e 5445 5252 5550 5449 4f4e  ESS INTERRUPTION
+00000700: 2920 484f 5745 5645 520d 0a20 2020 2020  ) HOWEVER..     
+00000710: 2020 2043 4155 5345 4420 414e 4420 4f4e     CAUSED AND ON
+00000720: 2041 4e59 2054 4845 4f52 5920 4f46 204c   ANY THEORY OF L
+00000730: 4941 4249 4c49 5459 2c20 5748 4554 4845  IABILITY, WHETHE
+00000740: 5220 494e 2043 4f4e 5452 4143 542c 2053  R IN CONTRACT, S
+00000750: 5452 4943 5420 4c49 4142 494c 4954 592c  TRICT LIABILITY,
+00000760: 0d0a 2020 2020 2020 2020 4f52 2054 4f52  ..        OR TOR
+00000770: 5420 2849 4e43 4c55 4449 4e47 204e 4547  T (INCLUDING NEG
+00000780: 4c49 4745 4e43 4520 4f52 204f 5448 4552  LIGENCE OR OTHER
+00000790: 5749 5345 2920 4152 4953 494e 4720 494e  WISE) ARISING IN
+000007a0: 2041 4e59 2057 4159 204f 5554 204f 4620   ANY WAY OUT OF 
+000007b0: 5448 4520 5553 450d 0a20 2020 2020 2020  THE USE..       
+000007c0: 204f 4620 5448 4953 2053 4f46 5457 4152   OF THIS SOFTWAR
+000007d0: 452c 2045 5645 4e20 4946 2041 4456 4953  E, EVEN IF ADVIS
+000007e0: 4544 204f 4620 5448 4520 504f 5353 4942  ED OF THE POSSIB
+000007f0: 494c 4954 5920 4f46 2053 5543 4820 4441  ILITY OF SUCH DA
+00000800: 4d41 4745 2e0d 0a20 2020 2020 2020 200d  MAGE...        .
+00000810: 0a50 726f 6a65 6374 2d55 524c 3a20 686f  .Project-URL: ho
+00000820: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
+00000830: 6769 7468 7562 2e63 6f6d 2f73 6b74 696d  github.com/sktim
+00000840: 652f 736b 6261 7365 0d0a 5072 6f6a 6563  e/skbase..Projec
+00000850: 742d 5552 4c3a 2072 6570 6f73 6974 6f72  t-URL: repositor
+00000860: 792c 2068 7474 7073 3a2f 2f67 6974 6875  y, https://githu
+00000870: 622e 636f 6d2f 736b 7469 6d65 2f73 6b62  b.com/sktime/skb
+00000880: 6173 650d 0a50 726f 6a65 6374 2d55 524c  ase..Project-URL
+00000890: 3a20 646f 6375 6d65 6e74 6174 696f 6e2c  : documentation,
+000008a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000008b0: 636f 6d2f 736b 7469 6d65 2f73 6b62 6173  com/sktime/skbas
+000008c0: 650d 0a50 726f 6a65 6374 2d55 524c 3a20  e..Project-URL: 
+000008d0: 646f 776e 6c6f 6164 2c20 6874 7470 733a  download, https:
+000008e0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+000008f0: 6374 2f73 6b62 6173 652f 2366 696c 6573  ct/skbase/#files
+00000900: 0d0a 4b65 7977 6f72 6473 3a20 6461 7461  ..Keywords: data
+00000910: 2d73 6369 656e 6365 2c6d 6163 6869 6e65  -science,machine
+00000920: 2d6c 6561 726e 696e 672c 7363 696b 6974  -learning,scikit
+00000930: 2d6c 6561 726e 0d0a 436c 6173 7369 6669  -learn..Classifi
+00000940: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+00000950: 6965 6e63 6520 3a3a 2053 6369 656e 6365  ience :: Science
+00000960: 2f52 6573 6561 7263 680d 0a43 6c61 7373  /Research..Class
+00000970: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
+00000980: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000990: 6c6f 7065 7273 0d0a 436c 6173 7369 6669  lopers..Classifi
+000009a0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+000009b0: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
+000009c0: 5344 204c 6963 656e 7365 0d0a 436c 6173  SD License..Clas
+000009d0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000009e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000009f0: 5079 7468 6f6e 0d0a 436c 6173 7369 6669  Python..Classifi
+00000a00: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
+00000a10: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
+00000a20: 740d 0a43 6c61 7373 6966 6965 723a 2054  t..Classifier: T
+00000a30: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+00000a40: 6963 2f45 6e67 696e 6565 7269 6e67 0d0a  ic/Engineering..
+00000a50: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+00000a60: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000a70: 4d69 6372 6f73 6f66 7420 3a3a 2057 696e  Microsoft :: Win
+00000a80: 646f 7773 0d0a 436c 6173 7369 6669 6572  dows..Classifier
+00000a90: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000aa0: 656d 203a 3a20 504f 5349 580d 0a43 6c61  em :: POSIX..Cla
+00000ab0: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
+00000ac0: 6e67 2053 7973 7465 6d20 3a3a 2055 6e69  ng System :: Uni
+00000ad0: 780d 0a43 6c61 7373 6966 6965 723a 204f  x..Classifier: O
+00000ae0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000af0: 3a3a 204d 6163 4f53 0d0a 436c 6173 7369  :: MacOS..Classi
+00000b00: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000b10: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000b20: 7468 6f6e 203a 3a20 332e 370d 0a43 6c61  thon :: 3.7..Cla
+00000b30: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000b40: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000b50: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
+00000b60: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000b70: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000b80: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000b90: 390d 0a43 6c61 7373 6966 6965 723a 2050  9..Classifier: P
+00000ba0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000bb0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000bc0: 2033 2e31 300d 0a43 6c61 7373 6966 6965   3.10..Classifie
+00000bd0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000be0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000bf0: 6e20 3a3a 2033 2e31 310d 0a52 6571 7569  n :: 3.11..Requi
+00000c00: 7265 732d 5079 7468 6f6e 3a20 3c33 2e31  res-Python: <3.1
+00000c10: 322c 3e3d 332e 370d 0a44 6573 6372 6970  2,>=3.7..Descrip
+00000c20: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000c30: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000c40: 0d0a 5072 6f76 6964 6573 2d45 7874 7261  ..Provides-Extra
+00000c50: 3a20 616c 6c5f 6578 7472 6173 0d0a 5072  : all_extras..Pr
+00000c60: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
+00000c70: 760d 0a50 726f 7669 6465 732d 4578 7472  v..Provides-Extr
+00000c80: 613a 206c 696e 7465 7273 0d0a 5072 6f76  a: linters..Prov
+00000c90: 6964 6573 2d45 7874 7261 3a20 6269 6e64  ides-Extra: bind
+00000ca0: 6572 0d0a 5072 6f76 6964 6573 2d45 7874  er..Provides-Ext
+00000cb0: 7261 3a20 646f 6373 0d0a 5072 6f76 6964  ra: docs..Provid
+00000cc0: 6573 2d45 7874 7261 3a20 7465 7374 0d0a  es-Extra: test..
+00000cd0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000ce0: 4345 4e53 450d 0a0d 0a3c 6120 6872 6566  CENSE....<a href
+00000cf0: 3d22 6874 7470 733a 2f2f 736b 6261 7365  ="https://skbase
+00000d00: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000d10: 656e 2f6c 6174 6573 742f 223e 3c69 6d67  en/latest/"><img
+00000d20: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000d30: 7468 7562 2e63 6f6d 2f73 6b74 696d 652f  thub.com/sktime/
+00000d40: 736b 6261 7365 2f62 6c6f 622f 6d61 696e  skbase/blob/main
+00000d50: 2f64 6f63 732f 736f 7572 6365 2f69 6d61  /docs/source/ima
+00000d60: 6765 732f 736b 6261 7365 2d6c 6f67 6f2d  ges/skbase-logo-
+00000d70: 7769 7468 2d6e 616d 652e 706e 6722 2077  with-name.png" w
+00000d80: 6964 7468 3d22 3137 3522 2061 6c69 676e  idth="175" align
+00000d90: 3d22 7269 6768 7422 202f 3e3c 2f61 3e0d  ="right" /></a>.
+00000da0: 0a0d 0a23 2057 656c 636f 6d65 2074 6f20  ...# Welcome to 
+00000db0: 736b 6261 7365 0d0a 0d0a 3e20 4120 6261  skbase....> A ba
+00000dc0: 7365 2063 6c61 7373 2066 6f72 2073 6369  se class for sci
+00000dd0: 6b69 742d 6c65 6172 6e2d 6c69 6b65 2061  kit-learn-like a
+00000de0: 6e64 2073 6b74 696d 652d 6c69 6b65 2070  nd sktime-like p
+00000df0: 6172 616d 6574 7269 6320 6f62 6a65 6374  arametric object
+00000e00: 730d 0a0d 0a60 736b 6261 7365 6020 7072  s....`skbase` pr
+00000e10: 6f76 6964 6573 2062 6173 6520 636c 6173  ovides base clas
+00000e20: 7365 7320 666f 7220 6372 6561 7469 6e67  ses for creating
+00000e30: 2073 6369 6b69 742d 6c65 6172 6e2d 6c69   scikit-learn-li
+00000e40: 6b65 2070 6172 616d 6574 7269 6320 6f62  ke parametric ob
+00000e50: 6a65 6374 732c 0d0a 616c 6f6e 6720 7769  jects,..along wi
+00000e60: 7468 2074 6f6f 6c73 2074 6f20 6d61 6b65  th tools to make
+00000e70: 2069 7420 6561 7369 6572 2074 6f20 6275   it easier to bu
+00000e80: 696c 6420 796f 7572 206f 776e 2070 6163  ild your own pac
+00000e90: 6b61 6765 7320 7468 6174 2066 6f6c 6c6f  kages that follo
+00000ea0: 7720 7468 6573 650d 0a64 6573 6967 6e20  w these..design 
+00000eb0: 7061 7474 6572 6e73 2e0d 0a0d 0a3a 726f  patterns.....:ro
+00000ec0: 636b 6574 3a20 5665 7273 696f 6e20 302e  cket: Version 0.
+00000ed0: 342e 3620 6973 206e 6f77 2061 7661 696c  4.6 is now avail
+00000ee0: 6162 6c65 2e20 4368 6563 6b6f 7574 206f  able. Checkout o
+00000ef0: 7572 0d0a 5b72 656c 6561 7365 206e 6f74  ur..[release not
+00000f00: 6573 5d28 6874 7470 733a 2f2f 736b 6261  es](https://skba
+00000f10: 7365 2e72 6561 6474 6865 646f 6373 2e69  se.readthedocs.i
+00000f20: 6f2f 656e 2f6c 6174 6573 742f 6368 616e  o/en/latest/chan
+00000f30: 6765 6c6f 672e 6874 6d6c 292e 0d0a 0d0a  gelog.html).....
+00000f40: 7c20 4f76 6572 7669 6577 207c 207c 0d0a  | Overview | |..
+00000f50: 7c2d 2d2d 7c2d 2d2d 7c0d 0a7c 202a 2a43  |---|---|..| **C
+00000f60: 492f 4344 2a2a 207c 205b 215b 5465 7374  I/CD** | [![Test
+00000f70: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000f80: 622e 636f 6d2f 736b 7469 6d65 2f73 6b62  b.com/sktime/skb
+00000f90: 6173 652f 6163 7469 6f6e 732f 776f 726b  ase/actions/work
+00000fa0: 666c 6f77 732f 7465 7374 2e79 6d6c 2f62  flows/test.yml/b
+00000fb0: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
+00000fc0: 6d61 696e 295d 2868 7474 7073 3a2f 2f67  main)](https://g
+00000fd0: 6974 6875 622e 636f 6d2f 736b 7469 6d65  ithub.com/sktime
+00000fe0: 2f73 6b62 6173 652f 6163 7469 6f6e 732f  /skbase/actions/
+00000ff0: 776f 726b 666c 6f77 732f 7465 7374 2e79  workflows/test.y
+00001000: 6d6c 2920 5b21 5b63 6f64 6563 6f76 5d28  ml) [![codecov](
+00001010: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00001020: 696f 2f67 682f 736b 7469 6d65 2f73 6b62  io/gh/sktime/skb
+00001030: 6173 652f 6272 616e 6368 2f6d 6169 6e2f  ase/branch/main/
+00001040: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00001050: 746f 6b65 6e3d 324a 3432 344e 4c4f 3832  token=2J424NLO82
+00001060: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00001070: 6f76 2e69 6f2f 6768 2f73 6b74 696d 652f  ov.io/gh/sktime/
+00001080: 736b 6261 7365 2920 5b21 5b44 6f63 756d  skbase) [![Docum
+00001090: 656e 7461 7469 6f6e 2053 7461 7475 735d  entation Status]
+000010a0: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
+000010b0: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
+000010c0: 732f 736b 6261 7365 2f62 6164 6765 2f3f  s/skbase/badge/?
+000010d0: 7665 7273 696f 6e3d 6c61 7465 7374 295d  version=latest)]
+000010e0: 2868 7474 7073 3a2f 2f73 6b62 6173 652e  (https://skbase.
+000010f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00001100: 6e2f 6c61 7465 7374 2f3f 6261 6467 653d  n/latest/?badge=
+00001110: 6c61 7465 7374 2920 5b21 5b70 7265 2d63  latest) [![pre-c
+00001120: 6f6d 6d69 742e 6369 2073 7461 7475 735d  ommit.ci status]
+00001130: 2868 7474 7073 3a2f 2f72 6573 756c 7473  (https://results
+00001140: 2e70 7265 2d63 6f6d 6d69 742e 6369 2f62  .pre-commit.ci/b
+00001150: 6164 6765 2f67 6974 6875 622f 736b 7469  adge/github/skti
+00001160: 6d65 2f73 6b62 6173 652f 6d61 696e 2e73  me/skbase/main.s
+00001170: 7667 295d 2868 7474 7073 3a2f 2f72 6573  vg)](https://res
+00001180: 756c 7473 2e70 7265 2d63 6f6d 6d69 742e  ults.pre-commit.
+00001190: 6369 2f6c 6174 6573 742f 6769 7468 7562  ci/latest/github
+000011a0: 2f73 6b74 696d 652f 736b 6261 7365 2f6d  /sktime/skbase/m
+000011b0: 6169 6e29 207c 0d0a 7c20 2a2a 436f 6465  ain) |..| **Code
+000011c0: 2a2a 207c 2020 5b21 5b21 7079 7069 5d28  ** |  [![!pypi](
+000011d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000011e0: 6c64 732e 696f 2f70 7970 692f 762f 7363  lds.io/pypi/v/sc
+000011f0: 696b 6974 2d62 6173 653f 636f 6c6f 723d  ikit-base?color=
+00001200: 6f72 616e 6765 295d 2868 7474 7073 3a2f  orange)](https:/
+00001210: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00001220: 742f 736b 6261 7365 2f29 2020 5b21 5b21  t/skbase/)  [![!
+00001230: 7079 7468 6f6e 2d76 6572 7369 6f6e 735d  python-versions]
+00001240: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00001250: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+00001260: 6572 7369 6f6e 732f 7363 696b 6974 2d62  ersions/scikit-b
+00001270: 6173 6529 5d28 6874 7470 733a 2f2f 7777  ase)](https://ww
+00001280: 772e 7079 7468 6f6e 2e6f 7267 2f29 205b  w.python.org/) [
+00001290: 215b 2162 6c61 636b 5d28 6874 7470 733a  ![!black](https:
+000012a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000012b0: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
+000012c0: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
+000012d0: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+000012e0: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
+000012f0: 6163 6b29 205b 215b 7365 6375 7269 7479  ack) [![security
+00001300: 3a20 6261 6e64 6974 5d28 6874 7470 733a  : bandit](https:
+00001310: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001320: 2f62 6164 6765 2f73 6563 7572 6974 792d  /badge/security-
+00001330: 6261 6e64 6974 2d79 656c 6c6f 772e 7376  bandit-yellow.sv
+00001340: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00001350: 7562 2e63 6f6d 2f50 7943 5141 2f62 616e  ub.com/PyCQA/ban
+00001360: 6469 7429 207c 0d0a 7c20 2a2a 446f 776e  dit) |..| **Down
+00001370: 6c6f 6164 732a 2a7c 205b 215b 446f 776e  loads**| [![Down
+00001380: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
+00001390: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
+000013a0: 7065 7273 6f6e 616c 697a 6564 2d62 6164  personalized-bad
+000013b0: 6765 2f73 6369 6b69 742d 6261 7365 3f70  ge/scikit-base?p
+000013c0: 6572 696f 643d 7765 656b 2675 6e69 7473  eriod=week&units
+000013d0: 3d69 6e74 6572 6e61 7469 6f6e 616c 5f73  =international_s
+000013e0: 7973 7465 6d26 6c65 6674 5f63 6f6c 6f72  ystem&left_color
+000013f0: 3d67 7265 7926 7269 6768 745f 636f 6c6f  =grey&right_colo
+00001400: 723d 626c 7565 266c 6566 745f 7465 7874  r=blue&left_text
+00001410: 3d77 6565 6b6c 7925 3230 2870 7970 6929  =weekly%20(pypi)
+00001420: 295d 2868 7474 7073 3a2f 2f70 6570 792e  )](https://pepy.
+00001430: 7465 6368 2f70 726f 6a65 6374 2f73 6369  tech/project/sci
+00001440: 6b69 742d 6261 7365 2920 5b21 5b44 6f77  kit-base) [![Dow
+00001450: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
+00001460: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
+00001470: 2f70 6572 736f 6e61 6c69 7a65 642d 6261  /personalized-ba
+00001480: 6467 652f 7363 696b 6974 2d62 6173 653f  dge/scikit-base?
+00001490: 7065 7269 6f64 3d6d 6f6e 7468 2675 6e69  period=month&uni
+000014a0: 7473 3d69 6e74 6572 6e61 7469 6f6e 616c  ts=international
+000014b0: 5f73 7973 7465 6d26 6c65 6674 5f63 6f6c  _system&left_col
+000014c0: 6f72 3d67 7265 7926 7269 6768 745f 636f  or=grey&right_co
+000014d0: 6c6f 723d 626c 7565 266c 6566 745f 7465  lor=blue&left_te
+000014e0: 7874 3d6d 6f6e 7468 6c79 2532 3028 7079  xt=monthly%20(py
+000014f0: 7069 2929 5d28 6874 7470 733a 2f2f 7065  pi))](https://pe
+00001500: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
+00001510: 7363 696b 6974 2d62 6173 6529 205b 215b  scikit-base) [![
+00001520: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
+00001530: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
+00001540: 6563 682f 7065 7273 6f6e 616c 697a 6564  ech/personalized
+00001550: 2d62 6164 6765 2f73 6369 6b69 742d 6261  -badge/scikit-ba
+00001560: 7365 3f70 6572 696f 643d 746f 7461 6c26  se?period=total&
+00001570: 756e 6974 733d 696e 7465 726e 6174 696f  units=internatio
+00001580: 6e61 6c5f 7379 7374 656d 266c 6566 745f  nal_system&left_
+00001590: 636f 6c6f 723d 6772 6579 2672 6967 6874  color=grey&right
+000015a0: 5f63 6f6c 6f72 3d62 6c75 6526 6c65 6674  _color=blue&left
+000015b0: 5f74 6578 743d 6375 6d75 6c61 7469 7665  _text=cumulative
+000015c0: 2532 3028 7079 7069 2929 5d28 6874 7470  %20(pypi))](http
+000015d0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+000015e0: 6f6a 6563 742f 7363 696b 6974 2d62 6173  oject/scikit-bas
+000015f0: 6529 207c 0d0a 0d0a 3c21 2d2d 2041 4c4c  e) |....<!-- ALL
+00001600: 2d43 4f4e 5452 4942 5554 4f52 532d 4241  -CONTRIBUTORS-BA
+00001610: 4447 453a 5354 4152 5420 2d20 446f 206e  DGE:START - Do n
+00001620: 6f74 2072 656d 6f76 6520 6f72 206d 6f64  ot remove or mod
+00001630: 6966 7920 7468 6973 2073 6563 7469 6f6e  ify this section
+00001640: 202d 2d3e 0d0a 5b21 5b41 6c6c 2043 6f6e   -->..[![All Con
+00001650: 7472 6962 7574 6f72 735d 2868 7474 7073  tributors](https
+00001660: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001670: 6f2f 6261 6467 652f 616c 6c5f 636f 6e74  o/badge/all_cont
+00001680: 7269 6275 746f 7273 2d31 332d 6f72 616e  ributors-13-oran
+00001690: 6765 2e73 7667 3f73 7479 6c65 3d66 6c61  ge.svg?style=fla
+000016a0: 742d 7371 7561 7265 295d 2823 636f 6e74  t-square)](#cont
+000016b0: 7269 6275 746f 7273 290d 0a3c 212d 2d20  ributors)..<!-- 
+000016c0: 414c 4c2d 434f 4e54 5249 4255 544f 5253  ALL-CONTRIBUTORS
+000016d0: 2d42 4144 4745 3a45 4e44 202d 2d3e 0d0a  -BADGE:END -->..
+000016e0: 0d0a 2323 2044 6f63 756d 656e 7461 7469  ..## Documentati
+000016f0: 6f6e 0d0a 0d0a 546f 206c 6561 726e 206d  on....To learn m
+00001700: 6f72 6520 6162 6f75 7420 7468 6520 7061  ore about the pa
+00001710: 636b 6167 6520 6368 6563 6b6f 7574 206f  ckage checkout o
+00001720: 7572 205b 646f 6375 6d65 6e74 6174 696f  ur [documentatio
+00001730: 6e5d 2868 7474 7073 3a2f 2f73 6b62 6173  n](https://skbas
+00001740: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00001750: 2f65 6e2f 6c61 7465 7374 2f29 2e0d 0a0d  /en/latest/)....
+00001760: 0a23 2320 3a68 6f75 7267 6c61 7373 5f66  .## :hourglass_f
+00001770: 6c6f 7769 6e67 5f73 616e 643a 2049 6e73  lowing_sand: Ins
+00001780: 7461 6c6c 2073 6b62 6173 650d 0a46 6f72  tall skbase..For
+00001790: 2074 726f 7562 6c65 2073 686f 6f74 696e   trouble shootin
+000017a0: 6720 6f72 206d 6f72 6520 696e 666f 726d  g or more inform
+000017b0: 6174 696f 6e2c 2073 6565 206f 7572 0d0a  ation, see our..
+000017c0: 5b64 6574 6169 6c65 6420 696e 7374 616c  [detailed instal
+000017d0: 6c61 7469 6f6e 2069 6e73 7472 7563 7469  lation instructi
+000017e0: 6f6e 735d 2868 7474 7073 3a2f 2f73 6b62  ons](https://skb
+000017f0: 6173 652e 7265 6164 7468 6564 6f63 732e  ase.readthedocs.
+00001800: 696f 2f65 6e2f 6c61 7465 7374 2f75 7365  io/en/latest/use
+00001810: 725f 646f 6375 6d65 6e74 6174 696f 6e2f  r_documentation/
+00001820: 696e 7374 616c 6c61 7469 6f6e 2e68 746d  installation.htm
+00001830: 6c29 2e0d 0a0d 0a2d 202a 2a4f 7065 7261  l).....- **Opera
+00001840: 7469 6e67 2073 7973 7465 6d2a 2a3a 206d  ting system**: m
+00001850: 6163 4f53 2058 20c2 b720 4c69 6e75 7820  acOS X .. Linux 
+00001860: c2b7 2057 696e 646f 7773 2038 2e31 206f  .. Windows 8.1 o
+00001870: 7220 6869 6768 6572 0d0a 2d20 2a2a 5079  r higher..- **Py
+00001880: 7468 6f6e 2076 6572 7369 6f6e 2a2a 3a20  thon version**: 
+00001890: 5079 7468 6f6e 2033 2e37 2c20 332e 382c  Python 3.7, 3.8,
+000018a0: 2033 2e39 2c20 332e 3130 2061 6e64 2033   3.9, 3.10 and 3
+000018b0: 2e31 310d 0a2d 202a 2a50 6163 6b61 6765  .11..- **Package
+000018c0: 206d 616e 6167 6572 732a 2a3a 205b 7069   managers**: [pi
+000018d0: 705d 0d0a 0d0a 5b70 6970 5d3a 2068 7474  p]....[pip]: htt
+000018e0: 7073 3a2f 2f70 6970 2e70 7970 612e 696f  ps://pip.pypa.io
+000018f0: 2f65 6e2f 7374 6162 6c65 2f0d 0a0d 0a23  /en/stable/....#
+00001900: 2323 2070 6970 0d0a 736b 6261 7365 2072  ## pip..skbase r
+00001910: 656c 6561 7365 7320 6172 6520 6176 6169  eleases are avai
+00001920: 6c61 626c 6520 6173 2073 6f75 7263 6520  lable as source 
+00001930: 7061 636b 6167 6573 2061 6e64 2062 696e  packages and bin
+00001940: 6172 7920 7768 6565 6c73 2076 6961 2050  ary wheels via P
+00001950: 7950 490d 0a61 6e64 2063 616e 2062 6520  yPI..and can be 
+00001960: 696e 7374 616c 6c65 6420 7573 696e 6720  installed using 
+00001970: 7069 702e 2043 6865 636b 6f75 7420 7468  pip. Checkout th
+00001980: 6520 6675 6c6c 206c 6973 7420 6f66 2070  e full list of p
+00001990: 7265 2d63 6f6d 7069 6c65 6420 5b77 6865  re-compiled [whe
+000019a0: 656c 7320 6f6e 2050 7950 695d 2868 7474  els on PyPi](htt
+000019b0: 7073 3a2f 2f70 7970 692e 6f72 672f 7369  ps://pypi.org/si
+000019c0: 6d70 6c65 2f73 6b62 6173 652f 292e 0d0a  mple/skbase/)...
+000019d0: 0d0a 546f 2069 6e73 7461 6c6c 2074 6865  ..To install the
+000019e0: 2063 6f72 6520 7061 636b 6167 6520 7573   core package us
+000019f0: 653a 0d0a 0d0a 6060 6062 6173 680d 0a70  e:....```bash..p
+00001a00: 6970 2069 6e73 7461 6c6c 2073 6369 6b69  ip install sciki
+00001a10: 742d 6261 7365 0d0a 6060 600d 0a0d 0a6f  t-base..```....o
+00001a20: 722c 2069 6620 796f 7520 7761 6e74 2074  r, if you want t
+00001a30: 6f20 696e 7374 616c 6c20 7769 7468 2074  o install with t
+00001a40: 6865 206d 6178 696d 756d 2073 6574 206f  he maximum set o
+00001a50: 6620 6465 7065 6e64 656e 6369 6573 2c20  f dependencies, 
+00001a60: 7573 653a 0d0a 0d0a 6060 6062 6173 680d  use:....```bash.
+00001a70: 0a70 6970 2069 6e73 7461 6c6c 2073 6369  .pip install sci
+00001a80: 6b69 742d 6261 7365 5b61 6c6c 5f65 7874  kit-base[all_ext
+00001a90: 7261 735d 0d0a 6060 600d 0a              ras]..```..
```

### Comparing `scikit-base-0.4.5/scikit_base.egg-info/SOURCES.txt` & `scikit-base-0.4.6/scikit_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/scikit_base.egg-info/requires.txt` & `scikit-base-0.4.6/scikit_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/_exceptions.py` & `scikit-base-0.4.6/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/_nopytest_tests.py` & `scikit-base-0.4.6/skbase/_nopytest_tests.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/base/__init__.py` & `scikit-base-0.4.6/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/base/_base.py` & `scikit-base-0.4.6/skbase/base/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         RuntimeError if the clone is non-conforming, due to faulty ``__init__``.
 
         Notes
         -----
         If successful, equal in value to ``type(self)(**self.get_params(deep=False))``.
         """
         self_params = self.get_params(deep=False)
-        self_clone = type(self)(**self_params)
+        self_clone = self._clone(self)
 
         # if checking the clone is turned off, return now
         if not self.get_config()["check_clone"]:
             return self_clone
 
         from skbase.utils.deep_equals import deep_equals
 
@@ -181,14 +181,85 @@
                 f"error in {self}.clone, __init__ must write all arguments "
                 f"to self and not mutate them, but this is not the case. "
                 f"Error on equality check of arguments (x) vs parameters (y): {msg}"
             )
 
         return self_clone
 
+    # copied from sklearn
+    def _clone(self, estimator, *, safe=True):
+        """Construct a new unfitted estimator with the same parameters.
+
+        Clone does a deep copy of the model in an estimator
+        without actually copying attached data. It returns a new estimator
+        with the same parameters that has not been fitted on any data.
+
+        Parameters
+        ----------
+        estimator : {list, tuple, set} of estimator instance or a single \
+                estimator instance
+            The estimator or group of estimators to be cloned.
+        safe : bool, default=True
+            If safe is False, clone will fall back to a deep copy on objects
+            that are not estimators.
+
+        Returns
+        -------
+        estimator : object
+            The deep copy of the input, an estimator if input is an estimator.
+
+        Notes
+        -----
+        If the estimator's `random_state` parameter is an integer (or if the
+        estimator doesn't have a `random_state` parameter), an *exact clone* is
+        returned: the clone and the original estimator will give the exact same
+        results. Otherwise, *statistical clone* is returned: the clone might
+        return different results from the original estimator. More details can be
+        found in :ref:`randomness`.
+        """
+        estimator_type = type(estimator)
+        # XXX: not handling dictionaries
+        if estimator_type in (list, tuple, set, frozenset):
+            return estimator_type([self._clone(e, safe=safe) for e in estimator])
+        elif not hasattr(estimator, "get_params") or isinstance(estimator, type):
+            if not safe:
+                return deepcopy(estimator)
+            else:
+                if isinstance(estimator, type):
+                    raise TypeError(
+                        "Cannot clone object. "
+                        + "You should provide an instance of "
+                        + "scikit-learn estimator instead of a class."
+                    )
+                else:
+                    raise TypeError(
+                        "Cannot clone object '%s' (type %s): "
+                        "it does not seem to be a scikit-learn "
+                        "estimator as it does not implement a "
+                        "'get_params' method." % (repr(estimator), type(estimator))
+                    )
+
+        klass = estimator.__class__
+        new_object_params = estimator.get_params(deep=False)
+        for name, param in new_object_params.items():
+            new_object_params[name] = self._clone(param, safe=False)
+        new_object = klass(**new_object_params)
+        params_set = new_object.get_params(deep=False)
+
+        # quick sanity check of the parameters of the clone
+        for name in new_object_params:
+            param1 = new_object_params[name]
+            param2 = params_set[name]
+            if param1 is not param2:
+                raise RuntimeError(
+                    "Cannot clone object %s, as the constructor "
+                    "either does not set or modifies parameter %s" % (estimator, name)
+                )
+        return new_object
+
     @classmethod
     def _get_init_signature(cls):
         """Get class init sigature.
 
         Useful in parameter inspection.
 
         Returns
```

### Comparing `scikit-base-0.4.5/skbase/base/_meta.py` & `scikit-base-0.4.6/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/base/_pretty_printing/_object_html_repr.py` & `scikit-base-0.4.6/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/base/_pretty_printing/_pprint.py` & `scikit-base-0.4.6/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/base/_tagmanager.py` & `scikit-base-0.4.6/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/lookup/__init__.py` & `scikit-base-0.4.6/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/lookup/_lookup.py` & `scikit-base-0.4.6/skbase/lookup/_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,34 +276,45 @@
         Whether to suppress stdout printout upon import.
 
     Returns
     -------
     imported_mod : ModuleType
         The module that was imported.
     """
-    if isinstance(module, str):
-        if suppress_import_stdout:
-            # setup text trap, import, then restore
-            sys.stdout = io.StringIO()
-            imported_mod = importlib.import_module(module)
-            sys.stdout = sys.__stdout__
-        else:
-            imported_mod = importlib.import_module(module)
-    elif isinstance(module, importlib.machinery.SourceFileLoader):
-        if suppress_import_stdout:
-            sys.stdout = io.StringIO()
-            imported_mod = module.load_module()
-            sys.stdout = sys.__stdout__
-        else:
-            imported_mod = module.load_module()
-    else:
+    # input check
+    if not isinstance(module, (str, importlib.machinery.SourceFileLoader)):
         raise ValueError(
             "`module` should be string module name or instance of "
             "importlib.machinery.SourceFileLoader."
         )
+
+    # if suppress_import_stdout:
+    # setup text trap, import
+    if suppress_import_stdout:
+        temp_stdout = sys.stdout
+        sys.stdout = io.StringIO()
+
+    try:
+        if isinstance(module, str):
+            imported_mod = importlib.import_module(module)
+        elif isinstance(module, importlib.machinery.SourceFileLoader):
+            imported_mod = module.load_module()
+        exc = None
+    except Exception as e:
+        # we store the exception so we can restore the stdout fisrt
+        exc = e
+
+    # if we set up a text trap, restore it to the initial value
+    if suppress_import_stdout:
+        sys.stdout = temp_stdout
+
+    # if we encountered an exception, now raise it
+    if exc is not None:
+        raise exc
+
     return imported_mod
 
 
 def _determine_module_path(
     package_name: str, path: Optional[Union[str, pathlib.Path]] = None
 ) -> Tuple[ModuleType, str, importlib.machinery.SourceFileLoader]:
     """Determine a package's path information.
```

### Comparing `scikit-base-0.4.5/skbase/lookup/tests/test_lookup.py` & `scikit-base-0.4.6/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/testing/test_all_objects.py` & `scikit-base-0.4.6/skbase/testing/test_all_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/testing/utils/_conditional_fixtures.py` & `scikit-base-0.4.6/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/testing/utils/inspect.py` & `scikit-base-0.4.6/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/testing/utils/tests/test_check_dependencies.py` & `scikit-base-0.4.6/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/testing/utils/tests/test_deep_equals.py` & `scikit-base-0.4.6/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/tests/conftest.py` & `scikit-base-0.4.6/skbase/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/tests/mock_package/test_mock_package.py` & `scikit-base-0.4.6/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/tests/test_base.py` & `scikit-base-0.4.6/skbase/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     "test_clone_raises_error_for_nonconforming_objects",
     "test_clone_param_is_none",
     "test_clone_empty_array",
     "test_clone_sparse_matrix",
     "test_clone_nan",
     "test_clone_estimator_types",
     "test_clone_class_rather_than_instance_raises_error",
+    "test_clone_sklearn_composite",
     "test_baseobject_repr",
     "test_baseobject_str",
     "test_baseobject_repr_mimebundle_",
     "test_repr_html_wraps",
     "test_get_test_params",
     "test_get_test_params_raises_error_when_params_required",
     "test_create_test_instance",
@@ -927,14 +928,29 @@
     from sklearn.base import clone
 
     msg = "You should provide an instance of scikit-learn estimator"
     with pytest.raises(TypeError, match=msg):
         clone(fixture_class_parent)
 
 
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
+def test_clone_sklearn_composite(fixture_class_parent: Type[Parent]):
+    """Test clone with keyword parameter set to None."""
+    from sklearn.ensemble import GradientBoostingRegressor
+
+    sklearn_obj = GradientBoostingRegressor(random_state=5, learning_rate=0.02)
+    composite = ResetTester(a=sklearn_obj)
+    composite_set = composite.clone().set_params(a__random_state=42)
+    assert composite.get_params()["a__random_state"] == 5
+    assert composite_set.get_params()["a__random_state"] == 42
+
+
 # Tests of BaseObject pretty printing representation inspired by sklearn
 def test_baseobject_repr(
     fixture_class_parent: Type[Parent],
     fixture_composition_dummy: Type[CompositionDummy],
 ):
     """Test BaseObject repr works as expected."""
     # Simple test where all parameters are left at defaults
```

### Comparing `scikit-base-0.4.5/skbase/tests/test_baseestimator.py` & `scikit-base-0.4.6/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/tests/test_exceptions.py` & `scikit-base-0.4.6/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/tests/test_meta.py` & `scikit-base-0.4.6/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/__init__.py` & `scikit-base-0.4.6/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/_check.py` & `scikit-base-0.4.6/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/_iter.py` & `scikit-base-0.4.6/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/_nested_iter.py` & `scikit-base-0.4.6/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/_utils.py` & `scikit-base-0.4.6/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/deep_equals.py` & `scikit-base-0.4.6/skbase/utils/deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/dependencies/_dependencies.py` & `scikit-base-0.4.6/skbase/utils/dependencies/_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/tests/test_check.py` & `scikit-base-0.4.6/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/tests/test_iter.py` & `scikit-base-0.4.6/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/tests/test_nested_iter.py` & `scikit-base-0.4.6/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/utils/tests/test_utils.py` & `scikit-base-0.4.6/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/validate/__init__.py` & `scikit-base-0.4.6/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/validate/_named_objects.py` & `scikit-base-0.4.6/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/validate/_types.py` & `scikit-base-0.4.6/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/validate/tests/test_iterable_named_objects.py` & `scikit-base-0.4.6/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.5/skbase/validate/tests/test_type_validations.py` & `scikit-base-0.4.6/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

