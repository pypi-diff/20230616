# Comparing `tmp/dissect-3.6.dev2.tar.gz` & `tmp/dissect-3.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect-3.6.dev2.tar", last modified: Thu May 25 08:03:54 2023, max compression
+gzip compressed data, was "dissect-3.7.dev1.tar", last modified: Fri Jun 16 12:48:28 2023, max compression
```

## Comparing `dissect-3.6.dev2.tar` & `dissect-3.7.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:03:54.308419 dissect-3.6.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 08:03:36.000000 dissect-3.6.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 08:03:36.000000 dissect-3.6.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 08:03:36.000000 dissect-3.6.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-25 08:03:54.308419 dissect-3.6.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-25 08:03:36.000000 dissect-3.6.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:03:54.308419 dissect-3.6.dev2/dissect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:03:54.000000 dissect-3.6.dev2/dissect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-25 08:03:42.000000 dissect-3.6.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 08:03:54.312419 dissect-3.6.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-25 08:03:36.000000 dissect-3.6.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:28.847288 dissect-3.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-16 12:48:15.000000 dissect-3.7.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:48:15.000000 dissect-3.7.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:15.000000 dissect-3.7.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-16 12:48:28.847288 dissect-3.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-16 12:48:15.000000 dissect-3.7.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:28.847288 dissect-3.7.dev1/dissect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-16 12:48:19.000000 dissect-3.7.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:48:28.847288 dissect-3.7.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-16 12:48:15.000000 dissect-3.7.dev1/tox.ini
```

### Comparing `dissect-3.6.dev2/LICENSE` & `dissect-3.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect-3.6.dev2/PKG-INFO` & `dissect-3.7.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.6.dev2
+Version: 3.7.dev1
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
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
 
 # dissect
```

### Comparing `dissect-3.6.dev2/README.md` & `dissect-3.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect-3.6.dev2/dissect.egg-info/PKG-INFO` & `dissect-3.7.dev1/dissect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.6.dev2
+Version: 3.7.dev1
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
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
 
 # dissect
```

### Comparing `dissect-3.6.dev2/tox.ini` & `dissect-3.7.dev1/tox.ini`

 * *Files identical despite different names*

