# Comparing `tmp/piel-0.0.21.tar.gz` & `tmp/piel-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.21.tar", last modified: Sun Jun 11 12:51:05 2023, max compression
+gzip compressed data, was "piel-0.0.22.tar", last modified: Fri Jun 16 14:49:04 2023, max compression
```

## Comparing `piel-0.0.21.tar` & `piel-0.0.22.tar`

### file list

```diff
@@ -1,36 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.613807 piel-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-11 12:50:49.000000 piel-0.0.21/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-11 12:50:49.000000 piel-0.0.21/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 12:50:49.000000 piel-0.0.21/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-11 12:50:49.000000 piel-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 12:50:49.000000 piel-0.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-11 12:51:05.613807 piel-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-11 12:50:49.000000 piel-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.609807 piel-0.0.21/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-11 12:50:49.000000 piel-0.0.21/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 12:50:49.000000 piel-0.0.21/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-11 12:50:49.000000 piel-0.0.21/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 12:50:49.000000 piel-0.0.21/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 12:50:49.000000 piel-0.0.21/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-11 12:50:49.000000 piel-0.0.21/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-11 12:50:49.000000 piel-0.0.21/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-11 12:50:49.000000 piel-0.0.21/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 12:50:49.000000 piel-0.0.21/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-11 12:50:49.000000 piel-0.0.21/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.613807 piel-0.0.21/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-11 12:50:49.000000 piel-0.0.21/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-11 12:50:49.000000 piel-0.0.21/piel/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 12:50:49.000000 piel-0.0.21/piel/piel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.613807 piel-0.0.21/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-11 12:51:05.613807 piel-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-11 12:50:49.000000 piel-0.0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.613807 piel-0.0.21/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 12:50:49.000000 piel-0.0.21/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-11 12:50:49.000000 piel-0.0.21/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.372829 piel-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 14:48:39.000000 piel-0.0.22/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-16 14:48:39.000000 piel-0.0.22/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 14:48:39.000000 piel-0.0.22/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 14:48:39.000000 piel-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 14:48:39.000000 piel-0.0.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-16 14:49:04.372829 piel-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-16 14:48:39.000000 piel-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.364829 piel-0.0.22/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-16 14:48:39.000000 piel-0.0.22/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 14:48:39.000000 piel-0.0.22/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.364829 piel-0.0.22/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.364829 piel-0.0.22/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.364829 piel-0.0.22/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.364829 piel-0.0.22/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.364829 piel-0.0.22/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/file_system/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.364829 piel-0.0.22/docs/autoapi/piel/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/gdsfactory/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.364829 piel-0.0.22/docs/autoapi/piel/openlane_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/openlane_v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.368829 piel-0.0.22/docs/autoapi/piel/openlane_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/openlane_v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.368829 piel-0.0.22/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.368829 piel-0.0.22/docs/autoapi/piel/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.368829 piel-0.0.22/docs/autoapi/piel/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-16 14:48:39.000000 piel-0.0.22/docs/autoapi/piel/simulation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-16 14:48:39.000000 piel-0.0.22/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 14:48:39.000000 piel-0.0.22/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.360829 piel-0.0.22/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.360829 piel-0.0.22/docs/examples/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.368829 piel-0.0.22/docs/examples/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-16 14:48:39.000000 piel-0.0.22/docs/examples/simple_design/tb/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 14:48:39.000000 piel-0.0.22/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 14:48:39.000000 piel-0.0.22/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-16 14:48:39.000000 piel-0.0.22/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 14:48:39.000000 piel-0.0.22/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.360829 piel-0.0.22/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.368829 piel-0.0.22/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 14:48:39.000000 piel-0.0.22/docs/sections/environment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 14:48:39.000000 piel-0.0.22/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.368829 piel-0.0.22/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-16 14:48:39.000000 piel-0.0.22/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 14:48:39.000000 piel-0.0.22/piel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-16 14:48:39.000000 piel-0.0.22/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-16 14:48:39.000000 piel-0.0.22/piel/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-16 14:48:39.000000 piel-0.0.22/piel/gdsfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 14:48:39.000000 piel-0.0.22/piel/openlane_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-16 14:48:39.000000 piel-0.0.22/piel/openlane_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-16 14:48:39.000000 piel-0.0.22/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 14:48:39.000000 piel-0.0.22/piel/piel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-16 14:48:39.000000 piel-0.0.22/piel/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.372829 piel-0.0.22/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-16 14:49:04.000000 piel-0.0.22/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-16 14:49:04.000000 piel-0.0.22/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:49:04.000000 piel-0.0.22/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 14:49:04.000000 piel-0.0.22/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:49:04.000000 piel-0.0.22/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-16 14:49:04.000000 piel-0.0.22/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 14:49:04.000000 piel-0.0.22/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-16 14:49:04.372829 piel-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-16 14:48:39.000000 piel-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:49:04.372829 piel-0.0.22/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 14:48:39.000000 piel-0.0.22/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-16 14:48:39.000000 piel-0.0.22/tests/test_piel.py
```

### Comparing `piel-0.0.21/CONTRIBUTING.rst` & `piel-0.0.22/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.21/LICENSE` & `piel-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.21/PKG-INFO` & `piel-0.0.22/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.21
+Version: 0.0.22
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -41,15 +41,15 @@
 * `OpenROAD OpenLane` for the micro-electronic layout design
 * `verilator` for the digital HDL simulations
 * `cocotb` for python-based testbench modelling
 * `porf` my custom package for `OpenROAD` data extraction.
 * [Future] FPGA modelling and integration
 
 ## Environment Requirements
