# Comparing `tmp/frosty-dag-0.0.1.tar.gz` & `tmp/frosty-dag-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frosty-dag-0.0.1.tar", last modified: Fri Jun 16 01:28:12 2023, max compression
+gzip compressed data, was "frosty-dag-0.0.2.tar", last modified: Fri Jun 16 01:52:06 2023, max compression
```

## Comparing `frosty-dag-0.0.1.tar` & `frosty-dag-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joshuabang   (501) staff       (20)        0 2023-06-16 01:28:12.278700 frosty-dag-0.0.1/
--rw-r--r--   0 joshuabang   (501) staff       (20)    35149 2023-06-16 01:18:33.000000 frosty-dag-0.0.1/LICENSE
--rw-r--r--   0 joshuabang   (501) staff       (20)      309 2023-06-16 01:28:12.278566 frosty-dag-0.0.1/PKG-INFO
--rw-r--r--   0 joshuabang   (501) staff       (20)      847 2023-06-16 01:22:41.000000 frosty-dag-0.0.1/README.md
-drwxr-xr-x   0 joshuabang   (501) staff       (20)        0 2023-06-16 01:28:12.277744 frosty-dag-0.0.1/frosty/
--rw-r--r--   0 joshuabang   (501) staff       (20)       21 2023-06-16 01:18:33.000000 frosty-dag-0.0.1/frosty/__init__.py
--rw-r--r--   0 joshuabang   (501) staff       (20)     1603 2023-06-16 01:18:33.000000 frosty-dag-0.0.1/frosty/frosty.py
-drwxr-xr-x   0 joshuabang   (501) staff       (20)        0 2023-06-16 01:28:12.278408 frosty-dag-0.0.1/frosty_dag.egg-info/
--rw-r--r--   0 joshuabang   (501) staff       (20)      309 2023-06-16 01:28:12.000000 frosty-dag-0.0.1/frosty_dag.egg-info/PKG-INFO
--rw-r--r--   0 joshuabang   (501) staff       (20)      231 2023-06-16 01:28:12.000000 frosty-dag-0.0.1/frosty_dag.egg-info/SOURCES.txt
--rw-r--r--   0 joshuabang   (501) staff       (20)        1 2023-06-16 01:28:12.000000 frosty-dag-0.0.1/frosty_dag.egg-info/dependency_links.txt
--rw-r--r--   0 joshuabang   (501) staff       (20)       65 2023-06-16 01:28:12.000000 frosty-dag-0.0.1/frosty_dag.egg-info/requires.txt
--rw-r--r--   0 joshuabang   (501) staff       (20)        7 2023-06-16 01:28:12.000000 frosty-dag-0.0.1/frosty_dag.egg-info/top_level.txt
--rw-r--r--   0 joshuabang   (501) staff       (20)       38 2023-06-16 01:28:12.278740 frosty-dag-0.0.1/setup.cfg
--rw-r--r--   0 joshuabang   (501) staff       (20)      505 2023-06-16 01:18:58.000000 frosty-dag-0.0.1/setup.py
+drwxr-xr-x   0 joshuabang   (501) staff       (20)        0 2023-06-16 01:52:06.115955 frosty-dag-0.0.2/
+-rw-r--r--   0 joshuabang   (501) staff       (20)    35149 2023-06-16 01:18:33.000000 frosty-dag-0.0.2/LICENSE
+-rw-r--r--   0 joshuabang   (501) staff       (20)     1234 2023-06-16 01:52:06.115808 frosty-dag-0.0.2/PKG-INFO
+-rw-r--r--   0 joshuabang   (501) staff       (20)      847 2023-06-16 01:22:41.000000 frosty-dag-0.0.2/README.md
+drwxr-xr-x   0 joshuabang   (501) staff       (20)        0 2023-06-16 01:52:06.115033 frosty-dag-0.0.2/frosty/
+-rw-r--r--   0 joshuabang   (501) staff       (20)       21 2023-06-16 01:18:33.000000 frosty-dag-0.0.2/frosty/__init__.py
+-rw-r--r--   0 joshuabang   (501) staff       (20)     1603 2023-06-16 01:18:33.000000 frosty-dag-0.0.2/frosty/frosty.py
+drwxr-xr-x   0 joshuabang   (501) staff       (20)        0 2023-06-16 01:52:06.115635 frosty-dag-0.0.2/frosty_dag.egg-info/
+-rw-r--r--   0 joshuabang   (501) staff       (20)     1234 2023-06-16 01:52:05.000000 frosty-dag-0.0.2/frosty_dag.egg-info/PKG-INFO
+-rw-r--r--   0 joshuabang   (501) staff       (20)      231 2023-06-16 01:52:06.000000 frosty-dag-0.0.2/frosty_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuabang   (501) staff       (20)        1 2023-06-16 01:52:05.000000 frosty-dag-0.0.2/frosty_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuabang   (501) staff       (20)       65 2023-06-16 01:52:05.000000 frosty-dag-0.0.2/frosty_dag.egg-info/requires.txt
+-rw-r--r--   0 joshuabang   (501) staff       (20)        7 2023-06-16 01:52:06.000000 frosty-dag-0.0.2/frosty_dag.egg-info/top_level.txt
+-rw-r--r--   0 joshuabang   (501) staff       (20)       38 2023-06-16 01:52:06.116001 frosty-dag-0.0.2/setup.cfg
+-rw-r--r--   0 joshuabang   (501) staff       (20)      664 2023-06-16 01:50:24.000000 frosty-dag-0.0.2/setup.py
```

### Comparing `frosty-dag-0.0.1/LICENSE` & `frosty-dag-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frosty-dag-0.0.1/README.md` & `frosty-dag-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `frosty-dag-0.0.1/frosty/frosty.py` & `frosty-dag-0.0.2/frosty/frosty.py`

 * *Files identical despite different names*

