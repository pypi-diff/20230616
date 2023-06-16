# Comparing `tmp/alsldlawef-0.1.0.tar.gz` & `tmp/alsldlawef-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alsldlawef-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "alsldlawef-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `alsldlawef-0.1.0.tar` & `alsldlawef-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1102 2023-06-13 14:49:07.619979 alsldlawef-0.1.0/LICENSE
--rw-r--r--   0        0        0      682 2023-06-16 13:18:48.335177 alsldlawef-0.1.0/alsldlawef/__init__.py
--rw-r--r--   0        0        0      325 2023-06-14 13:59:58.791492 alsldlawef-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      197 1970-01-01 00:00:00.000000 alsldlawef-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-06-13 14:49:07.619979 alsldlawef-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-16 13:21:01.177794 alsldlawef-0.1.1/alsldlawef/README.md
+-rw-r--r--   0        0        0      682 2023-06-16 13:22:44.511522 alsldlawef-0.1.1/alsldlawef/__init__.py
+-rw-r--r--   0        0        0      383 2023-06-16 13:22:29.702058 alsldlawef-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      197 1970-01-01 00:00:00.000000 alsldlawef-0.1.1/PKG-INFO
```

### Comparing `alsldlawef-0.1.0/LICENSE` & `alsldlawef-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alsldlawef-0.1.0/alsldlawef/__init__.py` & `alsldlawef-0.1.1/alsldlawef/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Let's find some podcasts!"""
 
 from dataclasses import dataclass
 from typing import List, Optional
 from .core import _get, _parse
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # ...
 
 SEARCH_URL = "https://itunes.apple.com/search"
 
 @dataclass
 class Podcast:
```

