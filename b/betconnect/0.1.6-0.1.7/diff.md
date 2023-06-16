# Comparing `tmp/betconnect-0.1.6.tar.gz` & `tmp/betconnect-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/betconnect-0.1.6.tar", last modified: Wed Feb 15 16:22:56 2023, max compression
+gzip compressed data, was "dist/betconnect-0.1.7.tar", last modified: Fri Jun 16 06:24:18 2023, max compression
```

## Comparing `betconnect-0.1.6.tar` & `betconnect-0.1.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-02-15 16:22:56.000000 betconnect-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-02-15 16:22:37.000000 betconnect-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/betconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/betconnect/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/endpoints/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/endpoints/baseendpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/endpoints/betting.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/betconnect/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/resources/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/resources/baseresource.py
--rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/resources/betting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/resources/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/resources/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-02-15 16:22:37.000000 betconnect-0.1.6/betconnect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/betconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-02-15 16:22:55.000000 betconnect-0.1.6/betconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-02-15 16:22:56.000000 betconnect-0.1.6/betconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 16:22:55.000000 betconnect-0.1.6/betconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-15 16:22:55.000000 betconnect-0.1.6/betconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-15 16:22:55.000000 betconnect-0.1.6/betconnect.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/bettinghistory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/bookpercentage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/dailyhorseracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/datarequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/football.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/handicap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/stopactivebetrequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-15 16:22:37.000000 betconnect-0.1.6/examples/viewactivemarketbets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 16:22:56.000000 betconnect-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-15 16:22:37.000000 betconnect-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29975 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/resources/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/resources/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/resources/endpoints/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/resources/endpoints/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/resources/endpoints/betting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/resources/endpoints/betting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/unit/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/unit/endpoints/test_account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/endpoints/test_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/endpoints/test_account/test_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/unit/endpoints/test_betting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/endpoints/test_betting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/endpoints/test_betting/test_betting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/unit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/unit/resources/test_accountresources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/resources/test_accountresources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/resources/test_accountresources/test_accountresources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/unit/resources/test_bettingresources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/resources/test_bettingresources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/resources/test_bettingresources/test_bettingresources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:56.000000 betconnect-0.1.6/tests/unit/resources/test_filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/resources/test_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/resources/test_filters/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/test_apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/test_baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-15 16:22:37.000000 betconnect-0.1.6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-16 06:24:18.000000 betconnect-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-16 06:23:55.000000 betconnect-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/endpoints/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/endpoints/baseendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/endpoints/betting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/resources/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/resources/baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/resources/betting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/resources/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/resources/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-16 06:23:55.000000 betconnect-0.1.7/betconnect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 06:24:18.000000 betconnect-0.1.7/betconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/bettinghistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/bookpercentage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/dailyhorseracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/datarequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/football.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/handicap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/stopactivebetrequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-16 06:23:55.000000 betconnect-0.1.7/examples/viewactivemarketbets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:24:18.000000 betconnect-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-16 06:23:55.000000 betconnect-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29975 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/resources/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/resources/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/resources/endpoints/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/resources/endpoints/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/resources/endpoints/betting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/resources/endpoints/betting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/unit/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/unit/endpoints/test_account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/endpoints/test_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/endpoints/test_account/test_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/unit/endpoints/test_betting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/endpoints/test_betting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/endpoints/test_betting/test_betting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/unit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/unit/resources/test_accountresources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/resources/test_accountresources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/resources/test_accountresources/test_accountresources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/unit/resources/test_bettingresources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/resources/test_bettingresources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/resources/test_bettingresources/test_bettingresources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:24:18.000000 betconnect-0.1.7/tests/unit/resources/test_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/resources/test_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/resources/test_filters/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/test_apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/test_baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-16 06:23:55.000000 betconnect-0.1.7/tests/utils.py
```

### Comparing `betconnect-0.1.6/PKG-INFO` & `betconnect-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betconnect
-Version: 0.1.6
+Version: 0.1.7
 Summary: A betconnect API client
 Home-page: https://github.com/betcode-org/betconnect
 Author: Oliver Varney
 Author-email: oliverashleyvarney@gmail.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: betconnect Version: 0.1.6 Summary: A betconnect API
