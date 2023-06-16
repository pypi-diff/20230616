# Comparing `tmp/smpgpt-1.0.tar.gz` & `tmp/smpgpt-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpgpt-1.0.tar", last modified: Fri Jun 16 20:45:08 2023, max compression
+gzip compressed data, was "smpgpt-3.0.tar", last modified: Fri Jun 16 20:55:10 2023, max compression
```

## Comparing `smpgpt-1.0.tar` & `smpgpt-3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:45:08.293337 smpgpt-1.0/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 20:45:08.293149 smpgpt-1.0/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-1.0/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-16 20:45:08.293389 smpgpt-1.0/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-16 20:44:39.000000 smpgpt-1.0/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:45:08.291360 smpgpt-1.0/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:45:08.292135 smpgpt-1.0/src/smper/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-1.0/src/smper/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     1485 2023-06-16 20:41:03.000000 smpgpt-1.0/src/smper/smper.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:45:08.292947 smpgpt-1.0/src/smpgpt.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 20:45:08.000000 smpgpt-1.0/src/smpgpt.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      228 2023-06-16 20:45:08.000000 smpgpt-1.0/src/smpgpt.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-1.0/src/smpgpt.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-1.0/src/smpgpt.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-16 20:45:08.000000 smpgpt-1.0/src/smpgpt.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:55:10.753975 smpgpt-3.0/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 20:55:10.753798 smpgpt-3.0/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-3.0/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-16 20:55:10.754051 smpgpt-3.0/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-16 20:55:07.000000 smpgpt-3.0/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:55:10.751820 smpgpt-3.0/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:55:10.752564 smpgpt-3.0/src/smpgpt/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-3.0/src/smpgpt/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     1736 2023-06-16 20:54:42.000000 smpgpt-3.0/src/smpgpt/smpgpt.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:55:10.753569 smpgpt-3.0/src/smpgpt.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 20:55:10.000000 smpgpt-3.0/src/smpgpt.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-16 20:55:10.000000 smpgpt-3.0/src/smpgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:55:10.000000 smpgpt-3.0/src/smpgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-3.0/src/smpgpt.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-16 20:55:10.000000 smpgpt-3.0/src/smpgpt.egg-info/top_level.txt
```

