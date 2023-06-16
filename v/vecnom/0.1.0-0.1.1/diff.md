# Comparing `tmp/vecnom-0.1.0.tar.gz` & `tmp/vecnom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecnom-0.1.0.tar", max compression
+gzip compressed data, was "vecnom-0.1.1.tar", max compression
```

## Comparing `vecnom-0.1.0.tar` & `vecnom-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      292 2023-06-16 09:45:09.205407 vecnom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.0/vecnom.py
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-06-16 09:58:34.251326 vecnom-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.1/vecnom.py
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.1/PKG-INFO
```