+Metadata-Version: 2.1 Name: betconnect Version: 0.1.7 Summary: A betconnect API
 client Home-page: https://github.com/betcode-org/betconnect Author: Oliver
 Varney Author-email: oliverashleyvarney@gmail.com License: MIT Description:
                           [docs/images/logo-full.png]
 ![Build Status](https://github.com/betcode-org/betconnect/actions/workflows/
 test.yml/badge.svg) [![PyPI version](https://badge.fury.io/py/betconnect.svg)]
 (https://pypi.python.org/pypi/betconnect) [![Downloads](https://pepy.tech/
 badge/betconnect)](https://pepy.tech/project/betconnect) # betconnect Simple
```

### Comparing `betconnect-0.1.6/README.md` & `betconnect-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/__init__.py` & `betconnect-0.1.7/betconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/apiclient.py` & `betconnect-0.1.7/betconnect/apiclient.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/baseclient.py` & `betconnect-0.1.7/betconnect/baseclient.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/endpoints/account.py` & `betconnect-0.1.7/betconnect/endpoints/account.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/endpoints/baseendpoint.py` & `betconnect-0.1.7/betconnect/endpoints/baseendpoint.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/endpoints/betting.py` & `betconnect-0.1.7/betconnect/endpoints/betting.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/enums.py` & `betconnect-0.1.7/betconnect/enums.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/exceptions.py` & `betconnect-0.1.7/betconnect/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,18 +136,15 @@
     """
 
     def __init__(self, stake_size: int):
         super(BetRequestIDStakeSizeException, self).__init__(stake_size)
         self.stake_size = stake_size
 
     def __str__(self) -> str:
-        return (
-            f"Supplied stake size {self.stake_size} is not a multiple of {config.SITE_STAKE_SIZE_MULTIPLE_REQUIREMENT} "
-            f"greater than the site minimum of {config.SITE_MINIMUM_STAKE_SIZE}"
-        )
+        return f"Supplied stake size {self.stake_size} is not greater than the site minimum of {config.SITE_MINIMUM_STAKE_SIZE}"
 
 
 class BetRequestInvalidCustomerOrderRefFormatException(BetConnectException):
     """
     raised when customer order ref is not between 1-36 character in length
     """
```

### Comparing `betconnect-0.1.6/betconnect/resources/__init__.py` & `betconnect-0.1.7/betconnect/resources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,12 +25,18 @@
     MyBetsBets,
     BetRequestStop,
     CustomerOrderRef,
     CustomerStrategyRef,
     LockBet,
     LineMarketsSelectionsForMarket,
 )
-from .filters import Filter, GetBetRequestFilter, CreateBetRequestFilter
+from .filters import (
+    Filter,
+    GetBetRequestFilter,
+    CreateBetRequestBySelectionFilter,
+    CreateBetRequestByCompetitorFilter,
+    CreateBetRequestFilter,
+)
 
 from .account import Login, Token, AccountPreferences
 
 from .messages import BaseRequestException, ResponseMessage
```

### Comparing `betconnect-0.1.6/betconnect/resources/account.py` & `betconnect-0.1.7/betconnect/resources/account.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/resources/baseresource.py` & `betconnect-0.1.7/betconnect/resources/baseresource.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/resources/betting.py` & `betconnect-0.1.7/betconnect/resources/betting.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect/utils.py` & `betconnect-0.1.7/betconnect/utils.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/betconnect.egg-info/PKG-INFO` & `betconnect-0.1.7/betconnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betconnect
-Version: 0.1.6
+Version: 0.1.7
 Summary: A betconnect API client
 Home-page: https://github.com/betcode-org/betconnect
 Author: Oliver Varney
 Author-email: oliverashleyvarney@gmail.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: betconnect Version: 0.1.6 Summary: A betconnect API
+Metadata-Version: 2.1 Name: betconnect Version: 0.1.7 Summary: A betconnect API
 client Home-page: https://github.com/betcode-org/betconnect Author: Oliver
 Varney Author-email: oliverashleyvarney@gmail.com License: MIT Description:
                           [docs/images/logo-full.png]
 ![Build Status](https://github.com/betcode-org/betconnect/actions/workflows/
 test.yml/badge.svg) [![PyPI version](https://badge.fury.io/py/betconnect.svg)]
 (https://pypi.python.org/pypi/betconnect) [![Downloads](https://pepy.tech/
 badge/betconnect)](https://pepy.tech/project/betconnect) # betconnect Simple
```

### Comparing `betconnect-0.1.6/betconnect.egg-info/SOURCES.txt` & `betconnect-0.1.7/betconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/account.py` & `betconnect-0.1.7/examples/account.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/bettinghistory.py` & `betconnect-0.1.7/examples/bettinghistory.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/bookpercentage.py` & `betconnect-0.1.7/examples/bookpercentage.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/dailyhorseracing.py` & `betconnect-0.1.7/examples/dailyhorseracing.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/datarequests.py` & `betconnect-0.1.7/examples/datarequests.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/football.py` & `betconnect-0.1.7/examples/football.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/handicap.py` & `betconnect-0.1.7/examples/handicap.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/stopactivebetrequest.py` & `betconnect-0.1.7/examples/stopactivebetrequest.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/examples/viewactivemarketbets.py` & `betconnect-0.1.7/examples/viewactivemarketbets.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/setup.py` & `betconnect-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/conftest.py` & `betconnect-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/unit/endpoints/test_account/test_account.py` & `betconnect-0.1.7/tests/unit/endpoints/test_account/test_account.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/unit/endpoints/test_betting/test_betting.py` & `betconnect-0.1.7/tests/unit/endpoints/test_betting/test_betting.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/unit/resources/test_accountresources/test_accountresources.py` & `betconnect-0.1.7/tests/unit/resources/test_accountresources/test_accountresources.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/unit/resources/test_bettingresources/test_bettingresources.py` & `betconnect-0.1.7/tests/unit/resources/test_bettingresources/test_bettingresources.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/unit/resources/test_filters/test_filters.py` & `betconnect-0.1.7/tests/unit/resources/test_filters/test_filters.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,16 +28,62 @@
             resources.GetBetRequestFilter(
                 bet_request_id="c9bf9e575168554c895bafb5ff5af830be8a"
             )
         # test min odds validation
         with pytest.raises(exceptions.MinOddException):
             resources.GetBetRequestFilter(min_odds=1)
 
-    def test_create_bet_request_filter(self):
-        request_filter = resources.CreateBetRequestFilter(
+    def test_create_bet_request_by_selection_filter(self):
+        request_filter = resources.CreateBetRequestBySelectionFilter(
+            selection_id=123,
+            price=10,
+            stake=50,
+            bet_type="WIN",
+        )
+        assert request_filter.selection_id == 123
+        assert request_filter.price == 10
+        assert request_filter.stake == 50
+        assert request_filter.bet_type == "WIN"
+        assert request_filter.handicap is None
+        assert request_filter.customer_strategy_ref is None
+        assert request_filter.customer_order_ref is None
+
+        # test min stake validation
+        with pytest.raises(exceptions.BetRequestIDStakeSizeException):
+            resources.CreateBetRequestBySelectionFilter(
+                selection_id=123,
+                price=10,
+                stake=0.99,
+                bet_type="WIN",
+            )
+
+        # test customer_strategy_ref length
+        with pytest.raises(
+            exceptions.BetRequestInvalidCustomerStrategyRefFormatException
+        ):
+            resources.CreateBetRequestBySelectionFilter(
+                selection_id=123,
+                price=10,
+                stake=10,
+                bet_type="WIN",
+                customer_strategy_ref="11111111111111111111111111111111111",
+            )
+
+        # test validate_customer_order_ref length
+        with pytest.raises(exceptions.BetRequestInvalidCustomerOrderRefFormatException):
+            resources.CreateBetRequestBySelectionFilter(
+                selection_id=123,
+                price=10,
+                stake=10,
+                bet_type="WIN",
+                customer_order_ref="1111111111111111111111111111111111111111111111111111",
+            )
+
+    def test_create_bet_request_by_competitor_filter(self):
+        request_filter = resources.CreateBetRequestByCompetitorFilter(
             fixture_id=1,
             market_type_id=1,
             competitor="123",
             price=10,
             stake=50,
             bet_type="WIN",
         )
@@ -49,52 +95,61 @@
         assert request_filter.bet_type == "WIN"
         assert request_filter.handicap is None
         assert request_filter.customer_strategy_ref is None
         assert request_filter.customer_order_ref is None
 
         # test min stake validation
         with pytest.raises(exceptions.BetRequestIDStakeSizeException):
-            resources.CreateBetRequestFilter(
-                fixture_id=1,
-                market_type_id=1,
-                competitor="123",
-                price=10,
-                stake=4,
-                bet_type="WIN",
-            )
-
-        # test stake multiple validation
-        with pytest.raises(exceptions.BetRequestIDStakeSizeException):
-            resources.CreateBetRequestFilter(
+            resources.CreateBetRequestByCompetitorFilter(
                 fixture_id=1,
                 market_type_id=1,
                 competitor="123",
                 price=10,
-                stake=11,
+                stake=0.99,
                 bet_type="WIN",
             )
 
         # test customer_strategy_ref length
         with pytest.raises(
             exceptions.BetRequestInvalidCustomerStrategyRefFormatException
         ):
-            resources.CreateBetRequestFilter(
+            resources.CreateBetRequestByCompetitorFilter(
                 fixture_id=1,
                 market_type_id=1,
                 competitor="123",
                 price=10,
                 stake=10,
                 bet_type="WIN",
                 customer_strategy_ref="11111111111111111111111111111111111",
             )
 
         # test validate_customer_order_ref length
         with pytest.raises(exceptions.BetRequestInvalidCustomerOrderRefFormatException):
-            resources.CreateBetRequestFilter(
+            resources.CreateBetRequestByCompetitorFilter(
                 fixture_id=1,
                 market_type_id=1,
                 competitor="123",
                 price=10,
                 stake=10,
                 bet_type="WIN",
                 customer_order_ref="1111111111111111111111111111111111111111111111111111",
             )
+
+    def test_create_bet_request_filter_alias_working(self):
+        request_filter = resources.CreateBetRequestFilter(
+            fixture_id=1,
+            market_type_id=1,
+            competitor="123",
+            price=10,
+            stake=50,
+            bet_type="WIN",
+        )
+        assert request_filter.fixture_id == 1
+        assert request_filter.market_type_id == 1
+        assert request_filter.competitor == "123"
+        assert request_filter.price == 10
+        assert request_filter.stake == 50
+        assert request_filter.bet_type == "WIN"
+        assert request_filter.handicap is None
+        assert request_filter.customer_strategy_ref is None
+        assert request_filter.customer_order_ref is None
+        assert isinstance(request_filter, resources.CreateBetRequestByCompetitorFilter)
```

### Comparing `betconnect-0.1.6/tests/unit/test_apiclient.py` & `betconnect-0.1.7/tests/unit/test_apiclient.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/unit/test_baseclient.py` & `betconnect-0.1.7/tests/unit/test_baseclient.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/unit/test_exceptions.py` & `betconnect-0.1.7/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/unit/test_utils.py` & `betconnect-0.1.7/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `betconnect-0.1.6/tests/utils.py` & `betconnect-0.1.7/tests/utils.py`

 * *Files identical despite different names*

