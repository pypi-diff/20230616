# Comparing `tmp/sqscraper-0.3.1.tar.gz` & `tmp/sqscraper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqscraper-0.3.1.tar", last modified: Fri Jun 16 18:39:38 2023, max compression
+gzip compressed data, was "sqscraper-0.3.2.tar", last modified: Fri Jun 16 21:35:07 2023, max compression
```

## Comparing `sqscraper-0.3.1.tar` & `sqscraper-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.972144 sqscraper-0.3.1/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     2312 2023-06-16 18:39:38.972144 sqscraper-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.3.1/README.md
--rw-rw-rw-   0        0        0     1837 2023-06-16 18:38:17.000000 sqscraper-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 18:39:38.972144 sqscraper-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.944140 sqscraper-0.3.1/sqscraper/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.3.1/sqscraper/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.3.1/sqscraper/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.964139 sqscraper-0.3.1/sqscraper/cnbc/
--rw-rw-rw-   0        0        0       50 2023-06-15 19:52:45.000000 sqscraper-0.3.1/sqscraper/cnbc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.968137 sqscraper-0.3.1/sqscraper/cnbc/_tabs/
--rw-rw-rw-   0        0        0      720 2023-06-16 17:52:52.000000 sqscraper-0.3.1/sqscraper/cnbc/_tabs/__init__.py
--rw-rw-rw-   0        0        0     8077 2023-06-16 18:29:37.000000 sqscraper-0.3.1/sqscraper/cnbc/_tabs/summary.py
--rw-rw-rw-   0        0        0     4961 2023-06-16 16:56:03.000000 sqscraper-0.3.1/sqscraper/cnbc/stock_quote.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.956134 sqscraper-0.3.1/sqscraper.egg-info/
--rw-rw-rw-   0        0        0     2312 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      397 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 21:35:07.197934 sqscraper-0.3.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2312 2023-06-16 21:35:07.197934 sqscraper-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.3.2/README.md
+-rw-rw-rw-   0        0        0     1837 2023-06-16 21:32:57.000000 sqscraper-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 21:35:07.197934 sqscraper-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 21:35:07.154843 sqscraper-0.3.2/sqscraper/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.3.2/sqscraper/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.3.2/sqscraper/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:35:07.187941 sqscraper-0.3.2/sqscraper/cnbc/
+-rw-rw-rw-   0        0        0       49 2023-06-16 21:14:25.000000 sqscraper-0.3.2/sqscraper/cnbc/__init__.py
+-rw-rw-rw-   0        0        0    13195 2023-06-16 21:27:34.000000 sqscraper-0.3.2/sqscraper/cnbc/quote_page.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:35:07.187941 sqscraper-0.3.2/sqscraper.egg-info/
+-rw-rw-rw-   0        0        0     2312 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      397 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/top_level.txt
```

### Comparing `sqscraper-0.3.1/LICENSE` & `sqscraper-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqscraper-0.3.1/PKG-INFO` & `sqscraper-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.3.1
+Version: 0.3.2
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqscraper-0.3.1/pyproject.toml` & `sqscraper-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqscraper"
-version = "0.3.1"
+version = "0.3.2"
 description = "API wrapper and web scraper for select stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Financial and Insurance Industry",
```

### Comparing `sqscraper-0.3.1/sqscraper.egg-info/PKG-INFO` & `sqscraper-0.3.2/sqscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.3.1
+Version: 0.3.2
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

