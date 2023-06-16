# Comparing `tmp/sqscraper-0.3.0.tar.gz` & `tmp/sqscraper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqscraper-0.3.0.tar", last modified: Thu Jun 15 19:47:31 2023, max compression
+gzip compressed data, was "sqscraper-0.3.1.tar", last modified: Fri Jun 16 18:39:38 2023, max compression
```

## Comparing `sqscraper-0.3.0.tar` & `sqscraper-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 19:47:31.897035 sqscraper-0.3.0/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     2312 2023-06-15 19:47:31.897035 sqscraper-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-06-14 06:29:52.000000 sqscraper-0.3.0/README.md
--rw-rw-rw-   0        0        0     1550 2023-06-15 19:43:45.000000 sqscraper-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 19:47:31.897035 sqscraper-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 19:47:31.856765 sqscraper-0.3.0/sqscraper/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:55:42.000000 sqscraper-0.3.0/sqscraper/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:16:53.000000 sqscraper-0.3.0/sqscraper/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:47:31.881403 sqscraper-0.3.0/sqscraper/cnbc/
--rw-rw-rw-   0        0        0       50 2023-06-14 22:43:38.000000 sqscraper-0.3.0/sqscraper/cnbc/__init__.py
--rw-rw-rw-   0        0        0     2337 2023-06-15 19:28:11.000000 sqscraper-0.3.0/sqscraper/cnbc/quote_strip.py
--rw-rw-rw-   0        0        0     2618 2023-06-15 19:29:01.000000 sqscraper-0.3.0/sqscraper/cnbc/stock_quote.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:47:31.881403 sqscraper-0.3.0/sqscraper.egg-info/
--rw-rw-rw-   0        0        0     2312 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      219 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.972144 sqscraper-0.3.1/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2312 2023-06-16 18:39:38.972144 sqscraper-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.3.1/README.md
+-rw-rw-rw-   0        0        0     1837 2023-06-16 18:38:17.000000 sqscraper-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 18:39:38.972144 sqscraper-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.944140 sqscraper-0.3.1/sqscraper/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.3.1/sqscraper/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.3.1/sqscraper/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.964139 sqscraper-0.3.1/sqscraper/cnbc/
+-rw-rw-rw-   0        0        0       50 2023-06-15 19:52:45.000000 sqscraper-0.3.1/sqscraper/cnbc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.968137 sqscraper-0.3.1/sqscraper/cnbc/_tabs/
+-rw-rw-rw-   0        0        0      720 2023-06-16 17:52:52.000000 sqscraper-0.3.1/sqscraper/cnbc/_tabs/__init__.py
+-rw-rw-rw-   0        0        0     8077 2023-06-16 18:29:37.000000 sqscraper-0.3.1/sqscraper/cnbc/_tabs/summary.py
+-rw-rw-rw-   0        0        0     4961 2023-06-16 16:56:03.000000 sqscraper-0.3.1/sqscraper/cnbc/stock_quote.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:39:38.956134 sqscraper-0.3.1/sqscraper.egg-info/
+-rw-rw-rw-   0        0        0     2312 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      397 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 18:39:38.000000 sqscraper-0.3.1/sqscraper.egg-info/top_level.txt
```

### Comparing `sqscraper-0.3.0/LICENSE` & `sqscraper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqscraper-0.3.0/PKG-INFO` & `sqscraper-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.3.0
+Version: 0.3.1
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqscraper-0.3.0/pyproject.toml` & `sqscraper-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqscraper"
-version = "0.3.0"
+version = "0.3.1"
 description = "API wrapper and web scraper for select stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Financial and Insurance Industry",
@@ -27,15 +27,20 @@
 ]
 requires-python = ">=3.6"
 dependencies = [
     "certifi==2023.5.7 ; python_version >= '3.6'",
     "charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'",
     "idna==3.4 ; python_version >= '3.5'",
     "numpy==1.24.3",
+    "pandas==2.0.2",
+    "python-dateutil==2.8.2 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+    "pytz==2023.3",
     "requests==2.31.0",
+    "six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+    "tzdata==2023.3 ; python_version >= '2'",
     "urllib3==2.0.3 ; python_version >= '3.7'"
 ]
 
 [project.urls]
 homepage = "https://github.com/JacobLee23/SQScraper"
 
 [tool.setuptools.packages.find]
```

### Comparing `sqscraper-0.3.0/sqscraper.egg-info/PKG-INFO` & `sqscraper-0.3.1/sqscraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.3.0
+Version: 0.3.1
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

