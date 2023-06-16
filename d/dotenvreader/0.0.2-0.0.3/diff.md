# Comparing `tmp/dotenvreader-0.0.2.tar.gz` & `tmp/dotenvreader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotenvreader-0.0.2.tar", last modified: Thu Jun 15 20:54:19 2023, max compression
+gzip compressed data, was "dotenvreader-0.0.3.tar", last modified: Fri Jun 16 14:01:51 2023, max compression
```

## Comparing `dotenvreader-0.0.2.tar` & `dotenvreader-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 20:54:19.499735 dotenvreader-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-06-15 20:07:39.000000 dotenvreader-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      759 2023-06-15 20:54:19.497736 dotenvreader-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-06-07 21:11:04.000000 dotenvreader-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 20:54:19.368740 dotenvreader-0.0.2/dotenvreader/
--rw-rw-rw-   0        0        0       29 2023-06-15 20:22:42.000000 dotenvreader-0.0.2/dotenvreader/__init__.py
--rw-rw-rw-   0        0        0     2298 2023-06-15 20:22:07.000000 dotenvreader-0.0.2/dotenvreader/main.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:54:19.491732 dotenvreader-0.0.2/dotenvreader.egg-info/
--rw-rw-rw-   0        0        0      759 2023-06-15 20:54:18.000000 dotenvreader-0.0.2/dotenvreader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-15 20:54:18.000000 dotenvreader-0.0.2/dotenvreader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 20:54:18.000000 dotenvreader-0.0.2/dotenvreader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-15 20:54:18.000000 dotenvreader-0.0.2/dotenvreader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 20:54:18.000000 dotenvreader-0.0.2/dotenvreader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 20:54:19.499735 dotenvreader-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-15 20:53:56.000000 dotenvreader-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:01:51.501577 dotenvreader-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-15 20:07:39.000000 dotenvreader-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      902 2023-06-16 14:01:51.498581 dotenvreader-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-06-16 14:01:24.000000 dotenvreader-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 14:01:51.417491 dotenvreader-0.0.3/dotenvreader/
+-rw-rw-rw-   0        0        0       29 2023-06-15 20:22:42.000000 dotenvreader-0.0.3/dotenvreader/__init__.py
+-rw-rw-rw-   0        0        0     2334 2023-06-16 13:46:14.000000 dotenvreader-0.0.3/dotenvreader/main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:01:51.495581 dotenvreader-0.0.3/dotenvreader.egg-info/
+-rw-rw-rw-   0        0        0      902 2023-06-16 14:01:50.000000 dotenvreader-0.0.3/dotenvreader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-16 14:01:51.000000 dotenvreader-0.0.3/dotenvreader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 14:01:50.000000 dotenvreader-0.0.3/dotenvreader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-16 14:01:51.000000 dotenvreader-0.0.3/dotenvreader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-16 14:01:51.000000 dotenvreader-0.0.3/dotenvreader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 14:01:51.502582 dotenvreader-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-16 13:42:53.000000 dotenvreader-0.0.3/setup.py
```

### Comparing `dotenvreader-0.0.2/LICENSE` & `dotenvreader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dotenvreader-0.0.2/dotenvreader/main.py` & `dotenvreader-0.0.3/dotenvreader/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+
+The DotENV Package
+
+"""
+
 import os as __os
 import time as __time
 import colorama as __colorama
 from colorama import Fore as __Fore
 
 __colorama.init()
```

### Comparing `dotenvreader-0.0.2/setup.py` & `dotenvreader-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "README.md"), encoding="utf-8") as file:
     long_description = "\n" + file.read()
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Read dotenv files with python"
 LONG_DESCRIPTION = "A Package that allows reading with DotENV"
 
 setup(
     name="dotenvreader",
     version=VERSION,
     author="ContentGamer",
```

