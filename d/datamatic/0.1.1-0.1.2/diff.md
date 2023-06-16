# Comparing `tmp/datamatic-0.1.1.tar.gz` & `tmp/datamatic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamatic-0.1.1.tar", max compression
+gzip compressed data, was "datamatic-0.1.2.tar", max compression
```

## Comparing `datamatic-0.1.1.tar` & `datamatic-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datamatic-0.1.1/LICENSE
--rw-r--r--   0        0        0     1389 2023-06-16 13:39:30.807722 datamatic-0.1.1/datamatic/__init__.py
--rw-r--r--   0        0        0      338 2023-06-16 12:59:32.220890 datamatic-0.1.1/datamatic/exceptions.py
--rw-r--r--   0        0        0      463 2023-06-16 13:40:44.698493 datamatic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 datamatic-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datamatic-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1650 2023-06-16 19:23:27.728215 datamatic-0.1.2/datamatic/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-16 12:59:32.220890 datamatic-0.1.2/datamatic/exceptions.py
+-rw-r--r--   0        0        0      463 2023-06-16 19:27:30.232475 datamatic-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 datamatic-0.1.2/PKG-INFO
```

### Comparing `datamatic-0.1.1/LICENSE` & `datamatic-0.1.2/LICENSE`

 * *Files identical despite different names*

