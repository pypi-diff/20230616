# Comparing `tmp/biochatter-0.0.0.tar.gz` & `tmp/biochatter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biochatter-0.0.0.tar", max compression
+gzip compressed data, was "biochatter-0.1.1.tar", max compression
```

## Comparing `biochatter-0.0.0.tar` & `biochatter-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.0.0/LICENSE
--rw-r--r--   0        0        0      144 2023-06-13 11:11:07.914635 biochatter-0.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.0.0/biochatter/__init__.py
--rw-r--r--   0        0        0      359 2023-06-13 11:09:07.125313 biochatter-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 biochatter-0.0.0/setup.py
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 biochatter-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.1/LICENSE
+-rw-r--r--   0        0        0      144 2023-06-13 11:11:07.914635 biochatter-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.1/biochatter/__init__.py
+-rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.1/biochatter/_stats.py
+-rw-r--r--   0        0        0    12406 2023-06-16 16:40:08.854325 biochatter-0.1.1/biochatter/llm_connect.py
+-rw-r--r--   0        0        0     5226 2023-06-16 12:53:15.891015 biochatter-0.1.1/biochatter/vectorstore.py
+-rw-r--r--   0        0        0      532 2023-06-16 16:53:37.078917 biochatter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 biochatter-0.1.1/setup.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 biochatter-0.1.1/PKG-INFO
```

### Comparing `biochatter-0.0.0/LICENSE` & `biochatter-0.1.1/LICENSE`

 * *Files identical despite different names*

