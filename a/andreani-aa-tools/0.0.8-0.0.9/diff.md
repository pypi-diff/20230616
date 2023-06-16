# Comparing `tmp/andreani_aa_tools-0.0.8.tar.gz` & `tmp/andreani_aa_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andreani_aa_tools-0.0.8.tar", last modified: Wed Sep 21 15:54:37 2022, max compression
+gzip compressed data, was "andreani_aa_tools-0.0.9.tar", last modified: Mon Sep 26 17:50:52 2022, max compression
```

## Comparing `andreani_aa_tools-0.0.8.tar` & `andreani_aa_tools-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-09-21 15:54:37.973367 andreani_aa_tools-0.0.8/
--rw-rw-rw-   0        0        0     1088 2022-09-14 18:27:16.000000 andreani_aa_tools-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3208 2022-09-21 15:54:37.973367 andreani_aa_tools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      910 2022-09-21 15:53:59.000000 andreani_aa_tools-0.0.8/README.md
--rw-rw-rw-   0        0        0     1343 2022-09-21 15:54:06.000000 andreani_aa_tools-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      631 2022-09-21 15:54:37.976138 andreani_aa_tools-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-21 15:54:37.933009 andreani_aa_tools-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-09-21 15:54:37.958790 andreani_aa_tools-0.0.8/src/aa_tools/
--rw-rw-rw-   0        0        0      100 2022-09-14 19:27:23.000000 andreani_aa_tools-0.0.8/src/aa_tools/__init__.py
--rw-rw-rw-   0        0        0     1627 2022-09-14 19:53:05.000000 andreani_aa_tools-0.0.8/src/aa_tools/datalake.py
--rw-rw-rw-   0        0        0      546 2022-09-21 15:48:28.000000 andreani_aa_tools-0.0.8/src/aa_tools/distances.py
--rw-rw-rw-   0        0        0     1306 2022-09-14 20:50:20.000000 andreani_aa_tools-0.0.8/src/aa_tools/logger.py
-drwxrwxrwx   0        0        0        0 2022-09-21 15:54:37.972359 andreani_aa_tools-0.0.8/src/andreani_aa_tools.egg-info/
--rw-rw-rw-   0        0        0     3208 2022-09-21 15:54:37.000000 andreani_aa_tools-0.0.8/src/andreani_aa_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2022-09-21 15:54:37.000000 andreani_aa_tools-0.0.8/src/andreani_aa_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-21 15:54:37.000000 andreani_aa_tools-0.0.8/src/andreani_aa_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-09-21 15:54:37.000000 andreani_aa_tools-0.0.8/src/andreani_aa_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-26 17:50:52.385944 andreani_aa_tools-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2022-09-14 18:27:16.000000 andreani_aa_tools-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3208 2022-09-26 17:50:52.386944 andreani_aa_tools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2022-09-21 15:53:59.000000 andreani_aa_tools-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1343 2022-09-26 17:49:08.000000 andreani_aa_tools-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      631 2022-09-26 17:50:52.389575 andreani_aa_tools-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-09-26 17:50:52.341178 andreani_aa_tools-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-09-26 17:50:52.371762 andreani_aa_tools-0.0.9/src/aa_tools/
+-rw-rw-rw-   0        0        0      100 2022-09-14 19:27:23.000000 andreani_aa_tools-0.0.9/src/aa_tools/__init__.py
+-rw-rw-rw-   0        0        0     1122 2022-09-26 17:48:32.000000 andreani_aa_tools-0.0.9/src/aa_tools/datalake.py
+-rw-rw-rw-   0        0        0      546 2022-09-21 15:48:28.000000 andreani_aa_tools-0.0.9/src/aa_tools/distances.py
+-rw-rw-rw-   0        0        0     1306 2022-09-14 20:50:20.000000 andreani_aa_tools-0.0.9/src/aa_tools/logger.py
+drwxrwxrwx   0        0        0        0 2022-09-26 17:50:52.384878 andreani_aa_tools-0.0.9/src/andreani_aa_tools.egg-info/
+-rw-rw-rw-   0        0        0     3208 2022-09-26 17:50:52.000000 andreani_aa_tools-0.0.9/src/andreani_aa_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2022-09-26 17:50:52.000000 andreani_aa_tools-0.0.9/src/andreani_aa_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-26 17:50:52.000000 andreani_aa_tools-0.0.9/src/andreani_aa_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-09-26 17:50:52.000000 andreani_aa_tools-0.0.9/src/andreani_aa_tools.egg-info/top_level.txt
```

### Comparing `andreani_aa_tools-0.0.8/LICENSE` & `andreani_aa_tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `andreani_aa_tools-0.0.8/PKG-INFO` & `andreani_aa_tools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andreani_aa_tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common functions and protocols used by the Andreani Advanced Analytics team
 Home-page: https://github.com/pypa/sampleproject
 Author-email: Ignacio Belogi <ibelogi@andreani.com>, Gabriel Aranda <garanda@andreani.com>, Mariana Liu <mliu@andreani.com>, Yasmin Ojeda <yojeda@andreani.com>, Ariel Fleiderman <afleiderman@andreani.com>, Daiana Alonso <dalonso@andreani.com>, Facundo Silvestre <fsilvestre@andreani.com>, Santiago Bergman <sbergman@andreani.com>, Matías Moyano <mmoyano@andreani.com>, Giuliana Vera <gvera@andreani.com>, Eloy Chang <echang@andreani.com>
 License: MIT License
         
         Copyright (c) 2022 Eloy Chang
```

