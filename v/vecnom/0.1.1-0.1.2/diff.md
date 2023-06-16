# Comparing `tmp/vecnom-0.1.1.tar.gz` & `tmp/vecnom-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecnom-0.1.1.tar", max compression
+gzip compressed data, was "vecnom-0.1.2.tar", max compression
```

## Comparing `vecnom-0.1.1.tar` & `vecnom-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,20 @@
--rw-r--r--   0        0        0      292 2023-06-16 09:58:34.251326 vecnom-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.1/vecnom.py
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2023-06-16 09:59:20.237400 vecnom-0.1.2/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253579 vecnom-0.1.2/README.md
+-rw-r--r--   0        0        0     1182 2023-06-10 10:14:19.937272 vecnom-0.1.2/data_types.py
+-rw-r--r--   0        0        0     6148 2023-06-16 09:59:20.236332 vecnom-0.1.2/dist/.DS_Store
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.2/dist/vecnom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-06-16 09:45:09.205407 vecnom-0.1.2/dist/vecnom-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.2/dist/vecnom-0.1.0/vecnom.py
+-rw-r--r--   0        0        0     1217 2023-06-16 09:57:54.791790 vecnom-0.1.2/dist/vecnom-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0      805 2023-06-16 09:57:54.737629 vecnom-0.1.2/dist/vecnom-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1216 2023-06-16 09:58:47.459517 vecnom-0.1.2/dist/vecnom-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0      805 2023-06-16 09:58:47.420965 vecnom-0.1.2/dist/vecnom-0.1.1.tar.gz
+-rw-r--r--   0        0        0     3202 2023-06-16 10:05:11.495380 vecnom-0.1.2/dist/vecnom-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0        0 2023-06-16 10:05:20.076700 vecnom-0.1.2/dist/vecnom-0.1.2.tar.gz
+-rw-r--r--   0        0        0      310 2023-06-16 10:05:02.757433 vecnom-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      460 2023-06-16 09:39:27.658274 vecnom-0.1.2/test.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253656 vecnom-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.2/vecnom.py
+-rw-r--r--   0        0        0     6148 2023-06-16 09:20:41.063109 vecnom-0.1.2/vecnom_/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253531 vecnom-0.1.2/vecnom_/__init__.py
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.2/PKG-INFO
```

