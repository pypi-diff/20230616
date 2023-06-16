# Comparing `tmp/climalysis-0.1.0.tar.gz` & `tmp/climalysis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climalysis-0.1.0.tar", last modified: Sun Jun 11 18:30:09 2023, max compression
+gzip compressed data, was "climalysis-0.2.0.tar", last modified: Fri Jun 16 17:38:58 2023, max compression
```

## Comparing `climalysis-0.1.0.tar` & `climalysis-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:30:09.183936 climalysis-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-11 18:29:53.000000 climalysis-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-11 18:30:09.183936 climalysis-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-11 18:29:53.000000 climalysis-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:30:09.179936 climalysis-0.1.0/climalysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:29:53.000000 climalysis-0.1.0/climalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:29:53.000000 climalysis-0.1.0/climalysis/module1.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:29:53.000000 climalysis-0.1.0/climalysis/module2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:30:09.183936 climalysis-0.1.0/climalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-11 18:30:09.000000 climalysis-0.1.0/climalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-11 18:30:09.000000 climalysis-0.1.0/climalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:30:09.000000 climalysis-0.1.0/climalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-11 18:30:09.000000 climalysis-0.1.0/climalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-11 18:30:09.000000 climalysis-0.1.0/climalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:30:09.183936 climalysis-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-11 18:29:53.000000 climalysis-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:30:09.183936 climalysis-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:29:53.000000 climalysis-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:29:53.000000 climalysis-0.1.0/tests/test_module1.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:29:53.000000 climalysis-0.1.0/tests/test_module2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:58.604428 climalysis-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 17:38:44.000000 climalysis-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-16 17:38:58.604428 climalysis-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-16 17:38:44.000000 climalysis-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:58.604428 climalysis-0.2.0/climalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:38:58.604428 climalysis-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-16 17:38:44.000000 climalysis-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:58.604428 climalysis-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:44.000000 climalysis-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:44.000000 climalysis-0.2.0/tests/test_module1.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:44.000000 climalysis-0.2.0/tests/test_module2.py
```

### Comparing `climalysis-0.1.0/LICENSE` & `climalysis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climalysis-0.1.0/PKG-INFO` & `climalysis-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: climalysis
-Version: 0.1.0
+Version: 0.2.0
 Summary: A comprehensive toolkit for climate impact analysis.
 Author: Jake Casselman
 Author-email: <jake.casselman@climalinks.com
 Keywords: python,climate,analysis,climate analysis,climate data,impact analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Climalysis: Your Toolkit for Climate Impact Analysis ☁️🌞
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) 
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/652251221.svg)](https://zenodo.org/badge/latestdoi/652251221)
 
-Developed by some of the current and past members of ETH's Subseasonal to Seasonal research group, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
+
+
+Developed by an assortment of active and past climate researchers, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
 
 **Our Mission:**
 
 We aim to:
 - Democratize climate research, bringing advanced tools and methods into the public sphere.
 - Foster collaboration and accelerate climate-related discoveries.
 - Involve everyone in the climate conversation - researchers, analysts, and enthusiasts alike.
```

### Comparing `climalysis-0.1.0/README.md` & `climalysis-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Climalysis: Your Toolkit for Climate Impact Analysis ☁️🌞
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) 
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/652251221.svg)](https://zenodo.org/badge/latestdoi/652251221)
 
-Developed by some of the current and past members of ETH's Subseasonal to Seasonal research group, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
+
+
+Developed by an assortment of active and past climate researchers, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
 
 **Our Mission:**
 
 We aim to:
 - Democratize climate research, bringing advanced tools and methods into the public sphere.
 - Foster collaboration and accelerate climate-related discoveries.
 - Involve everyone in the climate conversation - researchers, analysts, and enthusiasts alike.
```

### Comparing `climalysis-0.1.0/climalysis.egg-info/PKG-INFO` & `climalysis-0.2.0/climalysis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: climalysis
-Version: 0.1.0
+Version: 0.2.0
 Summary: A comprehensive toolkit for climate impact analysis.
 Author: Jake Casselman
 Author-email: <jake.casselman@climalinks.com
 Keywords: python,climate,analysis,climate analysis,climate data,impact analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Climalysis: Your Toolkit for Climate Impact Analysis ☁️🌞
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) 
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/652251221.svg)](https://zenodo.org/badge/latestdoi/652251221)
 
-Developed by some of the current and past members of ETH's Subseasonal to Seasonal research group, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
+
+
+Developed by an assortment of active and past climate researchers, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
 
 **Our Mission:**
 
 We aim to:
 - Democratize climate research, bringing advanced tools and methods into the public sphere.
 - Foster collaboration and accelerate climate-related discoveries.
 - Involve everyone in the climate conversation - researchers, analysts, and enthusiasts alike.
```

### Comparing `climalysis-0.1.0/setup.py` & `climalysis-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 DESCRIPTION = 'A comprehensive toolkit for climate impact analysis.'
 LONG_DESCRIPTION = 'A package that allows researchers, analysts, and climate enthusiasts to dissect complex climate data.'
 
 # Setting up
 setup(
     name="climalysis",
     version=VERSION,
```