-* This will only work in a linux system due to the tool dependencies.
+* Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
 
 - Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
 - `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `piel-0.0.21/README.md` & `piel-0.0.22/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 * `OpenROAD OpenLane` for the micro-electronic layout design
 * `verilator` for the digital HDL simulations
 * `cocotb` for python-based testbench modelling
 * `porf` my custom package for `OpenROAD` data extraction.
 * [Future] FPGA modelling and integration
 
 ## Environment Requirements
-* This will only work in a linux system due to the tool dependencies.
+* Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
 
 - Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
 - `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `piel-0.0.21/docs/Makefile` & `piel-0.0.22/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.21/docs/make.bat` & `piel-0.0.22/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.21/piel.egg-info/PKG-INFO` & `piel-0.0.22/piel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.21
+Version: 0.0.22
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -41,15 +41,15 @@
 * `OpenROAD OpenLane` for the micro-electronic layout design
 * `verilator` for the digital HDL simulations
 * `cocotb` for python-based testbench modelling
 * `porf` my custom package for `OpenROAD` data extraction.
 * [Future] FPGA modelling and integration
 
 ## Environment Requirements
-* This will only work in a linux system due to the tool dependencies.
+* Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
 
 - Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
 - `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `piel-0.0.21/setup.py` & `piel-0.0.22/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.md') as readme_file:
+with open("README.md") as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
+with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ['Click>=7.0', ]
-
-test_requirements = ['pytest>=3', ]
+requirements = [
+    "Click>=7.0",
+]
+
+test_requirements = [
+    "pytest>=3",
+]
 
 setup(
     author="Dario Quintero",
-    author_email='darioaquintero@gmail.com',
-    python_requires='>=3.6',
+    author_email="darioaquintero@gmail.com",
+    python_requires=">=3.6",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
     ],
     description="Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.",
     entry_points={
-        'console_scripts': [
-            'piel=piel.cli:main',
+        "console_scripts": [
+            "piel=piel.cli:main",
         ],
     },
     extras_require={
-                "develop": [
-                    "sphinx",
-                    "sphinx_autodoc_typehints",
-                    "sphinx-pydantic",
-                    "sphinx-autoapi",
-                    "sphinx-autobuild",
-                    "sphinx_rtd_theme",
-                    "sphinx-gallery",
-                    "nbsphinx",
-                    "myst_parser",
-                    "pandoc",
-                    "flake8"
-                ]
-            },
+        "develop": [
+            "sphinx",
+            "sphinx_autodoc_typehints",
+            "sphinx-pydantic",
+            "sphinx-autoapi",
+            "sphinx-autobuild",
+            "sphinx_rtd_theme",
+            "sphinx-gallery",
+            "nbsphinx",
+            "myst_parser",
+            "pandoc",
+            "flake8",
+        ]
+    },
     install_requires=requirements,
     license="MIT license",
-    long_description=readme + '\n\n' + history,
+    long_description=readme + "\n\n" + history,
     include_package_data=True,
-    keywords='piel',
-    name='piel',
-    packages=find_packages(include=['piel', 'piel.*']),
-    test_suite='tests',
+    keywords="piel",
+    name="piel",
+    packages=find_packages(include=["piel", "piel.*"]),
+    test_suite="tests",
     tests_require=test_requirements,
     url='https://github.com/daquintero/piel',
-    version='0.0.21',
+    version='0.0.22',
     zip_safe=False,
 )
```

### Comparing `piel-0.0.21/tests/test_piel.py` & `piel-0.0.22/tests/test_piel.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 
 
 def test_command_line_interface():
     """Test the CLI."""
     runner = CliRunner()
     result = runner.invoke(cli.main)
     assert result.exit_code == 0
-    assert 'piel.cli.main' in result.output
-    help_result = runner.invoke(cli.main, ['--help'])
+    assert "piel.cli.main" in result.output
+    help_result = runner.invoke(cli.main, ["--help"])
     assert help_result.exit_code == 0
-    assert '--help  Show this message and exit.' in help_result.output
+    assert "--help  Show this message and exit." in help_result.output
```

