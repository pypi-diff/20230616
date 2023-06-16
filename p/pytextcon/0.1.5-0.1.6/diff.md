# Comparing `tmp/pytextcon-0.1.5.tar.gz` & `tmp/pytextcon-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytextcon-0.1.5.tar", last modified: Fri Jun 16 03:41:58 2023, max compression
+gzip compressed data, was "pytextcon-0.1.6.tar", last modified: Fri Jun 16 03:51:52 2023, max compression
```

## Comparing `pytextcon-0.1.5.tar` & `pytextcon-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 03:41:58.978537 pytextcon-0.1.5/
--rw-rw-rw-   0        0        0     1069 2023-06-04 20:53:32.000000 pytextcon-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2018 2023-06-16 03:41:58.977507 pytextcon-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-06-16 03:35:54.000000 pytextcon-0.1.5/README.md
--rw-rw-rw-   0        0        0      694 2023-06-16 03:35:54.000000 pytextcon-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 03:41:58.979073 pytextcon-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 03:41:58.940519 pytextcon-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 03:41:58.951875 pytextcon-0.1.5/src/pytextcon/
--rw-rw-rw-   0        0        0       30 2023-06-16 03:35:54.000000 pytextcon-0.1.5/src/pytextcon/__init__.py
--rw-rw-rw-   0        0        0     2727 2023-06-16 03:24:32.000000 pytextcon-0.1.5/src/pytextcon/pytextcon.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:41:58.975242 pytextcon-0.1.5/src/pytextcon.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-16 03:41:58.000000 pytextcon-0.1.5/src/pytextcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-16 03:41:58.000000 pytextcon-0.1.5/src/pytextcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 03:41:58.000000 pytextcon-0.1.5/src/pytextcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 03:41:58.000000 pytextcon-0.1.5/src/pytextcon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 03:51:52.818968 pytextcon-0.1.6/
+-rw-rw-rw-   0        0        0     1069 2023-06-04 20:53:32.000000 pytextcon-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2018 2023-06-16 03:51:52.818433 pytextcon-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-06-16 03:35:54.000000 pytextcon-0.1.6/README.md
+-rw-rw-rw-   0        0        0      694 2023-06-16 03:51:11.000000 pytextcon-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 03:51:52.819499 pytextcon-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 03:51:52.784084 pytextcon-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 03:51:52.793068 pytextcon-0.1.6/src/pytextcon/
+-rw-rw-rw-   0        0        0       40 2023-06-16 03:50:24.000000 pytextcon-0.1.6/src/pytextcon/__init__.py
+-rw-rw-rw-   0        0        0     2727 2023-06-16 03:24:32.000000 pytextcon-0.1.6/src/pytextcon/pytextcon.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:51:52.815846 pytextcon-0.1.6/src/pytextcon.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-16 03:51:52.000000 pytextcon-0.1.6/src/pytextcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-16 03:51:52.000000 pytextcon-0.1.6/src/pytextcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 03:51:52.000000 pytextcon-0.1.6/src/pytextcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 03:51:52.000000 pytextcon-0.1.6/src/pytextcon.egg-info/top_level.txt
```

### Comparing `pytextcon-0.1.5/LICENSE` & `pytextcon-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytextcon-0.1.5/PKG-INFO` & `pytextcon-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytextcon
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple package to change the text color, text emphasis, and background color of print statements to the console.
 Author-email: Michael <michael.lokrosh@gmail.com>
 Project-URL: GitHub, https://github.com/Lokrosh/pytextcon
 Keywords: print,color,console,text,formatting,emphasis,underline,bright
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytextcon-0.1.5/README.md` & `pytextcon-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pytextcon-0.1.5/pyproject.toml` & `pytextcon-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytextcon"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Michael", email="michael.lokrosh@gmail.com" },
 ]
 description = "Simple package to change the text color, text emphasis, and background color of print statements to the console."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["print", "color", "console", "text", "formatting", "emphasis", "underline", "bright"]
```

### Comparing `pytextcon-0.1.5/src/pytextcon/pytextcon.py` & `pytextcon-0.1.6/src/pytextcon/pytextcon.py`

 * *Files identical despite different names*

### Comparing `pytextcon-0.1.5/src/pytextcon.egg-info/PKG-INFO` & `pytextcon-0.1.6/src/pytextcon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytextcon
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple package to change the text color, text emphasis, and background color of print statements to the console.
 Author-email: Michael <michael.lokrosh@gmail.com>
 Project-URL: GitHub, https://github.com/Lokrosh/pytextcon
 Keywords: print,color,console,text,formatting,emphasis,underline,bright
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