### Comparing `andreani_aa_tools-0.0.8/README.md` & `andreani_aa_tools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `andreani_aa_tools-0.0.8/pyproject.toml` & `andreani_aa_tools-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "andreani_aa_tools"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name = "Ignacio Belogi", email = "ibelogi@andreani.com" },
   { name = "Gabriel Aranda", email = "garanda@andreani.com" },
   { name = "Mariana Liu", email = "mliu@andreani.com" },
   { name = "Yasmin Ojeda", email = "yojeda@andreani.com" },
   { name = "Ariel Fleiderman", email = "afleiderman@andreani.com" },
   { name = "Daiana Alonso", email = "dalonso@andreani.com" },
```

### Comparing `andreani_aa_tools-0.0.8/setup.cfg` & `andreani_aa_tools-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `andreani_aa_tools-0.0.8/src/aa_tools/distances.py` & `andreani_aa_tools-0.0.9/src/aa_tools/distances.py`

 * *Files identical despite different names*

### Comparing `andreani_aa_tools-0.0.8/src/aa_tools/logger.py` & `andreani_aa_tools-0.0.9/src/aa_tools/logger.py`

 * *Files identical despite different names*

### Comparing `andreani_aa_tools-0.0.8/src/andreani_aa_tools.egg-info/PKG-INFO` & `andreani_aa_tools-0.0.9/src/andreani_aa_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andreani-aa-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common functions and protocols used by the Andreani Advanced Analytics team
 Home-page: https://github.com/pypa/sampleproject
 Author-email: Ignacio Belogi <ibelogi@andreani.com>, Gabriel Aranda <garanda@andreani.com>, Mariana Liu <mliu@andreani.com>, Yasmin Ojeda <yojeda@andreani.com>, Ariel Fleiderman <afleiderman@andreani.com>, Daiana Alonso <dalonso@andreani.com>, Facundo Silvestre <fsilvestre@andreani.com>, Santiago Bergman <sbergman@andreani.com>, Matías Moyano <mmoyano@andreani.com>, Giuliana Vera <gvera@andreani.com>, Eloy Chang <echang@andreani.com>
 License: MIT License
         
         Copyright (c) 2022 Eloy Chang
```

