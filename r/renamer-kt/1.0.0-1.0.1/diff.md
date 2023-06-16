# Comparing `tmp/renamer_kt-1.0.0.tar.gz` & `tmp/renamer_kt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renamer_kt-1.0.0.tar", last modified: Fri Jun 16 09:56:07 2023, max compression
+gzip compressed data, was "renamer_kt-1.0.1.tar", last modified: Fri Jun 16 12:03:44 2023, max compression
```

## Comparing `renamer_kt-1.0.0.tar` & `renamer_kt-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 09:56:07.009000 renamer_kt-1.0.0/
--rw-rw-rw-   0        0        0    35823 2022-02-06 05:44:47.000000 renamer_kt-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     5599 2023-06-16 09:56:06.998000 renamer_kt-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-06-16 09:02:31.000000 renamer_kt-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 09:56:07.007000 renamer_kt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4647 2023-06-16 09:55:58.000000 renamer_kt-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:56:06.691000 renamer_kt-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 09:56:06.816000 renamer_kt-1.0.0/src/core/
--rw-rw-rw-   0        0        0        0 2023-06-16 00:49:16.000000 renamer_kt-1.0.0/src/core/__init__.py
--rw-rw-rw-   0        0        0    10139 2023-06-16 09:32:01.000000 renamer_kt-1.0.0/src/core/decorators.py
--rw-rw-rw-   0        0        0     5860 2022-02-25 05:35:59.000000 renamer_kt-1.0.0/src/core/directory.py
--rw-rw-rw-   0        0        0     3633 2023-06-16 09:02:31.000000 renamer_kt-1.0.0/src/core/renamer.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:56:06.909000 renamer_kt-1.0.0/src/renamer_kt.egg-info/
--rw-rw-rw-   0        0        0     5599 2023-06-16 09:56:06.000000 renamer_kt-1.0.0/src/renamer_kt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      418 2023-06-16 09:56:06.000000 renamer_kt-1.0.0/src/renamer_kt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 09:56:06.000000 renamer_kt-1.0.0/src/renamer_kt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-16 09:56:06.000000 renamer_kt-1.0.0/src/renamer_kt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 09:56:06.000000 renamer_kt-1.0.0/src/renamer_kt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-16 09:56:06.000000 renamer_kt-1.0.0/src/renamer_kt.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-06-16 09:56:06.971000 renamer_kt-1.0.0/src/util/
--rw-rw-rw-   0        0        0        0 2023-06-16 00:50:45.000000 renamer_kt-1.0.0/src/util/__init__.py
--rw-rw-rw-   0        0        0     3428 2023-06-16 08:22:28.000000 renamer_kt-1.0.0/src/util/directedgraph.py
--rw-rw-rw-   0        0        0     1165 2022-02-07 00:22:17.000000 renamer_kt-1.0.0/src/util/util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:56:06.987000 renamer_kt-1.0.0/tests/
--rw-rw-rw-   0        0        0     4864 2022-09-01 05:55:53.000000 renamer_kt-1.0.0/tests/tester.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:03:44.279000 renamer_kt-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2022-02-06 05:44:47.000000 renamer_kt-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5536 2023-06-16 12:03:44.268000 renamer_kt-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4588 2023-06-16 11:57:35.000000 renamer_kt-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 12:03:44.275000 renamer_kt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     6178 2023-06-16 12:03:11.000000 renamer_kt-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:03:43.948000 renamer_kt-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 12:03:44.072000 renamer_kt-1.0.1/src/core/
+-rw-rw-rw-   0        0        0        0 2023-06-16 00:49:16.000000 renamer_kt-1.0.1/src/core/__init__.py
+-rw-rw-rw-   0        0        0    10139 2023-06-16 09:32:01.000000 renamer_kt-1.0.1/src/core/decorators.py
+-rw-rw-rw-   0        0        0     5860 2022-02-25 05:35:59.000000 renamer_kt-1.0.1/src/core/directory.py
+-rw-rw-rw-   0        0        0     3633 2023-06-16 09:02:31.000000 renamer_kt-1.0.1/src/core/renamer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:03:44.163000 renamer_kt-1.0.1/src/renamer_kt.egg-info/
+-rw-rw-rw-   0        0        0     5536 2023-06-16 12:03:43.000000 renamer_kt-1.0.1/src/renamer_kt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2023-06-16 12:03:43.000000 renamer_kt-1.0.1/src/renamer_kt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 12:03:43.000000 renamer_kt-1.0.1/src/renamer_kt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-16 12:03:43.000000 renamer_kt-1.0.1/src/renamer_kt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 12:03:43.000000 renamer_kt-1.0.1/src/renamer_kt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-16 12:03:43.000000 renamer_kt-1.0.1/src/renamer_kt.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-16 12:03:44.234000 renamer_kt-1.0.1/src/util/
+-rw-rw-rw-   0        0        0        0 2023-06-16 00:50:45.000000 renamer_kt-1.0.1/src/util/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-06-16 08:22:28.000000 renamer_kt-1.0.1/src/util/directedgraph.py
+-rw-rw-rw-   0        0        0     1165 2022-02-07 00:22:17.000000 renamer_kt-1.0.1/src/util/util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:03:44.256000 renamer_kt-1.0.1/tests/
+-rw-rw-rw-   0        0        0     4864 2022-09-01 05:55:53.000000 renamer_kt-1.0.1/tests/tester.py
```

### Comparing `renamer_kt-1.0.0/LICENSE` & `renamer_kt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `renamer_kt-1.0.0/PKG-INFO` & `renamer_kt-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renamer_kt
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI tool written in Python 3 used to systemically rename files in a directory while adhering to a variety of criteria.
 Home-page: https://github.com/KevinTyrrell/renamer
 Author: Kevin Tyrrell
 Author-email: KevinTearUl@gmail.com
 License: GPL-3.0
 Keywords: file renaming,CLI tool,Python 3,naming schemes,file organization,file sorting,file management,batch renaming,file renaming tool
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,26 +30,27 @@
 
 This program attempts to emulate the simplicity of the [CLI program FFmpeg](https://github.com/FFmpeg/FFmpeg) but for renaming files. Basic operations are straight-forward, while complex operations only invovle adding more flags and parameters to your operation. A directory with files that contain some numerical pattern are all that's required to get started. The application is well-paired for other software that require strict naming schemes, such as Plex, Kodi, or image managers.
 
 ![](res/HeaderImage.png)
 
 ## Installation
 
-OS X & Linux:
+[![PyPI](https://img.shields.io/pypi/v/renamer_kt.svg)](https://pypi.org/project/renamer_kt/)
 
-```sh
-bin/core.sh
-```
 
-Windows:
+Install `renamer-kt` using `pip`:
+
+### bash
 
 ```sh
