# Comparing `tmp/gerk-0.0.6.tar.gz` & `tmp/gerk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerk-0.0.6.tar", last modified: Fri Jun 16 00:55:09 2023, max compression
+gzip compressed data, was "gerk-0.0.7.tar", last modified: Fri Jun 16 00:57:08 2023, max compression
```

## Comparing `gerk-0.0.6.tar` & `gerk-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-16 00:55:09.221977 gerk-0.0.6/
--rw-r--r--   0 yasser     (501) staff       (20)     1093 2023-06-15 19:06:49.000000 gerk-0.0.6/LICENSE
--rw-r--r--   0 yasser     (501) staff       (20)    15435 2023-06-16 00:55:09.220863 gerk-0.0.6/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)    14974 2023-06-15 20:32:47.000000 gerk-0.0.6/README.md
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-16 00:55:09.214487 gerk-0.0.6/gerk/
--rw-r--r--   0 yasser     (501) staff       (20)       23 2023-06-15 20:05:46.000000 gerk-0.0.6/gerk/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     3277 2023-01-04 23:34:49.000000 gerk-0.0.6/gerk/_gerk_error.py
--rw-r--r--   0 yasser     (501) staff       (20)    10257 2023-06-15 19:26:27.000000 gerk-0.0.6/gerk/gerk.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-16 00:55:09.218526 gerk-0.0.6/gerk.egg-info/
--rw-r--r--   0 yasser     (501) staff       (20)    15435 2023-06-16 00:55:09.000000 gerk-0.0.6/gerk.egg-info/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)      215 2023-06-16 00:55:09.000000 gerk-0.0.6/gerk.egg-info/SOURCES.txt
--rw-r--r--   0 yasser     (501) staff       (20)        1 2023-06-16 00:55:09.000000 gerk-0.0.6/gerk.egg-info/dependency_links.txt
--rw-r--r--   0 yasser     (501) staff       (20)       17 2023-06-16 00:55:09.000000 gerk-0.0.6/gerk.egg-info/requires.txt
--rw-r--r--   0 yasser     (501) staff       (20)        5 2023-06-16 00:55:09.000000 gerk-0.0.6/gerk.egg-info/top_level.txt
--rw-r--r--   0 yasser     (501) staff       (20)       38 2023-06-16 00:55:09.222146 gerk-0.0.6/setup.cfg
--rw-r--r--   0 yasser     (501) staff       (20)      868 2023-06-16 00:54:56.000000 gerk-0.0.6/setup.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-16 00:57:08.239296 gerk-0.0.7/
+-rw-r--r--   0 yasser     (501) staff       (20)     1068 2023-06-16 00:56:38.000000 gerk-0.0.7/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)    15527 2023-06-16 00:57:08.238653 gerk-0.0.7/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)    15066 2023-06-16 00:56:38.000000 gerk-0.0.7/README.md
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-16 00:57:08.234244 gerk-0.0.7/gerk/
+-rw-r--r--   0 yasser     (501) staff       (20)       23 2023-06-15 20:05:46.000000 gerk-0.0.7/gerk/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3277 2023-01-04 23:34:49.000000 gerk-0.0.7/gerk/_gerk_error.py
+-rw-r--r--   0 yasser     (501) staff       (20)    10257 2023-06-15 19:26:27.000000 gerk-0.0.7/gerk/gerk.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-16 00:57:08.237950 gerk-0.0.7/gerk.egg-info/
+-rw-r--r--   0 yasser     (501) staff       (20)    15527 2023-06-16 00:57:08.000000 gerk-0.0.7/gerk.egg-info/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)      215 2023-06-16 00:57:08.000000 gerk-0.0.7/gerk.egg-info/SOURCES.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2023-06-16 00:57:08.000000 gerk-0.0.7/gerk.egg-info/dependency_links.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       17 2023-06-16 00:57:08.000000 gerk-0.0.7/gerk.egg-info/requires.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        5 2023-06-16 00:57:08.000000 gerk-0.0.7/gerk.egg-info/top_level.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       38 2023-06-16 00:57:08.239457 gerk-0.0.7/setup.cfg
+-rw-r--r--   0 yasser     (501) staff       (20)      868 2023-06-16 00:56:59.000000 gerk-0.0.7/setup.py
```

### Comparing `gerk-0.0.6/LICENSE` & `gerk-0.0.7/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-The MIT License (MIT)
+MIT License
 
-Copyright © 2023 <copyright holders>
+Copyright (c) 2023 Yasser Naji
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gerk-0.0.6/PKG-INFO` & `gerk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generalized Explicit Runge-Kutta
 Author: Yasser Naji
 Author-email: yfnaji@gmail.com
 Keywords: runge-kutta,runge,kutta,numerical,integration,approximation
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -12,14 +12,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Generalized Explicit Runge-Kutta (GERK)
 
 A package for the curious mathematicians and engineers who want to experiment the Runge-Kutta method with their own coefficients.
 
+[PyPI link](https://pypi.org/project/gerk/)
+
+[GitHub link](https://github.com/yfnaji/Gerk)
+
 # Contents
 
 1. [Runge-Kutta Overview](#rko)
 2. [What is Gerk?](#wig)
 3. [How to use Gerk](#h2ug)
     * [Attributes](#attr)
     * [Condition Arguments](#cond-arg)
```

### Comparing `gerk-0.0.6/README.md` & `gerk-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Generalized Explicit Runge-Kutta (GERK)
 
 A package for the curious mathematicians and engineers who want to experiment the Runge-Kutta method with their own coefficients.
 
+[PyPI link](https://pypi.org/project/gerk/)
+
+[GitHub link](https://github.com/yfnaji/Gerk)
+
 # Contents
 
 1. [Runge-Kutta Overview](#rko)
 2. [What is Gerk?](#wig)
 3. [How to use Gerk](#h2ug)
     * [Attributes](#attr)
     * [Condition Arguments](#cond-arg)
```

### Comparing `gerk-0.0.6/gerk/_gerk_error.py` & `gerk-0.0.7/gerk/_gerk_error.py`

 * *Files identical despite different names*

### Comparing `gerk-0.0.6/gerk/gerk.py` & `gerk-0.0.7/gerk/gerk.py`

 * *Files identical despite different names*

### Comparing `gerk-0.0.6/gerk.egg-info/PKG-INFO` & `gerk-0.0.7/gerk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generalized Explicit Runge-Kutta
 Author: Yasser Naji
 Author-email: yfnaji@gmail.com
 Keywords: runge-kutta,runge,kutta,numerical,integration,approximation
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -12,14 +12,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Generalized Explicit Runge-Kutta (GERK)
 
 A package for the curious mathematicians and engineers who want to experiment the Runge-Kutta method with their own coefficients.
 
+[PyPI link](https://pypi.org/project/gerk/)
+
+[GitHub link](https://github.com/yfnaji/Gerk)
+
 # Contents
 
 1. [Runge-Kutta Overview](#rko)
 2. [What is Gerk?](#wig)
 3. [How to use Gerk](#h2ug)
     * [Attributes](#attr)
     * [Condition Arguments](#cond-arg)
```

### Comparing `gerk-0.0.6/setup.py` & `gerk-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 import codecs
 import os
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "Generalized Explicit Runge-Kutta"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="gerk",
```

