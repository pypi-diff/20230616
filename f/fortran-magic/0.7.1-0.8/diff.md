# Comparing `tmp/fortran-magic-0.7.1.tar.gz` & `tmp/fortran-magic-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortran-magic-0.7.1.tar", last modified: Wed Apr 12 15:35:28 2023, max compression
+gzip compressed data, was "fortran-magic-0.8.tar", last modified: Fri Jun 16 11:02:18 2023, max compression
```

## Comparing `fortran-magic-0.7.1.tar` & `fortran-magic-0.8.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2023-04-12 15:35:28.216755 fortran-magic-0.7.1/
--rw-rw-r--   0 tin       (1000) tin       (1000)     2479 2023-04-12 15:34:29.000000 fortran-magic-0.7.1/CHANGES.rst
--rw-rw-r--   0 tin       (1000) tin       (1000)     1491 2023-04-12 15:25:00.000000 fortran-magic-0.7.1/LICENSE
--rw-rw-r--   0 tin       (1000) tin       (1000)       38 2023-04-12 15:25:00.000000 fortran-magic-0.7.1/MANIFEST.in
--rw-rw-r--   0 tin       (1000) tin       (1000)     5017 2023-04-12 15:35:28.216755 fortran-magic-0.7.1/PKG-INFO
--rw-rw-r--   0 tin       (1000) tin       (1000)     1674 2023-04-12 15:25:00.000000 fortran-magic-0.7.1/README.rst
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2023-04-12 15:35:28.216755 fortran-magic-0.7.1/fortran_magic.egg-info/
--rw-rw-r--   0 tin       (1000) tin       (1000)     5017 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/PKG-INFO
--rw-rw-r--   0 tin       (1000) tin       (1000)      251 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/SOURCES.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)        1 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/dependency_links.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)       14 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/requires.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)       13 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/top_level.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)    13133 2023-04-12 15:26:50.000000 fortran-magic-0.7.1/fortranmagic.py
--rw-rw-r--   0 tin       (1000) tin       (1000)       38 2023-04-12 15:35:28.216755 fortran-magic-0.7.1/setup.cfg
--rw-rw-r--   0 tin       (1000) tin       (1000)     1171 2023-04-12 15:35:23.000000 fortran-magic-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:18.060196 fortran-magic-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-16 11:02:08.000000 fortran-magic-0.8/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-16 11:02:08.000000 fortran-magic-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:02:08.000000 fortran-magic-0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-16 11:02:18.060196 fortran-magic-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-16 11:02:08.000000 fortran-magic-0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:18.056196 fortran-magic-0.8/fortran_magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-16 11:02:08.000000 fortran-magic-0.8/fortranmagic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:02:18.060196 fortran-magic-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-16 11:02:08.000000 fortran-magic-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:18.060196 fortran-magic-0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_010_init_cfg_and_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_documentation_ipynb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_f2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_fortran_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_oserror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_readme_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_zload_ext.py
```

### Comparing `fortran-magic-0.7.1/CHANGES.rst` & `fortran-magic-0.8/CHANGES.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,56 @@
 
 Changelog
 =========
 