-"bin/renamer.bat"
+pip install renamer-kt
 ```
 
+*Make sure you have Python and `pip` installed.*
+
 ## Usage
 
 | **Operation** | **Flag** | **Flag(Formal)** | **Parameter(s)**     | **Example**     | **Description**                                                                          |
 |---------------|----------|------------------|----------------------|-----------------|------------------------------------------------------------------------------------------|
 | _Shift_       | -s       | --shift          | Number Shift (int)   | --shift -1      | Shifts all numerical values by the specified offset                                      |
 | _Zeroes_      | -z       | --zeroes         | Leading Zeroes [int] | -z 3            | Prepends numerical values with the specified or inferred number of leading zeroes        |
 | _Format_      | -f       | --fmt            | Output Format (str)  | -f "Episode $d" | Customizes filename output ([see wiki](https://github.com/KevinTyrrell/Renamer/wiki/Format-Operator) for usage)|
@@ -69,45 +70,35 @@
   2021vacation0004.jpeg
   2021vacation0010.jpeg
 ```
 
 #### Clean-up
 > e.g. 1.jpeg, 3.jpeg, 4.jpeg, 10.jpeg
 ```sh
-core mydir
+renamer mydir
 ```
 
 #### Formalize & Fix Ordering
 > 01.jpeg, 02.jpeg, 03.jpeg, 04.jpeg
 ```sh
-core mydir -z 1 -c
+renamer mydir -z 1 -c
 ```
 
 #### Format & Modify Extension
 > 2021 Vacation - 1.png, 2021 Vacation - 3.png, 2021 Vacation - 4.png, 2021 Vacation - 10.png
 ```sh
-core mydir -e png -f "2021 Vacation - $d"
+renamer mydir -e png -f "2021 Vacation - $d"
 ```
 
 #### Shift & Flatten
 > 4.jpeg, 5.jpeg, 6.jpeg, 7.jpeg
 ```sh
-core mydir -s 3 -c
+renamer mydir -s 3 -c
 ```
 
