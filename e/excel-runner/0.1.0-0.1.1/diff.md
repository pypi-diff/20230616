# Comparing `tmp/excel-runner-0.1.0.tar.gz` & `tmp/excel-runner-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-runner-0.1.0.tar", last modified: Fri Jun 16 14:33:50 2023, max compression
+gzip compressed data, was "excel-runner-0.1.1.tar", last modified: Fri Jun 16 14:36:47 2023, max compression
```

## Comparing `excel-runner-0.1.0.tar` & `excel-runner-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-16 14:33:50.955408 excel-runner-0.1.0/
--rw-r--r--   0 superhin   (502) staff       (20)      173 2023-06-16 14:33:50.955098 excel-runner-0.1.0/PKG-INFO
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-16 14:33:50.950115 excel-runner-0.1.0/excel_runner/
--rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-16 13:55:27.000000 excel-runner-0.1.0/excel_runner/__init__.py
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-16 14:33:50.954347 excel-runner-0.1.0/excel_runner/lib/
--rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-16 14:05:58.000000 excel-runner-0.1.0/excel_runner/lib/__init__.py
--rw-r--r--   0 superhin   (502) staff       (20)       14 2023-06-16 14:16:30.000000 excel-runner-0.1.0/excel_runner/lib/a.txt
--rw-r--r--   0 superhin   (502) staff       (20)      184 2023-06-16 14:24:47.000000 excel-runner-0.1.0/excel_runner/lib/calc.py
--rw-r--r--   0 superhin   (502) staff       (20)      489 2023-06-16 14:03:17.000000 excel-runner-0.1.0/excel_runner/runner.py
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-16 14:33:50.952792 excel-runner-0.1.0/excel_runner.egg-info/
--rw-r--r--   0 superhin   (502) staff       (20)      173 2023-06-16 14:33:50.000000 excel-runner-0.1.0/excel_runner.egg-info/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)      312 2023-06-16 14:33:50.000000 excel-runner-0.1.0/excel_runner.egg-info/SOURCES.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-16 14:33:50.000000 excel-runner-0.1.0/excel_runner.egg-info/dependency_links.txt
--rw-r--r--   0 superhin   (502) staff       (20)        9 2023-06-16 14:33:50.000000 excel-runner-0.1.0/excel_runner.egg-info/requires.txt
--rw-r--r--   0 superhin   (502) staff       (20)       13 2023-06-16 14:33:50.000000 excel-runner-0.1.0/excel_runner.egg-info/top_level.txt
--rw-r--r--   0 superhin   (502) staff       (20)       38 2023-06-16 14:33:50.955549 excel-runner-0.1.0/setup.cfg
--rw-r--r--   0 superhin   (502) staff       (20)      381 2023-06-16 14:28:19.000000 excel-runner-0.1.0/setup.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-16 14:36:47.060210 excel-runner-0.1.1/
+-rw-r--r--   0 superhin   (502) staff       (20)      173 2023-06-16 14:36:47.059809 excel-runner-0.1.1/PKG-INFO
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-16 14:36:47.054072 excel-runner-0.1.1/excel_runner/
+-rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-16 13:55:27.000000 excel-runner-0.1.1/excel_runner/__init__.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-16 14:36:47.058917 excel-runner-0.1.1/excel_runner/lib/
+-rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-16 14:05:58.000000 excel-runner-0.1.1/excel_runner/lib/__init__.py
+-rw-r--r--   0 superhin   (502) staff       (20)       14 2023-06-16 14:16:30.000000 excel-runner-0.1.1/excel_runner/lib/a.txt
+-rw-r--r--   0 superhin   (502) staff       (20)      184 2023-06-16 14:24:47.000000 excel-runner-0.1.1/excel_runner/lib/calc.py
+-rw-r--r--   0 superhin   (502) staff       (20)      489 2023-06-16 14:03:17.000000 excel-runner-0.1.1/excel_runner/runner.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-16 14:36:47.057055 excel-runner-0.1.1/excel_runner.egg-info/
+-rw-r--r--   0 superhin   (502) staff       (20)      173 2023-06-16 14:36:46.000000 excel-runner-0.1.1/excel_runner.egg-info/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)      312 2023-06-16 14:36:46.000000 excel-runner-0.1.1/excel_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-16 14:36:46.000000 excel-runner-0.1.1/excel_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        9 2023-06-16 14:36:46.000000 excel-runner-0.1.1/excel_runner.egg-info/requires.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       13 2023-06-16 14:36:46.000000 excel-runner-0.1.1/excel_runner.egg-info/top_level.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       38 2023-06-16 14:36:47.060440 excel-runner-0.1.1/setup.cfg
+-rw-r--r--   0 superhin   (502) staff       (20)      381 2023-06-16 14:36:28.000000 excel-runner-0.1.1/setup.py
```

