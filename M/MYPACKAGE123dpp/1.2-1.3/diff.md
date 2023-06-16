# Comparing `tmp/MYPACKAGE123dpp-1.2.tar.gz` & `tmp/MYPACKAGE123dpp-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MYPACKAGE123dpp-1.2.tar", last modified: Fri Jun 16 19:03:03 2023, max compression
+gzip compressed data, was "MYPACKAGE123dpp-1.3.tar", last modified: Fri Jun 16 19:21:21 2023, max compression
```

## Comparing `MYPACKAGE123dpp-1.2.tar` & `MYPACKAGE123dpp-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 19:03:03.578400 MYPACKAGE123dpp-1.2/
-drwxrwxrwx   0        0        0        0 2023-06-16 19:03:03.556437 MYPACKAGE123dpp-1.2/FirstApi/
--rw-rw-rw-   0        0        0      531 2023-06-16 19:02:11.000000 MYPACKAGE123dpp-1.2/FirstApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 19:03:03.574442 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/
--rw-rw-rw-   0        0        0      124 2023-06-16 19:03:03.000000 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-06-16 19:03:03.000000 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 19:03:03.000000 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-16 19:03:03.000000 MYPACKAGE123dpp-1.2/MYPACKAGE123dpp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2023-06-16 19:03:03.577444 MYPACKAGE123dpp-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 19:03:03.575430 MYPACKAGE123dpp-1.2/SecondApi/
--rw-rw-rw-   0        0        0      462 2023-06-16 18:57:41.000000 MYPACKAGE123dpp-1.2/SecondApi/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-16 19:03:03.578400 MYPACKAGE123dpp-1.2/setup.cfg
--rw-rw-rw-   0        0        0      220 2023-06-16 18:48:58.000000 MYPACKAGE123dpp-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:21:21.024198 MYPACKAGE123dpp-1.3/
+drwxrwxrwx   0        0        0        0 2023-06-16 19:21:21.013198 MYPACKAGE123dpp-1.3/FirstApi/
+-rw-rw-rw-   0        0        0     1017 2023-06-16 19:19:39.000000 MYPACKAGE123dpp-1.3/FirstApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:21:21.020235 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-06-16 19:21:20.000000 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-06-16 19:21:20.000000 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:21:20.000000 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-16 19:21:20.000000 MYPACKAGE123dpp-1.3/MYPACKAGE123dpp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      212 2023-06-16 19:21:21.023199 MYPACKAGE123dpp-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 19:21:21.022233 MYPACKAGE123dpp-1.3/SecondApi/
+-rw-rw-rw-   0        0        0     1069 2023-06-16 19:19:53.000000 MYPACKAGE123dpp-1.3/SecondApi/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 19:21:21.024198 MYPACKAGE123dpp-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      220 2023-06-16 19:20:22.000000 MYPACKAGE123dpp-1.3/setup.py
```

