# Comparing `tmp/mypackagez123g-1.2.0.tar.gz` & `tmp/mypackagez123g-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagez123g-1.2.0.tar", max compression
+gzip compressed data, was "mypackagez123g-2.0.0.tar", max compression
```

## Comparing `mypackagez123g-1.2.0.tar` & `mypackagez123g-2.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-12 22:06:49.726259 mypackagez123g-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 22:06:49.726259 mypackagez123g-1.2.0/mypackagez123g/__init__.py
--rw-r--r--   0        0        0      267 2023-06-12 22:07:04.318462 mypackagez123g-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 mypackagez123g-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-06-16 07:14:42.894529 mypackagez123g-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 07:14:42.898529 mypackagez123g-2.0.0/mypackagez123g/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-16 07:14:59.074745 mypackagez123g-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 mypackagez123g-2.0.0/PKG-INFO
```

