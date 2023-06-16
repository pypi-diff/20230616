# Comparing `tmp/UComp-1.0.66.tar.gz` & `tmp/UComp-1.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.66.tar", last modified: Fri Jun 16 11:35:47 2023, max compression
+gzip compressed data, was "UComp-1.0.68.tar", last modified: Fri Jun 16 11:37:51 2023, max compression
```

## Comparing `UComp-1.0.66.tar` & `UComp-1.0.68.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:35:47.095420 UComp-1.0.66/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.66/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-16 11:35:47.096417 UComp-1.0.66/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.66/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 11:35:47.052484 UComp-1.0.66/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.66/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.66/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:39:21.000000 UComp-1.0.66/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11787 2023-06-16 10:57:22.000000 UComp-1.0.66/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.66/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   897024 2023-06-16 11:32:46.000000 UComp-1.0.66/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24515 2023-06-16 08:39:16.000000 UComp-1.0.66/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.66/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.66/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.66/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.66/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.66/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29804 2023-06-16 08:39:05.000000 UComp-1.0.66/UComp/tools.py
--rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.66/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:35:47.092434 UComp-1.0.66/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-16 11:35:46.000000 UComp-1.0.66/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-16 11:35:46.000000 UComp-1.0.66/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 11:35:46.000000 UComp-1.0.66/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-16 11:35:46.000000 UComp-1.0.66/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 11:35:46.000000 UComp-1.0.66/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 11:35:47.099408 UComp-1.0.66/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-16 11:35:35.000000 UComp-1.0.66/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:37:51.142896 UComp-1.0.68/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.68/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-16 11:37:51.142896 UComp-1.0.68/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.68/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 11:37:51.114137 UComp-1.0.68/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.68/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.68/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11378 2023-06-16 11:36:35.000000 UComp-1.0.68/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11787 2023-06-16 11:36:22.000000 UComp-1.0.68/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.68/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   897024 2023-06-16 11:32:46.000000 UComp-1.0.68/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24515 2023-06-16 11:36:30.000000 UComp-1.0.68/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.68/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.68/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.68/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.68/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.68/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29804 2023-06-16 11:36:12.000000 UComp-1.0.68/UComp/tools.py
+-rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.68/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:37:51.140859 UComp-1.0.68/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 11:37:51.145853 UComp-1.0.68/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-16 11:37:45.000000 UComp-1.0.68/setup.py
```

### Comparing `UComp-1.0.66/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.68/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/ETSmodule.py` & `UComp-1.0.68/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/PTSmodule.py` & `UComp-1.0.68/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.68/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/UCmodule.py` & `UComp-1.0.68/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/airpas.bin` & `UComp-1.0.68/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/gdp.bin` & `UComp-1.0.68/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/ipi.bin` & `UComp-1.0.68/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/libopenblas.dll` & `UComp-1.0.68/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/tools.py` & `UComp-1.0.68/UComp/tools.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/UComp/tsfile.py` & `UComp-1.0.68/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.66/setup.py` & `UComp-1.0.68/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.66',
+    version='1.0.68',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

