# Comparing `tmp/numerical_py-0.0.9.tar.gz` & `tmp/numerical_py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerical_py-0.0.9.tar", last modified: Thu Jun 15 09:41:59 2023, max compression
+gzip compressed data, was "numerical_py-1.0.0.tar", last modified: Thu Jun 15 23:24:55 2023, max compression
```

## Comparing `numerical_py-0.0.9.tar` & `numerical_py-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:41:59.390175 numerical_py-0.0.9/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:41:59.390175 numerical_py-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 09:41:59.390175 numerical_py-0.0.9/numerical_py.egg-info/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:41:59.000000 numerical_py-0.0.9/numerical_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-06-15 09:41:59.000000 numerical_py-0.0.9/numerical_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:41:59.000000 numerical_py-0.0.9/numerical_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:41:59.000000 numerical_py-0.0.9/numerical_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 09:41:59.390175 numerical_py-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-06-15 09:41:56.000000 numerical_py-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 23:24:55.410183 numerical_py-1.0.0/
+-rw-rw-rw-   0        0        0      144 2023-06-15 23:24:55.399184 numerical_py-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 23:24:55.392184 numerical_py-1.0.0/numerical_py/
+-rw-rw-rw-   0        0        0      277 2023-06-15 23:19:21.000000 numerical_py-1.0.0/numerical_py/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-15 21:14:08.000000 numerical_py-1.0.0/numerical_py/derivative.py
+-rw-rw-rw-   0        0        0     1126 2023-06-15 21:13:57.000000 numerical_py-1.0.0/numerical_py/differentional.py
+-rw-rw-rw-   0        0        0     1533 2023-06-15 21:59:45.000000 numerical_py-1.0.0/numerical_py/eigenvals.py
+-rw-rw-rw-   0        0        0     5994 2023-06-15 23:23:32.000000 numerical_py-1.0.0/numerical_py/equations.py
+-rw-rw-rw-   0        0        0     3763 2023-06-15 21:59:48.000000 numerical_py-1.0.0/numerical_py/integrals.py
+-rw-rw-rw-   0        0        0     1589 2023-06-15 22:35:42.000000 numerical_py-1.0.0/numerical_py/interpolation.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:55:38.000000 numerical_py-1.0.0/numerical_py/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 23:24:55.399184 numerical_py-1.0.0/numerical_py.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-06-15 23:24:55.000000 numerical_py-1.0.0/numerical_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-06-15 23:24:55.000000 numerical_py-1.0.0/numerical_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 23:24:55.000000 numerical_py-1.0.0/numerical_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 23:24:55.000000 numerical_py-1.0.0/numerical_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 23:24:55.411185 numerical_py-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      240 2023-06-15 23:24:44.000000 numerical_py-1.0.0/setup.py
```

