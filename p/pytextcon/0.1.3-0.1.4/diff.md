# Comparing `tmp/pytextcon-0.1.3.tar.gz` & `tmp/pytextcon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytextcon-0.1.3.tar", last modified: Thu Jun 15 21:03:06 2023, max compression
+gzip compressed data, was "pytextcon-0.1.4.tar", last modified: Fri Jun 16 02:32:09 2023, max compression
```

## Comparing `pytextcon-0.1.3.tar` & `pytextcon-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:03:06.224669 pytextcon-0.1.3/
--rw-rw-rw-   0        0        0     1069 2023-06-04 20:53:32.000000 pytextcon-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1996 2023-06-15 21:03:06.223475 pytextcon-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2023-06-15 02:54:10.000000 pytextcon-0.1.3/README.md
--rw-rw-rw-   0        0        0      694 2023-06-15 21:02:34.000000 pytextcon-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 21:03:06.225183 pytextcon-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 21:03:06.194782 pytextcon-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 21:03:06.204668 pytextcon-0.1.3/src/pytextcon/
--rw-rw-rw-   0        0        0        0 2023-06-15 01:18:50.000000 pytextcon-0.1.3/src/pytextcon/__init__.py
--rw-rw-rw-   0        0        0     2733 2023-06-15 21:02:34.000000 pytextcon-0.1.3/src/pytextcon/pytextcon.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:03:06.221204 pytextcon-0.1.3/src/pytextcon.egg-info/
--rw-rw-rw-   0        0        0     1996 2023-06-15 21:03:06.000000 pytextcon-0.1.3/src/pytextcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-15 21:03:06.000000 pytextcon-0.1.3/src/pytextcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:03:06.000000 pytextcon-0.1.3/src/pytextcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 21:03:06.000000 pytextcon-0.1.3/src/pytextcon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 02:32:09.758878 pytextcon-0.1.4/
+-rw-rw-rw-   0        0        0     1069 2023-06-04 20:53:32.000000 pytextcon-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1996 2023-06-16 02:32:09.758326 pytextcon-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2023-06-15 02:54:10.000000 pytextcon-0.1.4/README.md
+-rw-rw-rw-   0        0        0      694 2023-06-16 02:31:30.000000 pytextcon-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 02:32:09.759423 pytextcon-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 02:32:09.725302 pytextcon-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:32:09.735984 pytextcon-0.1.4/src/pytextcon/
+-rw-rw-rw-   0        0        0        0 2023-06-15 01:18:50.000000 pytextcon-0.1.4/src/pytextcon/__init__.py
+-rw-rw-rw-   0        0        0     1888 2023-06-16 02:31:30.000000 pytextcon-0.1.4/src/pytextcon/pytextcon.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:32:09.756109 pytextcon-0.1.4/src/pytextcon.egg-info/
+-rw-rw-rw-   0        0        0     1996 2023-06-16 02:32:09.000000 pytextcon-0.1.4/src/pytextcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-16 02:32:09.000000 pytextcon-0.1.4/src/pytextcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 02:32:09.000000 pytextcon-0.1.4/src/pytextcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 02:32:09.000000 pytextcon-0.1.4/src/pytextcon.egg-info/top_level.txt
```

### Comparing `pytextcon-0.1.3/LICENSE` & `pytextcon-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytextcon-0.1.3/PKG-INFO` & `pytextcon-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytextcon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple package to change the text color, text emphasis, and background color of print statements to the console.
 Author-email: Michael <michael.lokrosh@gmail.com>
 Project-URL: GitHub, https://github.com/Lokrosh/pytextcon
 Keywords: print,color,console,text,formatting,emphasis,underline,bright
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytextcon-0.1.3/README.md` & `pytextcon-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pytextcon-0.1.3/pyproject.toml` & `pytextcon-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytextcon"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Michael", email="michael.lokrosh@gmail.com" },
 ]
 description = "Simple package to change the text color, text emphasis, and background color of print statements to the console."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["print", "color", "console", "text", "formatting", "emphasis", "underline", "bright"]
```

### Comparing `pytextcon-0.1.3/src/pytextcon.egg-info/PKG-INFO` & `pytextcon-0.1.4/src/pytextcon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytextcon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple package to change the text color, text emphasis, and background color of print statements to the console.
 Author-email: Michael <michael.lokrosh@gmail.com>
 Project-URL: GitHub, https://github.com/Lokrosh/pytextcon
 Keywords: print,color,console,text,formatting,emphasis,underline,bright
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

