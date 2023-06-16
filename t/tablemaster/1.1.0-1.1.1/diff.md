# Comparing `tmp/tablemaster-1.1.0.tar.gz` & `tmp/tablemaster-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.1.0.tar", last modified: Thu Jun 15 08:46:37 2023, max compression
+gzip compressed data, was "tablemaster-1.1.1.tar", last modified: Fri Jun 16 08:50:16 2023, max compression
```

## Comparing `tablemaster-1.1.0.tar` & `tablemaster-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-15 08:46:37.625527 tablemaster-1.1.0/
--rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.1.0/LICENSE
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-06-15 08:46:37.625410 tablemaster-1.1.0/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)     1484 2023-05-24 06:49:43.000000 tablemaster-1.1.0/README.md
--rw-r--r--   0 livid      (501) staff       (20)       38 2023-06-15 08:46:37.625561 tablemaster-1.1.0/setup.cfg
--rw-r--r--   0 livid      (501) staff       (20)      559 2023-06-15 08:45:44.000000 tablemaster-1.1.0/setup.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-15 08:46:37.624624 tablemaster-1.1.0/tablemaster/
--rw-r--r--   0 livid      (501) staff       (20)      540 2023-06-15 08:44:02.000000 tablemaster-1.1.0/tablemaster/__init__.py
--rw-r--r--   0 livid      (501) staff       (20)     1009 2023-05-31 07:12:09.000000 tablemaster-1.1.0/tablemaster/gspread.py
--rw-r--r--   0 livid      (501) staff       (20)     2342 2023-06-15 08:35:52.000000 tablemaster-1.1.0/tablemaster/local.py
--rw-r--r--   0 livid      (501) staff       (20)     3523 2023-06-15 07:01:48.000000 tablemaster-1.1.0/tablemaster/mysql.py
--rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.1.0/tablemaster/utils.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-15 08:46:37.625276 tablemaster-1.1.0/tablemaster.egg-info/
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      310 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/SOURCES.txt
--rw-r--r--   0 livid      (501) staff       (20)        1 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/dependency_links.txt
--rw-r--r--   0 livid      (501) staff       (20)      108 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/requires.txt
--rw-r--r--   0 livid      (501) staff       (20)       12 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/top_level.txt
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-16 08:50:16.771778 tablemaster-1.1.1/
+-rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.1.1/LICENSE
+-rw-r--r--   0 livid      (501) staff       (20)      239 2023-06-16 08:50:16.771654 tablemaster-1.1.1/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)     1487 2023-06-15 08:49:46.000000 tablemaster-1.1.1/README.md
+-rw-r--r--   0 livid      (501) staff       (20)       38 2023-06-16 08:50:16.771815 tablemaster-1.1.1/setup.cfg
+-rw-r--r--   0 livid      (501) staff       (20)      559 2023-06-16 08:50:02.000000 tablemaster-1.1.1/setup.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-16 08:50:16.770886 tablemaster-1.1.1/tablemaster/
+-rw-r--r--   0 livid      (501) staff       (20)      554 2023-06-16 08:49:52.000000 tablemaster-1.1.1/tablemaster/__init__.py
+-rw-r--r--   0 livid      (501) staff       (20)     1009 2023-05-31 07:12:09.000000 tablemaster-1.1.1/tablemaster/gspread.py
+-rw-r--r--   0 livid      (501) staff       (20)     3437 2023-06-16 08:49:07.000000 tablemaster-1.1.1/tablemaster/local.py
+-rw-r--r--   0 livid      (501) staff       (20)     3523 2023-06-15 07:01:48.000000 tablemaster-1.1.1/tablemaster/mysql.py
+-rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.1.1/tablemaster/utils.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-16 08:50:16.771506 tablemaster-1.1.1/tablemaster.egg-info/
+-rw-r--r--   0 livid      (501) staff       (20)      239 2023-06-16 08:50:16.000000 tablemaster-1.1.1/tablemaster.egg-info/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      310 2023-06-16 08:50:16.000000 tablemaster-1.1.1/tablemaster.egg-info/SOURCES.txt
+-rw-r--r--   0 livid      (501) staff       (20)        1 2023-06-16 08:50:16.000000 tablemaster-1.1.1/tablemaster.egg-info/dependency_links.txt
+-rw-r--r--   0 livid      (501) staff       (20)      108 2023-06-16 08:50:16.000000 tablemaster-1.1.1/tablemaster.egg-info/requires.txt
+-rw-r--r--   0 livid      (501) staff       (20)       12 2023-06-16 08:50:16.000000 tablemaster-1.1.1/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.1.0/LICENSE` & `tablemaster-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.0/README.md` & `tablemaster-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # tablemaster
 A Python package makes it easy to manage tables anywhere.
 
 # Install
 ```
-pip install tablemaster
+pip install -U tablemaster
 ```
 
 # Preparation
 ### To use the function related to mysql, need to put a file named cfg.yaml in the same path, which is like:
 ```
  db_name_example:
    name: db_name_example
```

### Comparing `tablemaster-1.1.0/setup.py` & `tablemaster-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.1.0',
+    version='1.1.1',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy==1.4.46',
         'pandas',
         'python-dateutil',
         'gspread',
```

### Comparing `tablemaster-1.1.0/tablemaster/__init__.py` & `tablemaster-1.1.1/tablemaster/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,9 +22,10 @@
     gs_read_df,
     gs_write_df,
 )
 
 from .local import (
     read,
     batch_read,
+    read_dfs,
 )
```

### Comparing `tablemaster-1.1.0/tablemaster/gspread.py` & `tablemaster-1.1.1/tablemaster/gspread.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.0/tablemaster/mysql.py` & `tablemaster-1.1.1/tablemaster/mysql.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.0/tablemaster/utils.py` & `tablemaster-1.1.1/tablemaster/utils.py`

 * *Files identical despite different names*

