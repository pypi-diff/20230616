# Comparing `tmp/yunopyutils-0.1.0.tar.gz` & `tmp/yunopyutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunopyutils-0.1.0.tar", last modified: Fri Jun 16 19:48:29 2023, max compression
+gzip compressed data, was "yunopyutils-0.1.1.tar", last modified: Fri Jun 16 19:56:27 2023, max compression
```

## Comparing `yunopyutils-0.1.0.tar` & `yunopyutils-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2023-06-16 19:17:43.383888 yunopyutils-0.1.0/README.md
--rw-r--r--   0        0        0      543 2023-06-16 19:48:29.903174 yunopyutils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-16 19:26:11.035607 yunopyutils-0.1.0/src/logger/__init__.py
--rwxr-xr-x   0        0        0     3206 2023-06-16 19:22:26.604963 yunopyutils-0.1.0/src/logger/create_log.py
--rw-r--r--   0        0        0      274 1970-01-01 00:00:00.000000 yunopyutils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-06-16 19:17:43.383888 yunopyutils-0.1.1/README.md
+-rw-r--r--   0        0        0      489 2023-06-16 19:56:27.118617 yunopyutils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-16 19:26:11.035607 yunopyutils-0.1.1/src/logger/__init__.py
+-rwxr-xr-x   0        0        0     3206 2023-06-16 19:22:26.604963 yunopyutils-0.1.1/src/logger/create_log.py
+-rw-r--r--   0        0        0      274 1970-01-01 00:00:00.000000 yunopyutils-0.1.1/PKG-INFO
```

### Comparing `yunopyutils-0.1.0/src/logger/create_log.py` & `yunopyutils-0.1.1/src/logger/create_log.py`

 * *Files identical despite different names*