-0.7.1 / 2022-04-12
+0.8 / 2023-06-08
+----------------
+
+- Fix use deprecating ``imp`` module (removed from Python 3.12b2)
+
+- Fix exponential duplication any not boolean flags of
+  ``%%fortran_config``
+
+- Include stored ``%%fortran_config``'s args in hashing
+
+- Don't rebuild cell if the module already loaded and hash not changed
+  (Unix don't reload already loaded shared library with same name.
+  Windows can't rewrite already loaded DLL)
+
+- Repair fortran highlighting in a ``%%fortran`` cell for ``nbclassic``
+  (Fortran highlighting for ``JupyterLab`` - unimplemented, for
+  ``IPython 3.x`` - removed)
+
+- Printing compilers diagnostics for build errors by ``%%fortran``
+  without ``-vvv`` flag
+
+`Serguei E. Leontiev`_
+
+.. _Serguei E. Leontiev: https://github.com/Serge3leo
+
+
+0.7.1 / 2023-04-12
 ------------------
 
-- Synchronize version number in fortranmagic.py & setup.py (TBD, TBD, https://github.com/Serge3leo)
+- Synchronize version number in fortranmagic.py & setup.py (2023-04-10,
+  https://github.com/Serge3leo)
 
-- Patch fortran source in compiled object. (029d890, 2020-08-01, https://github.com/mgaitan)
+- Patch fortran source in compiled object. (029d890, 2020-08-01,
+  https://github.com/mgaitan)
 
 - Fix deprecation warning (3667bc1, 2017-08-18, https://github.com/guihigashi)
-  [IPython.utils.path removed from IPython 8.x] 
+  [IPython.utils.path removed from IPython 8.x]
 
 - Simplify f2py execution. (d8a058f, 2016-06-04, https://github.com/QuLogic)
   Don't change directories, and don't mangle `sys.argv`. The former can be
   specified directly in the `Popen` constructor, and the latter is cruft
   from when the f2py module was imported directly.
 
 
-0.7 / 2016-03-13 
+0.7 / 2016-03-13
 ----------------
 
 - Fix cross compatibility with older NumPy and Python 3. (15ab10c)
 
 Thanks to `Elliott Sales de Andrade`_ for this contribution
 
 .. _Elliott Sales de Andrade: https://github.com/QuLogic
@@ -87,8 +115,8 @@
 - Improved documentation
 
 .. _Bradley Froehle: https://github.com/bfroehle
 
 0.1 / 2013-09-08
 ----------------
 
-- First public release
+- First public release
```

### Comparing `fortran-magic-0.7.1/LICENSE` & `fortran-magic-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fortran-magic-0.7.1/PKG-INFO` & `fortran-magic-0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fortran-magic
-Version: 0.7.1
+Version: 0.8
 Summary: An extension for IPython that help to use Fortran in your interactive session.
 Home-page: https://github.com/mgaitan/fortran_magic
 Author: Martin Gaitan
 Author-email: gaitan@gmail.com
 License: BSD
 Keywords: ipython notebook fortran f2py science
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -21,33 +20,39 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =============
 Fortran magic
 =============
 
-.. image:: https://pypip.in/v/fortran-magic/badge.png
+.. image:: https://img.shields.io/pypi/v/fortran-magic
    :target: https://pypi.python.org/pypi/fortran-magic
-   :alt: Latest PyPI version
-
-.. image:: https://pypip.in/d/fortran-magic/badge.png
+   :alt: PyPI
+   
+.. image:: https://img.shields.io/pypi/dm/fortran-magic
    :target: https://pypi.python.org/pypi/fortran-magic
-   :alt: Number of PyPI downloads
-
+   :alt: PyPI - Downloads
+   
 
 Compile and import symbols from a cell with Fortran code, using f2py.
 
+------
+
+..  attention::
+    I am looking for collaborators to maintain this project. If you are interested, 
+    please open an issue (or PRs) with your proposals for improvements and volunteer to be a maintainer. 
+
+------
+
 The contents of the cell are written to a `.f90` file in the
 directory `IPYTHONDIR/fortran` using a filename with the hash of the
 code. This file is then compiled. The resulting module
 is imported and all of its symbols are injected into the user's
 namespace.
 
-
-:author: Martín Gaitán <gaitan@gmail.com>
 :homepage: https://github.com/mgaitan/fortran_magic
 :documentation: see `this notebook`__
 
 __ documentation_
 .. _documentation:  http://nbviewer.ipython.org/urls/raw.github.com/mgaitan/fortran_magic/master/documentation.ipynb
 
 
@@ -62,15 +67,22 @@
 Basic usage
 ===========
 
 Once it's installed, you can load it with ``%load_ext fortranmagic``.
 Then put your Fortran code in a cell started with the cell magic ``%%fortran``. For example::
 
 
-    In[2]: %load_ext fortranmagic
+    In[1]: %load_ext fortranmagic
+
+    In[2]: import sys
+
+           if sys.platform.startswith("win"):
+               # Depends of system, python builds, and compilers compatibility.
+               # See `documentation.ipnb`.
+               %fortran_config --fcompiler=gnu95 --compiler=mingw32
 
     In[3]: %%fortran
 
            subroutine f1(x, y, z)
                 real, intent(in) :: x,y
                 real, intent(out) :: z
 
@@ -88,31 +100,59 @@
 See the documentation_ for further details.
 
 
 
 Changelog
 =========
 
-0.7.1 / 2022-04-12
+0.8 / 2023-06-08
+----------------
+
+- Fix use deprecating ``imp`` module (removed from Python 3.12b2)
+
+- Fix exponential duplication any not boolean flags of
+  ``%%fortran_config``
+
+- Include stored ``%%fortran_config``'s args in hashing
+
+- Don't rebuild cell if the module already loaded and hash not changed
+  (Unix don't reload already loaded shared library with same name.
+  Windows can't rewrite already loaded DLL)
+
+- Repair fortran highlighting in a ``%%fortran`` cell for ``nbclassic``
+  (Fortran highlighting for ``JupyterLab`` - unimplemented, for
+  ``IPython 3.x`` - removed)
+
+- Printing compilers diagnostics for build errors by ``%%fortran``
+  without ``-vvv`` flag
+
+`Serguei E. Leontiev`_
+
+.. _Serguei E. Leontiev: https://github.com/Serge3leo
+
+
+0.7.1 / 2023-04-12
 ------------------
 
-- Synchronize version number in fortranmagic.py & setup.py (TBD, TBD, https://github.com/Serge3leo)
+- Synchronize version number in fortranmagic.py & setup.py (2023-04-10,
+  https://github.com/Serge3leo)
 
-- Patch fortran source in compiled object. (029d890, 2020-08-01, https://github.com/mgaitan)
+- Patch fortran source in compiled object. (029d890, 2020-08-01,
+  https://github.com/mgaitan)
 
 - Fix deprecation warning (3667bc1, 2017-08-18, https://github.com/guihigashi)
-  [IPython.utils.path removed from IPython 8.x] 
+  [IPython.utils.path removed from IPython 8.x]
 
 - Simplify f2py execution. (d8a058f, 2016-06-04, https://github.com/QuLogic)
   Don't change directories, and don't mangle `sys.argv`. The former can be
   specified directly in the `Popen` constructor, and the latter is cruft
   from when the f2py module was imported directly.
 
 
-0.7 / 2016-03-13 
+0.7 / 2016-03-13
 ----------------
 
 - Fix cross compatibility with older NumPy and Python 3. (15ab10c)
 
 Thanks to `Elliott Sales de Andrade`_ for this contribution
 
 .. _Elliott Sales de Andrade: https://github.com/QuLogic
@@ -178,8 +218,7 @@
 
 .. _Bradley Froehle: https://github.com/bfroehle
 
 0.1 / 2013-09-08
 ----------------
 
 - First public release
-
```

### Comparing `fortran-magic-0.7.1/README.rst` & `fortran-magic-0.8/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 =============
 Fortran magic
 =============
 
-.. image:: https://pypip.in/v/fortran-magic/badge.png
+.. image:: https://img.shields.io/pypi/v/fortran-magic
    :target: https://pypi.python.org/pypi/fortran-magic
-   :alt: Latest PyPI version
-
-.. image:: https://pypip.in/d/fortran-magic/badge.png
+   :alt: PyPI
+   
+.. image:: https://img.shields.io/pypi/dm/fortran-magic
    :target: https://pypi.python.org/pypi/fortran-magic
-   :alt: Number of PyPI downloads
-
+   :alt: PyPI - Downloads
+   
 
 Compile and import symbols from a cell with Fortran code, using f2py.
 
+------
+
+..  attention::
+    I am looking for collaborators to maintain this project. If you are interested, 
+    please open an issue (or PRs) with your proposals for improvements and volunteer to be a maintainer. 
+
+------
+
 The contents of the cell are written to a `.f90` file in the
 directory `IPYTHONDIR/fortran` using a filename with the hash of the
 code. This file is then compiled. The resulting module
 is imported and all of its symbols are injected into the user's
 namespace.
 
-
-:author: Martín Gaitán <gaitan@gmail.com>
 :homepage: https://github.com/mgaitan/fortran_magic
 :documentation: see `this notebook`__
 
 __ documentation_
 .. _documentation:  http://nbviewer.ipython.org/urls/raw.github.com/mgaitan/fortran_magic/master/documentation.ipynb
 
 
@@ -39,15 +45,22 @@
 Basic usage
 ===========
 
 Once it's installed, you can load it with ``%load_ext fortranmagic``.
 Then put your Fortran code in a cell started with the cell magic ``%%fortran``. For example::
 
 
-    In[2]: %load_ext fortranmagic
+    In[1]: %load_ext fortranmagic
+
+    In[2]: import sys
+
+           if sys.platform.startswith("win"):
+               # Depends of system, python builds, and compilers compatibility.
+               # See `documentation.ipnb`.
+               %fortran_config --fcompiler=gnu95 --compiler=mingw32
 
     In[3]: %%fortran
 
            subroutine f1(x, y, z)
                 real, intent(in) :: x,y
                 real, intent(out) :: z
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fortran-magic-0.7.1/fortran_magic.egg-info/PKG-INFO` & `fortran-magic-0.8/fortran_magic.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fortran-magic
-Version: 0.7.1
+Version: 0.8
 Summary: An extension for IPython that help to use Fortran in your interactive session.
 Home-page: https://github.com/mgaitan/fortran_magic
 Author: Martin Gaitan
 Author-email: gaitan@gmail.com
 License: BSD
 Keywords: ipython notebook fortran f2py science
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -21,33 +20,39 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =============
 Fortran magic
 =============
 
-.. image:: https://pypip.in/v/fortran-magic/badge.png
+.. image:: https://img.shields.io/pypi/v/fortran-magic
    :target: https://pypi.python.org/pypi/fortran-magic
-   :alt: Latest PyPI version
-
-.. image:: https://pypip.in/d/fortran-magic/badge.png
+   :alt: PyPI
+   
+.. image:: https://img.shields.io/pypi/dm/fortran-magic
    :target: https://pypi.python.org/pypi/fortran-magic
-   :alt: Number of PyPI downloads
-
+   :alt: PyPI - Downloads
+   
 
 Compile and import symbols from a cell with Fortran code, using f2py.
 
+------
+
+..  attention::
+    I am looking for collaborators to maintain this project. If you are interested, 
+    please open an issue (or PRs) with your proposals for improvements and volunteer to be a maintainer. 
+
+------
+
 The contents of the cell are written to a `.f90` file in the
 directory `IPYTHONDIR/fortran` using a filename with the hash of the
 code. This file is then compiled. The resulting module
 is imported and all of its symbols are injected into the user's
 namespace.
 
-
-:author: Martín Gaitán <gaitan@gmail.com>
 :homepage: https://github.com/mgaitan/fortran_magic
 :documentation: see `this notebook`__
 
 __ documentation_
 .. _documentation:  http://nbviewer.ipython.org/urls/raw.github.com/mgaitan/fortran_magic/master/documentation.ipynb
 
 
@@ -62,15 +67,22 @@
 Basic usage
 ===========
 
 Once it's installed, you can load it with ``%load_ext fortranmagic``.
 Then put your Fortran code in a cell started with the cell magic ``%%fortran``. For example::
 
 
-    In[2]: %load_ext fortranmagic
+    In[1]: %load_ext fortranmagic
+
+    In[2]: import sys
+
+           if sys.platform.startswith("win"):
+               # Depends of system, python builds, and compilers compatibility.
+               # See `documentation.ipnb`.
+               %fortran_config --fcompiler=gnu95 --compiler=mingw32
 
     In[3]: %%fortran
 
            subroutine f1(x, y, z)
                 real, intent(in) :: x,y
                 real, intent(out) :: z
 
@@ -88,31 +100,59 @@
 See the documentation_ for further details.
 
 
 
 Changelog
 =========
 
-0.7.1 / 2022-04-12
+0.8 / 2023-06-08
+----------------
+
+- Fix use deprecating ``imp`` module (removed from Python 3.12b2)
+
+- Fix exponential duplication any not boolean flags of
+  ``%%fortran_config``
+
+- Include stored ``%%fortran_config``'s args in hashing
+
+- Don't rebuild cell if the module already loaded and hash not changed
+  (Unix don't reload already loaded shared library with same name.
+  Windows can't rewrite already loaded DLL)
+
+- Repair fortran highlighting in a ``%%fortran`` cell for ``nbclassic``
+  (Fortran highlighting for ``JupyterLab`` - unimplemented, for
+  ``IPython 3.x`` - removed)
+
+- Printing compilers diagnostics for build errors by ``%%fortran``
+  without ``-vvv`` flag
+
+`Serguei E. Leontiev`_
+
+.. _Serguei E. Leontiev: https://github.com/Serge3leo
+
+
+0.7.1 / 2023-04-12
 ------------------
 
-- Synchronize version number in fortranmagic.py & setup.py (TBD, TBD, https://github.com/Serge3leo)
+- Synchronize version number in fortranmagic.py & setup.py (2023-04-10,
+  https://github.com/Serge3leo)
 
-- Patch fortran source in compiled object. (029d890, 2020-08-01, https://github.com/mgaitan)
+- Patch fortran source in compiled object. (029d890, 2020-08-01,
+  https://github.com/mgaitan)
 
 - Fix deprecation warning (3667bc1, 2017-08-18, https://github.com/guihigashi)
-  [IPython.utils.path removed from IPython 8.x] 
+  [IPython.utils.path removed from IPython 8.x]
 
 - Simplify f2py execution. (d8a058f, 2016-06-04, https://github.com/QuLogic)
   Don't change directories, and don't mangle `sys.argv`. The former can be
   specified directly in the `Popen` constructor, and the latter is cruft
   from when the f2py module was imported directly.
 
 
-0.7 / 2016-03-13 
+0.7 / 2016-03-13
 ----------------
 
 - Fix cross compatibility with older NumPy and Python 3. (15ab10c)
 
 Thanks to `Elliott Sales de Andrade`_ for this contribution
 
 .. _Elliott Sales de Andrade: https://github.com/QuLogic
@@ -178,8 +218,7 @@
 
 .. _Bradley Froehle: https://github.com/bfroehle
 
 0.1 / 2013-09-08
 ----------------
 
 - First public release
-
```

### Comparing `fortran-magic-0.7.1/fortranmagic.py` & `fortran-magic-0.8/fortranmagic.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,47 +10,56 @@
 
 Author:
 * Martín Gaitán <gaitan@gmail.com>
 """
 
 from __future__ import print_function
 
-import imp
+import errno
+import hashlib
 import io
 import os
+import random
+import shutil
 import sys
-#import subprocess
-from subprocess import Popen, PIPE
-
-import errno
-
-try:
-    import hashlib
-except ImportError:
-    import md5 as hashlib
+from distutils.ccompiler import compiler_class
+from distutils.command.build_ext import build_ext
+from distutils.core import Distribution
+from distutils.version import LooseVersion
+from subprocess import PIPE, Popen
 
-from IPython.core.error import UsageError
-from IPython.core.magic import Magics, magics_class, line_magic, cell_magic
+import numpy as np
 from IPython.core import display, magic_arguments
+from IPython.core.magic import Magics, cell_magic, line_magic, magics_class
+from IPython.paths import get_ipython_cache_dir
 from IPython.utils import py3compat
 from IPython.utils.io import capture_output
-from IPython.paths import get_ipython_cache_dir
-import numpy as np
-from numpy.f2py import f2py2e
 from numpy.distutils import fcompiler
-from distutils.core import Distribution
-from distutils.ccompiler import compiler_class
-from distutils.command.build_ext import build_ext
-from distutils.version import LooseVersion
-
+from numpy.f2py import f2py2e
 
-__version__ = '0.7.1'
+__version__ = '0.8'
 fcompiler.load_all_fcompiler_classes()
 
 
+try:
+    import importlib.machinery
+    import importlib.util
+
+    def _imp_load_dynamic(name, path):
+        loader = importlib.machinery.ExtensionFileLoader(name, path)
+        spec = importlib.machinery.ModuleSpec(name=name, loader=loader,
+                                              origin=path)
+        return importlib.util.module_from_spec(spec)
+except ImportError:
+    import imp
+
+    def _imp_load_dynamic(name, path):
+        return imp.load_dynamic(name, path)
+
+
 def compose(*decorators):
     """Helper to compose decorators::
 
         @a
         @b
         def f():
             pass
@@ -68,16 +77,15 @@
     return composed
 
 
 def unquote(v):
     if ((v.startswith('"') and v.endswith('"')) or
             (v.startswith("'") and v.endswith("'"))):
         return v[1:-1]
-    else:
-        return v
+    return v
 
 
 @magics_class
 class FortranMagics(Magics):
 
     allowed_fcompilers = sorted(fcompiler.fcompiler_class.keys())
     allowed_compilers = sorted(compiler_class.keys())
@@ -134,23 +142,73 @@
         magic_arguments.argument(
             '--extra', action='append', default=[],
             help="""Use --extra to pass any other argument in the f2py call. For example
                     --extra '-L/path/to/lib/ -l<libname>'
                     --extra '-D<define> -U<name>'
                     --extra '-DPREPEND_FORTRAN -DUPPERCASE_FORTRAN'
                     etc. """
-        ))
+        ),
+        magic_arguments.argument(
+            '--add-hash', action='append', default=[],
+            help="Additional string to hash of code, flags, etc."
+        ),
+        )
+
+    def _cache_init(self):
+        """Create random cache directory."""
+
+        while True:
+            cdir = os.path.join(get_ipython_cache_dir(),
+                                'fortranmagic',
+                                "%08x" % random.getrandbits(32))
+            try:
+                os.makedirs(cdir)
+                break
+            except OSError:
+                pass
+        self.shell.db['fortranmagic_cache'] = cdir
+        self._lib_dir = cdir
+
+    def _cache_open(self):
+        """Open cache directory on session start"""
+
+        try:
+            cdir = self.shell.db['fortranmagic_cache']
+            if os.path.isdir(cdir):
+                self._lib_dir = cdir
+                return
+        except (KeyError, OSError):
+            pass
+        self._cache_init()
+
+    def _cache_check(self):
+        """Check cache directory.
+
+        If the parallel session executed `__cache_init()`, then the
+        current session still continues to use the old directory (the
+        one that was considered at the start).
+        """
+
+        if not os.path.isdir(self._lib_dir):
+            try:
+                os.makedirs(self._lib_dir)
+            except OSError:
+                self._cache_init()
+
+    def _cache_clean(self):
+        shutil.rmtree(os.path.join(get_ipython_cache_dir(),
+                                   'fortranmagic'),
+                      ignore_errors=True)
+        self._cache_init()
 
     def __init__(self, shell):
         super(FortranMagics, self).__init__(shell=shell)
         self._reloads = {}
         self._code_cache = {}
-        self._lib_dir = os.path.join(get_ipython_cache_dir(), 'fortran')
-        if not os.path.exists(self._lib_dir):
-            os.makedirs(self._lib_dir)
+        self._cache_open()
 
     def _import_all(self, module, verbosity=0, code=''):
         imported = []
         for k, v in module.__dict__.items():
             if not k.startswith('__'):
                 v.__source__ = code
                 self.shell.push({k: v})
@@ -171,38 +229,37 @@
         else:
             command = [sys.executable, '-m', 'numpy.f2py']
         command += map(str, argv)
 
         if verbosity > 1:
             print("Running...\n   %s" % ' '.join(command))
 
-        with capture_output() as captured:
-            # subprocess.call(command)
-            # Refactor subprocess call to work with jupyterhub
-            try:
-                p = Popen(command, stdout=PIPE, stderr=PIPE, stdin=PIPE,
-                          cwd=self._lib_dir)
-            except OSError as e:
-                if e.errno == errno.ENOENT:
-                    print("Couldn't find program: %r" % command[0])
-                    return
-                else:
+        p, out, err = None, None, None
+        try:
+            with capture_output() as captured:
+                # subprocess.call(command)
+                # Refactor subprocess call to work with jupyterhub
+                try:
+                    p = Popen(command, stdout=PIPE, stderr=PIPE, stdin=PIPE,
+                              cwd=self._lib_dir)
+                except OSError as e:
+                    if e.errno == errno.ENOENT:
+                        print("Couldn't find program: %r" % command[0])
+                        return -1
                     raise
-            try:
                 out, err = p.communicate(input=None)
-            except:
-                pass
-            if err:
-                sys.stderr.write(err.decode())
-                sys.stderr.flush()
-        if show_captured or verbosity > 2:
-            if out:
-                sys.stdout.write(out.decode())
-                sys.stdout.flush()
-            captured()
+        finally:
+            if show_captured or verbosity > 2 or p is None or p.returncode:
+                if err:
+                    sys.stderr.write(err.decode())
+                    sys.stderr.flush()
+                if out:
+                    sys.stdout.write(out.decode())
+                    sys.stdout.flush()
+                captured()
 
         return p.returncode
 
     @magic_arguments.magic_arguments()
     @magic_arguments.argument(
         '--resources', action="store_true",
         help="""List system resources found by system_info.py.
@@ -241,92 +298,100 @@
             self._run_f2py(['--help-link', args.link], True)
 
     @my_magic_arguments
     @magic_arguments.argument(
         '--defaults', action="store_true", help="Delete custom configuration "
         "and back to default"
     )
+    @magic_arguments.argument(
+        '--clean-cache', action="store_true", help="Clean fortran modules "
+        "build cache"
+    )
     @line_magic
     def fortran_config(self, line):
         """
         View and handle the custom configuration for %%fortran magic.
 
             %fortran_config
 
                 Show the current custom configuration
 
+            %fortran_config --clean-cache
+
+                Clean fortran modules build cache
+
             %fortran_config --defaults
 
                 Delete the current configuration and back to defaults
 
             %fortran_config <other options>
 
                 Save <other options> to use with %%fortran
         """
 
         args = magic_arguments.parse_argstring(self.fortran_config, line)
-        if args.defaults:
+        if args.clean_cache:
+            print("Clean cache:", self._lib_dir)
+            self._cache_clean()
+            if args.verbosity >= 1:
+                print("New cache:", self._lib_dir)
+        elif args.defaults:
             try:
-                del self.shell.db['fortran']
+                del self.shell.db['fortranmagic']
                 print("Deleted custom config. Back to default arguments for %%fortran")
             except KeyError:
                 print("No custom config found for %%fortran")
         elif not line:
             try:
-                line = self.shell.db['fortran']
+                line = self.shell.db['fortranmagic']
+                print("Current defaults arguments for %%fortran:\n\t%s" % line)
             except KeyError:
                 print("No custom config found for %%fortran")
-            print("Current defaults arguments for %%fortran:\n\t%s" % line)
         else:
-            self.shell.db['fortran'] = line
+            self.shell.db['fortranmagic'] = line
             print("New default arguments for %%fortran:\n\t%s" % line)
 
     @my_magic_arguments
     @cell_magic
     def fortran(self, line, cell):
         """Compile and import everything from a Fortran code cell, using f2py.
 
         The content of the cell is written to a `.f90` file in the
-        directory `IPYTHONDIR/fortran` using a filename with the hash of the
-        code. This file is then compiled. The resulting module
-        is imported and all of its symbols are injected into the user's
-        namespace.
+        directory `IPYTHONDIR/fortran` using a filename with the hash of
+        the code, flags and configuration data. This file is then
+        compiled. The resulting module is imported and all of its
+        symbols are injected into the user's namespace.
 
 
         Usage
         =====
         Prepend ``%%fortran`` to your fortran code in a cell::
 
         ``%%fortran
 
         ! put your code here.
         ``
 
 
         """
 
-        try:
-            # custom saved arguments
-            saved_defaults = vars(
-                magic_arguments.parse_argstring(self.fortran,
-                                                self.shell.db['fortran']))
-            self.fortran.parser.set_defaults(**saved_defaults)
-        except KeyError:
-            saved_defaults = {'verbosity': 0}
-
         # verbosity is a "count" argument were each ocurrence is
         # added implicit.
         # so, for instance, -vv in %fortran_config and -vvv in %%fortran means
         # a nonsense verbosity=5.
         # To override: if verbosity is given for the magic cell
         # we ignore the saved config.
-        if '-v' in line:
-            self.fortran.parser.set_defaults(verbosity=0)
-
         args = magic_arguments.parse_argstring(self.fortran, line)
+        f_config = self.shell.db.get('fortranmagic', "")
+        if f_config:
+            sverbosity = args.verbosity
+            args = magic_arguments.parse_argstring(self.fortran,
+                                                   f_config + " " + line)
+            if sverbosity > 0:
+                args.verbosity = sverbosity
 
         # boolean flags
         f2py_args = ['--%s' % k for k, v in vars(args).items() if v is True]
 
         try:
             base_str_class = basestring
         except NameError:
@@ -345,34 +410,43 @@
 
         if args.extra:
             extras = ' '.join(map(unquote, args.extra))
             extras = extras.split()
             f2py_args.extend(extras)
 
         code = cell if cell.endswith('\n') else cell + '\n'
-        key = code, line, sys.version_info, sys.executable, f2py2e.f2py_version
+        self._cache_check()
+        key = (code, line, f_config,
+               self._lib_dir,
+               sys.version_info, sys.executable, f2py2e.f2py_version)
 
         module_name = "_fortran_magic_" + \
                       hashlib.md5(str(key).encode('utf-8')).hexdigest()
 
-        module_path = os.path.join(self._lib_dir, module_name + self.so_ext)
+        if module_name in sys.modules:
+            module = sys.modules[module_name]
+            print("The extension", module_name,
+                  "is already loaded. To reload it, use:")
+            print("  %fortran_config --clean-cache")
+        else:
+            module_path = os.path.join(self._lib_dir, module_name + self.so_ext)
 
-        f90_file = os.path.join(self._lib_dir, module_name + '.f90')
-        f90_file = py3compat.cast_bytes_py2(f90_file,
-                                            encoding=sys.getfilesystemencoding())
-        with io.open(f90_file, 'w', encoding='utf-8') as f:
-            f.write(code)
-
-        res = self._run_f2py(f2py_args + ['-m', module_name, '-c', f90_file],
-                             verbosity=args.verbosity)
-        if res != 0:
-           raise RuntimeError("f2py failed, see output")
+            f90_file = os.path.join(self._lib_dir, module_name + '.f90')
+            f90_file = py3compat.cast_bytes_py2(f90_file,
+                                                encoding=sys.getfilesystemencoding())
+            with io.open(f90_file, 'w', encoding='utf-8') as f:
+                f.write(code)
+
+            res = self._run_f2py(f2py_args + ['-m', module_name, '-c', f90_file],
+                                 verbosity=args.verbosity)
+            if res != 0:
+                raise RuntimeError("f2py failed, see output")
 
-        self._code_cache[key] = module_name
-        module = imp.load_dynamic(module_name, module_path)
+            self._code_cache[key] = module_name
+            module = _imp_load_dynamic(module_name, module_path)
         self._import_all(module, verbosity=args.verbosity, code=code)
 
     @property
     def so_ext(self):
         """The extension suffix for compiled modules."""
         try:
             return self._so_ext
@@ -386,21 +460,27 @@
                 pass
             dist.parse_config_files(config_files)
             build_extension = build_ext(dist)
             build_extension.finalize_options()
             self._so_ext = build_extension.get_ext_filename('')
             return self._so_ext
 
+
 __doc__ = __doc__.format(FORTRAN_DOC=' ' * 8 + FortranMagics.fortran.__doc__)
 
 
 def load_ipython_extension(ip):
     """Load the extension in IPython."""
     ip.register_magics(FortranMagics)
 
     # enable fortran highlight
-    patch = ("IPython.config.cell_magic_highlight['magic_fortran'] = "
-             "{'reg':[/^%%fortran/]};")
-    js = display.Javascript(data=patch,
-                            lib=["https://raw.github.com/marijnh/CodeMirror/master/mode/"
-                                 "fortran/fortran.js"])
+    patch = """
+        if(typeof IPython === 'undefined') {
+            console.log('fortranmagic.py: TDOO: JupyterLab ' +
+                        'syntax highlight - unimplemented.');
+        } else {
+            IPython.CodeCell.options_default
+            .highlight_modes['magic_fortran'] = {'reg':[/^%%fortran/]};
+        }
+        """
+    js = display.Javascript(data=patch)
     display.display_javascript(js)
```

### Comparing `fortran-magic-0.7.1/setup.py` & `fortran-magic-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 long_description = (open('README.rst').read() + '\n\n' +
                     open('CHANGES.rst').read())
 
 setup(
     name='fortran-magic',
-    version='0.7.1',
+    version='0.8',
     description='An extension for IPython that help to use Fortran in '
                 'your interactive session.',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author='Martin Gaitan',
     author_email='gaitan@gmail.com',
     url='https://github.com/mgaitan/fortran_magic',
```

