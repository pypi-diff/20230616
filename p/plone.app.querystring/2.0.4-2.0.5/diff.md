# Comparing `tmp/plone.app.querystring-2.0.4.tar.gz` & `tmp/plone.app.querystring-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.querystring-2.0.4.tar", last modified: Mon May 22 18:01:36 2023, max compression
+gzip compressed data, was "plone.app.querystring-2.0.5.tar", last modified: Fri Jun 16 16:34:55 2023, max compression
```

## Comparing `plone.app.querystring-2.0.4.tar` & `plone.app.querystring-2.0.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.269214 plone.app.querystring-2.0.4/
--rw-r--r--   0 maurits    (501) staff       (20)    12787 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    14678 2023-05-22 18:01:36.269335 plone.app.querystring-2.0.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      966 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.253178 plone.app.querystring-2.0.4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      683 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.253423 plone.app.querystring-2.0.4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.255989 plone.app.querystring-2.0.4/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.260054 plone.app.querystring-2.0.4/plone/app/querystring/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1811 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/hiddenprofiles.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.260908 plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1240 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2644 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/query_index_modifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1562 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.248683 plone.app.querystring-2.0.4/plone/app/querystring/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.261393 plone.app.querystring-2.0.4/plone/app/querystring/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      185 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)    32950 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.250192 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.261735 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_10/
--rw-r--r--   0 maurits    (501) staff       (20)      539 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_10/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.262108 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_11/
--rw-r--r--   0 maurits    (501) staff       (20)     3366 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_11/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.262466 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_14/
--rw-r--r--   0 maurits    (501) staff       (20)     2961 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_14/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.262738 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_3/
--rw-r--r--   0 maurits    (501) staff       (20)     1411 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_3/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.263016 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_5/
--rw-r--r--   0 maurits    (501) staff       (20)     1819 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_5/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.263506 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_6/
--rw-r--r--   0 maurits    (501) staff       (20)     1772 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_6/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.263775 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_7/
--rw-r--r--   0 maurits    (501) staff       (20)      339 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_7/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.264032 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_8/
--rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_8/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.264308 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_9/
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_9/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2785 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9157 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/querybuilder.py
--rw-r--r--   0 maurits    (501) staff       (20)      715 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/querymodifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    11264 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/queryparser.py
--rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/registryreader.py
--rw-r--r--   0 maurits    (501) staff       (20)     4662 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.268469 plone.app.querystring-2.0.4/plone/app/querystring/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      481 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      863 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/index_testmodifier.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.250566 plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.269016 plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/registry/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1283 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/registry/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_minimal_correct.xml
--rw-r--r--   0 maurits    (501) staff       (20)      984 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_test_missing_operator.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_test_vocabulary.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2806 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_testdata.py
--rw-r--r--   0 maurits    (501) staff       (20)     2405 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testIndexmodifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    15001 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryBuilder.py
--rw-r--r--   0 maurits    (501) staff       (20)     3515 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryBuilderModifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    21787 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryParser.py
--rw-r--r--   0 maurits    (501) staff       (20)     2941 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testRegistryIntegration.py
--rw-r--r--   0 maurits    (501) staff       (20)     5653 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testRegistryReader.py
--rw-r--r--   0 maurits    (501) staff       (20)      532 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testVocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     5147 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2634 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.255751 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    14678 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2665 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      297 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1690 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-22 18:01:36.269782 plone.app.querystring-2.0.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1996 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.153420 plone.app.querystring-2.0.5/
+-rw-r--r--   0 maurits    (501) staff       (20)    13155 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    15046 2023-06-16 16:34:55.153056 plone.app.querystring-2.0.5/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      966 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.133099 plone.app.querystring-2.0.5/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      683 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.133687 plone.app.querystring-2.0.5/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.138066 plone.app.querystring-2.0.5/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.143318 plone.app.querystring-2.0.5/plone/app/querystring/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1811 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/hiddenprofiles.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.144177 plone.app.querystring-2.0.5/plone/app/querystring/indexmodifiers/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/indexmodifiers/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1240 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/indexmodifiers/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2644 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/indexmodifiers/query_index_modifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1562 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.127432 plone.app.querystring-2.0.5/plone/app/querystring/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.144819 plone.app.querystring-2.0.5/plone/app/querystring/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      185 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    32950 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.129132 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.145206 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_10/
+-rw-r--r--   0 maurits    (501) staff       (20)      539 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_10/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.145521 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_11/
+-rw-r--r--   0 maurits    (501) staff       (20)     3366 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_11/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.145830 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_14/
+-rw-r--r--   0 maurits    (501) staff       (20)     2961 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_14/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.146135 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_3/
+-rw-r--r--   0 maurits    (501) staff       (20)     1411 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_3/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.146444 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_5/
+-rw-r--r--   0 maurits    (501) staff       (20)     1819 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_5/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.146752 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_6/
+-rw-r--r--   0 maurits    (501) staff       (20)     1772 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_6/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.147064 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_7/
+-rw-r--r--   0 maurits    (501) staff       (20)      339 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_7/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.147368 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_8/
+-rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_8/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.147676 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_9/
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_9/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2785 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9157 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/querybuilder.py
+-rw-r--r--   0 maurits    (501) staff       (20)      715 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/querymodifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12082 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/queryparser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/registryreader.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4662 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.152025 plone.app.querystring-2.0.5/plone/app/querystring/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      481 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      863 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/index_testmodifier.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.129770 plone.app.querystring-2.0.5/plone/app/querystring/tests/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.152641 plone.app.querystring-2.0.5/plone/app/querystring/tests/profiles/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/profiles/registry/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1283 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/profiles/registry/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/registry_minimal_correct.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      984 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/registry_test_missing_operator.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/registry_test_vocabulary.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2806 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/registry_testdata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2405 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/testIndexmodifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15001 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/testQueryBuilder.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3515 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/testQueryBuilderModifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    23168 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/testQueryParser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2941 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/testRegistryIntegration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5653 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/testRegistryReader.py
+-rw-r--r--   0 maurits    (501) staff       (20)      532 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/tests/testVocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5147 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2634 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/plone/app/querystring/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:34:55.137592 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    15046 2023-06-16 16:34:55.000000 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2655 2023-06-16 16:34:55.000000 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:34:55.000000 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-16 16:34:55.000000 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-06-16 16:34:55.000000 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:34:55.000000 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      297 2023-06-16 16:34:55.000000 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-16 16:34:55.000000 plone.app.querystring-2.0.5/plone.app.querystring.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3850 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-06-16 16:34:55.153502 plone.app.querystring-2.0.5/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1996 2023-06-16 16:34:54.000000 plone.app.querystring-2.0.5/setup.py
```

### Comparing `plone.app.querystring-2.0.4/CHANGES.rst` & `plone.app.querystring-2.0.5/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Fix integer operations to accept integers. @davisagli
+  Fix integer operations to avoid adding None to the query when the input is not valid. @davisagli (#131)
+- Merge range queries on the same index instead of overwriting. @davisagli (#132)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (dd37b9f9)
+
+
 2.0.4 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix a circular transitive dependency to `plone.app.querystring`.
```

### Comparing `plone.app.querystring-2.0.4/PKG-INFO` & `plone.app.querystring-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.querystring
-Version: 2.0.4
+Version: 2.0.5
 Summary: A queryparser, querybuilder and extra helper tools, to parse stored queries to actual results, used in new style Plone collections
 Home-page: https://github.com/plone/plone.app.querystring
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection queries
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Fix integer operations to accept integers. @davisagli
+  Fix integer operations to avoid adding None to the query when the input is not valid. @davisagli (#131)
+- Merge range queries on the same index instead of overwriting. @davisagli (#132)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (dd37b9f9)
+
+
 2.0.4 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix a circular transitive dependency to `plone.app.querystring`.
```

### Comparing `plone.app.querystring-2.0.4/README.rst` & `plone.app.querystring-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/docs/LICENSE.GPL` & `plone.app.querystring-2.0.5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/docs/LICENSE.txt` & `plone.app.querystring-2.0.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/configure.zcml` & `plone.app.querystring-2.0.5/plone/app/querystring/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/hiddenprofiles.py` & `plone.app.querystring-2.0.5/plone/app/querystring/hiddenprofiles.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/configure.zcml` & `plone.app.querystring-2.0.5/plone/app/querystring/indexmodifiers/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/query_index_modifiers.py` & `plone.app.querystring-2.0.5/plone/app/querystring/indexmodifiers/query_index_modifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/interfaces.py` & `plone.app.querystring-2.0.5/plone/app/querystring/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/default/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_10/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_10/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_11/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_11/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_14/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_14/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_3/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_3/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_5/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_5/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_6/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_6/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_8/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_8/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_9/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles/upgrades/to_9/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/profiles.zcml` & `plone.app.querystring-2.0.5/plone/app/querystring/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/querybuilder.py` & `plone.app.querystring-2.0.5/plone/app/querystring/querybuilder.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/querymodifiers.py` & `plone.app.querystring-2.0.5/plone/app/querystring/querymodifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/queryparser.py` & `plone.app.querystring-2.0.5/plone/app/querystring/queryparser.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,30 +33,48 @@
 
         # The functions expect this pattern of object, so lets give it to
         # them in a named tuple instead of jamming things onto the request
         row = Row(
             index=row.get("i", None), operator=function_path, values=row.get("v", None)
         )
 
-        kwargs = {}
         parser = resolve(row.operator)
         kwargs = parser(context, row)
 
         # Special path handling - since multipath queries are possible
         path_index = PATH_INDICES & set(kwargs)
         if len(path_index) == 1:
             path_index = list(path_index)[0]
             if path_index in query:
                 query[path_index]["query"].extend(kwargs[path_index]["query"])
             else:
                 query.update(kwargs)
+            continue
         elif len(path_index) > 1:
             raise IndexError("Too many path indices in one row.")
-        else:
-            query.update(kwargs)
+
+        for index, value in kwargs.items():
+            # Merge range queries on the same index
+            if isinstance(value, dict) and "range" in value:
+                existing = query.get(index)
+                if isinstance(existing, dict) and "range" in existing:
+                    existing_query = existing["query"]
+                    if not isinstance(existing_query, list):
+                        existing_query = [existing_query]
+                    new_query = value["query"]
+                    if not isinstance(new_query, list):
+                        new_query = [new_query]
+                    existing["query"] = sorted(existing_query + new_query)
+                    if (existing["range"] == "min" and value["range"] == "max") or (
+                        existing["range"] == "max" and value["range"] == "min"
+                    ):
+                        existing["range"] = "minmax"
+                    continue
+            # Other cases: simply overwrite the query for the index
+            query[index] = value
 
     if not query:
         # If the query is empty fall back onto the equality query
         query = _equal(context, row)
 
     # Add sorting (sort_on and sort_order) to the query
     if sort_on:
@@ -108,19 +126,21 @@
 def _intEqual(context, row):
     values = None
     if type(row.values) is list:
         try:
             values = [int(v) for v in row.values]
         except (ValueError, TypeError, AttributeError):
             pass
-    elif not isinstance(row.values, int):
+    else:
         try:
             values = int(row.values)
         except (ValueError, TypeError, AttributeError):
             pass
+    if values is None:
+        return {}
     return {row.index: {"query": values}}
 
 
 def _isTrue(context, row):
     return {row.index: {"query": True}}
 
 
@@ -150,54 +170,47 @@
             "range": "min",
         },
     }
     return tmp
 
 
 def _intLargerThan(context, row):
-    value = None
-    if not isinstance(row.values, int):
-        try:
-            value = int(row.values)
-        except (ValueError, TypeError, AttributeError):
-            pass
-    tmp = {
+    try:
+        value = int(row.values)
+    except (ValueError, TypeError, AttributeError):
+        return {}
+    return {
         row.index: {
             "query": value,
             "range": "min",
         },
     }
-    return tmp
 
 
 def _lessThan(context, row):
     tmp = {
         row.index: {
             "query": row.values,
             "range": "max",
         },
     }
     return tmp
 
 
 def _intLessThan(context, row):
-    value = None
-    if not isinstance(row.values, int):
-        try:
-            value = int(row.values)
-        except (ValueError, TypeError, AttributeError):
-            # value = 0
-            pass
-    tmp = {
+    try:
+        value = int(row.values)
+    except (ValueError, TypeError, AttributeError):
+        return {}
+    return {
         row.index: {
             "query": value,
             "range": "max",
         },
     }
-    return tmp
 
 
 def _currentUser(context, row):
     """Current user lookup"""
     mt = getToolByName(context, "portal_membership")
     user = mt.getAuthenticatedMember()
     return {row.index: {"query": user.getUserName()}}
```

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/registryreader.py` & `plone.app.querystring-2.0.5/plone/app/querystring/registryreader.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/results.pt` & `plone.app.querystring-2.0.5/plone/app/querystring/results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/testing.py` & `plone.app.querystring-2.0.5/plone/app/querystring/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/index_testmodifier.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/index_testmodifier.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/registry/registry.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/profiles/registry/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_minimal_correct.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/registry_minimal_correct.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_test_missing_operator.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/registry_test_missing_operator.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_test_vocabulary.xml` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/registry_test_vocabulary.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_testdata.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/registry_testdata.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/testIndexmodifiers.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/testIndexmodifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryBuilder.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/testQueryBuilder.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryBuilderModifiers.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/testQueryBuilderModifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryParser.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/testQueryParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,14 +281,30 @@
                 "path": {
                     "query": ["/%s/foo" % MOCK_SITE_ID, "/%s/bar" % MOCK_SITE_ID],
                     "depth": 2,
                 }
             },
         )
 
+    def test_merge_ranges(self):
+        data = [
+            {
+                "i": "modified",
+                "o": "plone.app.querystring.operation.int.largerThan",
+                "v": 10,
+            },
+            {
+                "i": "modified",
+                "o": "plone.app.querystring.operation.int.lessThan",
+                "v": 20,
+            },
+        ]
+        parsed = queryparser.parseFormquery(MockSite(), data)
+        self.assertEqual(parsed, {"modified": {"query": [10, 20], "range": "minmax"}})
+
 
 class TestQueryGenerators(TestQueryParserBase):
     def test__between(self):
         data = Row(
             index="modified", operator="_between", values=["2009/08/12", "2009/08/14"]
         )
         parsed = queryparser._between(MockSite(), data)
@@ -323,14 +339,26 @@
             index="modified", operator="_equal", values=["2010/03/18", "2010/03/19"]
         )
         parsed = queryparser._equal(MockSite(), data)
         expected = {"modified": {"query": ["2010/03/18", "2010/03/19"]}}
         self.assertEqual(parsed, expected)
 
     def test__intEqual(self):
+        # int
+        data = Row(index="modified", operator="_intEqual", values=20)
+        parsed = queryparser._intEqual(MockSite(), data)
+        expected = {"modified": {"query": 20}}
+        self.assertEqual(parsed, expected)
+
+        # list of ints
+        data = Row(index="modified", operator="_intEqual", values=[20, 21])
+        parsed = queryparser._intEqual(MockSite(), data)
+        expected = {"modified": {"query": [20, 21]}}
+        self.assertEqual(parsed, expected)
+
         # bytes
         data = Row(index="modified", operator="_intEqual", values=b"20")
         parsed = queryparser._intEqual(MockSite(), data)
         expected = {"modified": {"query": 20}}
         self.assertEqual(parsed, expected)
 
         # list of bytes
@@ -350,32 +378,38 @@
         parsed = queryparser._intEqual(MockSite(), data)
         expected = {"modified": {"query": [20, 21]}}
         self.assertEqual(parsed, expected)
 
         # bad text
         data = Row(index="modified", operator="_intEqual", values="bad")
         parsed = queryparser._intEqual(MockSite(), data)
-        expected = {"modified": {"query": None}}
+        expected = {}
         self.assertEqual(parsed, expected)
 
         # list of bad text
         data = Row(
             index="modified", operator="_intEqual", values=[b"bad", "text", "values"]
         )
         parsed = queryparser._intEqual(MockSite(), data)
-        expected = {"modified": {"query": None}}
+        expected = {}
         self.assertEqual(parsed, expected)
 
     def test__lessThan(self):
         data = Row(index="modified", operator="_lessThan", values="2010/03/18")
         parsed = queryparser._lessThan(MockSite(), data)
         expected = {"modified": {"query": "2010/03/18", "range": "max"}}
         self.assertEqual(parsed, expected)
 
     def test__intLessThan(self):
+        # int
+        data = Row(index="modified", operator="_intLessThan", values=20)
+        parsed = queryparser._intLessThan(MockSite(), data)
+        expected = {"modified": {"query": 20, "range": "max"}}
+        self.assertEqual(parsed, expected)
+
         # bytes
         data = Row(index="modified", operator="_intLessThan", values=b"20")
         parsed = queryparser._intLessThan(MockSite(), data)
         expected = {"modified": {"query": 20, "range": "max"}}
         self.assertEqual(parsed, expected)
 
         # text
@@ -383,24 +417,30 @@
         parsed = queryparser._intLessThan(MockSite(), data)
         expected = {"modified": {"query": 20, "range": "max"}}
         self.assertEqual(parsed, expected)
 
         # bad value
         data = Row(index="modified", operator="_intLessThan", values="bad")
         parsed = queryparser._intLessThan(MockSite(), data)
-        expected = {"modified": {"query": None, "range": "max"}}
+        expected = {}
         self.assertEqual(parsed, expected)
 
     def test__largerThan(self):
         data = Row(index="modified", operator="_largerThan", values="2010/03/18")
         parsed = queryparser._largerThan(MockSite(), data)
         expected = {"modified": {"query": "2010/03/18", "range": "min"}}
         self.assertEqual(parsed, expected)
 
     def test__intLargerThan(self):
+        # int
+        data = Row(index="modified", operator="_intLargerThan", values=20)
+        parsed = queryparser._intLargerThan(MockSite(), data)
+        expected = {"modified": {"query": 20, "range": "min"}}
+        self.assertEqual(parsed, expected)
+
         # bytes
         data = Row(index="modified", operator="_intLargerThan", values=b"20")
         parsed = queryparser._intLargerThan(MockSite(), data)
         expected = {"modified": {"query": 20, "range": "min"}}
         self.assertEqual(parsed, expected)
 
         # text
@@ -408,15 +448,15 @@
         parsed = queryparser._intLargerThan(MockSite(), data)
         expected = {"modified": {"query": 20, "range": "min"}}
         self.assertEqual(parsed, expected)
 
         # bad value
         data = Row(index="modified", operator="_intLargerThan", values="bad")
         parsed = queryparser._intLargerThan(MockSite(), data)
-        expected = {"modified": {"query": None, "range": "min"}}
+        expected = {}
         self.assertEqual(parsed, expected)
 
     def test__currentUser(self):
         # Anonymous user
         u = MockUser()
         pm = MockPortal_membership(user=u)
         context = MockSite(portal_membership=pm)
```

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/testRegistryIntegration.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/testRegistryIntegration.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/testRegistryReader.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/testRegistryReader.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/tests/testVocabularies.py` & `plone.app.querystring-2.0.5/plone/app/querystring/tests/testVocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/upgrades.py` & `plone.app.querystring-2.0.5/plone/app/querystring/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/upgrades.zcml` & `plone.app.querystring-2.0.5/plone/app/querystring/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone/app/querystring/vocabularies.py` & `plone.app.querystring-2.0.5/plone/app/querystring/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.4/plone.app.querystring.egg-info/PKG-INFO` & `plone.app.querystring-2.0.5/plone.app.querystring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.querystring
-Version: 2.0.4
+Version: 2.0.5
 Summary: A queryparser, querybuilder and extra helper tools, to parse stored queries to actual results, used in new style Plone collections
 Home-page: https://github.com/plone/plone.app.querystring
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection queries
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Fix integer operations to accept integers. @davisagli
+  Fix integer operations to avoid adding None to the query when the input is not valid. @davisagli (#131)
+- Merge range queries on the same index instead of overwriting. @davisagli (#132)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (dd37b9f9)
+
+
 2.0.4 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix a circular transitive dependency to `plone.app.querystring`.
```

### Comparing `plone.app.querystring-2.0.4/plone.app.querystring.egg-info/SOURCES.txt` & `plone.app.querystring-2.0.5/plone.app.querystring.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.app.querystring.egg-info/PKG-INFO
 plone.app.querystring.egg-info/SOURCES.txt
 plone.app.querystring.egg-info/dependency_links.txt
```

### Comparing `plone.app.querystring-2.0.4/setup.py` & `plone.app.querystring-2.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.4"
+version = "2.0.5"
 
 long_description = open("README.rst").read() + "\n"
 long_description += open("CHANGES.rst").read()
 
 setup(
     name="plone.app.querystring",
     version=version,
```

