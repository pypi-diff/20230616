# Comparing `tmp/twiss-0.1.0.tar.gz` & `tmp/twiss-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twiss-0.1.0.tar", last modified: Mon May 22 04:05:29 2023, max compression
+gzip compressed data, was "twiss-0.1.1.tar", last modified: Fri Jun 16 19:50:46 2023, max compression
```

## Comparing `twiss-0.1.0.tar` & `twiss-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-22 04:05:29.900697 twiss-0.1.0/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1799 2023-05-22 04:02:39.000000 twiss-0.1.0/.gitignore
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      152 2023-05-22 04:02:39.000000 twiss-0.1.0/.readthedocs.yml
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2023-05-22 04:02:39.000000 twiss-0.1.0/LICENSE
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2685 2023-05-22 04:05:29.900697 twiss-0.1.0/PKG-INFO
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2272 2023-05-22 04:02:39.000000 twiss-0.1.0/README.MD
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-22 04:05:29.900697 twiss-0.1.0/docs/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/Makefile
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/make.bat
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       25 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/requirements.txt
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-22 04:05:29.900697 twiss-0.1.0/docs/source/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2137 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/conf.py
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-22 04:05:29.900697 twiss-0.1.0/docs/source/examples/
--rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)   203608 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/examples/twiss.ipynb
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      539 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/index.rst
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-22 04:05:29.900697 twiss-0.1.0/docs/source/modules/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/modules/convert.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/modules/invariant.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       40 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/modules/math.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/modules/matrix.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/modules/normal.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/modules/transport.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-22 04:02:39.000000 twiss-0.1.0/docs/source/modules/twiss.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      561 2023-05-22 04:02:39.000000 twiss-0.1.0/pyproject.toml
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2023-05-22 04:05:29.900697 twiss-0.1.0/setup.cfg
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-22 04:05:29.900697 twiss-0.1.0/twiss/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        0 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss/__init__.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     4427 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss/convert.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3165 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss/invariant.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      716 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss/math.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6134 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss/matrix.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5994 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss/normal.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7434 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss/transport.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7472 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss/twiss.py
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-22 04:05:29.900697 twiss-0.1.0/twiss.egg-info/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2685 2023-05-22 04:05:29.000000 twiss-0.1.0/twiss.egg-info/PKG-INFO
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      696 2023-05-22 04:05:29.000000 twiss-0.1.0/twiss.egg-info/SOURCES.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2023-05-22 04:05:29.000000 twiss-0.1.0/twiss.egg-info/dependency_links.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       13 2023-05-22 04:05:29.000000 twiss-0.1.0/twiss.egg-info/requires.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        6 2023-05-22 04:05:29.000000 twiss-0.1.0/twiss.egg-info/top_level.txt
--rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)   203608 2023-05-22 04:02:39.000000 twiss-0.1.0/twiss.ipynb
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-16 19:50:46.919291 twiss-0.1.1/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1799 2023-05-17 05:51:35.000000 twiss-0.1.1/.gitignore
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      152 2023-05-17 05:51:39.000000 twiss-0.1.1/.readthedocs.yml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2023-05-17 05:51:18.000000 twiss-0.1.1/LICENSE
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2685 2023-06-16 19:50:46.919291 twiss-0.1.1/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2272 2023-05-20 17:41:48.000000 twiss-0.1.1/README.MD
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-16 19:50:46.915291 twiss-0.1.1/docs/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2023-05-20 17:06:50.000000 twiss-0.1.1/docs/Makefile
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2023-05-20 17:06:46.000000 twiss-0.1.1/docs/make.bat
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       25 2023-05-20 05:02:26.000000 twiss-0.1.1/docs/requirements.txt
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-16 19:50:46.915291 twiss-0.1.1/docs/source/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2137 2023-05-20 17:14:30.000000 twiss-0.1.1/docs/source/conf.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-16 19:50:46.915291 twiss-0.1.1/docs/source/examples/
+-rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)   203608 2023-05-20 17:06:12.000000 twiss-0.1.1/docs/source/examples/twiss.ipynb
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      539 2023-05-20 17:24:19.000000 twiss-0.1.1/docs/source/index.rst
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-16 19:50:46.915291 twiss-0.1.1/docs/source/modules/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-05-20 17:12:36.000000 twiss-0.1.1/docs/source/modules/convert.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2023-05-20 17:12:08.000000 twiss-0.1.1/docs/source/modules/invariant.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       40 2023-05-20 17:11:50.000000 twiss-0.1.1/docs/source/modules/math.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-20 17:11:59.000000 twiss-0.1.1/docs/source/modules/matrix.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-20 17:12:44.000000 twiss-0.1.1/docs/source/modules/normal.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2023-05-20 17:12:49.000000 twiss-0.1.1/docs/source/modules/transport.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-20 17:12:57.000000 twiss-0.1.1/docs/source/modules/twiss.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      561 2023-06-16 19:47:54.000000 twiss-0.1.1/pyproject.toml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2023-06-16 19:50:46.919291 twiss-0.1.1/setup.cfg
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-16 19:50:46.919291 twiss-0.1.1/twiss/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        0 2023-05-17 05:52:32.000000 twiss-0.1.1/twiss/__init__.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     4427 2023-05-20 17:17:21.000000 twiss-0.1.1/twiss/convert.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3165 2023-05-20 17:17:31.000000 twiss-0.1.1/twiss/invariant.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      716 2023-05-20 17:17:38.000000 twiss-0.1.1/twiss/math.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6134 2023-05-20 17:18:09.000000 twiss-0.1.1/twiss/matrix.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5994 2023-05-20 17:18:02.000000 twiss-0.1.1/twiss/normal.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7434 2023-05-20 18:08:01.000000 twiss-0.1.1/twiss/transport.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7473 2023-06-16 19:44:04.000000 twiss-0.1.1/twiss/twiss.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-16 19:50:46.919291 twiss-0.1.1/twiss.egg-info/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2685 2023-06-16 19:50:46.000000 twiss-0.1.1/twiss.egg-info/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      696 2023-06-16 19:50:46.000000 twiss-0.1.1/twiss.egg-info/SOURCES.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2023-06-16 19:50:46.000000 twiss-0.1.1/twiss.egg-info/dependency_links.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       13 2023-06-16 19:50:46.000000 twiss-0.1.1/twiss.egg-info/requires.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        6 2023-06-16 19:50:46.000000 twiss-0.1.1/twiss.egg-info/top_level.txt
+-rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)   203608 2023-05-20 17:06:12.000000 twiss-0.1.1/twiss.ipynb
```

### Comparing `twiss-0.1.0/.gitignore` & `twiss-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/LICENSE` & `twiss-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/PKG-INFO` & `twiss-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twiss
-Version: 0.1.0
+Version: 0.1.1
 Summary: Differentiable Wolski twiss matrices computation for arbitrary dimension stable symplectic matrices
 Author-email: Ivan Morozov <i.a.morozov@inp.nsk.su>
 License: MIT
 Keywords: torch,twiss,differentiable,symplectic,matrix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `twiss-0.1.0/README.MD` & `twiss-0.1.1/README.MD`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/docs/Makefile` & `twiss-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/docs/make.bat` & `twiss-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/docs/source/conf.py` & `twiss-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/docs/source/examples/twiss.ipynb` & `twiss-0.1.1/docs/source/examples/twiss.ipynb`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/docs/source/index.rst` & `twiss-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/pyproject.toml` & `twiss-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twiss"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name = "Ivan Morozov", email = "i.a.morozov@inp.nsk.su"}]
 description = "Differentiable Wolski twiss matrices computation for arbitrary dimension stable symplectic matrices"
 readme = "README.MD"
 requires-python = ">=3.10"
 keywords = ["torch", "twiss", "differentiable", "symplectic", "matrix"]
 license = {text = "MIT"}
 classifiers = ["Programming Language :: Python :: 3"]
```

