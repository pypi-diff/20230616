# Comparing `tmp/bn_keyword_extractor-1.0.1.tar.gz` & `tmp/bn_keyword_extractor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bn_keyword_extractor-1.0.1.tar", last modified: Fri Jun 16 07:28:47 2023, max compression
+gzip compressed data, was "bn_keyword_extractor-1.0.2.tar", last modified: Fri Jun 16 07:54:33 2023, max compression
```

## Comparing `bn_keyword_extractor-1.0.1.tar` & `bn_keyword_extractor-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:28:47.776596 bn_keyword_extractor-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-16 07:28:47.775596 bn_keyword_extractor-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-16 07:23:32.000000 bn_keyword_extractor-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:28:47.775596 bn_keyword_extractor-1.0.1/bn_keyword_extractor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-16 07:28:47.000000 bn_keyword_extractor-1.0.1/bn_keyword_extractor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-16 07:28:47.000000 bn_keyword_extractor-1.0.1/bn_keyword_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 07:28:47.000000 bn_keyword_extractor-1.0.1/bn_keyword_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-16 07:28:47.000000 bn_keyword_extractor-1.0.1/bn_keyword_extractor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 07:28:47.000000 bn_keyword_extractor-1.0.1/bn_keyword_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:28:47.775596 bn_keyword_extractor-1.0.1/keyword_extractor/
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-16 07:23:32.000000 bn_keyword_extractor-1.0.1/keyword_extractor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2822 2023-06-16 07:23:32.000000 bn_keyword_extractor-1.0.1/keyword_extractor/keyword_extractor.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 07:28:47.776596 bn_keyword_extractor-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-16 07:23:32.000000 bn_keyword_extractor-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:54:33.363119 bn_keyword_extractor-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-16 07:54:33.363119 bn_keyword_extractor-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-16 07:53:52.000000 bn_keyword_extractor-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:54:33.362119 bn_keyword_extractor-1.0.2/bn_keyword_extractor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-16 07:54:33.000000 bn_keyword_extractor-1.0.2/bn_keyword_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-16 07:54:33.000000 bn_keyword_extractor-1.0.2/bn_keyword_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 07:54:33.000000 bn_keyword_extractor-1.0.2/bn_keyword_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-16 07:54:33.000000 bn_keyword_extractor-1.0.2/bn_keyword_extractor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 07:54:33.000000 bn_keyword_extractor-1.0.2/bn_keyword_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:54:33.363119 bn_keyword_extractor-1.0.2/keyword_extractor/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-16 07:53:52.000000 bn_keyword_extractor-1.0.2/keyword_extractor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-06-16 07:53:52.000000 bn_keyword_extractor-1.0.2/keyword_extractor/keyword_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 07:54:33.363119 bn_keyword_extractor-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      518 2023-06-16 07:53:52.000000 bn_keyword_extractor-1.0.2/setup.py
```

### Comparing `bn_keyword_extractor-1.0.1/keyword_extractor/keyword_extractor.py` & `bn_keyword_extractor-1.0.2/keyword_extractor/keyword_extractor.py`

 * *Files identical despite different names*

