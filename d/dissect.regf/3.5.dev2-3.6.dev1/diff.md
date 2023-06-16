# Comparing `tmp/dissect.regf-3.5.dev2.tar.gz` & `tmp/dissect.regf-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.regf-3.5.dev2.tar", last modified: Tue May 16 13:26:40 2023, max compression
+gzip compressed data, was "dissect.regf-3.6.dev1.tar", last modified: Fri Jun 16 12:50:30 2023, max compression
```

## Comparing `dissect.regf-3.5.dev2.tar` & `dissect.regf-3.6.dev1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:40.789853 dissect.regf-3.5.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-16 13:26:40.789853 dissect.regf-3.5.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:40.777853 dissect.regf-3.5.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:40.785853 dissect.regf-3.5.dev2/dissect/regf/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/dissect/regf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/dissect/regf/c_regf.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/dissect/regf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/dissect/regf/regf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:40.785853 dissect.regf-3.5.dev2/dissect.regf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-16 13:26:40.000000 dissect.regf-3.5.dev2/dissect.regf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-16 13:26:40.000000 dissect.regf-3.5.dev2/dissect.regf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:40.000000 dissect.regf-3.5.dev2/dissect.regf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:40.000000 dissect.regf-3.5.dev2/dissect.regf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:40.000000 dissect.regf-3.5.dev2/dissect.regf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:40.785853 dissect.regf-3.5.dev2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/examples/walkhive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-16 13:26:30.000000 dissect.regf-3.5.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:40.789853 dissect.regf-3.5.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:40.785853 dissect.regf-3.5.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:40.785853 dissect.regf-3.5.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1969086 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/tests/data/SYSTEM.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:40.789853 dissect.regf-3.5.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/tests/test_regf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:26:25.000000 dissect.regf-3.5.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:30.635397 dissect.regf-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-16 12:50:30.635397 dissect.regf-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:30.627397 dissect.regf-3.6.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:30.631397 dissect.regf-3.6.dev1/dissect/regf/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/dissect/regf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/dissect/regf/c_regf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/dissect/regf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/dissect/regf/regf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:30.631397 dissect.regf-3.6.dev1/dissect.regf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-16 12:50:30.000000 dissect.regf-3.6.dev1/dissect.regf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-16 12:50:30.000000 dissect.regf-3.6.dev1/dissect.regf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:50:30.000000 dissect.regf-3.6.dev1/dissect.regf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:50:30.000000 dissect.regf-3.6.dev1/dissect.regf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:50:30.000000 dissect.regf-3.6.dev1/dissect.regf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:30.631397 dissect.regf-3.6.dev1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/examples/walkhive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-16 12:50:20.000000 dissect.regf-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:50:30.635397 dissect.regf-3.6.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:30.631397 dissect.regf-3.6.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:30.631397 dissect.regf-3.6.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1969086 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/tests/data/SYSTEM.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:30.635397 dissect.regf-3.6.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/tests/test_regf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:50:16.000000 dissect.regf-3.6.dev1/tox.ini
```

### Comparing `dissect.regf-3.5.dev2/LICENSE` & `dissect.regf-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.5.dev2/PKG-INFO` & `dissect.regf-3.6.dev1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dissect.regf
-Version: 3.5.dev2
-Summary: A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration on Windows operating systems
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.regf
-Project-URL: repository, https://github.com/fox-it/dissect.regf
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.regf
 
 A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration
 on Windows operating systems. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.regf/index.html).
 
 ## Requirements
```

### Comparing `dissect.regf-3.5.dev2/dissect/regf/c_regf.py` & `dissect.regf-3.6.dev1/dissect/regf/c_regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.5.dev2/dissect/regf/regf.py` & `dissect.regf-3.6.dev1/dissect/regf/regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.5.dev2/dissect.regf.egg-info/PKG-INFO` & `dissect.regf-3.6.dev1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.regf
-Version: 3.5.dev2
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.regf
 Project-URL: repository, https://github.com/fox-it/dissect.regf
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
 
 # dissect.regf
```

### Comparing `dissect.regf-3.5.dev2/pyproject.toml` & `dissect.regf-3.6.dev1/pyproject.toml`

 * *Files 21% similar despite different names*

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
 dependencies = [
     "dissect.cstruct>=3.0.dev,<4.0.dev",
     "dissect.util>=3.0.dev,<4.0.dev",
 ]
 dynamic = ["version"]
```

### Comparing `dissect.regf-3.5.dev2/tests/data/SYSTEM.gz` & `dissect.regf-3.6.dev1/tests/data/SYSTEM.gz`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.5.dev2/tests/docs/Makefile` & `dissect.regf-3.6.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.5.dev2/tests/docs/conf.py` & `dissect.regf-3.6.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.5.dev2/tests/test_regf.py` & `dissect.regf-3.6.dev1/tests/test_regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.5.dev2/tox.ini` & `dissect.regf-3.6.dev1/tox.ini`

 * *Files identical despite different names*

