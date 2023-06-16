# Comparing `tmp/blin-0.0.1.tar.gz` & `tmp/blin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blin-0.0.1.tar", last modified: Sat May 27 00:55:58 2023, max compression
+gzip compressed data, was "blin-0.1.0.tar", last modified: Fri Jun 16 01:01:15 2023, max compression
```

## Comparing `blin-0.0.1.tar` & `blin-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 00:55:58.200580 blin-0.0.1/
--rw-rw-rw-   0        0        0      187 2023-05-27 00:55:58.200580 blin-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-27 00:54:36.000000 blin-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 00:55:58.182577 blin-0.0.1/blin/
--rw-rw-rw-   0        0        0       32 2023-05-27 00:51:43.000000 blin-0.0.1/blin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:55:58.198579 blin-0.0.1/blin.egg-info/
--rw-rw-rw-   0        0        0      187 2023-05-27 00:55:58.000000 blin-0.0.1/blin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-27 00:55:58.000000 blin-0.0.1/blin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 00:55:58.000000 blin-0.0.1/blin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-27 00:55:58.000000 blin-0.0.1/blin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1063 2023-05-27 00:54:38.000000 blin-0.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 00:55:58.200580 blin-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      221 2023-05-27 00:49:24.000000 blin-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:01:15.681123 blin-0.1.0/
+-rw-rw-rw-   0        0        0      177 2023-06-16 01:01:15.680124 blin-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-27 00:54:36.000000 blin-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 01:01:15.659119 blin-0.1.0/blin/
+-rw-rw-rw-   0        0        0     5343 2023-06-15 23:33:53.000000 blin-0.1.0/blin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:01:15.679124 blin-0.1.0/blin.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-06-16 01:01:15.000000 blin-0.1.0/blin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-06-16 01:01:15.000000 blin-0.1.0/blin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 01:01:15.000000 blin-0.1.0/blin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-16 01:01:15.000000 blin-0.1.0/blin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1063 2023-05-27 00:54:38.000000 blin-0.1.0/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 01:01:15.681123 blin-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      211 2023-06-16 01:00:20.000000 blin-0.1.0/setup.py
```

### Comparing `blin-0.0.1/license.txt` & `blin-0.1.0/license.txt`

 * *Files identical despite different names*

