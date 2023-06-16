# Comparing `tmp/dissect.fat-3.5.dev2.tar.gz` & `tmp/dissect.fat-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.fat-3.5.dev2.tar", last modified: Tue May 16 13:26:04 2023, max compression
+gzip compressed data, was "dissect.fat-3.6.dev1.tar", last modified: Fri Jun 16 12:49:54 2023, max compression
```

## Comparing `dissect.fat-3.5.dev2.tar` & `dissect.fat-3.6.dev1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.590538 dissect.fat-3.5.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-16 13:26:04.590538 dissect.fat-3.5.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.546538 dissect.fat-3.5.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.550538 dissect.fat-3.5.dev2/dissect/fat/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/c_exfat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/c_fat.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/exfat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/fat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.546538 dissect.fat-3.5.dev2/dissect.fat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-16 13:25:54.000000 dissect.fat-3.5.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:04.590538 dissect.fat-3.5.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.550538 dissect.fat-3.5.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.554538 dissect.fat-3.5.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/data/exfat.bin
--rw-r--r--   0 runner    (1001) docker     (123)  1474560 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/data/fat12.bin
--rw-r--r--   0 runner    (1001) docker     (123)  3072000 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/data/fat16.bin
--rw-r--r--   0 runner    (1001) docker     (123) 34304000 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/data/fat32.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.590538 dissect.fat-3.5.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/test_exfat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/test_fat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.508628 dissect.fat-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-16 12:49:54.508628 dissect.fat-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.432628 dissect.fat-3.6.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.440628 dissect.fat-3.6.dev1/dissect/fat/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/dissect/fat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/dissect/fat/c_exfat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/dissect/fat/c_fat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/dissect/fat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/dissect/fat/exfat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/dissect/fat/fat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.436628 dissect.fat-3.6.dev1/dissect.fat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-16 12:49:54.000000 dissect.fat-3.6.dev1/dissect.fat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-16 12:49:54.000000 dissect.fat-3.6.dev1/dissect.fat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:49:54.000000 dissect.fat-3.6.dev1/dissect.fat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:49:54.000000 dissect.fat-3.6.dev1/dissect.fat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:49:54.000000 dissect.fat-3.6.dev1/dissect.fat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-16 12:49:41.000000 dissect.fat-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:49:54.508628 dissect.fat-3.6.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.444628 dissect.fat-3.6.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.452628 dissect.fat-3.6.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/data/exfat.bin
+-rw-r--r--   0 runner    (1001) docker     (123)  1474560 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/data/fat12.bin
+-rw-r--r--   0 runner    (1001) docker     (123)  3072000 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/data/fat16.bin
+-rw-r--r--   0 runner    (1001) docker     (123) 34304000 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/data/fat32.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.508628 dissect.fat-3.6.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/test_exfat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tests/test_fat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:49:36.000000 dissect.fat-3.6.dev1/tox.ini
```

### Comparing `dissect.fat-3.5.dev2/LICENSE` & `dissect.fat-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/PKG-INFO` & `dissect.fat-3.6.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.fat
-Version: 3.5.dev2
+Version: 3.6.dev1
 Summary: A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage devices and UEFI partitions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.fat
 Project-URL: repository, https://github.com/fox-it/dissect.fat
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
 
 # dissect.fat
```

### Comparing `dissect.fat-3.5.dev2/README.md` & `dissect.fat-3.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/dissect/fat/__init__.py` & `dissect.fat-3.6.dev1/dissect/fat/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/dissect/fat/c_exfat.py` & `dissect.fat-3.6.dev1/dissect/fat/c_exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/dissect/fat/c_fat.py` & `dissect.fat-3.6.dev1/dissect/fat/c_fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/dissect/fat/exfat.py` & `dissect.fat-3.6.dev1/dissect/fat/exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/dissect/fat/fat.py` & `dissect.fat-3.6.dev1/dissect/fat/fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/dissect.fat.egg-info/PKG-INFO` & `dissect.fat-3.6.dev1/dissect.fat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.fat
-Version: 3.5.dev2
+Version: 3.6.dev1
 Summary: A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage devices and UEFI partitions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.fat
 Project-URL: repository, https://github.com/fox-it/dissect.fat
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
 
 # dissect.fat
```

### Comparing `dissect.fat-3.5.dev2/dissect.fat.egg-info/SOURCES.txt` & `dissect.fat-3.6.dev1/dissect.fat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/pyproject.toml` & `dissect.fat-3.6.dev1/pyproject.toml`

 * *Files 15% similar despite different names*

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

### Comparing `dissect.fat-3.5.dev2/tests/conftest.py` & `dissect.fat-3.6.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tests/data/exfat.bin` & `dissect.fat-3.6.dev1/tests/data/exfat.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tests/data/fat12.bin` & `dissect.fat-3.6.dev1/tests/data/fat12.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tests/data/fat16.bin` & `dissect.fat-3.6.dev1/tests/data/fat16.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tests/data/fat32.bin` & `dissect.fat-3.6.dev1/tests/data/fat32.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tests/docs/Makefile` & `dissect.fat-3.6.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tests/docs/conf.py` & `dissect.fat-3.6.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tests/test_exfat.py` & `dissect.fat-3.6.dev1/tests/test_exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tests/test_fat.py` & `dissect.fat-3.6.dev1/tests/test_fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev2/tox.ini` & `dissect.fat-3.6.dev1/tox.ini`

 * *Files identical despite different names*

