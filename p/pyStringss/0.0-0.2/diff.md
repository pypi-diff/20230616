# Comparing `tmp/pyStringss-0.0.tar.gz` & `tmp/pyStringss-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyStringss-0.0.tar", last modified: Fri Jun 16 12:03:45 2023, max compression
+gzip compressed data, was "pyStringss-0.2.tar", last modified: Fri Jun 16 14:17:01 2023, max compression
```

## Comparing `pyStringss-0.0.tar` & `pyStringss-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:03:45.494122 pyStringss-0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 12:03:34.000000 pyStringss-0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:03:45.494122 pyStringss-0.0/LegendSS/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-16 12:03:34.000000 pyStringss-0.0/LegendSS/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:03:34.000000 pyStringss-0.0/LegendSS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-16 12:03:34.000000 pyStringss-0.0/LegendSS/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-16 12:03:45.494122 pyStringss-0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 12:03:34.000000 pyStringss-0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:03:45.494122 pyStringss-0.0/pyStringss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-16 12:03:45.000000 pyStringss-0.0/pyStringss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 12:03:45.000000 pyStringss-0.0/pyStringss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:03:45.000000 pyStringss-0.0/pyStringss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 12:03:45.000000 pyStringss-0.0/pyStringss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 12:03:45.000000 pyStringss-0.0/pyStringss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:03:45.494122 pyStringss-0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-16 12:03:34.000000 pyStringss-0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:17:01.301784 pyStringss-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 14:16:51.000000 pyStringss-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 14:17:01.301784 pyStringss-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 14:16:51.000000 pyStringss-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:17:01.297784 pyStringss-0.2/Stringss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-16 14:16:51.000000 pyStringss-0.2/Stringss/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:16:51.000000 pyStringss-0.2/Stringss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-16 14:16:51.000000 pyStringss-0.2/Stringss/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:17:01.301784 pyStringss-0.2/pyStringss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:17:01.301784 pyStringss-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-16 14:16:51.000000 pyStringss-0.2/setup.py
```

### Comparing `pyStringss-0.0/LICENSE` & `pyStringss-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyStringss-0.0/LegendSS/Data.py` & `pyStringss-0.2/Stringss/Data.py`

 * *Files identical despite different names*

### Comparing `pyStringss-0.0/LegendSS/generate.py` & `pyStringss-0.2/Stringss/generate.py`

 * *Files identical despite different names*

### Comparing `pyStringss-0.0/PKG-INFO` & `pyStringss-0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyStringss
-Version: 0.0
+Version: 0.2
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/AvishekBhattacharjee/pyStringss
 Author: wbavishek
 Author-email: wbavishekbhattacharjee@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyStringss,Stringss
 Classifier: Framework :: AsyncIO
@@ -19,8 +19,12 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyStringss
+<<<<<<< HEAD
+This is package of String Generator Bot
+=======
 This is a package of String Generator Bot. Use the package with the code available.
+>>>>>>> f506cd1510edbc868cdf70b38f54510cf7e8b074
```

### Comparing `pyStringss-0.0/pyStringss.egg-info/PKG-INFO` & `pyStringss-0.2/pyStringss.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyStringss
-Version: 0.0
+Version: 0.2
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/AvishekBhattacharjee/pyStringss
 Author: wbavishek
 Author-email: wbavishekbhattacharjee@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyStringss,Stringss
 Classifier: Framework :: AsyncIO
@@ -19,8 +19,12 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyStringss
+<<<<<<< HEAD
+This is package of String Generator Bot
+=======
 This is a package of String Generator Bot. Use the package with the code available.
+>>>>>>> f506cd1510edbc868cdf70b38f54510cf7e8b074
```

### Comparing `pyStringss-0.0/setup.py` & `pyStringss-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write("Warning: Could not open README.md due %s\n" % error)
 
 
 setup(
     name="pyStringss",
     author="wbavishek",
     author_email="wbavishekbhattacharjee@gmail.com",
-    version="0.0",
+    version="0.2",
     description="This is a simple package which is used in String Generator Bot",
     long_description=readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/AvishekBhattacharjee/pyStringss",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

