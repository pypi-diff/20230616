# Comparing `tmp/Mold2_pywrapper-0.0.3.post4.tar.gz` & `tmp/Mold2_pywrapper-0.0.3.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mold2_pywrapper-0.0.3.post4.tar", last modified: Thu Jun 15 07:42:45 2023, max compression
+gzip compressed data, was "Mold2_pywrapper-0.0.3.post5.tar", last modified: Fri Jun 16 17:05:33 2023, max compression
```

## Comparing `Mold2_pywrapper-0.0.3.post4.tar` & `Mold2_pywrapper-0.0.3.post5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:42:45.454887 Mold2_pywrapper-0.0.3.post4/
--rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post4/LICENSE
--rw-rw-rw-   0        0        0     4964 2023-06-15 07:42:45.454887 Mold2_pywrapper-0.0.3.post4/PKG-INFO
--rw-rw-rw-   0        0        0     4047 2023-02-07 12:55:23.000000 Mold2_pywrapper-0.0.3.post4/README.md
--rw-rw-rw-   0        0        0     1301 2023-06-15 07:42:45.464887 Mold2_pywrapper-0.0.3.post4/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:42:45.404372 Mold2_pywrapper-0.0.3.post4/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 07:42:45.422376 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper/
--rw-rw-rw-   0        0        0      127 2023-06-15 07:42:07.000000 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper/__init__.py
--rw-rw-rw-   0        0        0    47122 2023-06-05 09:19:01.000000 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper/descriptors.json
--rw-rw-rw-   0        0        0    13996 2023-06-14 08:06:08.000000 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper/mold2_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:42:45.451885 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     4964 2023-06-15 07:42:45.000000 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-06-15 07:42:45.000000 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:42:45.000000 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-06-15 07:42:45.000000 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 07:42:45.000000 Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 17:05:32.948719 Mold2_pywrapper-0.0.3.post5/
+-rw-rw-rw-   0        0        0     1100 2023-01-14 16:21:14.000000 Mold2_pywrapper-0.0.3.post5/LICENSE
+-rw-rw-rw-   0        0        0     4964 2023-06-16 17:05:32.949697 Mold2_pywrapper-0.0.3.post5/PKG-INFO
+-rw-rw-rw-   0        0        0     4047 2023-02-06 18:52:51.000000 Mold2_pywrapper-0.0.3.post5/README.md
+-rw-rw-rw-   0        0        0     1301 2023-06-16 17:05:32.959473 Mold2_pywrapper-0.0.3.post5/setup.cfg
+-rw-rw-rw-   0        0        0      123 2020-09-22 21:34:54.000000 Mold2_pywrapper-0.0.3.post5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:05:32.894950 Mold2_pywrapper-0.0.3.post5/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 17:05:32.911569 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/
+-rw-rw-rw-   0        0        0      127 2023-06-16 17:04:00.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0    47122 2023-06-16 16:57:59.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/descriptors.json
+-rw-rw-rw-   0        0        0    14004 2023-06-16 17:01:25.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/mold2_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:05:32.945786 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     4964 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/top_level.txt
```

### Comparing `Mold2_pywrapper-0.0.3.post4/LICENSE` & `Mold2_pywrapper-0.0.3.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post4/PKG-INFO` & `Mold2_pywrapper-0.0.3.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mold2_pywrapper
-Version: 0.0.3.post4
+Version: 0.0.3.post5
 Summary: Python wrapper for Mold2 descriptors
 Home-page: https://github.com/OlivierBeq/Mold2_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: mold2,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `Mold2_pywrapper-0.0.3.post4/README.md` & `Mold2_pywrapper-0.0.3.post5/README.md`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post4/setup.cfg` & `Mold2_pywrapper-0.0.3.post5/setup.cfg`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper/descriptors.json` & `Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/descriptors.json`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper/mold2_wrapper.py` & `Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/mold2_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """Python wrapper for Mold2 descriptors"""
 
 from __future__ import annotations
 
 import json
 import os
 import re
-import stat
 import shutil
+import stat
 import subprocess
 import tempfile
 import zipfile
 from platform import architecture
 from sys import platform
 from typing import Iterable, List, Optional
 
@@ -31,15 +31,15 @@
     def __init__(self, verbose: bool = True):
         """Instantiate a wrapper to calculate Mold2 molecular descriptors.
 
         :param verbose: Should details about the download of executables be printed out
         """
         # Default folder for Mold2 executables
         self._zipfile = os.path.abspath(os.path.join(pystow.join('Mold2').as_posix(),
-                                                                'Mold2-Executable-File.zip'))
+                                                     'Mold2-Executable-File.zip'))
         # Ensure executables are available
         self._download_executables(verbose)
 
     def __del__(self):
         """Remove downloaded executables."""
         if os.path.isdir(self._dir):
             shutil.rmtree(self._dir)
@@ -247,15 +247,15 @@
         if data.iloc[0, 0] != 'D001':
             # Header is not provided if first molecule failed
             data.columns = [f'D{x:03d}' for x in range(1, 778)]
         else:
             data.columns = data.iloc[0, :]
             data.drop(index=0, inplace=True)
         data.reset_index(drop=True, inplace=True)
-        data = pd.to_numeric(data, errors='coerce')
+        data = data.apply(lambda x: pd.to_numeric(x, errors='coerce'))
         data = data.convert_dtypes()
         return data
 
     def _calculate(self, mols: List[Chem.Mol]) -> pd.DataFrame:
         """Caclulate Mold2 descriptors on one process.
 
         :param mols: RDkit molecules for which Mold2 descriptors should be calculated
```

### Comparing `Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper.egg-info/PKG-INFO` & `Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mold2-pywrapper
-Version: 0.0.3.post4
+Version: 0.0.3.post5
 Summary: Python wrapper for Mold2 descriptors
 Home-page: https://github.com/OlivierBeq/Mold2_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: mold2,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `Mold2_pywrapper-0.0.3.post4/src/Mold2_pywrapper.egg-info/SOURCES.txt` & `Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