-<!--
-## Development setup
-
-Describe how to install all development dependencies and how to run an automated test-suite of some kind. Potentially do this for multiple platforms.
-
-```sh
-make install
-npm test
-```
--->
 
 ## Meta
 
 Kevin Tyrrell – [KevinTearUl@gmail.com](mailto:KevinTearUl@gmail.com)
 
 Distributed under the GPL3 license. See ``LICENSE`` for more information.
```

### Comparing `renamer_kt-1.0.0/README.md` & `renamer_kt-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 
 This program attempts to emulate the simplicity of the [CLI program FFmpeg](https://github.com/FFmpeg/FFmpeg) but for renaming files. Basic operations are straight-forward, while complex operations only invovle adding more flags and parameters to your operation. A directory with files that contain some numerical pattern are all that's required to get started. The application is well-paired for other software that require strict naming schemes, such as Plex, Kodi, or image managers.
 
 ![](res/HeaderImage.png)
 
 ## Installation
 
-OS X & Linux:
+[![PyPI](https://img.shields.io/pypi/v/renamer_kt.svg)](https://pypi.org/project/renamer_kt/)
 
-```sh
-bin/core.sh
-```
 
-Windows:
+Install `renamer-kt` using `pip`:
+
+### bash
 
 ```sh
-"bin/renamer.bat"
+pip install renamer-kt
 ```
 
+*Make sure you have Python and `pip` installed.*
+
 ## Usage
 
 | **Operation** | **Flag** | **Flag(Formal)** | **Parameter(s)**     | **Example**     | **Description**                                                                          |
 |---------------|----------|------------------|----------------------|-----------------|------------------------------------------------------------------------------------------|
 | _Shift_       | -s       | --shift          | Number Shift (int)   | --shift -1      | Shifts all numerical values by the specified offset                                      |
 | _Zeroes_      | -z       | --zeroes         | Leading Zeroes [int] | -z 3            | Prepends numerical values with the specified or inferred number of leading zeroes        |
 | _Format_      | -f       | --fmt            | Output Format (str)  | -f "Episode $d" | Customizes filename output ([see wiki](https://github.com/KevinTyrrell/Renamer/wiki/Format-Operator) for usage)|
@@ -48,45 +49,35 @@
   2021vacation0004.jpeg
   2021vacation0010.jpeg
 ```
 
 #### Clean-up
 > e.g. 1.jpeg, 3.jpeg, 4.jpeg, 10.jpeg
 ```sh
-core mydir
+renamer mydir
 ```
 
 #### Formalize & Fix Ordering
 > 01.jpeg, 02.jpeg, 03.jpeg, 04.jpeg
 ```sh
-core mydir -z 1 -c
+renamer mydir -z 1 -c
 ```
 
 #### Format & Modify Extension
 > 2021 Vacation - 1.png, 2021 Vacation - 3.png, 2021 Vacation - 4.png, 2021 Vacation - 10.png
 ```sh
-core mydir -e png -f "2021 Vacation - $d"
+renamer mydir -e png -f "2021 Vacation - $d"
 ```
 
 #### Shift & Flatten
 > 4.jpeg, 5.jpeg, 6.jpeg, 7.jpeg
 ```sh
-core mydir -s 3 -c
+renamer mydir -s 3 -c
 ```
 
-<!--
-## Development setup
-
-Describe how to install all development dependencies and how to run an automated test-suite of some kind. Potentially do this for multiple platforms.
-
-```sh
-make install
-npm test
-```
--->
 
 ## Meta
 
 Kevin Tyrrell – [KevinTearUl@gmail.com](mailto:KevinTearUl@gmail.com)
 
 Distributed under the GPL3 license. See ``LICENSE`` for more information.
```

### Comparing `renamer_kt-1.0.0/src/core/decorators.py` & `renamer_kt-1.0.1/src/core/decorators.py`

 * *Files identical despite different names*

### Comparing `renamer_kt-1.0.0/src/core/directory.py` & `renamer_kt-1.0.1/src/core/directory.py`

 * *Files identical despite different names*

### Comparing `renamer_kt-1.0.0/src/core/renamer.py` & `renamer_kt-1.0.1/src/core/renamer.py`

 * *Files identical despite different names*

### Comparing `renamer_kt-1.0.0/src/renamer_kt.egg-info/PKG-INFO` & `renamer_kt-1.0.1/src/renamer_kt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renamer-kt
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI tool written in Python 3 used to systemically rename files in a directory while adhering to a variety of criteria.
 Home-page: https://github.com/KevinTyrrell/renamer
 Author: Kevin Tyrrell
 Author-email: KevinTearUl@gmail.com
 License: GPL-3.0
 Keywords: file renaming,CLI tool,Python 3,naming schemes,file organization,file sorting,file management,batch renaming,file renaming tool
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,26 +30,27 @@
 
 This program attempts to emulate the simplicity of the [CLI program FFmpeg](https://github.com/FFmpeg/FFmpeg) but for renaming files. Basic operations are straight-forward, while complex operations only invovle adding more flags and parameters to your operation. A directory with files that contain some numerical pattern are all that's required to get started. The application is well-paired for other software that require strict naming schemes, such as Plex, Kodi, or image managers.
 
 ![](res/HeaderImage.png)
 
 ## Installation
 
-OS X & Linux:
+[![PyPI](https://img.shields.io/pypi/v/renamer_kt.svg)](https://pypi.org/project/renamer_kt/)
 
-```sh
-bin/core.sh
-```
 
-Windows:
+Install `renamer-kt` using `pip`:
+
+### bash
 
 ```sh
-"bin/renamer.bat"
+pip install renamer-kt
 ```
 
+*Make sure you have Python and `pip` installed.*
+
 ## Usage
 
 | **Operation** | **Flag** | **Flag(Formal)** | **Parameter(s)**     | **Example**     | **Description**                                                                          |
 |---------------|----------|------------------|----------------------|-----------------|------------------------------------------------------------------------------------------|
 | _Shift_       | -s       | --shift          | Number Shift (int)   | --shift -1      | Shifts all numerical values by the specified offset                                      |
 | _Zeroes_      | -z       | --zeroes         | Leading Zeroes [int] | -z 3            | Prepends numerical values with the specified or inferred number of leading zeroes        |
 | _Format_      | -f       | --fmt            | Output Format (str)  | -f "Episode $d" | Customizes filename output ([see wiki](https://github.com/KevinTyrrell/Renamer/wiki/Format-Operator) for usage)|
@@ -69,45 +70,35 @@
   2021vacation0004.jpeg
   2021vacation0010.jpeg
 ```
 
 #### Clean-up
 > e.g. 1.jpeg, 3.jpeg, 4.jpeg, 10.jpeg
 ```sh
-core mydir
+renamer mydir
 ```
 
 #### Formalize & Fix Ordering
 > 01.jpeg, 02.jpeg, 03.jpeg, 04.jpeg
 ```sh
-core mydir -z 1 -c
+renamer mydir -z 1 -c
 ```
 
 #### Format & Modify Extension
 > 2021 Vacation - 1.png, 2021 Vacation - 3.png, 2021 Vacation - 4.png, 2021 Vacation - 10.png
 ```sh
-core mydir -e png -f "2021 Vacation - $d"
+renamer mydir -e png -f "2021 Vacation - $d"
 ```
 
 #### Shift & Flatten
 > 4.jpeg, 5.jpeg, 6.jpeg, 7.jpeg
 ```sh
-core mydir -s 3 -c
+renamer mydir -s 3 -c
 ```
 
-<!--
-## Development setup
-
-Describe how to install all development dependencies and how to run an automated test-suite of some kind. Potentially do this for multiple platforms.
-
-```sh
-make install
-npm test
-```
--->
 
 ## Meta
 
 Kevin Tyrrell – [KevinTearUl@gmail.com](mailto:KevinTearUl@gmail.com)
 
 Distributed under the GPL3 license. See ``LICENSE`` for more information.
```

### Comparing `renamer_kt-1.0.0/src/util/directedgraph.py` & `renamer_kt-1.0.1/src/util/directedgraph.py`

 * *Files identical despite different names*

### Comparing `renamer_kt-1.0.0/src/util/util.py` & `renamer_kt-1.0.1/src/util/util.py`

 * *Files identical despite different names*

### Comparing `renamer_kt-1.0.0/tests/tester.py` & `renamer_kt-1.0.1/tests/tester.py`

 * *Files identical despite different names*

