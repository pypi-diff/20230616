# Comparing `tmp/dissect.contrib-1.3.dev1.tar.gz` & `tmp/dissect.contrib-1.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.contrib-1.3.dev1.tar", last modified: Thu Mar 16 13:02:44 2023, max compression
+gzip compressed data, was "dissect.contrib-1.4.dev1.tar", last modified: Fri Jun 16 12:48:49 2023, max compression
```

## Comparing `dissect.contrib-1.3.dev1.tar` & `dissect.contrib-1.4.dev1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:44.853341 dissect.contrib-1.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-16 13:02:44.853341 dissect.contrib-1.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:44.849341 dissect.contrib-1.3.dev1/dissect.contrib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-16 13:02:44.000000 dissect.contrib-1.3.dev1/dissect.contrib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-16 13:02:44.000000 dissect.contrib-1.3.dev1/dissect.contrib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:02:44.000000 dissect.contrib-1.3.dev1/dissect.contrib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:02:44.000000 dissect.contrib-1.3.dev1/dissect.contrib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-16 13:02:31.000000 dissect.contrib-1.3.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:02:44.853341 dissect.contrib-1.3.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:44.849341 dissect.contrib-1.3.dev1/template/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:44.849341 dissect.contrib-1.3.dev1/template/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:44.849341 dissect.contrib-1.3.dev1/template/dissect/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:44.853341 dissect.contrib-1.3.dev1/template/dissect/contrib/template/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/template/dissect/contrib/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-16 13:02:23.000000 dissect.contrib-1.3.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.296563 dissect.contrib-1.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-16 12:48:49.296563 dissect.contrib-1.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.292563 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-16 12:48:49.000000 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 12:48:49.000000 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:49.000000 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:49.000000 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-16 12:48:39.000000 dissect.contrib-1.4.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:48:49.296563 dissect.contrib-1.4.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.292563 dissect.contrib-1.4.dev1/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.288563 dissect.contrib-1.4.dev1/template/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.288563 dissect.contrib-1.4.dev1/template/dissect/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.296563 dissect.contrib-1.4.dev1/template/dissect/contrib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/template/dissect/contrib/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/tox.ini
```

### Comparing `dissect.contrib-1.3.dev1/LICENSE` & `dissect.contrib-1.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.3.dev1/PKG-INFO` & `dissect.contrib-1.4.dev1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: dissect.contrib
-Version: 1.3.dev1
-Summary: This project is a meta package: it reserves the namespace for Dissect packages made by external contributors
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: repository, https://github.com/fox-it/dissect.contrib
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.contrib
 
 This project is a meta package. It reserves the namespace for Dissect packages made by external contributors.
 
 We encourage contributions to the Dissect project, in both the existing projects as well as entirely new ones.
 We kindly request that you use the `dissect.contrib` namespace prefix for your package names. For example, a new project for
 `myfilesystem` would be called `dissect.contrib.myfilesystem`.
```

### Comparing `dissect.contrib-1.3.dev1/dissect.contrib.egg-info/PKG-INFO` & `dissect.contrib-1.4.dev1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 Metadata-Version: 2.1
 Name: dissect.contrib
-Version: 1.3.dev1
+Version: 1.4.dev1
 Summary: This project is a meta package: it reserves the namespace for Dissect packages made by external contributors
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect.contrib
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYRIGHT
 
 # dissect.contrib
```

### Comparing `dissect.contrib-1.3.dev1/pyproject.toml` & `dissect.contrib-1.4.dev1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,25 @@
 readme = "README.md"
 requires-python = "~=3.9"
 license.text = "Affero General Public License v3"
 authors = [
   {name = "Dissect Team", email = "dissect@fox-it.com"}
 ]
 classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "Environment :: Console",
+  "Intended Audience :: Developers",
+  "Intended Audience :: Information Technology",
+  "License :: OSI Approved",
+  "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
+  "Topic :: Internet :: Log Analysis",
+  "Topic :: Scientific/Engineering :: Information Analysis",
+  "Topic :: Security",
+  "Topic :: Utilities",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://dissect.tools"
 repository = "https://github.com/fox-it/dissect.contrib"
```

### Comparing `dissect.contrib-1.3.dev1/template/pyproject.toml` & `dissect.contrib-1.4.dev1/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.3.dev1/tox.ini` & `dissect.contrib-1.4.dev1/tox.ini`

 * *Files identical despite different names*