### Comparing `twiss-0.1.0/twiss/convert.py` & `twiss-0.1.1/twiss/convert.py`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/twiss/invariant.py` & `twiss-0.1.1/twiss/invariant.py`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/twiss/math.py` & `twiss-0.1.1/twiss/math.py`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/twiss/matrix.py` & `twiss-0.1.1/twiss/matrix.py`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/twiss/normal.py` & `twiss-0.1.1/twiss/normal.py`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/twiss/transport.py` & `twiss-0.1.1/twiss/transport.py`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/twiss/twiss.py` & `twiss-0.1.1/twiss/twiss.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .matrix import rotation
 
 def twiss(m:Tensor, *,
           epsilon:float=1.0E-12) -> tuple[Tensor, Tensor, Tensor]:
     """
     Compute coupled Wolski twiss parameters for a given one-turn input matrix
     
-    Returns fractionaltunes, normalization matrix (standard gauge) and Wolski twiss matrices
+    Returns fractional tunes, normalization matrix (standard gauge) and Wolski twiss matrices
     
     Input matrix can have arbitrary even dimension
     Input matrix stability is not checked
 
     Symplectic block is [[0, 1], [-1, 0]]
     Rotation block is [[cos(alpha), sin(alpha)], [-sin(alpha), cos(alpha)]]
     Complex block is 1/sqrt(2)*[[1, 1j], [1, -1j]]
```

### Comparing `twiss-0.1.0/twiss.egg-info/PKG-INFO` & `twiss-0.1.1/twiss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twiss
-Version: 0.1.0
+Version: 0.1.1
 Summary: Differentiable Wolski twiss matrices computation for arbitrary dimension stable symplectic matrices
 Author-email: Ivan Morozov <i.a.morozov@inp.nsk.su>
 License: MIT
 Keywords: torch,twiss,differentiable,symplectic,matrix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `twiss-0.1.0/twiss.egg-info/SOURCES.txt` & `twiss-0.1.1/twiss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twiss-0.1.0/twiss.ipynb` & `twiss-0.1.1/twiss.ipynb`

 * *Files identical despite different names*

