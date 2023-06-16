# Comparing `tmp/dissect.cim-3.6.dev2.tar.gz` & `tmp/dissect.cim-3.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.cim-3.6.dev2.tar", last modified: Tue May 16 13:25:38 2023, max compression
+gzip compressed data, was "dissect.cim-3.7.dev1.tar", last modified: Fri Jun 16 12:48:33 2023, max compression
```

## Comparing `dissect.cim-3.6.dev2.tar` & `dissect.cim-3.7.dev1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:38.313893 dissect.cim-3.6.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-16 13:25:38.313893 dissect.cim-3.6.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:38.277893 dissect.cim-3.6.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:38.293893 dissect.cim-3.6.dev2/dissect/cim/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/c_cim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/cim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/dissect/cim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:38.285893 dissect.cim-3.6.dev2/dissect.cim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-16 13:25:38.000000 dissect.cim-3.6.dev2/dissect.cim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 13:25:38.000000 dissect.cim-3.6.dev2/dissect.cim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:38.000000 dissect.cim-3.6.dev2/dissect.cim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:25:38.000000 dissect.cim-3.6.dev2/dissect.cim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:38.000000 dissect.cim-3.6.dev2/dissect.cim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-16 13:25:23.000000 dissect.cim-3.6.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:38.313893 dissect.cim-3.6.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:38.297893 dissect.cim-3.6.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:38.305893 dissect.cim-3.6.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2018815 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/data/INDEX.BTR.gz
--rw-r--r--   0 runner    (1001) docker     (123)    29367 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/data/MAPPING1.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (123)    29375 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/data/MAPPING2.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/data/MAPPING3.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (123)  4105816 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/data/OBJECTS.DATA.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:38.313893 dissect.cim-3.6.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tests/test_cim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:16.000000 dissect.cim-3.6.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:33.905687 dissect.cim-3.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-16 12:48:33.905687 dissect.cim-3.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:33.893687 dissect.cim-3.7.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:33.897687 dissect.cim-3.7.dev1/dissect/cim/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/c_cim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/cim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/dissect/cim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:33.897687 dissect.cim-3.7.dev1/dissect.cim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-16 12:48:33.000000 dissect.cim-3.7.dev1/dissect.cim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-16 12:48:33.000000 dissect.cim-3.7.dev1/dissect.cim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:33.000000 dissect.cim-3.7.dev1/dissect.cim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:48:33.000000 dissect.cim-3.7.dev1/dissect.cim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:48:33.000000 dissect.cim-3.7.dev1/dissect.cim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-16 12:48:23.000000 dissect.cim-3.7.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:48:33.905687 dissect.cim-3.7.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:33.897687 dissect.cim-3.7.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:33.901687 dissect.cim-3.7.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2018815 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/data/INDEX.BTR.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    29367 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/data/MAPPING1.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    29375 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/data/MAPPING2.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/data/MAPPING3.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  4105816 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/data/OBJECTS.DATA.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:33.905687 dissect.cim-3.7.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tests/test_cim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:48:19.000000 dissect.cim-3.7.dev1/tox.ini
```

### Comparing `dissect.cim-3.6.dev2/LICENSE` & `dissect.cim-3.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/PKG-INFO` & `dissect.cim-3.7.dev1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.cim
-Version: 3.6.dev2
+Version: 3.7.dev1
 Summary: A Dissect module implementing a parser for the Windows Common Information Model (CIM) database, used in the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cim
 Project-URL: repository, https://github.com/fox-it/dissect.cim
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
 
 # dissect.cim
```

### Comparing `dissect.cim-3.6.dev2/README.md` & `dissect.cim-3.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/dissect/cim/c_cim.py` & `dissect.cim-3.7.dev1/dissect/cim/c_cim.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/dissect/cim/cim.py` & `dissect.cim-3.7.dev1/dissect/cim/cim.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/dissect/cim/classes.py` & `dissect.cim-3.7.dev1/dissect/cim/classes.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/dissect/cim/index.py` & `dissect.cim-3.7.dev1/dissect/cim/index.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/dissect/cim/mappings.py` & `dissect.cim-3.7.dev1/dissect/cim/mappings.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/dissect/cim/objects.py` & `dissect.cim-3.7.dev1/dissect/cim/objects.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/dissect/cim/utils.py` & `dissect.cim-3.7.dev1/dissect/cim/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/dissect.cim.egg-info/PKG-INFO` & `dissect.cim-3.7.dev1/dissect.cim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.cim
-Version: 3.6.dev2
+Version: 3.7.dev1
 Summary: A Dissect module implementing a parser for the Windows Common Information Model (CIM) database, used in the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cim
 Project-URL: repository, https://github.com/fox-it/dissect.cim
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
 
 # dissect.cim
```

### Comparing `dissect.cim-3.6.dev2/dissect.cim.egg-info/SOURCES.txt` & `dissect.cim-3.7.dev1/dissect.cim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/pyproject.toml` & `dissect.cim-3.7.dev1/pyproject.toml`

 * *Files 22% similar despite different names*

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

### Comparing `dissect.cim-3.6.dev2/tests/conftest.py` & `dissect.cim-3.7.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/tests/data/INDEX.BTR.gz` & `dissect.cim-3.7.dev1/tests/data/INDEX.BTR.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/tests/data/MAPPING1.MAP.gz` & `dissect.cim-3.7.dev1/tests/data/MAPPING1.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/tests/data/MAPPING2.MAP.gz` & `dissect.cim-3.7.dev1/tests/data/MAPPING2.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/tests/data/MAPPING3.MAP.gz` & `dissect.cim-3.7.dev1/tests/data/MAPPING3.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/tests/data/OBJECTS.DATA.gz` & `dissect.cim-3.7.dev1/tests/data/OBJECTS.DATA.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/tests/docs/Makefile` & `dissect.cim-3.7.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/tests/docs/conf.py` & `dissect.cim-3.7.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.6.dev2/tox.ini` & `dissect.cim-3.7.dev1/tox.ini`

 * *Files identical despite different names*

