# Comparing `tmp/MYPACKAGE123dpp-1.1.tar.gz` & `tmp/MYPACKAGE123dpp-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MYPACKAGE123dpp-1.1.tar", last modified: Tue Jun  6 20:04:01 2023, max compression
+gzip compressed data, was "MYPACKAGE123dpp-1.2.tar", last modified: Fri Jun 16 19:03:03 2023, max compression
```

## Comparing `MYPACKAGE123dpp-1.1.tar` & `MYPACKAGE123dpp-1.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 20:04:01.652594 MYPACKAGE123dpp-1.1/
-drwxrwxrwx   0        0        0        0 2023-06-06 20:04:01.648594 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/
--rw-rw-rw-   0        0        0      131 2023-06-06 20:04:01.000000 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-06-06 20:04:01.000000 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 20:04:01.000000 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 20:04:01.000000 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2023-06-06 20:04:01.651594 MYPACKAGE123dpp-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 20:04:01.650596 MYPACKAGE123dpp-1.1/TranslateApi/
--rw-rw-rw-   0        0        0      902 2023-06-06 20:03:44.000000 MYPACKAGE123dpp-1.1/TranslateApi/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-06 20:04:01.652594 MYPACKAGE123dpp-1.1/setup.cfg
--rw-rw-rw-   0        0        0      227 2023-06-06 20:03:04.000000 MYPACKAGE123dpp-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:03:03.578400 MYPACKAGE123dpp-1.2/
+drwxrwxrwx   0        0        0        0 2023-06-16 19:03:03.556437 MYPACKAGE123dpp-1.2/FirstApi/
+-rw-rw-rw-   0        0        0      531 2023-06-16 19:02:11.000000 MYPACKAGE123dpp-1.2/FirstApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:03:03.574442 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/
+-rw-rw-rw-   0        0        0      124 2023-06-16 19:03:03.000000 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-06-16 19:03:03.000000 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:03:03.000000 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-16 19:03:03.000000 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2023-06-16 19:03:03.577444 MYPACKAGE123dpp-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 19:03:03.575430 MYPACKAGE123dpp-1.2/SecondApi/
+-rw-rw-rw-   0        0        0      462 2023-06-16 18:57:41.000000 MYPACKAGE123dpp-1.2/SecondApi/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 19:03:03.578400 MYPACKAGE123dpp-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      220 2023-06-16 18:48:58.000000 MYPACKAGE123dpp-1.2/setup.py
```

