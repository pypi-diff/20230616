# Comparing `tmp/pdm-invoke-0.0.2.tar.gz` & `tmp/pdm-invoke-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-invoke-0.0.2.tar", last modified: Thu Oct  6 05:38:50 2022, max compression
+gzip compressed data, was "pdm-invoke-0.0.5.tar", last modified: Fri Jun 16 07:37:22 2023, max compression
```

## Comparing `pdm-invoke-0.0.2.tar` & `pdm-invoke-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0 sicksid    (501) staff       (20)     1069 2022-10-06 04:13:27.186860 pdm-invoke-0.0.2/LICENSE
--rw-r--r--   0 sicksid    (501) staff       (20)      531 2022-10-06 05:04:53.177244 pdm-invoke-0.0.2/README.md
--rw-r--r--   0 sicksid    (501) staff       (20)        0 2022-10-06 04:13:27.194088 pdm-invoke-0.0.2/pdm_invoke/__init__.py
--rw-r--r--   0 sicksid    (501) staff       (20)     1258 2022-10-06 05:38:37.005419 pdm-invoke-0.0.2/pdm_invoke/main.py
--rw-r--r--   0 sicksid    (501) staff       (20)      884 2022-10-06 05:33:03.355322 pdm-invoke-0.0.2/pyproject.toml
--rw-------   0 sicksid    (501) staff       (20)      817 2022-10-06 05:38:50.346711 pdm-invoke-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-06 04:13:27.186860 pdm-invoke-0.0.5/LICENSE
+-rw-r--r--   0        0        0      531 2022-10-06 05:04:53.177244 pdm-invoke-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2022-10-06 04:13:27.194088 pdm-invoke-0.0.5/pdm_invoke/__init__.py
+-rw-r--r--   0        0        0     1258 2022-10-06 05:38:37.005419 pdm-invoke-0.0.5/pdm_invoke/main.py
+-rw-r--r--   0        0        0      884 2023-06-16 07:32:07.281427 pdm-invoke-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 pdm-invoke-0.0.5/PKG-INFO
```

### Comparing `pdm-invoke-0.0.2/LICENSE` & `pdm-invoke-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-invoke-0.0.2/README.md` & `pdm-invoke-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pdm-invoke-0.0.2/pdm_invoke/main.py` & `pdm-invoke-0.0.5/pdm_invoke/main.py`

 * *Files identical despite different names*

### Comparing `pdm-invoke-0.0.2/pyproject.toml` & `pdm-invoke-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-invoke"
-version = "0.0.2"
+version = "0.0.5"
 description = "pdm shortcuts for invoke projects"
 authors = [
     { name = "Abdul Hamid", email = "abdulachik@icloud.com" },
 ]
 dependencies = []
 requires-python = ">=3.7"
 readme = "README.md"
```

### Comparing `pdm-invoke-0.0.2/PKG-INFO` & `pdm-invoke-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-invoke
-Version: 0.0.2
+Version: 0.0.5
 Summary: pdm shortcuts for invoke projects
 License: MIT
 Author-email: Abdul Hamid <abdulachik@icloud.com>
 Requires-Python: >=3.7
 Project-URL: homepage, https://github.com/sicksid/pdm-invoke
 Description-Content-Type: text/markdown
```

