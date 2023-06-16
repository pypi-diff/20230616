# Comparing `tmp/VLCDA-1.0.1.tar.gz` & `tmp/VLCDA-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VLCDA-1.0.1.tar", last modified: Fri Jun 16 00:29:28 2023, max compression
+gzip compressed data, was "VLCDA-1.0.2.tar", last modified: Fri Jun 16 00:32:04 2023, max compression
```

## Comparing `VLCDA-1.0.1.tar` & `VLCDA-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 00:29:28.341119 VLCDA-1.0.1/
--rw-rw-rw-   0        0        0     1077 2023-06-16 00:19:36.000000 VLCDA-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      592 2023-06-16 00:29:28.340124 VLCDA-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      922 2023-06-16 00:29:05.000000 VLCDA-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 00:29:28.310246 VLCDA-1.0.1/VLCDA/
--rw-rw-rw-   0        0        0    19570 2023-06-16 00:20:07.000000 VLCDA-1.0.1/VLCDA/Logic_Circuits_Evolution.py
--rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 VLCDA-1.0.1/VLCDA/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:29:28.337108 VLCDA-1.0.1/VLCDA.egg-info/
--rw-rw-rw-   0        0        0      592 2023-06-16 00:29:27.000000 VLCDA-1.0.1/VLCDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-06-16 00:29:28.000000 VLCDA-1.0.1/VLCDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 00:29:27.000000 VLCDA-1.0.1/VLCDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 00:29:27.000000 VLCDA-1.0.1/VLCDA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 00:29:28.342129 VLCDA-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      654 2023-06-16 00:29:13.000000 VLCDA-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:32:04.093872 VLCDA-1.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-06-16 00:19:36.000000 VLCDA-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      592 2023-06-16 00:32:04.100401 VLCDA-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1406 2023-06-16 00:30:13.000000 VLCDA-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 00:32:04.062755 VLCDA-1.0.2/VLCDA/
+-rw-rw-rw-   0        0        0    19570 2023-06-16 00:20:07.000000 VLCDA-1.0.2/VLCDA/Logic_Circuits_Evolution.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 VLCDA-1.0.2/VLCDA/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:32:04.089866 VLCDA-1.0.2/VLCDA.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-06-16 00:32:03.000000 VLCDA-1.0.2/VLCDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-06-16 00:32:03.000000 VLCDA-1.0.2/VLCDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 00:32:03.000000 VLCDA-1.0.2/VLCDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 00:32:03.000000 VLCDA-1.0.2/VLCDA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-16 00:32:04.103396 VLCDA-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      654 2023-06-16 00:31:56.000000 VLCDA-1.0.2/setup.py
```

### Comparing `VLCDA-1.0.1/LICENSE.txt` & `VLCDA-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.1/PKG-INFO` & `VLCDA-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VLCDA
-Version: 1.0.1
+Version: 1.0.2
 Summary: Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos
 Home-page: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Download-URL: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Author: Humberto Távora, Stefan Blawid, Yasmin Maria
 License: UNKNOWN
 Keywords: Genetic,Algorithm,Logic Circuits,Evolution,Optimization
 Platform: UNKNOWN
```

### Comparing `VLCDA-1.0.1/README.md` & `VLCDA-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,7 +13,36 @@
 > Mind you, these are characteristics of biological systems shaped by evolution. algorithms
 > genetics can be used for the synthesis of digital systems when hard-
 > fully integrated ware, such as those imposed by programmable devices.
 > It has even been pointed out that as digital circuits evolve, fault handling strategies
 > recognized by evolution reappear naturally.
 
 
+## Installation
+
+VEDA module requires [Python 3](https://www.python.org/) and some basics modules to run. 
+
+- Random
+- Datetime
+- Bisect
+
+If you don't have theses modules, run the following commands:
+
+```sh
+pip install random
+pip install datetime
+pip install bisect
+```
+
+To install the module VEDA run the following commands...
+
+```sh
+pip install VEDA
+```
+Be sure to maintain pip updated ...
+```sh
+python -m pip install --upgrade pip
+```
+## License
+
+MIT
+
```

### Comparing `VLCDA-1.0.1/VLCDA/Logic_Circuits_Evolution.py` & `VLCDA-1.0.2/VLCDA/Logic_Circuits_Evolution.py`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.1/VLCDA.egg-info/PKG-INFO` & `VLCDA-1.0.2/VLCDA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VLCDA
-Version: 1.0.1
+Version: 1.0.2
 Summary: Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos
 Home-page: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Download-URL: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Author: Humberto Távora, Stefan Blawid, Yasmin Maria
 License: UNKNOWN
 Keywords: Genetic,Algorithm,Logic Circuits,Evolution,Optimization
 Platform: UNKNOWN
```

### Comparing `VLCDA-1.0.1/setup.py` & `VLCDA-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name = "VLCDA",
-    version = "1.0.1",
+    version = "1.0.2",
     description = "Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos",
     author = "Humberto Távora, Stefan Blawid, Yasmin Maria",
     url = 'https://github.com/HumbertoTavora/Logic-Circuits-Evolution',
     download_url = 'https://github.com/HumbertoTavora/Logic-Circuits-Evolution',
     keywords = ['Genetic', 'Algorithm', 'Logic Circuits', 'Evolution', 'Optimization'],
     classifiers=['Programming Language :: Python :: 3','Intended Audience :: Developers'],
     packages=find_packages()
```

