# Comparing `tmp/gsd-2.9.0.tar.gz` & `tmp/gsd-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsd-2.9.0.tar", last modified: Fri May 19 18:14:19 2023, max compression
+gzip compressed data, was "gsd-3.0.0.tar", last modified: Fri Jun 16 16:02:16 2023, max compression
```

## Comparing `gsd-2.9.0.tar` & `gsd-3.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:14:19.489557 gsd-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-19 18:14:04.000000 gsd-2.9.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-19 18:14:04.000000 gsd-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-19 18:14:04.000000 gsd-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-19 18:14:19.489557 gsd-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-19 18:14:04.000000 gsd-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:14:19.485557 gsd-2.9.0/gsd/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   722119 2023-05-19 18:14:18.000000 gsd-2.9.0/gsd/fl.c
--rw-r--r--   0 runner    (1001) docker     (123)    38073 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/fl.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    70351 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/gsd.c
--rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/gsd.h
--rw-r--r--   0 runner    (1001) docker     (123)    47184 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/libgsd.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/pygsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/pytest_plugin_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:14:19.489557 gsd-2.9.0/gsd/test/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)    34820 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/test_fl.py
--rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/test_gsd_v1.gsd
--rw-r--r--   0 runner    (1001) docker     (123)    34233 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/test_hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/test_largefile.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:14:19.485557 gsd-2.9.0/gsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-19 18:14:04.000000 gsd-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-19 18:14:19.489557 gsd-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-19 18:14:04.000000 gsd-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:02:16.929646 gsd-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-16 16:02:02.000000 gsd-3.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-16 16:02:02.000000 gsd-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 16:02:02.000000 gsd-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-16 16:02:16.929646 gsd-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-16 16:02:02.000000 gsd-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:02:16.925646 gsd-3.0.0/gsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   722151 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd/fl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/fl.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    73766 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/gsd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/gsd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45314 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/libgsd.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/pygsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/pytest_plugin_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:02:16.929646 gsd-3.0.0/gsd/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/test_fl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/test_gsd_v1.gsd
+-rw-r--r--   0 runner    (1001) docker     (123)    34233 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/test_hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/test_largefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:02:16.929646 gsd-3.0.0/gsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-16 16:02:02.000000 gsd-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-16 16:02:16.929646 gsd-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 16:02:02.000000 gsd-3.0.0/setup.py
```

### Comparing `gsd-2.9.0/CHANGELOG.rst` & `gsd-3.0.0/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,57 @@
 
 Change Log
 ==========
 
 `GSD <https://github.com/glotzerlab/gsd>`_ releases follow `semantic versioning
 <https://semver.org/>`_.
 
-v2.x
-----
+3.x
+---
 
-v2.9.0 (2023-05-19)
-^^^^^^^^^^^^^^^^^^^
+3.0.0 (2023-06-16)
+^^^^^^^^^^^^^^^^^^
+
+*Added:*
+
+* ``gsd.version.version`` - version string identifier. PEP8 compliant name replaces ``__version__``.
+* ``GSDFile.flush`` - flush write buffers (C API ``gsd_flush``)
+  (`#237 <https://github.com/glotzerlab/gsd/pull/237>`__).
+* ``GSDFile.maximum_write_buffer_size`` - get/set the write buffer size
+  (C API ``gsd_get_maximum_write_buffer_size`` / ``gsd_set_maximum_write_buffer_size``)
+  (`#237 <https://github.com/glotzerlab/gsd/pull/237>`__).
+* ``GSDFile.index_entries_to_buffer`` - get/set the write buffer size
+  (C API ``index_entries_to_buffer`` / ``index_entries_to_buffer``)
+  (`#237 <https://github.com/glotzerlab/gsd/pull/237>`__).
+* On importing `gsd`, install a ``SIGTERM`` handler that calls ``sys.exit(1)``
+  (`#237 <https://github.com/glotzerlab/gsd/pull/237>`__).
+
+*Changed:*
+
+* ``write_chunk`` buffers writes across frames to increase performance
+  (`#237 <https://github.com/glotzerlab/gsd/pull/237>`__).
+* Use *Doxygen* and *breathe* to generate C API documentation in Sphinx
+  (`#237 <https://github.com/glotzerlab/gsd/pull/237>`__).
+
+*Removed:*
+
+* ``gsd.__version__`` - use ``gsd.version.version``.
+* ``gsd.hoomd.Snapshot`` - use ``gsd.hoomd.Frame``
+  (`#249 <https://github.com/glotzerlab/gsd/pull/249>`__).
+* ``gsd.hoomd.HOOMDTrajectory.read_frame`` - use ``gsd.hoomd.HOOMDTrajectory.__getitem__``
+  (`#249 <https://github.com/glotzerlab/gsd/pull/249>`__).
+* The file modes ``'wb'``, ``'wb+'``, ``'rb'``,  ``'rb+'``, ``'ab'``, ``'xb'``, and ``'xb+'``. Use
+  ``'r'``, ``'r+'``, ``'w'``, ``'x'``, or ``'a'``
+  (`#249 <https://github.com/glotzerlab/gsd/pull/249>`__).
+
+2.x
+---
+
+2.9.0 (2023-05-19)
+^^^^^^^^^^^^^^^^^^
 
 *Added:*
 
 * File modes ``'r'``, ``'r+'``, ``'w'``, ``'x'``, and ``'a'``
   (`#238 <https://github.com/glotzerlab/gsd/pull/238>`__).
 
 *Changed:*
```

### Comparing `gsd-2.9.0/LICENSE` & `gsd-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gsd-2.9.0/PKG-INFO` & `gsd-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 2.9.0
+Version: 3.0.0
 Summary: General simulation data file format.
 Author-email: "Joshua A. Anderson" <joaander@umich.edu>
 License: BSD-2-Clause
 Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v2.9.0/gsd-v2.9.0.tar.gz
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.0.0/gsd-3.0.0.tar.gz
 Project-URL: Source, https://github.com/glotzerlab/gsd
 Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
@@ -58,15 +58,15 @@
 ```python
 >>> def create_frame(i):
 ...     s = gsd.hoomd.Frame();
 ...     s.configuration.step = i;
 ...     s.particles.N = 4+i;
 ...     s.particles.position = numpy.random.random(size=(4+i,3))
 ...     return s;
->>> with gsd.hoomd.open('test.gsd', 'ab') as t:
+>>> with gsd.hoomd.open('test.gsd', 'a') as t:
 ...     t.extend( (create_frame(i) for i in range(10)) )
 ...     print(len(t))
 11
 ```
 
 Randomly index frames:
 ```python
```

### Comparing `gsd-2.9.0/README.md` & `gsd-3.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ```python
 >>> def create_frame(i):
 ...     s = gsd.hoomd.Frame();
 ...     s.configuration.step = i;
 ...     s.particles.N = 4+i;
 ...     s.particles.position = numpy.random.random(size=(4+i,3))
 ...     return s;
->>> with gsd.hoomd.open('test.gsd', 'ab') as t:
+>>> with gsd.hoomd.open('test.gsd', 'a') as t:
 ...     t.extend( (create_frame(i) for i in range(10)) )
 ...     print(len(t))
 11
 ```
 
 Randomly index frames:
 ```python
```

### Comparing `gsd-2.9.0/gsd/__main__.py` & `gsd-3.0.0/gsd/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     accepted by :func:`gsd.fl.open`.
 """
 
 import sys
 import argparse
 import code
 
-from .version import __version__
+from . import version
 from .hoomd import open as hoomd_open
 from . import fl
 
 
 def _print_err(msg=None, *args):
     print(msg, *args, file=sys.stderr)
 
@@ -76,15 +76,15 @@
         })
 
     extras = "\n".join(
         "{}: {}".format(key, val) for key, val in attributes.items())
 
     code.interact(local=local_ns,
                   banner=SHELL_BANNER.format(python_version=sys.version,
-                                             gsd_version=__version__,
+                                             gsd_version=version.version,
                                              fn=args.file,
                                              extras=extras + "\n"))
 
 
 def main():
     """Entry point to the GSD command-line interface.
 
@@ -137,15 +137,15 @@
                              help="The file mode.")
     parser_read.set_defaults(func=main_read)
 
     # This is a hack, as argparse itself does not
     # allow to parse only --version without any
     # of the other required arguments.
     if '--version' in sys.argv:
-        print('gsd', __version__)
+        print('gsd', version.version)
         sys.exit(0)
 
     args = parser.parse_args()
 
     if not hasattr(args, 'func'):
         parser.print_usage()
         sys.exit(2)
```

### Comparing `gsd-2.9.0/gsd/fl.c` & `gsd-3.0.0/gsd/fl.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "gsd/gsd.h"
         ],
         "include_dirs": [
             "./gsd",
-            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "gsd.fl",
         "sources": [
             "gsd/fl.pyx",
             "gsd/gsd.c"
         ]
     },
@@ -36,16 +36,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -105,16 +105,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1065,195 +1069,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1281,51 +1285,51 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_3gsd_2fl_GSDFile;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "gsd/fl.pyx":251
+/* "gsd/fl.pyx":229
  * 
  * 
  * cdef class GSDFile:             # <<<<<<<<<<<<<<
  *     """GSDFile
  * 
  */
 struct __pyx_obj_3gsd_2fl_GSDFile {
@@ -1729,30 +1733,30 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -2034,50 +2038,43 @@
 extern int __pyx_module_is_main_gsd__fl;
 int __pyx_module_is_main_gsd__fl = 0;
 
 /* Implementation of 'gsd.fl' */
 static PyObject *__pyx_builtin_IOError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_MemoryError;
-static PyObject *__pyx_builtin_FutureWarning;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_KeyError;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_r[] = "r";
 static const char __pyx_k_w[] = "w";
 static const char __pyx_k_x[] = "x";
-static const char __pyx_k_ab[] = "ab";
+static const char __pyx_k__5[] = " - ";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_rb[] = "rb";
-static const char __pyx_k_wb[] = "wb";
-static const char __pyx_k_xb[] = "xb";
-static const char __pyx_k__12[] = " - ";
 static const char __pyx_k_r_2[] = "r+";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_file[] = "file ";
 static const char __pyx_k_info[] = "info";
 static const char __pyx_k_int8[] = "int8";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_open[] = "open";
 static const char __pyx_k_path[] = "path";
-static const char __pyx_k_rb_2[] = "rb+";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_view[] = "view";
-static const char __pyx_k_warn[] = "warn";
-static const char __pyx_k_wb_2[] = "wb+";
-static const char __pyx_k_xb_2[] = "xb+";
 static const char __pyx_k_chunk[] = " / chunk ";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_debug[] = "debug";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
+static const char __pyx_k_flush[] = "flush: ";
 static const char __pyx_k_frame[] = "frame";
 static const char __pyx_k_int16[] = "int16";
 static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_int64[] = "int64";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_uint8[] = "uint8";
@@ -2121,15 +2118,14 @@
 static const char __pyx_k_write_chunk[] = "write chunk: ";
 static const char __pyx_k_Invalid_mode[] = "Invalid mode: ";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_chunk_exists[] = "chunk exists: ";
 static const char __pyx_k_closing_file[] = "closing file: ";
 static const char __pyx_k_not_found_in[] = " not found in: ";
 static const char __pyx_k_opening_file[] = "opening file: ";
-static const char __pyx_k_FutureWarning[] = "FutureWarning";
 static const char __pyx_k_Unknown_error[] = "Unknown error: ";
 static const char __pyx_k_application_2[] = ", application: ";
 static const char __pyx_k_Not_a_GSD_file[] = "Not a GSD file: ";
 static const char __pyx_k_schema_version[] = "schema_version";
 static const char __pyx_k_upgrading_file[] = "upgrading file: ";
 static const char __pyx_k_truncating_file[] = "truncating file: ";
 static const char __pyx_k_Corrupt_GSD_file[] = "Corrupt GSD file: ";
@@ -2142,35 +2138,27 @@
 static const char __pyx_k_Invalid_gsd_argument[] = "Invalid gsd argument: ";
 static const char __pyx_k_has_incorrect_schema[] = " has incorrect schema: ";
 static const char __pyx_k_File_must_be_readable[] = "File must be readable: ";
 static const char __pyx_k_File_must_be_writable[] = "File must be writable: ";
 static const char __pyx_k_invalid_type_for_chunk[] = "invalid type for chunk: ";
 static const char __pyx_k_Memory_allocation_failed[] = "Memory allocation failed: ";
 static const char __pyx_k_Unsupported_GSD_file_version[] = "Unsupported GSD file version: ";
-static const char __pyx_k_The_ab_mode_is_deprecated_use_r[] = "The 'ab' mode is deprecated, use 'r+'";
-static const char __pyx_k_The_rb_mode_is_deprecated_use_r[] = "The 'rb' mode is deprecated, use 'r'";
-static const char __pyx_k_The_wb_mode_is_deprecated_use_w[] = "The 'wb' mode is deprecated, use 'w'";
-static const char __pyx_k_The_xb_mode_is_deprecated_use_x[] = "The 'xb' mode is deprecated, use 'x'";
 static const char __pyx_k_implicit_data_copy_when_writing[] = "implicit data copy when writing chunk: ";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_GSD_can_only_write_1_or_2_dimens[] = "GSD can only write 1 or 2 dimensional arrays: ";
 static const char __pyx_k_GSD_file_layer_API_Low_level_acc[] = "GSD file layer API.\n\nLow level access to gsd files. :py:mod:`gsd.fl` allows direct access to create,\nread, and write ``gsd`` files. The module is implemented in C and is optimized.\nSee :ref:`fl-examples` for detailed example code.\n\n* :py:class:`GSDFile` - Class interface to read and write gsd files.\n* :py:func:`open` - Open a gsd file.\n\n";
 static const char __pyx_k_Only_read_only_GSDFiles_can_be_p[] = "Only read only GSDFiles can be pickled.";
 static const char __pyx_k_Provide_application_when_creatin[] = "Provide application when creating a file";
 static const char __pyx_k_Provide_schema_version_when_crea[] = "Provide schema_version when creating a file";
 static const char __pyx_k_Provide_schema_when_creating_a_f[] = "Provide schema when creating a file";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static const char __pyx_k_The_rb_mode_is_deprecated_use_r_2[] = "The 'rb+' mode is deprecated, use 'r+'";
-static const char __pyx_k_The_wb_mode_is_deprecated_use_w_2[] = "The 'wb+' mode is deprecated, use 'w'";
-static const char __pyx_k_The_xb_mode_is_deprecated_use_x_2[] = "The 'xb+' mode is deprecated, use 'x'";
 static PyObject *__pyx_kp_u_Corrupt_GSD_file;
 static PyObject *__pyx_kp_u_File_is_not_open;
 static PyObject *__pyx_kp_u_File_must_be_readable;
 static PyObject *__pyx_kp_u_File_must_be_writable;
-static PyObject *__pyx_n_s_FutureWarning;
 static PyObject *__pyx_n_s_GSDFile;
 static PyObject *__pyx_kp_u_GSD_can_only_write_1_or_2_dimens;
 static PyObject *__pyx_kp_u_GSD_namelist_is_full;
 static PyObject *__pyx_n_s_IOError;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_u_Invalid_gsd_argument;
 static PyObject *__pyx_kp_u_Invalid_mode;
@@ -2180,27 +2168,19 @@
 static PyObject *__pyx_kp_u_Not_a_GSD_file;
 static PyObject *__pyx_kp_u_Only_read_only_GSDFiles_can_be_p;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_kp_u_Provide_application_when_creatin;
 static PyObject *__pyx_kp_u_Provide_schema_version_when_crea;
 static PyObject *__pyx_kp_u_Provide_schema_when_creating_a_f;
 static PyObject *__pyx_n_s_RuntimeError;
-static PyObject *__pyx_kp_u_The_ab_mode_is_deprecated_use_r;
-static PyObject *__pyx_kp_u_The_rb_mode_is_deprecated_use_r;
-static PyObject *__pyx_kp_u_The_rb_mode_is_deprecated_use_r_2;
-static PyObject *__pyx_kp_u_The_wb_mode_is_deprecated_use_w;
-static PyObject *__pyx_kp_u_The_wb_mode_is_deprecated_use_w_2;
-static PyObject *__pyx_kp_u_The_xb_mode_is_deprecated_use_x;
-static PyObject *__pyx_kp_u_The_xb_mode_is_deprecated_use_x_2;
 static PyObject *__pyx_kp_u_Unknown_error;
 static PyObject *__pyx_kp_u_Unsupported_GSD_file_version;
 static PyObject *__pyx_n_s_ValueError;
-static PyObject *__pyx_kp_u__12;
+static PyObject *__pyx_kp_u__5;
 static PyObject *__pyx_n_u_a;
-static PyObject *__pyx_n_u_ab;
 static PyObject *__pyx_kp_u_and_schema_version;
 static PyObject *__pyx_n_s_application;
 static PyObject *__pyx_kp_u_application_2;
 static PyObject *__pyx_n_s_ascontiguousarray;
 static PyObject *__pyx_kp_u_chunk;
 static PyObject *__pyx_kp_u_chunk_exists;
 static PyObject *__pyx_n_s_cline_in_traceback;
@@ -2214,14 +2194,15 @@
 static PyObject *__pyx_kp_u_end_frame;
 static PyObject *__pyx_n_s_exc_type;
 static PyObject *__pyx_n_s_exc_value;
 static PyObject *__pyx_n_s_exists;
 static PyObject *__pyx_kp_u_file;
 static PyObject *__pyx_n_s_float32;
 static PyObject *__pyx_n_s_float64;
+static PyObject *__pyx_kp_u_flush;
 static PyObject *__pyx_n_s_frame;
 static PyObject *__pyx_kp_u_frame_2;
 static PyObject *__pyx_n_s_getLogger;
 static PyObject *__pyx_n_s_gsd_fl;
 static PyObject *__pyx_kp_u_gsd_fl;
 static PyObject *__pyx_kp_s_gsd_fl_pyx;
 static PyObject *__pyx_kp_u_has_incorrect_schema;
@@ -2248,15 +2229,14 @@
 static PyObject *__pyx_n_s_os;
 static PyObject *__pyx_kp_u_overwriting_file;
 static PyObject *__pyx_n_s_path;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_u_r;
 static PyObject *__pyx_kp_u_r_2;
 static PyObject *__pyx_n_u_rb;
-static PyObject *__pyx_kp_u_rb_2;
 static PyObject *__pyx_kp_u_read_chunk;
 static PyObject *__pyx_n_s_reshape;
 static PyObject *__pyx_n_s_schema;
 static PyObject *__pyx_kp_u_schema_2;
 static PyObject *__pyx_n_s_schema_version;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
@@ -2268,64 +2248,57 @@
 static PyObject *__pyx_n_s_uint32;
 static PyObject *__pyx_n_s_uint64;
 static PyObject *__pyx_n_s_uint8;
 static PyObject *__pyx_kp_u_upgrading_file;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_view;
 static PyObject *__pyx_n_u_w;
-static PyObject *__pyx_n_s_warn;
 static PyObject *__pyx_n_s_warning;
 static PyObject *__pyx_n_s_warnings;
-static PyObject *__pyx_n_u_wb;
-static PyObject *__pyx_kp_u_wb_2;
 static PyObject *__pyx_kp_u_with_mode;
 static PyObject *__pyx_kp_u_write_chunk;
 static PyObject *__pyx_n_u_x;
-static PyObject *__pyx_n_u_xb;
-static PyObject *__pyx_kp_u_xb_2;
 static PyObject *__pyx_pf_3gsd_2fl_open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name, PyObject *__pyx_v_mode, PyObject *__pyx_v_application, PyObject *__pyx_v_schema, PyObject *__pyx_v_schema_version); /* proto */
 static int __pyx_pf_3gsd_2fl_7GSDFile___init__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_mode, PyObject *__pyx_v_application, PyObject *__pyx_v_schema, PyObject *__pyx_v_schema_version); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_2close(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4truncate(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_6end_frame(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_8write_chunk(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_10chunk_exists(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_12read_chunk(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_14find_matching_chunk_names(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_match); /* proto */
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_16upgrade(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_18__enter__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_20__exit__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_type, CYTHON_UNUSED PyObject *__pyx_v_exc_value, CYTHON_UNUSED PyObject *__pyx_v_traceback); /* proto */
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_22__reduce__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_8flush(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_10write_chunk(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_12chunk_exists(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_14read_chunk(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_16find_matching_chunk_names(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_match); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_18upgrade(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_20__enter__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_22__exit__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_type, CYTHON_UNUSED PyObject *__pyx_v_exc_value, CYTHON_UNUSED PyObject *__pyx_v_traceback); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_24__reduce__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4name___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4mode___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_11gsd_version___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_14schema_version___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_6schema___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_11application___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_7nframes___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
-static void __pyx_pf_3gsd_2fl_7GSDFile_24__dealloc__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_25maximum_write_buffer_size___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
+static int __pyx_pf_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_2__set__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_size); /* proto */
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_23index_entries_to_buffer___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
+static int __pyx_pf_3gsd_2fl_7GSDFile_23index_entries_to_buffer_2__set__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_number); /* proto */
+static void __pyx_pf_3gsd_2fl_7GSDFile_26__dealloc__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_tp_new_3gsd_2fl_GSDFile(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_tuple__13;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__15;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_codeobj__17;
+static PyObject *__pyx_codeobj__10;
 /* Late includes */
 
 /* "gsd/fl.pyx":31
  * # Helper functions #
  * 
  * cdef __format_errno(fname):             # <<<<<<<<<<<<<<
  *     """Return a tuple for constructing an IOError."""
@@ -4394,15 +4367,15 @@
  * def open(name, mode, application=None, schema=None, schema_version=None):             # <<<<<<<<<<<<<<
  *     """open(name, mode, application=None, schema=None, schema_version=None)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_1open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_3gsd_2fl_open[] = "open(name, mode, application=None, schema=None, schema_version=None)\n\n    :py:func:`open` opens a GSD file and returns a :py:class:`GSDFile` instance.\n    The return value of :py:func:`open` can be used as a context manager.\n\n    Args:\n        name (str): File name to open.\n\n        mode (str): File access mode.\n\n        application (str): Name of the application creating the file.\n\n        schema (str): Name of the data schema.\n\n        schema_version (tuple[int, int]): Schema version number\n            (major, minor).\n\n    Valid values for ``mode``:\n\n    +------------------+---------------------------------------------+\n    | mode             | description                                 |\n    +==================+=============================================+\n    | ``'r'``          | Open an existing file for reading.          |\n    +------------------+---------------------------------------------+\n    | ``'r+'``         | Open an existing file for reading and       |\n    |                  | writing.                                    |\n    +------------------+---------------------------------------------+\n    | ``'w'``          | Open a file for reading and writing.        |\n    |                  | Creates the file if needed, or overwrites   |\n    |                  | an existing file.                           |\n    +------------------+---------------------------------------------+\n    | ``'x'``          | Create a gsd file exclusively and opens it  |\n    |                  | for reading and writing.                    |\n    |                  | Raise :py:exc:`FileExistsError`             |\n    |                  | if it already exists.                       |\n    +------------------+---------------------------------------------+\n    | ``'a'``          | Open a file for reading and writing.        |\n    |                  | Creates the file if it doesn't exist.       |\n    +------------------+------------------------------""---------------+\n\n    When opening a file for reading (``'r'`` and ``'r+'`` modes):\n    ``application`` and ``schema_version`` are ignored and may be ``None``.\n    When ``schema`` is not ``None``, :py:func:`open` throws an exception if the\n    file's schema does not match ``schema``.\n\n    When opening a file for writing (``'w'``, ``'x'``, or ``'a'`` modes): The\n    given ``application``, ``schema``, and ``schema_version`` must not be None.\n\n    .. deprecated:: 2.9.0\n\n        The following values to ``mode`` are deprecated:\n\n        +------------------+---------------------------------------------+\n        | mode             | description                                 |\n        +==================+=============================================+\n        | ``'rb'``         | Equivalent to ``'r'``                       |\n        +------------------+---------------------------------------------+\n        | ``'rb+'``        | Equivalent to ``'r+'``                      |\n        +------------------+---------------------------------------------+\n        | ``'wb'``         | Equivalent to ``'w'``                       |\n        +------------------+---------------------------------------------+\n        | ``'wb+'``        | Equivalent to ``'w'``                       |\n        +------------------+---------------------------------------------+\n        | ``'xb'``         | Equivalent to ``'x'``                       |\n        +------------------+---------------------------------------------+\n        | ``'xb+'``        | Equivalent to ``'x'``                       |\n        +------------------+---------------------------------------------+\n        | ``'ab'``         | Equivalent to ``'r+'``                      |\n        +------------------+---------------------------------------------+\n\n    Example:\n\n        .. ipython:: python\n\n            with gsd.fl.open(name='file.gsd', mode='w',\n                             application=\"My application""\", schema=\"My Schema\",\n                             schema_version=[1,0]) as f:\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([1,2,3,4], dtype=numpy.float32))\n                f.write_chunk(name='chunk2',\n                              data=numpy.array([[5,6],[7,8]],\n                                               dtype=numpy.float32))\n                f.end_frame()\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([9,10,11,12],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='chunk2',\n                              data=numpy.array([[13,14],[15,16]],\n                                               dtype=numpy.float32))\n                f.end_frame()\n\n            f = gsd.fl.open(name='file.gsd', mode='r')\n            if f.chunk_exists(frame=0, name='chunk1'):\n                data = f.read_chunk(frame=0, name='chunk1')\n            data\n            f.close()\n    ";
+static char __pyx_doc_3gsd_2fl_open[] = "open(name, mode, application=None, schema=None, schema_version=None)\n\n    :py:func:`open` opens a GSD file and returns a :py:class:`GSDFile` instance.\n    The return value of :py:func:`open` can be used as a context manager.\n\n    Args:\n        name (str): File name to open.\n\n        mode (str): File access mode.\n\n        application (str): Name of the application creating the file.\n\n        schema (str): Name of the data schema.\n\n        schema_version (tuple[int, int]): Schema version number\n            (major, minor).\n\n    Valid values for ``mode``:\n\n    +------------------+---------------------------------------------+\n    | mode             | description                                 |\n    +==================+=============================================+\n    | ``'r'``          | Open an existing file for reading.          |\n    +------------------+---------------------------------------------+\n    | ``'r+'``         | Open an existing file for reading and       |\n    |                  | writing.                                    |\n    +------------------+---------------------------------------------+\n    | ``'w'``          | Open a file for reading and writing.        |\n    |                  | Creates the file if needed, or overwrites   |\n    |                  | an existing file.                           |\n    +------------------+---------------------------------------------+\n    | ``'x'``          | Create a gsd file exclusively and opens it  |\n    |                  | for reading and writing.                    |\n    |                  | Raise :py:exc:`FileExistsError`             |\n    |                  | if it already exists.                       |\n    +------------------+---------------------------------------------+\n    | ``'a'``          | Open a file for reading and writing.        |\n    |                  | Creates the file if it doesn't exist.       |\n    +------------------+------------------------------""---------------+\n\n    When opening a file for reading (``'r'`` and ``'r+'`` modes):\n    ``application`` and ``schema_version`` are ignored and may be ``None``.\n    When ``schema`` is not ``None``, :py:func:`open` throws an exception if the\n    file's schema does not match ``schema``.\n\n    When opening a file for writing (``'w'``, ``'x'``, or ``'a'`` modes): The\n    given ``application``, ``schema``, and ``schema_version`` must not be None.\n\n    Example:\n\n        .. ipython:: python\n\n            with gsd.fl.open(name='file.gsd', mode='w',\n                             application=\"My application\", schema=\"My Schema\",\n                             schema_version=[1,0]) as f:\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([1,2,3,4], dtype=numpy.float32))\n                f.write_chunk(name='chunk2',\n                              data=numpy.array([[5,6],[7,8]],\n                                               dtype=numpy.float32))\n                f.end_frame()\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([9,10,11,12],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='chunk2',\n                              data=numpy.array([[13,14],[15,16]],\n                                               dtype=numpy.float32))\n                f.end_frame()\n\n            f = gsd.fl.open(name='file.gsd', mode='r')\n            if f.chunk_exists(frame=0, name='chunk1'):\n                data = f.read_chunk(frame=0, name='chunk1')\n            data\n            f.close()\n    ";
 static PyMethodDef __pyx_mdef_3gsd_2fl_1open = {"open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_1open, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3gsd_2fl_open};
 static PyObject *__pyx_pw_3gsd_2fl_1open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
   PyObject *__pyx_v_mode = 0;
   PyObject *__pyx_v_application = 0;
   PyObject *__pyx_v_schema = 0;
   PyObject *__pyx_v_schema_version = 0;
@@ -4509,25 +4482,25 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
 
-  /* "gsd/fl.pyx":248
+  /* "gsd/fl.pyx":226
  *     """
  * 
  *     return GSDFile(str(name), mode, application, schema, schema_version)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_v_mode);
   __Pyx_GIVEREF(__pyx_v_mode);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_mode);
   __Pyx_INCREF(__pyx_v_application);
@@ -4536,15 +4509,15 @@
   __Pyx_INCREF(__pyx_v_schema);
   __Pyx_GIVEREF(__pyx_v_schema);
   PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_v_schema);
   __Pyx_INCREF(__pyx_v_schema_version);
   __Pyx_GIVEREF(__pyx_v_schema_version);
   PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_v_schema_version);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "gsd/fl.pyx":149
@@ -4563,15 +4536,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":303
+/* "gsd/fl.pyx":286
  *     cdef str name
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  name,
  *                  mode,
  */
 
@@ -4614,37 +4587,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 1); __PYX_ERR(0, 303, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 1); __PYX_ERR(0, 286, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_application)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 2); __PYX_ERR(0, 303, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 2); __PYX_ERR(0, 286, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 3); __PYX_ERR(0, 303, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 3); __PYX_ERR(0, 286, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_schema_version)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 4); __PYX_ERR(0, 303, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 4); __PYX_ERR(0, 286, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 303, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 286, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 5) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -4655,15 +4628,15 @@
     __pyx_v_mode = values[1];
     __pyx_v_application = values[2];
     __pyx_v_schema = values[3];
     __pyx_v_schema_version = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 303, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 286, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile___init__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_name, __pyx_v_mode, __pyx_v_application, __pyx_v_schema, __pyx_v_schema_version);
 
@@ -4698,866 +4671,480 @@
   unsigned int __pyx_t_9;
   unsigned int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_INCREF(__pyx_v_mode);
 
-  /* "gsd/fl.pyx":310
+  /* "gsd/fl.pyx":293
  *                  schema_version):
  *         cdef libgsd.gsd_open_flag c_flags
  *         cdef int exclusive_create = 0             # <<<<<<<<<<<<<<
  *         cdef int overwrite = 0
  * 
  */
   __pyx_v_exclusive_create = 0;
 
-  /* "gsd/fl.pyx":311
+  /* "gsd/fl.pyx":294
  *         cdef libgsd.gsd_open_flag c_flags
  *         cdef int exclusive_create = 0
  *         cdef int overwrite = 0             # <<<<<<<<<<<<<<
  * 
  *         self.mode = mode
  */
   __pyx_v_overwrite = 0;
 
-  /* "gsd/fl.pyx":313
+  /* "gsd/fl.pyx":296
  *         cdef int overwrite = 0
  * 
  *         self.mode = mode             # <<<<<<<<<<<<<<
  * 
- *         if mode == 'wb':
+ *         if mode == 'w':
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_mode))||((__pyx_v_mode) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_mode)->tp_name), 0))) __PYX_ERR(0, 313, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_mode))||((__pyx_v_mode) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_mode)->tp_name), 0))) __PYX_ERR(0, 296, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_mode;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->mode);
   __Pyx_DECREF(__pyx_v_self->mode);
   __pyx_v_self->mode = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":315
+  /* "gsd/fl.pyx":298
  *         self.mode = mode
  * 
- *         if mode == 'wb':             # <<<<<<<<<<<<<<
- *             mode = 'w'
- *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
- */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_wb, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 315, __pyx_L1_error)
-  if (__pyx_t_2) {
-
-    /* "gsd/fl.pyx":316
- * 
- *         if mode == 'wb':
- *             mode = 'w'             # <<<<<<<<<<<<<<
- *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
- *                            FutureWarning)
- */
-    __Pyx_INCREF(__pyx_n_u_w);
-    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_w);
-
-    /* "gsd/fl.pyx":317
- *         if mode == 'wb':
- *             mode = 'w'
- *             warnings.warn("The 'wb' mode is deprecated, use 'w'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'wb+':
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 317, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":318
- *             mode = 'w'
- *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
- *                            FutureWarning)             # <<<<<<<<<<<<<<
- *         elif mode == 'wb+':
- *             mode = 'w'
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":315
- *         self.mode = mode
- * 
- *         if mode == 'wb':             # <<<<<<<<<<<<<<
- *             mode = 'w'
- *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
- */
-    goto __pyx_L3;
-  }
-
-  /* "gsd/fl.pyx":319
- *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
- *                            FutureWarning)
- *         elif mode == 'wb+':             # <<<<<<<<<<<<<<
- *             mode = 'w'
- *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
- */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_wb_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 319, __pyx_L1_error)
-  if (__pyx_t_2) {
-
-    /* "gsd/fl.pyx":320
- *                            FutureWarning)
- *         elif mode == 'wb+':
- *             mode = 'w'             # <<<<<<<<<<<<<<
- *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
- *                            FutureWarning)
- */
-    __Pyx_INCREF(__pyx_n_u_w);
-    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_w);
-
-    /* "gsd/fl.pyx":321
- *         elif mode == 'wb+':
- *             mode = 'w'
- *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'rb':
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 321, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":322
- *             mode = 'w'
- *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
- *                            FutureWarning)             # <<<<<<<<<<<<<<
- *         elif mode == 'rb':
- *             mode = 'r'
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":319
- *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
- *                            FutureWarning)
- *         elif mode == 'wb+':             # <<<<<<<<<<<<<<
- *             mode = 'w'
- *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
- */
-    goto __pyx_L3;
-  }
-
-  /* "gsd/fl.pyx":323
- *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
- *                            FutureWarning)
- *         elif mode == 'rb':             # <<<<<<<<<<<<<<
- *             mode = 'r'
- *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
- */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_rb, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 323, __pyx_L1_error)
-  if (__pyx_t_2) {
-
-    /* "gsd/fl.pyx":324
- *                            FutureWarning)
- *         elif mode == 'rb':
- *             mode = 'r'             # <<<<<<<<<<<<<<
- *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
- *                            FutureWarning)
- */
-    __Pyx_INCREF(__pyx_n_u_r);
-    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_r);
-
-    /* "gsd/fl.pyx":325
- *         elif mode == 'rb':
- *             mode = 'r'
- *             warnings.warn("The 'rb' mode is deprecated, use 'r'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'rb+':
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 325, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":326
- *             mode = 'r'
- *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
- *                            FutureWarning)             # <<<<<<<<<<<<<<
- *         elif mode == 'rb+':
- *             mode = 'r+'
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":323
- *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
- *                            FutureWarning)
- *         elif mode == 'rb':             # <<<<<<<<<<<<<<
- *             mode = 'r'
- *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
- */
-    goto __pyx_L3;
-  }
-
-  /* "gsd/fl.pyx":327
- *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
- *                            FutureWarning)
- *         elif mode == 'rb+':             # <<<<<<<<<<<<<<
- *             mode = 'r+'
- *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
- */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_rb_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 327, __pyx_L1_error)
-  if (__pyx_t_2) {
-
-    /* "gsd/fl.pyx":328
- *                            FutureWarning)
- *         elif mode == 'rb+':
- *             mode = 'r+'             # <<<<<<<<<<<<<<
- *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
- *                            FutureWarning)
- */
-    __Pyx_INCREF(__pyx_kp_u_r_2);
-    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_kp_u_r_2);
-
-    /* "gsd/fl.pyx":329
- *         elif mode == 'rb+':
- *             mode = 'r+'
- *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'xb':
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 329, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":330
- *             mode = 'r+'
- *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
- *                            FutureWarning)             # <<<<<<<<<<<<<<
- *         elif mode == 'xb':
- *             mode = 'x'
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":327
- *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
- *                            FutureWarning)
- *         elif mode == 'rb+':             # <<<<<<<<<<<<<<
- *             mode = 'r+'
- *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
- */
-    goto __pyx_L3;
-  }
-
-  /* "gsd/fl.pyx":331
- *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
- *                            FutureWarning)
- *         elif mode == 'xb':             # <<<<<<<<<<<<<<
- *             mode = 'x'
- *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
- */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_xb, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 331, __pyx_L1_error)
-  if (__pyx_t_2) {
-
-    /* "gsd/fl.pyx":332
- *                            FutureWarning)
- *         elif mode == 'xb':
- *             mode = 'x'             # <<<<<<<<<<<<<<
- *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
- *                            FutureWarning)
- */
-    __Pyx_INCREF(__pyx_n_u_x);
-    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_x);
-
-    /* "gsd/fl.pyx":333
- *         elif mode == 'xb':
- *             mode = 'x'
- *             warnings.warn("The 'xb' mode is deprecated, use 'x'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'xb+':
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 333, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":334
- *             mode = 'x'
- *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
- *                            FutureWarning)             # <<<<<<<<<<<<<<
- *         elif mode == 'xb+':
- *             mode = 'x'
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":331
- *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
- *                            FutureWarning)
- *         elif mode == 'xb':             # <<<<<<<<<<<<<<
- *             mode = 'x'
- *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
- */
-    goto __pyx_L3;
-  }
-
-  /* "gsd/fl.pyx":335
- *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
- *                            FutureWarning)
- *         elif mode == 'xb+':             # <<<<<<<<<<<<<<
- *             mode = 'x'
- *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
- */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_xb_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 335, __pyx_L1_error)
-  if (__pyx_t_2) {
-
-    /* "gsd/fl.pyx":336
- *                            FutureWarning)
- *         elif mode == 'xb+':
- *             mode = 'x'             # <<<<<<<<<<<<<<
- *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
- *                            FutureWarning)
- */
-    __Pyx_INCREF(__pyx_n_u_x);
-    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_x);
-
-    /* "gsd/fl.pyx":337
- *         elif mode == 'xb+':
- *             mode = 'x'
- *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'ab':
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":338
- *             mode = 'x'
- *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
- *                            FutureWarning)             # <<<<<<<<<<<<<<
- *         elif mode == 'ab':
- *             mode = 'r+'
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":335
- *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
- *                            FutureWarning)
- *         elif mode == 'xb+':             # <<<<<<<<<<<<<<
- *             mode = 'x'
- *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
- */
-    goto __pyx_L3;
-  }
-
-  /* "gsd/fl.pyx":339
- *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
- *                            FutureWarning)
- *         elif mode == 'ab':             # <<<<<<<<<<<<<<
- *             mode = 'r+'
- *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",
- */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_ab, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 339, __pyx_L1_error)
-  if (__pyx_t_2) {
-
-    /* "gsd/fl.pyx":340
- *                            FutureWarning)
- *         elif mode == 'ab':
- *             mode = 'r+'             # <<<<<<<<<<<<<<
- *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",
- *                            FutureWarning)
- */
-    __Pyx_INCREF(__pyx_kp_u_r_2);
-    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_kp_u_r_2);
-
-    /* "gsd/fl.pyx":341
- *         elif mode == 'ab':
- *             mode = 'r+'
- *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- * 
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":342
- *             mode = 'r+'
- *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",
- *                            FutureWarning)             # <<<<<<<<<<<<<<
- * 
- *         if mode == 'w':
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "gsd/fl.pyx":339
- *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
- *                            FutureWarning)
- *         elif mode == 'ab':             # <<<<<<<<<<<<<<
- *             mode = 'r+'
- *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",
- */
-  }
-  __pyx_L3:;
-
-  /* "gsd/fl.pyx":344
- *                            FutureWarning)
- * 
  *         if mode == 'w':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_w, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_w, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 298, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":345
+    /* "gsd/fl.pyx":299
  * 
  *         if mode == 'w':
  *             c_flags = libgsd.GSD_OPEN_READWRITE             # <<<<<<<<<<<<<<
  *             overwrite = 1
  *         elif mode == 'r':
  */
     __pyx_v_c_flags = GSD_OPEN_READWRITE;
 
-    /* "gsd/fl.pyx":346
+    /* "gsd/fl.pyx":300
  *         if mode == 'w':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1             # <<<<<<<<<<<<<<
  *         elif mode == 'r':
  *             c_flags = libgsd.GSD_OPEN_READONLY
  */
     __pyx_v_overwrite = 1;
 
-    /* "gsd/fl.pyx":344
- *                            FutureWarning)
+    /* "gsd/fl.pyx":298
+ *         self.mode = mode
  * 
  *         if mode == 'w':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  */
-    goto __pyx_L4;
+    goto __pyx_L3;
   }
 
-  /* "gsd/fl.pyx":347
+  /* "gsd/fl.pyx":301
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  *         elif mode == 'r':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READONLY
  *         elif mode == 'r+':
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_r, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 347, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_r, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 301, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":348
+    /* "gsd/fl.pyx":302
  *             overwrite = 1
  *         elif mode == 'r':
  *             c_flags = libgsd.GSD_OPEN_READONLY             # <<<<<<<<<<<<<<
  *         elif mode == 'r+':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  */
     __pyx_v_c_flags = GSD_OPEN_READONLY;
 
-    /* "gsd/fl.pyx":347
+    /* "gsd/fl.pyx":301
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  *         elif mode == 'r':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READONLY
  *         elif mode == 'r+':
  */
-    goto __pyx_L4;
+    goto __pyx_L3;
   }
 
-  /* "gsd/fl.pyx":349
+  /* "gsd/fl.pyx":303
  *         elif mode == 'r':
  *             c_flags = libgsd.GSD_OPEN_READONLY
  *         elif mode == 'r+':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *         elif mode == 'x':
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_r_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_r_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 303, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":350
+    /* "gsd/fl.pyx":304
  *             c_flags = libgsd.GSD_OPEN_READONLY
  *         elif mode == 'r+':
  *             c_flags = libgsd.GSD_OPEN_READWRITE             # <<<<<<<<<<<<<<
  *         elif mode == 'x':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  */
     __pyx_v_c_flags = GSD_OPEN_READWRITE;
 
-    /* "gsd/fl.pyx":349
+    /* "gsd/fl.pyx":303
  *         elif mode == 'r':
  *             c_flags = libgsd.GSD_OPEN_READONLY
  *         elif mode == 'r+':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *         elif mode == 'x':
  */
-    goto __pyx_L4;
+    goto __pyx_L3;
   }
 
-  /* "gsd/fl.pyx":351
+  /* "gsd/fl.pyx":305
  *         elif mode == 'r+':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *         elif mode == 'x':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_x, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_x, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 305, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":352
+    /* "gsd/fl.pyx":306
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *         elif mode == 'x':
  *             c_flags = libgsd.GSD_OPEN_READWRITE             # <<<<<<<<<<<<<<
  *             overwrite = 1
  *             exclusive_create = 1
  */
     __pyx_v_c_flags = GSD_OPEN_READWRITE;
 
-    /* "gsd/fl.pyx":353
+    /* "gsd/fl.pyx":307
  *         elif mode == 'x':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1             # <<<<<<<<<<<<<<
  *             exclusive_create = 1
  *         elif mode == 'a':
  */
     __pyx_v_overwrite = 1;
 
-    /* "gsd/fl.pyx":354
+    /* "gsd/fl.pyx":308
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  *             exclusive_create = 1             # <<<<<<<<<<<<<<
  *         elif mode == 'a':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  */
     __pyx_v_exclusive_create = 1;
 
-    /* "gsd/fl.pyx":351
+    /* "gsd/fl.pyx":305
  *         elif mode == 'r+':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *         elif mode == 'x':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  */
-    goto __pyx_L4;
+    goto __pyx_L3;
   }
 
-  /* "gsd/fl.pyx":355
+  /* "gsd/fl.pyx":309
  *             overwrite = 1
  *             exclusive_create = 1
  *         elif mode == 'a':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             if not os.path.exists(name):
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_a, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_a, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 309, __pyx_L1_error)
   if (likely(__pyx_t_2)) {
 
-    /* "gsd/fl.pyx":356
+    /* "gsd/fl.pyx":310
  *             exclusive_create = 1
  *         elif mode == 'a':
  *             c_flags = libgsd.GSD_OPEN_READWRITE             # <<<<<<<<<<<<<<
  *             if not os.path.exists(name):
  *                 overwrite = 1
  */
     __pyx_v_c_flags = GSD_OPEN_READWRITE;
 
-    /* "gsd/fl.pyx":357
+    /* "gsd/fl.pyx":311
  *         elif mode == 'a':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             if not os.path.exists(name):             # <<<<<<<<<<<<<<
  *                 overwrite = 1
  *         else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_path); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_path); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_exists); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_exists); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_name);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_5 = ((!__pyx_t_2) != 0);
     if (__pyx_t_5) {
 
-      /* "gsd/fl.pyx":358
+      /* "gsd/fl.pyx":312
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             if not os.path.exists(name):
  *                 overwrite = 1             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("Invalid mode: " + mode)
  */
       __pyx_v_overwrite = 1;
 
-      /* "gsd/fl.pyx":357
+      /* "gsd/fl.pyx":311
  *         elif mode == 'a':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             if not os.path.exists(name):             # <<<<<<<<<<<<<<
  *                 overwrite = 1
  *         else:
  */
     }
 
-    /* "gsd/fl.pyx":355
+    /* "gsd/fl.pyx":309
  *             overwrite = 1
  *             exclusive_create = 1
  *         elif mode == 'a':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             if not os.path.exists(name):
  */
-    goto __pyx_L4;
+    goto __pyx_L3;
   }
 
-  /* "gsd/fl.pyx":360
+  /* "gsd/fl.pyx":314
  *                 overwrite = 1
  *         else:
  *             raise ValueError("Invalid mode: " + mode)             # <<<<<<<<<<<<<<
  * 
  *         self.name = name
  */
   /*else*/ {
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Invalid_mode, __pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Invalid_mode, __pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 360, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 314, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 360, __pyx_L1_error)
+    __PYX_ERR(0, 314, __pyx_L1_error)
   }
-  __pyx_L4:;
+  __pyx_L3:;
 
-  /* "gsd/fl.pyx":362
+  /* "gsd/fl.pyx":316
  *             raise ValueError("Invalid mode: " + mode)
  * 
  *         self.name = name             # <<<<<<<<<<<<<<
  * 
  *         cdef char * c_name
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_name))||((__pyx_v_name) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_name)->tp_name), 0))) __PYX_ERR(0, 362, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_name))||((__pyx_v_name) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_name)->tp_name), 0))) __PYX_ERR(0, 316, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_name;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":370
+  /* "gsd/fl.pyx":324
  *         cdef str schema_truncated
  * 
  *         if overwrite:             # <<<<<<<<<<<<<<
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")
  */
   __pyx_t_5 = (__pyx_v_overwrite != 0);
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":371
+    /* "gsd/fl.pyx":325
  * 
  *         if overwrite:
  *             if application is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:
  */
     __pyx_t_5 = (__pyx_v_application == Py_None);
     __pyx_t_2 = (__pyx_t_5 != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "gsd/fl.pyx":372
+      /* "gsd/fl.pyx":326
  *         if overwrite:
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")             # <<<<<<<<<<<<<<
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 326, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 372, __pyx_L1_error)
+      __PYX_ERR(0, 326, __pyx_L1_error)
 
-      /* "gsd/fl.pyx":371
+      /* "gsd/fl.pyx":325
  * 
  *         if overwrite:
  *             if application is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:
  */
     }
 
-    /* "gsd/fl.pyx":373
+    /* "gsd/fl.pyx":327
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:
  */
     __pyx_t_2 = (__pyx_v_schema == Py_None);
     __pyx_t_5 = (__pyx_t_2 != 0);
     if (unlikely(__pyx_t_5)) {
 
-      /* "gsd/fl.pyx":374
+      /* "gsd/fl.pyx":328
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")             # <<<<<<<<<<<<<<
  *             if schema_version is None:
  *                 raise ValueError("Provide schema_version when creating a file")
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 328, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 374, __pyx_L1_error)
+      __PYX_ERR(0, 328, __pyx_L1_error)
 
-      /* "gsd/fl.pyx":373
+      /* "gsd/fl.pyx":327
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:
  */
     }
 
-    /* "gsd/fl.pyx":375
+    /* "gsd/fl.pyx":329
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide schema_version when creating a file")
  * 
  */
     __pyx_t_5 = (__pyx_v_schema_version == Py_None);
     __pyx_t_2 = (__pyx_t_5 != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "gsd/fl.pyx":376
+      /* "gsd/fl.pyx":330
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:
  *                 raise ValueError("Provide schema_version when creating a file")             # <<<<<<<<<<<<<<
  * 
  *             # create a new file or overwrite an existing one
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 376, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 376, __pyx_L1_error)
+      __PYX_ERR(0, 330, __pyx_L1_error)
 
-      /* "gsd/fl.pyx":375
+      /* "gsd/fl.pyx":329
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide schema_version when creating a file")
  * 
  */
     }
 
-    /* "gsd/fl.pyx":379
+    /* "gsd/fl.pyx":333
  * 
  *             # create a new file or overwrite an existing one
  *             logger.info('overwriting file: ' + name + ' with mode: ' + mode             # <<<<<<<<<<<<<<
  *                         + ', application: ' + application
  *                         + ', schema: ' + schema
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_overwriting_file, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_overwriting_file, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_with_mode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_with_mode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "gsd/fl.pyx":380
+    /* "gsd/fl.pyx":334
  *             # create a new file or overwrite an existing one
  *             logger.info('overwriting file: ' + name + ' with mode: ' + mode
  *                         + ', application: ' + application             # <<<<<<<<<<<<<<
  *                         + ', schema: ' + schema
  *                         + ', and schema_version: ' + str(schema_version))
  */
-    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_application_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 380, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_application_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_application); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 380, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_application); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "gsd/fl.pyx":381
+    /* "gsd/fl.pyx":335
  *             logger.info('overwriting file: ' + name + ' with mode: ' + mode
  *                         + ', application: ' + application
  *                         + ', schema: ' + schema             # <<<<<<<<<<<<<<
  *                         + ', and schema_version: ' + str(schema_version))
  *             name_e = name.encode('utf-8')
  */
-    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_schema_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 381, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_schema_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_schema); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 381, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_schema); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "gsd/fl.pyx":382
+    /* "gsd/fl.pyx":336
  *                         + ', application: ' + application
  *                         + ', schema: ' + schema
  *                         + ', and schema_version: ' + str(schema_version))             # <<<<<<<<<<<<<<
  *             name_e = name.encode('utf-8')
  *             c_name = name_e
  */
-    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_and_schema_version); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_and_schema_version); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_schema_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_schema_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = PyNumber_Add(__pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_Add(__pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_1)) {
@@ -5566,236 +5153,236 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_7);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":383
+    /* "gsd/fl.pyx":337
  *                         + ', schema: ' + schema
  *                         + ', and schema_version: ' + str(schema_version))
  *             name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *             c_name = name_e
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 383, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_name_e = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":384
+    /* "gsd/fl.pyx":338
  *                         + ', and schema_version: ' + str(schema_version))
  *             name_e = name.encode('utf-8')
  *             c_name = name_e             # <<<<<<<<<<<<<<
  * 
  *             application_e = application.encode('utf-8')
  */
-    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 384, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 338, __pyx_L1_error)
     __pyx_v_c_name = __pyx_t_8;
 
-    /* "gsd/fl.pyx":386
+    /* "gsd/fl.pyx":340
  *             c_name = name_e
  * 
  *             application_e = application.encode('utf-8')             # <<<<<<<<<<<<<<
  *             c_application = application_e
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_application, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_application, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 340, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 340, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_application_e = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":387
+    /* "gsd/fl.pyx":341
  * 
  *             application_e = application.encode('utf-8')
  *             c_application = application_e             # <<<<<<<<<<<<<<
  * 
  *             schema_e = schema.encode('utf-8')
  */
-    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_application_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_application_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
     __pyx_v_c_application = __pyx_t_8;
 
-    /* "gsd/fl.pyx":389
+    /* "gsd/fl.pyx":343
  *             c_application = application_e
  * 
  *             schema_e = schema.encode('utf-8')             # <<<<<<<<<<<<<<
  *             c_schema = schema_e
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_schema, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 389, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_schema, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 343, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 343, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_schema_e = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":390
+    /* "gsd/fl.pyx":344
  * 
  *             schema_e = schema.encode('utf-8')
  *             c_schema = schema_e             # <<<<<<<<<<<<<<
  * 
  *             _c_schema_version = libgsd.gsd_make_version(schema_version[0],
  */
-    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_schema_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_schema_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 344, __pyx_L1_error)
     __pyx_v_c_schema = __pyx_t_8;
 
-    /* "gsd/fl.pyx":392
+    /* "gsd/fl.pyx":346
  *             c_schema = schema_e
  * 
  *             _c_schema_version = libgsd.gsd_make_version(schema_version[0],             # <<<<<<<<<<<<<<
  *                                                         schema_version[1])
  * 
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_schema_version, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_schema_version, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_9 = __Pyx_PyInt_As_unsigned_int(__pyx_t_3); if (unlikely((__pyx_t_9 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_unsigned_int(__pyx_t_3); if (unlikely((__pyx_t_9 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":393
+    /* "gsd/fl.pyx":347
  * 
  *             _c_schema_version = libgsd.gsd_make_version(schema_version[0],
  *                                                         schema_version[1])             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_schema_version, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_schema_version, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyInt_As_unsigned_int(__pyx_t_3); if (unlikely((__pyx_t_10 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_unsigned_int(__pyx_t_3); if (unlikely((__pyx_t_10 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":392
+    /* "gsd/fl.pyx":346
  *             c_schema = schema_e
  * 
  *             _c_schema_version = libgsd.gsd_make_version(schema_version[0],             # <<<<<<<<<<<<<<
  *                                                         schema_version[1])
  * 
  */
     __pyx_v__c_schema_version = gsd_make_version(__pyx_t_9, __pyx_t_10);
 
-    /* "gsd/fl.pyx":395
+    /* "gsd/fl.pyx":349
  *                                                         schema_version[1])
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_create_and_open(&self.__handle,
  *                                                     c_name,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":396
+          /* "gsd/fl.pyx":350
  * 
  *             with nogil:
  *                 retval = libgsd.gsd_create_and_open(&self.__handle,             # <<<<<<<<<<<<<<
  *                                                     c_name,
  *                                                     c_application,
  */
           __pyx_v_retval = gsd_create_and_open((&__pyx_v_self->__pyx___handle), __pyx_v_c_name, __pyx_v_c_application, __pyx_v_c_schema, __pyx_v__c_schema_version, __pyx_v_c_flags, __pyx_v_exclusive_create);
         }
 
-        /* "gsd/fl.pyx":395
+        /* "gsd/fl.pyx":349
  *                                                         schema_version[1])
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_create_and_open(&self.__handle,
  *                                                     c_name,
  */
         /*finally:*/ {
           /*normal exit:*/{
             #ifdef WITH_THREAD
             __Pyx_FastGIL_Forget();
             Py_BLOCK_THREADS
             #endif
-            goto __pyx_L12;
+            goto __pyx_L11;
           }
-          __pyx_L12:;
+          __pyx_L11:;
         }
     }
 
-    /* "gsd/fl.pyx":370
+    /* "gsd/fl.pyx":324
  *         cdef str schema_truncated
  * 
  *         if overwrite:             # <<<<<<<<<<<<<<
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")
  */
-    goto __pyx_L6;
+    goto __pyx_L5;
   }
 
-  /* "gsd/fl.pyx":405
+  /* "gsd/fl.pyx":359
  *         else:
  *             # open an existing file
  *             logger.info('opening file: ' + name + ' with mode: ' + mode)             # <<<<<<<<<<<<<<
  *             name_e = name.encode('utf-8')
  *             c_name = name_e
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_info); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_info); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_opening_file, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_opening_file, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_with_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_with_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Add(__pyx_t_1, __pyx_v_mode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Add(__pyx_t_1, __pyx_v_mode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -5803,262 +5390,262 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":406
+    /* "gsd/fl.pyx":360
  *             # open an existing file
  *             logger.info('opening file: ' + name + ' with mode: ' + mode)
  *             name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *             c_name = name_e
  * 
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_4, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_name_e = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":407
+    /* "gsd/fl.pyx":361
  *             logger.info('opening file: ' + name + ' with mode: ' + mode)
  *             name_e = name.encode('utf-8')
  *             c_name = name_e             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L1_error)
     __pyx_v_c_name = __pyx_t_8;
 
-    /* "gsd/fl.pyx":409
+    /* "gsd/fl.pyx":363
  *             c_name = name_e
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_open(&self.__handle, c_name, c_flags)
  * 
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":410
+          /* "gsd/fl.pyx":364
  * 
  *             with nogil:
  *                 retval = libgsd.gsd_open(&self.__handle, c_name, c_flags)             # <<<<<<<<<<<<<<
  * 
  *         __raise_on_error(retval, name)
  */
           __pyx_v_retval = gsd_open((&__pyx_v_self->__pyx___handle), __pyx_v_c_name, __pyx_v_c_flags);
         }
 
-        /* "gsd/fl.pyx":409
+        /* "gsd/fl.pyx":363
  *             c_name = name_e
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_open(&self.__handle, c_name, c_flags)
  * 
  */
         /*finally:*/ {
           /*normal exit:*/{
             #ifdef WITH_THREAD
             __Pyx_FastGIL_Forget();
             Py_BLOCK_THREADS
             #endif
-            goto __pyx_L15;
+            goto __pyx_L14;
           }
-          __pyx_L15:;
+          __pyx_L14:;
         }
     }
   }
-  __pyx_L6:;
+  __pyx_L5:;
 
-  /* "gsd/fl.pyx":412
+  /* "gsd/fl.pyx":366
  *                 retval = libgsd.gsd_open(&self.__handle, c_name, c_flags)
  * 
  *         __raise_on_error(retval, name)             # <<<<<<<<<<<<<<
  * 
  *         # validate schema
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_3, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_7 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_3, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "gsd/fl.pyx":415
+  /* "gsd/fl.pyx":369
  * 
  *         # validate schema
  *         if schema is not None:             # <<<<<<<<<<<<<<
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:
  */
   __pyx_t_2 = (__pyx_v_schema != Py_None);
   __pyx_t_5 = (__pyx_t_2 != 0);
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":416
+    /* "gsd/fl.pyx":370
  *         # validate schema
  *         if schema is not None:
  *             schema_truncated = schema             # <<<<<<<<<<<<<<
  *             if len(schema_truncated) > 64:
  *                 schema_truncated = schema_truncated[0:63]
  */
-    if (!(likely(PyUnicode_CheckExact(__pyx_v_schema))||((__pyx_v_schema) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_schema)->tp_name), 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_v_schema))||((__pyx_v_schema) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_schema)->tp_name), 0))) __PYX_ERR(0, 370, __pyx_L1_error)
     __pyx_t_7 = __pyx_v_schema;
     __Pyx_INCREF(__pyx_t_7);
     __pyx_v_schema_truncated = ((PyObject*)__pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":417
+    /* "gsd/fl.pyx":371
  *         if schema is not None:
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:             # <<<<<<<<<<<<<<
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:
  */
     if (unlikely(__pyx_v_schema_truncated == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 417, __pyx_L1_error)
+      __PYX_ERR(0, 371, __pyx_L1_error)
     }
-    __pyx_t_11 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_schema_truncated); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_schema_truncated); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 371, __pyx_L1_error)
     __pyx_t_5 = ((__pyx_t_11 > 64) != 0);
     if (__pyx_t_5) {
 
-      /* "gsd/fl.pyx":418
+      /* "gsd/fl.pyx":372
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:
  *                 schema_truncated = schema_truncated[0:63]             # <<<<<<<<<<<<<<
  *             if self.schema != schema_truncated:
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '
  */
       if (unlikely(__pyx_v_schema_truncated == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 418, __pyx_L1_error)
+        __PYX_ERR(0, 372, __pyx_L1_error)
       }
-      __pyx_t_7 = __Pyx_PyUnicode_Substring(__pyx_v_schema_truncated, 0, 63); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyUnicode_Substring(__pyx_v_schema_truncated, 0, 63); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 372, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF_SET(__pyx_v_schema_truncated, ((PyObject*)__pyx_t_7));
       __pyx_t_7 = 0;
 
-      /* "gsd/fl.pyx":417
+      /* "gsd/fl.pyx":371
  *         if schema is not None:
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:             # <<<<<<<<<<<<<<
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:
  */
     }
 
-    /* "gsd/fl.pyx":419
+    /* "gsd/fl.pyx":373
  *             if len(schema_truncated) > 64:
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '
  *                                    + self.schema)
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_7, __pyx_v_schema_truncated, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_7, __pyx_v_schema_truncated, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (unlikely(__pyx_t_5)) {
 
-      /* "gsd/fl.pyx":420
+      /* "gsd/fl.pyx":374
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '             # <<<<<<<<<<<<<<
  *                                    + self.schema)
  * 
  */
-      __pyx_t_7 = PyNumber_Add(__pyx_kp_u_file, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_7 = PyNumber_Add(__pyx_kp_u_file, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 374, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_7, __pyx_kp_u_has_incorrect_schema); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_7, __pyx_kp_u_has_incorrect_schema); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "gsd/fl.pyx":421
+      /* "gsd/fl.pyx":375
  *             if self.schema != schema_truncated:
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '
  *                                    + self.schema)             # <<<<<<<<<<<<<<
  * 
  *         self.__is_open = True
  */
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 375, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "gsd/fl.pyx":420
+      /* "gsd/fl.pyx":374
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '             # <<<<<<<<<<<<<<
  *                                    + self.schema)
  * 
  */
-      __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 374, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_7, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __PYX_ERR(0, 420, __pyx_L1_error)
+      __PYX_ERR(0, 374, __pyx_L1_error)
 
-      /* "gsd/fl.pyx":419
+      /* "gsd/fl.pyx":373
  *             if len(schema_truncated) > 64:
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '
  *                                    + self.schema)
  */
     }
 
-    /* "gsd/fl.pyx":415
+    /* "gsd/fl.pyx":369
  * 
  *         # validate schema
  *         if schema is not None:             # <<<<<<<<<<<<<<
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:
  */
   }
 
-  /* "gsd/fl.pyx":423
+  /* "gsd/fl.pyx":377
  *                                    + self.schema)
  * 
  *         self.__is_open = True             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
   __pyx_v_self->__pyx___is_open = 1;
 
-  /* "gsd/fl.pyx":303
+  /* "gsd/fl.pyx":286
  *     cdef str name
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  name,
  *                  mode,
  */
 
@@ -6074,20 +5661,19 @@
   __Pyx_AddTraceback("gsd.fl.GSDFile.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_schema_truncated);
   __Pyx_XDECREF(__pyx_v_name_e);
   __Pyx_XDECREF(__pyx_v_application_e);
   __Pyx_XDECREF(__pyx_v_schema_e);
-  __Pyx_XDECREF(__pyx_v_mode);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":425
+/* "gsd/fl.pyx":379
  *         self.__is_open = True
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """close()
  * 
  */
 
@@ -6115,82 +5701,82 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "gsd/fl.pyx":452
+  /* "gsd/fl.pyx":406
  * 
  *         """
  *         if self.__is_open:             # <<<<<<<<<<<<<<
  *             logger.info('closing file: ' + self.name)
  *             with nogil:
  */
   __pyx_t_1 = (__pyx_v_self->__pyx___is_open != 0);
   if (__pyx_t_1) {
 
-    /* "gsd/fl.pyx":453
+    /* "gsd/fl.pyx":407
  *         """
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)             # <<<<<<<<<<<<<<
  *             with nogil:
  *                 retval = libgsd.gsd_close(&self.__handle)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 453, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_closing_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_closing_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":454
+    /* "gsd/fl.pyx":408
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":455
+          /* "gsd/fl.pyx":409
  *             logger.info('closing file: ' + self.name)
  *             with nogil:
  *                 retval = libgsd.gsd_close(&self.__handle)             # <<<<<<<<<<<<<<
  *             self.__is_open = False
  * 
  */
           __pyx_v_retval = gsd_close((&__pyx_v_self->__pyx___handle));
         }
 
-        /* "gsd/fl.pyx":454
+        /* "gsd/fl.pyx":408
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False
  */
         /*finally:*/ {
@@ -6201,50 +5787,50 @@
             #endif
             goto __pyx_L6;
           }
           __pyx_L6:;
         }
     }
 
-    /* "gsd/fl.pyx":456
+    /* "gsd/fl.pyx":410
  *             with nogil:
  *                 retval = libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False             # <<<<<<<<<<<<<<
  * 
  *             __raise_on_error(retval, self.name)
  */
     __pyx_v_self->__pyx___is_open = 0;
 
-    /* "gsd/fl.pyx":458
+    /* "gsd/fl.pyx":412
  *             self.__is_open = False
  * 
  *             __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def truncate(self):
  */
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __pyx_v_self->name;
     __Pyx_INCREF(__pyx_t_4);
-    __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":452
+    /* "gsd/fl.pyx":406
  * 
  *         """
  *         if self.__is_open:             # <<<<<<<<<<<<<<
  *             logger.info('closing file: ' + self.name)
  *             with nogil:
  */
   }
 
-  /* "gsd/fl.pyx":425
+  /* "gsd/fl.pyx":379
  *         self.__is_open = True
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """close()
  * 
  */
 
@@ -6260,15 +5846,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":460
+/* "gsd/fl.pyx":414
  *             __raise_on_error(retval, self.name)
  * 
  *     def truncate(self):             # <<<<<<<<<<<<<<
  *         """truncate()
  * 
  */
 
@@ -6296,104 +5882,104 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("truncate", 0);
 
-  /* "gsd/fl.pyx":490
+  /* "gsd/fl.pyx":444
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":491
+    /* "gsd/fl.pyx":445
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         logger.info('truncating file: ' + self.name)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 445, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 491, __pyx_L1_error)
+    __PYX_ERR(0, 445, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":490
+    /* "gsd/fl.pyx":444
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":493
+  /* "gsd/fl.pyx":447
  *             raise ValueError("File is not open")
  * 
  *         logger.info('truncating file: ' + self.name)             # <<<<<<<<<<<<<<
  *         with nogil:
  *             retval = libgsd.gsd_truncate(&self.__handle)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_truncating_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_truncating_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":494
+  /* "gsd/fl.pyx":448
  * 
  *         logger.info('truncating file: ' + self.name)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_truncate(&self.__handle)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":495
+        /* "gsd/fl.pyx":449
  *         logger.info('truncating file: ' + self.name)
  *         with nogil:
  *             retval = libgsd.gsd_truncate(&self.__handle)             # <<<<<<<<<<<<<<
  * 
  *         __raise_on_error(retval, self.name)
  */
         __pyx_v_retval = gsd_truncate((&__pyx_v_self->__pyx___handle));
       }
 
-      /* "gsd/fl.pyx":494
+      /* "gsd/fl.pyx":448
  * 
  *         logger.info('truncating file: ' + self.name)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_truncate(&self.__handle)
  * 
  */
       /*finally:*/ {
@@ -6404,32 +5990,32 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":497
+  /* "gsd/fl.pyx":451
  *             retval = libgsd.gsd_truncate(&self.__handle)
  * 
  *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def end_frame(self):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 497, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_4);
-  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":460
+  /* "gsd/fl.pyx":414
  *             __raise_on_error(retval, self.name)
  * 
  *     def truncate(self):             # <<<<<<<<<<<<<<
  *         """truncate()
  * 
  */
 
@@ -6445,15 +6031,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":499
+/* "gsd/fl.pyx":453
  *         __raise_on_error(retval, self.name)
  * 
  *     def end_frame(self):             # <<<<<<<<<<<<<<
  *         """end_frame()
  * 
  */
 
@@ -6481,104 +6067,104 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("end_frame", 0);
 
-  /* "gsd/fl.pyx":535
+  /* "gsd/fl.pyx":489
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":536
+    /* "gsd/fl.pyx":490
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         logger.debug('end frame: ' + self.name)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 536, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 490, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 536, __pyx_L1_error)
+    __PYX_ERR(0, 490, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":535
+    /* "gsd/fl.pyx":489
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":538
+  /* "gsd/fl.pyx":492
  *             raise ValueError("File is not open")
  * 
  *         logger.debug('end frame: ' + self.name)             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 538, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 538, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_end_frame, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 538, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_end_frame, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":540
+  /* "gsd/fl.pyx":494
  *         logger.debug('end frame: ' + self.name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_end_frame(&self.__handle)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":541
+        /* "gsd/fl.pyx":495
  * 
  *         with nogil:
  *             retval = libgsd.gsd_end_frame(&self.__handle)             # <<<<<<<<<<<<<<
  * 
  *         __raise_on_error(retval, self.name)
  */
         __pyx_v_retval = gsd_end_frame((&__pyx_v_self->__pyx___handle));
       }
 
-      /* "gsd/fl.pyx":540
+      /* "gsd/fl.pyx":494
  *         logger.debug('end frame: ' + self.name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_end_frame(&self.__handle)
  * 
  */
       /*finally:*/ {
@@ -6589,32 +6175,32 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":543
+  /* "gsd/fl.pyx":497
  *             retval = libgsd.gsd_end_frame(&self.__handle)
  * 
  *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
- *     def write_chunk(self, name, data):
+ *     def flush(self):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_4);
-  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":499
+  /* "gsd/fl.pyx":453
  *         __raise_on_error(retval, self.name)
  * 
  *     def end_frame(self):             # <<<<<<<<<<<<<<
  *         """end_frame()
  * 
  */
 
@@ -6630,26 +6216,211 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":545
+/* "gsd/fl.pyx":499
+ *         __raise_on_error(retval, self.name)
+ * 
+ *     def flush(self):             # <<<<<<<<<<<<<<
+ *         """flush()
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_9flush(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_3gsd_2fl_7GSDFile_8flush[] = "flush()\n\n        Flush all buffered frames to the file.\n        ";
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_9flush(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("flush (wrapper)", 0);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_8flush(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_8flush(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
+  int __pyx_v_retval;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("flush", 0);
+
+  /* "gsd/fl.pyx":505
+ *         """
+ * 
+ *         if not self.__is_open:             # <<<<<<<<<<<<<<
+ *             raise ValueError("File is not open")
+ * 
+ */
+  __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
+  if (unlikely(__pyx_t_1)) {
+
+    /* "gsd/fl.pyx":506
+ * 
+ *         if not self.__is_open:
+ *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
+ * 
+ *         logger.debug('flush: ' + self.name)
+ */
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 506, __pyx_L1_error)
+
+    /* "gsd/fl.pyx":505
+ *         """
+ * 
+ *         if not self.__is_open:             # <<<<<<<<<<<<<<
+ *             raise ValueError("File is not open")
+ * 
+ */
+  }
+
+  /* "gsd/fl.pyx":508
+ *             raise ValueError("File is not open")
+ * 
+ *         logger.debug('flush: ' + self.name)             # <<<<<<<<<<<<<<
+ * 
+ *         with nogil:
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_flush, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "gsd/fl.pyx":510
+ *         logger.debug('flush: ' + self.name)
+ * 
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             retval = libgsd.gsd_flush(&self.__handle)
+ * 
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "gsd/fl.pyx":511
+ * 
+ *         with nogil:
+ *             retval = libgsd.gsd_flush(&self.__handle)             # <<<<<<<<<<<<<<
+ * 
+ *         __raise_on_error(retval, self.name)
+ */
+        __pyx_v_retval = gsd_flush((&__pyx_v_self->__pyx___handle));
+      }
+
+      /* "gsd/fl.pyx":510
+ *         logger.debug('flush: ' + self.name)
+ * 
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             retval = libgsd.gsd_flush(&self.__handle)
+ * 
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L6;
+        }
+        __pyx_L6:;
+      }
+  }
+
+  /* "gsd/fl.pyx":513
+ *             retval = libgsd.gsd_flush(&self.__handle)
+ * 
+ *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
+ * 
+ *     def write_chunk(self, name, data):
+ */
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __pyx_v_self->name;
+  __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "gsd/fl.pyx":499
+ *         __raise_on_error(retval, self.name)
+ * 
+ *     def flush(self):             # <<<<<<<<<<<<<<
+ *         """flush()
+ * 
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("gsd.fl.GSDFile.flush", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "gsd/fl.pyx":515
  *         __raise_on_error(retval, self.name)
  * 
  *     def write_chunk(self, name, data):             # <<<<<<<<<<<<<<
  *         """write_chunk(name, data)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_9write_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_8write_chunk[] = "write_chunk(name, data)\n\n        Write a data chunk to the file. After writing all chunks in the\n        current frame, call :py:meth:`end_frame()`.\n\n        Args:\n            name (str): Name of the chunk\n            data: Data to write into the chunk. Must be a numpy\n                  array, or array-like, with 2 or fewer\n                  dimensions.\n\n        Warning:\n            :py:meth:`write_chunk()` will implicitly converts array-like and\n            non-contiguous numpy arrays to contiguous numpy arrays with\n            ``numpy.ascontiguousarray(data)``. This may or may not produce\n            desired data types in the output file and incurs overhead.\n\n        Example:\n            .. ipython:: python\n\n                f = gsd.fl.open(name='file.gsd', mode='w',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.write_chunk(name='float1d',\n                              data=numpy.array([1,2,3,4],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='float2d',\n                              data=numpy.array([[13,14],[15,16],[17,19]],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='double2d',\n                              data=numpy.array([[1,4],[5,6],[7,9]],\n                                               dtype=numpy.float64))\n                f.write_chunk(name='int1d',\n                              data=numpy.array([70,80,90],\n                                               dtype=numpy.int64))\n                f.end_frame()\n                f.nframes\n                f.close()\n        ";
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_9write_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_11write_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_3gsd_2fl_7GSDFile_10write_chunk[] = "write_chunk(name, data)\n\n        Write a data chunk to the file. After writing all chunks in the\n        current frame, call :py:meth:`end_frame()`.\n\n        Args:\n            name (str): Name of the chunk\n            data: Data to write into the chunk. Must be a numpy\n                  array, or array-like, with 2 or fewer\n                  dimensions.\n\n        Warning:\n            :py:meth:`write_chunk()` will implicitly converts array-like and\n            non-contiguous numpy arrays to contiguous numpy arrays with\n            ``numpy.ascontiguousarray(data)``. This may or may not produce\n            desired data types in the output file and incurs overhead.\n\n        Example:\n            .. ipython:: python\n\n                f = gsd.fl.open(name='file.gsd', mode='w',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.write_chunk(name='float1d',\n                              data=numpy.array([1,2,3,4],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='float2d',\n                              data=numpy.array([[13,14],[15,16],[17,19]],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='double2d',\n                              data=numpy.array([[1,4],[5,6],[7,9]],\n                                               dtype=numpy.float64))\n                f.write_chunk(name='int1d',\n                              data=numpy.array([70,80,90],\n                                               dtype=numpy.int64))\n                f.end_frame()\n                f.nframes\n                f.close()\n        ";
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_11write_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
   PyObject *__pyx_v_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6673,45 +6444,45 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("write_chunk", 1, 2, 2, 1); __PYX_ERR(0, 545, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("write_chunk", 1, 2, 2, 1); __PYX_ERR(0, 515, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write_chunk") < 0)) __PYX_ERR(0, 545, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write_chunk") < 0)) __PYX_ERR(0, 515, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("write_chunk", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 545, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("write_chunk", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 515, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.write_chunk", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_8write_chunk(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_name, __pyx_v_data);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_10write_chunk(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_name, __pyx_v_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_8write_chunk(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_10write_chunk(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_data) {
   PyObject *__pyx_v_data_array = NULL;
   uint64_t __pyx_v_N;
   uint32_t __pyx_v_M;
   enum gsd_type __pyx_v_gsd_type;
   void *__pyx_v_data_ptr;
   char *__pyx_v_c_name;
   PyObject *__pyx_v_name_e = NULL;
@@ -6729,231 +6500,231 @@
   uint32_t __pyx_t_9;
   char *__pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("write_chunk", 0);
 
-  /* "gsd/fl.pyx":587
+  /* "gsd/fl.pyx":557
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":588
+    /* "gsd/fl.pyx":558
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         data_array = numpy.ascontiguousarray(data)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 558, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 588, __pyx_L1_error)
+    __PYX_ERR(0, 558, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":587
+    /* "gsd/fl.pyx":557
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":590
+  /* "gsd/fl.pyx":560
  *             raise ValueError("File is not open")
  * 
  *         data_array = numpy.ascontiguousarray(data)             # <<<<<<<<<<<<<<
  *         if data_array is not data:
  *             logger.warning('implicit data copy when writing chunk: ' + name)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 590, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 590, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 590, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_data_array = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":591
+  /* "gsd/fl.pyx":561
  * 
  *         data_array = numpy.ascontiguousarray(data)
  *         if data_array is not data:             # <<<<<<<<<<<<<<
  *             logger.warning('implicit data copy when writing chunk: ' + name)
  *         data_array = data_array.view()
  */
   __pyx_t_1 = (__pyx_v_data_array != __pyx_v_data);
   __pyx_t_5 = (__pyx_t_1 != 0);
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":592
+    /* "gsd/fl.pyx":562
  *         data_array = numpy.ascontiguousarray(data)
  *         if data_array is not data:
  *             logger.warning('implicit data copy when writing chunk: ' + name)             # <<<<<<<<<<<<<<
  *         data_array = data_array.view()
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 562, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 562, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_implicit_data_copy_when_writing, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_implicit_data_copy_when_writing, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 562, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":591
+    /* "gsd/fl.pyx":561
  * 
  *         data_array = numpy.ascontiguousarray(data)
  *         if data_array is not data:             # <<<<<<<<<<<<<<
  *             logger.warning('implicit data copy when writing chunk: ' + name)
  *         data_array = data_array.view()
  */
   }
 
-  /* "gsd/fl.pyx":593
+  /* "gsd/fl.pyx":563
  *         if data_array is not data:
  *             logger.warning('implicit data copy when writing chunk: ' + name)
  *         data_array = data_array.view()             # <<<<<<<<<<<<<<
  * 
  *         cdef uint64_t N
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_view); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_view); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 593, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_data_array, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":598
+  /* "gsd/fl.pyx":568
  *         cdef uint32_t M
  * 
  *         if len(data_array.shape) > 2:             # <<<<<<<<<<<<<<
  *             raise ValueError("GSD can only write 1 or 2 dimensional arrays: "
  *                              + name)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_5 = ((__pyx_t_7 > 2) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "gsd/fl.pyx":600
+    /* "gsd/fl.pyx":570
  *         if len(data_array.shape) > 2:
  *             raise ValueError("GSD can only write 1 or 2 dimensional arrays: "
  *                              + name)             # <<<<<<<<<<<<<<
  * 
  *         if len(data_array.shape) == 1:
  */
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_GSD_can_only_write_1_or_2_dimens, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_GSD_can_only_write_1_or_2_dimens, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 570, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "gsd/fl.pyx":599
+    /* "gsd/fl.pyx":569
  * 
  *         if len(data_array.shape) > 2:
  *             raise ValueError("GSD can only write 1 or 2 dimensional arrays: "             # <<<<<<<<<<<<<<
  *                              + name)
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 599, __pyx_L1_error)
+    __PYX_ERR(0, 569, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":598
+    /* "gsd/fl.pyx":568
  *         cdef uint32_t M
  * 
  *         if len(data_array.shape) > 2:             # <<<<<<<<<<<<<<
  *             raise ValueError("GSD can only write 1 or 2 dimensional arrays: "
  *                              + name)
  */
   }
 
-  /* "gsd/fl.pyx":602
+  /* "gsd/fl.pyx":572
  *                              + name)
  * 
  *         if len(data_array.shape) == 1:             # <<<<<<<<<<<<<<
  *             data_array = data_array.reshape([data_array.shape[0], 1])
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 602, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 602, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = ((__pyx_t_7 == 1) != 0);
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":603
+    /* "gsd/fl.pyx":573
  * 
  *         if len(data_array.shape) == 1:
  *             data_array = data_array.reshape([data_array.shape[0], 1])             # <<<<<<<<<<<<<<
  * 
  *         N = data_array.shape[0]
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_reshape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_reshape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 603, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 603, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 603, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_6);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyList_SET_ITEM(__pyx_t_4, 1, __pyx_int_1);
     __pyx_t_6 = 0;
@@ -6966,588 +6737,588 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_data_array, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":602
+    /* "gsd/fl.pyx":572
  *                              + name)
  * 
  *         if len(data_array.shape) == 1:             # <<<<<<<<<<<<<<
  *             data_array = data_array.reshape([data_array.shape[0], 1])
  * 
  */
   }
 
-  /* "gsd/fl.pyx":605
+  /* "gsd/fl.pyx":575
  *             data_array = data_array.reshape([data_array.shape[0], 1])
  * 
  *         N = data_array.shape[0]             # <<<<<<<<<<<<<<
  *         M = data_array.shape[1]
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 605, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_t_2); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 605, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_t_2); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 575, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_N = __pyx_t_8;
 
-  /* "gsd/fl.pyx":606
+  /* "gsd/fl.pyx":576
  * 
  *         N = data_array.shape[0]
  *         M = data_array.shape[1]             # <<<<<<<<<<<<<<
  * 
  *         cdef libgsd.gsd_type gsd_type
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_M = __pyx_t_9;
 
-  /* "gsd/fl.pyx":610
+  /* "gsd/fl.pyx":580
  *         cdef libgsd.gsd_type gsd_type
  *         cdef void *data_ptr
  *         if data_array.dtype == numpy.uint8:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":611
+    /* "gsd/fl.pyx":581
  *         cdef void *data_ptr
  *         if data_array.dtype == numpy.uint8:
  *             gsd_type = libgsd.GSD_TYPE_UINT8             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_uint8(data_array)
  *         elif data_array.dtype == numpy.uint16:
  */
     __pyx_v_gsd_type = GSD_TYPE_UINT8;
 
-    /* "gsd/fl.pyx":612
+    /* "gsd/fl.pyx":582
  *         if data_array.dtype == numpy.uint8:
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.uint16:
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint8(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":610
+    /* "gsd/fl.pyx":580
  *         cdef libgsd.gsd_type gsd_type
  *         cdef void *data_ptr
  *         if data_array.dtype == numpy.uint8:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":613
+  /* "gsd/fl.pyx":583
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)
  *         elif data_array.dtype == numpy.uint16:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":614
+    /* "gsd/fl.pyx":584
  *             data_ptr = __get_ptr_uint8(data_array)
  *         elif data_array.dtype == numpy.uint16:
  *             gsd_type = libgsd.GSD_TYPE_UINT16             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_uint16(data_array)
  *         elif data_array.dtype == numpy.uint32:
  */
     __pyx_v_gsd_type = GSD_TYPE_UINT16;
 
-    /* "gsd/fl.pyx":615
+    /* "gsd/fl.pyx":585
  *         elif data_array.dtype == numpy.uint16:
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.uint32:
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint16(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":613
+    /* "gsd/fl.pyx":583
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)
  *         elif data_array.dtype == numpy.uint16:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":616
+  /* "gsd/fl.pyx":586
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)
  *         elif data_array.dtype == numpy.uint32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":617
+    /* "gsd/fl.pyx":587
  *             data_ptr = __get_ptr_uint16(data_array)
  *         elif data_array.dtype == numpy.uint32:
  *             gsd_type = libgsd.GSD_TYPE_UINT32             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_uint32(data_array)
  *         elif data_array.dtype == numpy.uint64:
  */
     __pyx_v_gsd_type = GSD_TYPE_UINT32;
 
-    /* "gsd/fl.pyx":618
+    /* "gsd/fl.pyx":588
  *         elif data_array.dtype == numpy.uint32:
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.uint64:
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint32(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":616
+    /* "gsd/fl.pyx":586
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)
  *         elif data_array.dtype == numpy.uint32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":619
+  /* "gsd/fl.pyx":589
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)
  *         elif data_array.dtype == numpy.uint64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":620
+    /* "gsd/fl.pyx":590
  *             data_ptr = __get_ptr_uint32(data_array)
  *         elif data_array.dtype == numpy.uint64:
  *             gsd_type = libgsd.GSD_TYPE_UINT64             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_uint64(data_array)
  *         elif data_array.dtype == numpy.int8:
  */
     __pyx_v_gsd_type = GSD_TYPE_UINT64;
 
-    /* "gsd/fl.pyx":621
+    /* "gsd/fl.pyx":591
  *         elif data_array.dtype == numpy.uint64:
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.int8:
  *             gsd_type = libgsd.GSD_TYPE_INT8
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint64(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":619
+    /* "gsd/fl.pyx":589
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)
  *         elif data_array.dtype == numpy.uint64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":622
+  /* "gsd/fl.pyx":592
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)
  *         elif data_array.dtype == numpy.int8:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 622, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 622, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 622, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 622, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 622, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":623
+    /* "gsd/fl.pyx":593
  *             data_ptr = __get_ptr_uint64(data_array)
  *         elif data_array.dtype == numpy.int8:
  *             gsd_type = libgsd.GSD_TYPE_INT8             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_int8(data_array)
  *         elif data_array.dtype == numpy.int16:
  */
     __pyx_v_gsd_type = GSD_TYPE_INT8;
 
-    /* "gsd/fl.pyx":624
+    /* "gsd/fl.pyx":594
  *         elif data_array.dtype == numpy.int8:
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.int16:
  *             gsd_type = libgsd.GSD_TYPE_INT16
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int8(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":622
+    /* "gsd/fl.pyx":592
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)
  *         elif data_array.dtype == numpy.int8:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":625
+  /* "gsd/fl.pyx":595
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)
  *         elif data_array.dtype == numpy.int16:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 595, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 595, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 595, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 595, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 595, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":626
+    /* "gsd/fl.pyx":596
  *             data_ptr = __get_ptr_int8(data_array)
  *         elif data_array.dtype == numpy.int16:
  *             gsd_type = libgsd.GSD_TYPE_INT16             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_int16(data_array)
  *         elif data_array.dtype == numpy.int32:
  */
     __pyx_v_gsd_type = GSD_TYPE_INT16;
 
-    /* "gsd/fl.pyx":627
+    /* "gsd/fl.pyx":597
  *         elif data_array.dtype == numpy.int16:
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.int32:
  *             gsd_type = libgsd.GSD_TYPE_INT32
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int16(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":625
+    /* "gsd/fl.pyx":595
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)
  *         elif data_array.dtype == numpy.int16:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":628
+  /* "gsd/fl.pyx":598
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)
  *         elif data_array.dtype == numpy.int32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":629
+    /* "gsd/fl.pyx":599
  *             data_ptr = __get_ptr_int16(data_array)
  *         elif data_array.dtype == numpy.int32:
  *             gsd_type = libgsd.GSD_TYPE_INT32             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_int32(data_array)
  *         elif data_array.dtype == numpy.int64:
  */
     __pyx_v_gsd_type = GSD_TYPE_INT32;
 
-    /* "gsd/fl.pyx":630
+    /* "gsd/fl.pyx":600
  *         elif data_array.dtype == numpy.int32:
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.int64:
  *             gsd_type = libgsd.GSD_TYPE_INT64
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int32(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":628
+    /* "gsd/fl.pyx":598
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)
  *         elif data_array.dtype == numpy.int32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":631
+  /* "gsd/fl.pyx":601
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)
  *         elif data_array.dtype == numpy.int64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 631, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 631, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 631, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 631, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 631, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":632
+    /* "gsd/fl.pyx":602
  *             data_ptr = __get_ptr_int32(data_array)
  *         elif data_array.dtype == numpy.int64:
  *             gsd_type = libgsd.GSD_TYPE_INT64             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_int64(data_array)
  *         elif data_array.dtype == numpy.float32:
  */
     __pyx_v_gsd_type = GSD_TYPE_INT64;
 
-    /* "gsd/fl.pyx":633
+    /* "gsd/fl.pyx":603
  *         elif data_array.dtype == numpy.int64:
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.float32:
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int64(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":631
+    /* "gsd/fl.pyx":601
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)
  *         elif data_array.dtype == numpy.int64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":634
+  /* "gsd/fl.pyx":604
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)
  *         elif data_array.dtype == numpy.float32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":635
+    /* "gsd/fl.pyx":605
  *             data_ptr = __get_ptr_int64(data_array)
  *         elif data_array.dtype == numpy.float32:
  *             gsd_type = libgsd.GSD_TYPE_FLOAT             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_float32(data_array)
  *         elif data_array.dtype == numpy.float64:
  */
     __pyx_v_gsd_type = GSD_TYPE_FLOAT;
 
-    /* "gsd/fl.pyx":636
+    /* "gsd/fl.pyx":606
  *         elif data_array.dtype == numpy.float32:
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.float64:
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_float32(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":634
+    /* "gsd/fl.pyx":604
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)
  *         elif data_array.dtype == numpy.float32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":637
+  /* "gsd/fl.pyx":607
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)
  *         elif data_array.dtype == numpy.float64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE
  *             data_ptr = __get_ptr_float64(data_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(__pyx_t_5)) {
 
-    /* "gsd/fl.pyx":638
+    /* "gsd/fl.pyx":608
  *             data_ptr = __get_ptr_float32(data_array)
  *         elif data_array.dtype == numpy.float64:
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_float64(data_array)
  *         else:
  */
     __pyx_v_gsd_type = GSD_TYPE_DOUBLE;
 
-    /* "gsd/fl.pyx":639
+    /* "gsd/fl.pyx":609
  *         elif data_array.dtype == numpy.float64:
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE
  *             data_ptr = __get_ptr_float64(data_array)             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("invalid type for chunk: " + name)
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_float64(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":637
+    /* "gsd/fl.pyx":607
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)
  *         elif data_array.dtype == numpy.float64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE
  *             data_ptr = __get_ptr_float64(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":641
+  /* "gsd/fl.pyx":611
  *             data_ptr = __get_ptr_float64(data_array)
  *         else:
  *             raise ValueError("invalid type for chunk: " + name)             # <<<<<<<<<<<<<<
  * 
  *         logger.debug('write chunk: ' + self.name + ' - ' + name)
  */
   /*else*/ {
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 641, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 641, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 641, __pyx_L1_error)
+    __PYX_ERR(0, 611, __pyx_L1_error)
   }
   __pyx_L7:;
 
-  /* "gsd/fl.pyx":643
+  /* "gsd/fl.pyx":613
  *             raise ValueError("invalid type for chunk: " + name)
  * 
  *         logger.debug('write chunk: ' + self.name + ' - ' + name)             # <<<<<<<<<<<<<<
  * 
  *         cdef char * c_name
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_write_chunk, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_write_chunk, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7555,82 +7326,82 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 643, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "gsd/fl.pyx":646
+  /* "gsd/fl.pyx":616
  * 
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *         c_name = name_e
  *         with nogil:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 646, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 646, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_name_e = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "gsd/fl.pyx":647
+  /* "gsd/fl.pyx":617
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')
  *         c_name = name_e             # <<<<<<<<<<<<<<
  *         with nogil:
  *             retval = libgsd.gsd_write_chunk(&self.__handle,
  */
-  __pyx_t_10 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 647, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 617, __pyx_L1_error)
   __pyx_v_c_name = __pyx_t_10;
 
-  /* "gsd/fl.pyx":648
+  /* "gsd/fl.pyx":618
  *         name_e = name.encode('utf-8')
  *         c_name = name_e
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_write_chunk(&self.__handle,
  *                                             c_name,
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":649
+        /* "gsd/fl.pyx":619
  *         c_name = name_e
  *         with nogil:
  *             retval = libgsd.gsd_write_chunk(&self.__handle,             # <<<<<<<<<<<<<<
  *                                             c_name,
  *                                             gsd_type,
  */
         __pyx_v_retval = gsd_write_chunk((&__pyx_v_self->__pyx___handle), __pyx_v_c_name, __pyx_v_gsd_type, __pyx_v_N, __pyx_v_M, 0, __pyx_v_data_ptr);
       }
 
-      /* "gsd/fl.pyx":648
+      /* "gsd/fl.pyx":618
  *         name_e = name.encode('utf-8')
  *         c_name = name_e
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_write_chunk(&self.__handle,
  *                                             c_name,
  */
       /*finally:*/ {
@@ -7641,32 +7412,32 @@
           #endif
           goto __pyx_L10;
         }
         __pyx_L10:;
       }
   }
 
-  /* "gsd/fl.pyx":657
+  /* "gsd/fl.pyx":627
  *                                             data_ptr)
  * 
  *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def chunk_exists(self, frame, name):
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 657, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_3);
-  __pyx_t_2 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 657, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":545
+  /* "gsd/fl.pyx":515
  *         __raise_on_error(retval, self.name)
  * 
  *     def write_chunk(self, name, data):             # <<<<<<<<<<<<<<
  *         """write_chunk(name, data)
  * 
  */
 
@@ -7684,26 +7455,26 @@
   __Pyx_XDECREF(__pyx_v_data_array);
   __Pyx_XDECREF(__pyx_v_name_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":659
+/* "gsd/fl.pyx":629
  *         __raise_on_error(retval, self.name)
  * 
  *     def chunk_exists(self, frame, name):             # <<<<<<<<<<<<<<
  *         """chunk_exists(frame, name)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_11chunk_exists(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_10chunk_exists[] = "chunk_exists(frame, name)\n\n        Test if a chunk exists.\n\n        Args:\n            frame (int): Index of the frame to check\n            name (str): Name of the chunk\n\n        Returns:\n            bool: ``True`` if the chunk exists in the file at the given frame.              ``False`` if it does not.\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([9,10,11,12],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[13,14],[15,16]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.chunk_exists(frame=0, name='chunk1')\n                f.chunk_exists(frame=0, name='chunk2')\n                f.chunk_exists(frame=0, name='chunk3')\n                f.chunk_exists(frame=10, name='chunk1')\n                f.close()\n        ";
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_11chunk_exists(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_13chunk_exists(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_3gsd_2fl_7GSDFile_12chunk_exists[] = "chunk_exists(frame, name)\n\n        Test if a chunk exists.\n\n        Args:\n            frame (int): Index of the frame to check\n            name (str): Name of the chunk\n\n        Returns:\n            bool: ``True`` if the chunk exists in the file at the given frame.              ``False`` if it does not.\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([9,10,11,12],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[13,14],[15,16]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.chunk_exists(frame=0, name='chunk1')\n                f.chunk_exists(frame=0, name='chunk2')\n                f.chunk_exists(frame=0, name='chunk3')\n                f.chunk_exists(frame=10, name='chunk1')\n                f.close()\n        ";
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_13chunk_exists(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_frame = 0;
   PyObject *__pyx_v_name = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7727,45 +7498,45 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("chunk_exists", 1, 2, 2, 1); __PYX_ERR(0, 659, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("chunk_exists", 1, 2, 2, 1); __PYX_ERR(0, 629, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "chunk_exists") < 0)) __PYX_ERR(0, 659, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "chunk_exists") < 0)) __PYX_ERR(0, 629, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_frame = values[0];
     __pyx_v_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("chunk_exists", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 659, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("chunk_exists", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 629, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.chunk_exists", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_10chunk_exists(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_frame, __pyx_v_name);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_12chunk_exists(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_frame, __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_10chunk_exists(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_12chunk_exists(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_name) {
   struct gsd_index_entry const *__pyx_v_index_entry;
   char *__pyx_v_c_name;
   PyObject *__pyx_v_name_e = NULL;
   int64_t __pyx_v_c_frame;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -7775,79 +7546,79 @@
   int64_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chunk_exists", 0);
 
-  /* "gsd/fl.pyx":706
+  /* "gsd/fl.pyx":676
  *         cdef const libgsd.gsd_index_entry* index_entry
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *         c_name = name_e
  *         cdef int64_t c_frame
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 676, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 676, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_name_e = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":707
+  /* "gsd/fl.pyx":677
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')
  *         c_name = name_e             # <<<<<<<<<<<<<<
  *         cdef int64_t c_frame
  *         c_frame = frame
  */
-  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 677, __pyx_L1_error)
   __pyx_v_c_name = __pyx_t_4;
 
-  /* "gsd/fl.pyx":709
+  /* "gsd/fl.pyx":679
  *         c_name = name_e
  *         cdef int64_t c_frame
  *         c_frame = frame             # <<<<<<<<<<<<<<
  * 
  *         logger.debug('chunk exists: ' + self.name + ' - ' + name)
  */
-  __pyx_t_5 = __Pyx_PyInt_As_int64_t(__pyx_v_frame); if (unlikely((__pyx_t_5 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int64_t(__pyx_v_frame); if (unlikely((__pyx_t_5 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 679, __pyx_L1_error)
   __pyx_v_c_frame = __pyx_t_5;
 
-  /* "gsd/fl.pyx":711
+  /* "gsd/fl.pyx":681
  *         c_frame = frame
  * 
  *         logger.debug('chunk exists: ' + self.name + ' - ' + name)             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_chunk_exists, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_chunk_exists, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7855,45 +7626,45 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":713
+  /* "gsd/fl.pyx":683
  *         logger.debug('chunk exists: ' + self.name + ' - ' + name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":714
+        /* "gsd/fl.pyx":684
  * 
  *         with nogil:
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)             # <<<<<<<<<<<<<<
  * 
  *         return index_entry != NULL
  */
         __pyx_v_index_entry = gsd_find_chunk((&__pyx_v_self->__pyx___handle), __pyx_v_c_frame, __pyx_v_c_name);
       }
 
-      /* "gsd/fl.pyx":713
+      /* "gsd/fl.pyx":683
  *         logger.debug('chunk exists: ' + self.name + ' - ' + name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  */
       /*finally:*/ {
@@ -7904,29 +7675,29 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "gsd/fl.pyx":716
+  /* "gsd/fl.pyx":686
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  *         return index_entry != NULL             # <<<<<<<<<<<<<<
  * 
  *     def read_chunk(self, frame, name):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_index_entry != NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_index_entry != NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 686, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":659
+  /* "gsd/fl.pyx":629
  *         __raise_on_error(retval, self.name)
  * 
  *     def chunk_exists(self, frame, name):             # <<<<<<<<<<<<<<
  *         """chunk_exists(frame, name)
  * 
  */
 
@@ -7941,26 +7712,26 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_name_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":718
+/* "gsd/fl.pyx":688
  *         return index_entry != NULL
  * 
  *     def read_chunk(self, frame, name):             # <<<<<<<<<<<<<<
  *         """read_chunk(frame, name)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_13read_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_12read_chunk[] = "read_chunk(frame, name)\n\n        Read a data chunk from the file and return it as a numpy array.\n\n        Args:\n            frame (int): Index of the frame to read\n            name (str): Name of the chunk\n\n        Returns:\n            ``(N,M)`` or ``(N,)`` `numpy.ndarray` of ``type``: Data read from\n            file. ``N``, ``M``, and ``type`` are determined by the chunk\n            metadata. If the data is NxM in the file and M > 1, return a 2D\n            array. If the data is Nx1, return a 1D array.\n\n        .. tip::\n            Each call invokes a disk read and allocation of a\n            new numpy array for storage. To avoid overhead, call\n            :py:meth:`read_chunk()` on the same chunk only once.\n\n        Example:\n            .. ipython:: python\n                :okexcept:\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([9,10,11,12],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[13,14],[15,16]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n         ""                       schema=\"My Schema\", schema_version=[1,0])\n                f.read_chunk(frame=0, name='chunk1')\n                f.read_chunk(frame=1, name='chunk1')\n                f.read_chunk(frame=2, name='chunk1')\n                f.close()\n        ";
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_13read_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_15read_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_3gsd_2fl_7GSDFile_14read_chunk[] = "read_chunk(frame, name)\n\n        Read a data chunk from the file and return it as a numpy array.\n\n        Args:\n            frame (int): Index of the frame to read\n            name (str): Name of the chunk\n\n        Returns:\n            ``(N,M)`` or ``(N,)`` `numpy.ndarray` of ``type``: Data read from\n            file. ``N``, ``M``, and ``type`` are determined by the chunk\n            metadata. If the data is NxM in the file and M > 1, return a 2D\n            array. If the data is Nx1, return a 1D array.\n\n        .. tip::\n            Each call invokes a disk read and allocation of a\n            new numpy array for storage. To avoid overhead, call\n            :py:meth:`read_chunk()` on the same chunk only once.\n\n        Example:\n            .. ipython:: python\n                :okexcept:\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([9,10,11,12],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[13,14],[15,16]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n         ""                       schema=\"My Schema\", schema_version=[1,0])\n                f.read_chunk(frame=0, name='chunk1')\n                f.read_chunk(frame=1, name='chunk1')\n                f.read_chunk(frame=2, name='chunk1')\n                f.close()\n        ";
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_15read_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_frame = 0;
   PyObject *__pyx_v_name = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7984,45 +7755,45 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_chunk", 1, 2, 2, 1); __PYX_ERR(0, 718, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_chunk", 1, 2, 2, 1); __PYX_ERR(0, 688, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_chunk") < 0)) __PYX_ERR(0, 718, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_chunk") < 0)) __PYX_ERR(0, 688, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_frame = values[0];
     __pyx_v_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_chunk", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 718, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_chunk", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 688, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.read_chunk", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_12read_chunk(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_frame, __pyx_v_name);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_14read_chunk(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_frame, __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_12read_chunk(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_14read_chunk(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_name) {
   struct gsd_index_entry const *__pyx_v_index_entry;
   char *__pyx_v_c_name;
   PyObject *__pyx_v_name_e = NULL;
   int64_t __pyx_v_c_frame;
   enum gsd_type __pyx_v_gsd_type;
   void *__pyx_v_data_ptr;
   PyObject *__pyx_v_data_array = NULL;
@@ -8039,119 +7810,119 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_chunk", 0);
 
-  /* "gsd/fl.pyx":769
+  /* "gsd/fl.pyx":739
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":770
+    /* "gsd/fl.pyx":740
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         cdef const libgsd.gsd_index_entry* index_entry
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 740, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 770, __pyx_L1_error)
+    __PYX_ERR(0, 740, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":769
+    /* "gsd/fl.pyx":739
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":774
+  /* "gsd/fl.pyx":744
  *         cdef const libgsd.gsd_index_entry* index_entry
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *         c_name = name_e
  *         cdef int64_t c_frame
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 774, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_name_e = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":775
+  /* "gsd/fl.pyx":745
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')
  *         c_name = name_e             # <<<<<<<<<<<<<<
  *         cdef int64_t c_frame
  *         c_frame = frame
  */
-  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 775, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 745, __pyx_L1_error)
   __pyx_v_c_name = __pyx_t_5;
 
-  /* "gsd/fl.pyx":777
+  /* "gsd/fl.pyx":747
  *         c_name = name_e
  *         cdef int64_t c_frame
  *         c_frame = frame             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_v_frame); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 777, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_v_frame); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 747, __pyx_L1_error)
   __pyx_v_c_frame = __pyx_t_6;
 
-  /* "gsd/fl.pyx":779
+  /* "gsd/fl.pyx":749
  *         c_frame = frame
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":780
+        /* "gsd/fl.pyx":750
  * 
  *         with nogil:
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)             # <<<<<<<<<<<<<<
  * 
  *         if index_entry == NULL:
  */
         __pyx_v_index_entry = gsd_find_chunk((&__pyx_v_self->__pyx___handle), __pyx_v_c_frame, __pyx_v_c_name);
       }
 
-      /* "gsd/fl.pyx":779
+      /* "gsd/fl.pyx":749
  *         c_frame = frame
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  */
       /*finally:*/ {
@@ -8162,832 +7933,832 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":782
+  /* "gsd/fl.pyx":752
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  *         if index_entry == NULL:             # <<<<<<<<<<<<<<
  *             raise KeyError("frame " + str(frame) + " / chunk " + name
  *                            + " not found in: " + self.name)
  */
   __pyx_t_1 = ((__pyx_v_index_entry == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":783
+    /* "gsd/fl.pyx":753
  * 
  *         if index_entry == NULL:
  *             raise KeyError("frame " + str(frame) + " / chunk " + name             # <<<<<<<<<<<<<<
  *                            + " not found in: " + self.name)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 753, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_frame_2, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_frame_2, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 753, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_3, __pyx_kp_u_chunk); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_3, __pyx_kp_u_chunk); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 753, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 753, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":784
+    /* "gsd/fl.pyx":754
  *         if index_entry == NULL:
  *             raise KeyError("frame " + str(frame) + " / chunk " + name
  *                            + " not found in: " + self.name)             # <<<<<<<<<<<<<<
  * 
  *         cdef libgsd.gsd_type gsd_type
  */
-    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_kp_u_not_found_in); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 784, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_kp_u_not_found_in); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 754, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 784, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 754, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":783
+    /* "gsd/fl.pyx":753
  * 
  *         if index_entry == NULL:
  *             raise KeyError("frame " + str(frame) + " / chunk " + name             # <<<<<<<<<<<<<<
  *                            + " not found in: " + self.name)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 753, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 783, __pyx_L1_error)
+    __PYX_ERR(0, 753, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":782
+    /* "gsd/fl.pyx":752
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  *         if index_entry == NULL:             # <<<<<<<<<<<<<<
  *             raise KeyError("frame " + str(frame) + " / chunk " + name
  *                            + " not found in: " + self.name)
  */
   }
 
-  /* "gsd/fl.pyx":787
+  /* "gsd/fl.pyx":757
  * 
  *         cdef libgsd.gsd_type gsd_type
  *         gsd_type = <libgsd.gsd_type>index_entry.type             # <<<<<<<<<<<<<<
  * 
  *         cdef void *data_ptr
  */
   __pyx_v_gsd_type = ((enum gsd_type)__pyx_v_index_entry->type);
 
-  /* "gsd/fl.pyx":790
+  /* "gsd/fl.pyx":760
  * 
  *         cdef void *data_ptr
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint8,
  *                                      shape=[index_entry.N, index_entry.M])
  */
   switch (__pyx_v_gsd_type) {
     case GSD_TYPE_UINT8:
 
-    /* "gsd/fl.pyx":791
+    /* "gsd/fl.pyx":761
  *         cdef void *data_ptr
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:
  *             data_array = numpy.empty(dtype=numpy.uint8,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 791, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 791, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 791, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 791, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 791, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":792
+    /* "gsd/fl.pyx":762
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:
  *             data_array = numpy.empty(dtype=numpy.uint8,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *             data_array = numpy.empty(dtype=numpy.uint16,
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 792, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 762, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 792, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 762, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 792, __pyx_L1_error)
+    __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 762, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
     __pyx_t_7 = 0;
     __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_t_8) < 0) __PYX_ERR(0, 791, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_t_8) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":791
+    /* "gsd/fl.pyx":761
  *         cdef void *data_ptr
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:
  *             data_array = numpy.empty(dtype=numpy.uint8,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  */
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 791, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_data_array = __pyx_t_8;
     __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":790
+    /* "gsd/fl.pyx":760
  * 
  *         cdef void *data_ptr
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint8,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_UINT16:
 
-    /* "gsd/fl.pyx":794
+    /* "gsd/fl.pyx":764
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *             data_array = numpy.empty(dtype=numpy.uint16,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 794, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 764, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 794, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 764, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 794, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 764, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 794, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 764, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 794, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 764, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 794, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 764, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":795
+    /* "gsd/fl.pyx":765
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *             data_array = numpy.empty(dtype=numpy.uint16,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *             data_array = numpy.empty(dtype=numpy.uint32,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 795, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 765, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 795, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 765, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 795, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 765, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 794, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 764, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":794
+    /* "gsd/fl.pyx":764
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *             data_array = numpy.empty(dtype=numpy.uint16,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  */
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 794, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 764, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_v_data_array = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":793
+    /* "gsd/fl.pyx":763
  *             data_array = numpy.empty(dtype=numpy.uint8,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint16,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_UINT32:
 
-    /* "gsd/fl.pyx":797
+    /* "gsd/fl.pyx":767
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *             data_array = numpy.empty(dtype=numpy.uint32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 797, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":798
+    /* "gsd/fl.pyx":768
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *             data_array = numpy.empty(dtype=numpy.uint32,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *             data_array = numpy.empty(dtype=numpy.uint64,
  */
-    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 798, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 768, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 798, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 768, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 798, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 768, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_4) < 0) __PYX_ERR(0, 797, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_4) < 0) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":797
+    /* "gsd/fl.pyx":767
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *             data_array = numpy.empty(dtype=numpy.uint32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_data_array = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":796
+    /* "gsd/fl.pyx":766
  *             data_array = numpy.empty(dtype=numpy.uint16,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint32,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_UINT64:
 
-    /* "gsd/fl.pyx":800
+    /* "gsd/fl.pyx":770
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *             data_array = numpy.empty(dtype=numpy.uint64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 800, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 800, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 800, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 800, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 800, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":801
+    /* "gsd/fl.pyx":771
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *             data_array = numpy.empty(dtype=numpy.uint64,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  *             data_array = numpy.empty(dtype=numpy.int8,
  */
-    __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 801, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 771, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 801, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 771, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 801, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 771, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_8);
     PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_8);
     __pyx_t_2 = 0;
     __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_3) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_3) < 0) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":800
+    /* "gsd/fl.pyx":770
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *             data_array = numpy.empty(dtype=numpy.uint64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 800, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_data_array = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":799
+    /* "gsd/fl.pyx":769
  *             data_array = numpy.empty(dtype=numpy.uint32,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint64,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_INT8:
 
-    /* "gsd/fl.pyx":803
+    /* "gsd/fl.pyx":773
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  *             data_array = numpy.empty(dtype=numpy.int8,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 803, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 803, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 803, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 803, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 803, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 803, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 773, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":804
+    /* "gsd/fl.pyx":774
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  *             data_array = numpy.empty(dtype=numpy.int8,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  *             data_array = numpy.empty(dtype=numpy.int16,
  */
-    __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 804, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 774, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 804, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 774, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 804, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 774, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_8);
     PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_2, 1, __pyx_t_7);
     __pyx_t_8 = 0;
     __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_t_2) < 0) __PYX_ERR(0, 803, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_t_2) < 0) __PYX_ERR(0, 773, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":803
+    /* "gsd/fl.pyx":773
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  *             data_array = numpy.empty(dtype=numpy.int8,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 803, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_data_array = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":802
+    /* "gsd/fl.pyx":772
  *             data_array = numpy.empty(dtype=numpy.uint64,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.int8,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_INT16:
 
-    /* "gsd/fl.pyx":806
+    /* "gsd/fl.pyx":776
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  *             data_array = numpy.empty(dtype=numpy.int16,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 806, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 806, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 806, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 806, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 806, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 806, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":807
+    /* "gsd/fl.pyx":777
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  *             data_array = numpy.empty(dtype=numpy.int16,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  *             data_array = numpy.empty(dtype=numpy.int32,
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 807, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 807, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 807, __pyx_L1_error)
+    __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
     __pyx_t_7 = 0;
     __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_t_8) < 0) __PYX_ERR(0, 806, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_t_8) < 0) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":806
+    /* "gsd/fl.pyx":776
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  *             data_array = numpy.empty(dtype=numpy.int16,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  */
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 806, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_data_array = __pyx_t_8;
     __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":805
+    /* "gsd/fl.pyx":775
  *             data_array = numpy.empty(dtype=numpy.int8,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.int16,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_INT32:
 
-    /* "gsd/fl.pyx":809
+    /* "gsd/fl.pyx":779
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  *             data_array = numpy.empty(dtype=numpy.int32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 809, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":810
+    /* "gsd/fl.pyx":780
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  *             data_array = numpy.empty(dtype=numpy.int32,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  *             data_array = numpy.empty(dtype=numpy.int64,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 810, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 780, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 810, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 780, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 810, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 780, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 809, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":809
+    /* "gsd/fl.pyx":779
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  *             data_array = numpy.empty(dtype=numpy.int32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  */
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_v_data_array = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":808
+    /* "gsd/fl.pyx":778
  *             data_array = numpy.empty(dtype=numpy.int16,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.int32,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_INT64:
 
-    /* "gsd/fl.pyx":812
+    /* "gsd/fl.pyx":782
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  *             data_array = numpy.empty(dtype=numpy.int64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 812, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 812, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 812, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 812, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 812, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 812, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":813
+    /* "gsd/fl.pyx":783
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  *             data_array = numpy.empty(dtype=numpy.int64,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *             data_array = numpy.empty(dtype=numpy.float32,
  */
-    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 813, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 813, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 813, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_4) < 0) __PYX_ERR(0, 812, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_4) < 0) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":812
+    /* "gsd/fl.pyx":782
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  *             data_array = numpy.empty(dtype=numpy.int64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 812, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_data_array = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":811
+    /* "gsd/fl.pyx":781
  *             data_array = numpy.empty(dtype=numpy.int32,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.int64,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_FLOAT:
 
-    /* "gsd/fl.pyx":815
+    /* "gsd/fl.pyx":785
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *             data_array = numpy.empty(dtype=numpy.float32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 815, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 815, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 815, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 815, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 815, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 815, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":816
+    /* "gsd/fl.pyx":786
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *             data_array = numpy.empty(dtype=numpy.float32,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *             data_array = numpy.empty(dtype=numpy.float64,
  */
-    __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 816, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 786, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 816, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 786, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 816, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 786, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_8);
     PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_8);
     __pyx_t_2 = 0;
     __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_3) < 0) __PYX_ERR(0, 815, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_3) < 0) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":815
+    /* "gsd/fl.pyx":785
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *             data_array = numpy.empty(dtype=numpy.float32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 815, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_data_array = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":814
+    /* "gsd/fl.pyx":784
  *             data_array = numpy.empty(dtype=numpy.int64,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.float32,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_DOUBLE:
 
-    /* "gsd/fl.pyx":818
+    /* "gsd/fl.pyx":788
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *             data_array = numpy.empty(dtype=numpy.float64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 818, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 818, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 818, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 818, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float64); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 818, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float64); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 818, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":819
+    /* "gsd/fl.pyx":789
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *             data_array = numpy.empty(dtype=numpy.float64,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("invalid type for chunk: " + name)
  */
-    __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 819, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 789, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 819, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 789, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 819, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 789, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_8);
     PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_2, 1, __pyx_t_7);
     __pyx_t_8 = 0;
     __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_t_2) < 0) __PYX_ERR(0, 818, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_t_2) < 0) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":818
+    /* "gsd/fl.pyx":788
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *             data_array = numpy.empty(dtype=numpy.float64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         else:
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 818, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_data_array = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":817
+    /* "gsd/fl.pyx":787
  *             data_array = numpy.empty(dtype=numpy.float32,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.float64,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     default:
 
-    /* "gsd/fl.pyx":821
+    /* "gsd/fl.pyx":791
  *                                      shape=[index_entry.N, index_entry.M])
  *         else:
  *             raise ValueError("invalid type for chunk: " + name)             # <<<<<<<<<<<<<<
  * 
  *         logger.debug('read chunk: ' + self.name + ' - '
  */
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 821, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 821, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 821, __pyx_L1_error)
+    __PYX_ERR(0, 791, __pyx_L1_error)
     break;
   }
 
-  /* "gsd/fl.pyx":823
+  /* "gsd/fl.pyx":793
  *             raise ValueError("invalid type for chunk: " + name)
  * 
  *         logger.debug('read chunk: ' + self.name + ' - '             # <<<<<<<<<<<<<<
  *                      + str(frame) + ' - ' + name)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 823, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 823, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_read_chunk, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 823, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_read_chunk, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 823, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":824
+  /* "gsd/fl.pyx":794
  * 
  *         logger.debug('read chunk: ' + self.name + ' - '
  *                      + str(frame) + ' - ' + name)             # <<<<<<<<<<<<<<
  * 
  *         # only read chunk if we have data
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 794, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = __Pyx_PyUnicode_Concat(__pyx_t_7, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyUnicode_Concat(__pyx_t_7, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 794, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_8, __pyx_kp_u__12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_8, __pyx_kp_u__5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 794, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyNumber_Add(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __pyx_t_8 = PyNumber_Add(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 794, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -8995,20 +8766,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 823, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":827
+  /* "gsd/fl.pyx":797
  * 
  *         # only read chunk if we have data
  *         if index_entry.N != 0 and index_entry.M != 0:             # <<<<<<<<<<<<<<
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:
  *                 data_ptr = __get_ptr_uint8(data_array)
  */
   __pyx_t_9 = ((__pyx_v_index_entry->N != 0) != 0);
@@ -9018,258 +8789,258 @@
     goto __pyx_L9_bool_binop_done;
   }
   __pyx_t_9 = ((__pyx_v_index_entry->M != 0) != 0);
   __pyx_t_1 = __pyx_t_9;
   __pyx_L9_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "gsd/fl.pyx":828
+    /* "gsd/fl.pyx":798
  *         # only read chunk if we have data
  *         if index_entry.N != 0 and index_entry.M != 0:
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  */
     switch (__pyx_v_gsd_type) {
       case GSD_TYPE_UINT8:
 
-      /* "gsd/fl.pyx":829
+      /* "gsd/fl.pyx":799
  *         if index_entry.N != 0 and index_entry.M != 0:
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:
  *                 data_ptr = __get_ptr_uint8(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *                 data_ptr = __get_ptr_uint16(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint8(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":828
+      /* "gsd/fl.pyx":798
  *         # only read chunk if we have data
  *         if index_entry.N != 0 and index_entry.M != 0:
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  */
       break;
       case GSD_TYPE_UINT16:
 
-      /* "gsd/fl.pyx":831
+      /* "gsd/fl.pyx":801
  *                 data_ptr = __get_ptr_uint8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *                 data_ptr = __get_ptr_uint16(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *                 data_ptr = __get_ptr_uint32(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint16(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":830
+      /* "gsd/fl.pyx":800
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:
  *                 data_ptr = __get_ptr_uint8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:
  */
       break;
       case GSD_TYPE_UINT32:
 
-      /* "gsd/fl.pyx":833
+      /* "gsd/fl.pyx":803
  *                 data_ptr = __get_ptr_uint16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *                 data_ptr = __get_ptr_uint32(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *                 data_ptr = __get_ptr_uint64(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint32(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":832
+      /* "gsd/fl.pyx":802
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *                 data_ptr = __get_ptr_uint16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:
  */
       break;
       case GSD_TYPE_UINT64:
 
-      /* "gsd/fl.pyx":835
+      /* "gsd/fl.pyx":805
  *                 data_ptr = __get_ptr_uint32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *                 data_ptr = __get_ptr_uint64(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:
  *                 data_ptr = __get_ptr_int8(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint64(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":834
+      /* "gsd/fl.pyx":804
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *                 data_ptr = __get_ptr_uint32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:
  */
       break;
       case GSD_TYPE_INT8:
 
-      /* "gsd/fl.pyx":837
+      /* "gsd/fl.pyx":807
  *                 data_ptr = __get_ptr_uint64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:
  *                 data_ptr = __get_ptr_int8(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:
  *                 data_ptr = __get_ptr_int16(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int8(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":836
+      /* "gsd/fl.pyx":806
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *                 data_ptr = __get_ptr_uint64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_int8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:
  */
       break;
       case GSD_TYPE_INT16:
 
-      /* "gsd/fl.pyx":839
+      /* "gsd/fl.pyx":809
  *                 data_ptr = __get_ptr_int8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:
  *                 data_ptr = __get_ptr_int16(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:
  *                 data_ptr = __get_ptr_int32(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int16(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":838
+      /* "gsd/fl.pyx":808
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:
  *                 data_ptr = __get_ptr_int8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_int16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:
  */
       break;
       case GSD_TYPE_INT32:
 
-      /* "gsd/fl.pyx":841
+      /* "gsd/fl.pyx":811
  *                 data_ptr = __get_ptr_int16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:
  *                 data_ptr = __get_ptr_int32(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:
  *                 data_ptr = __get_ptr_int64(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int32(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":840
+      /* "gsd/fl.pyx":810
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:
  *                 data_ptr = __get_ptr_int16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_int32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:
  */
       break;
       case GSD_TYPE_INT64:
 
-      /* "gsd/fl.pyx":843
+      /* "gsd/fl.pyx":813
  *                 data_ptr = __get_ptr_int32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:
  *                 data_ptr = __get_ptr_int64(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *                 data_ptr = __get_ptr_float32(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int64(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":842
+      /* "gsd/fl.pyx":812
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:
  *                 data_ptr = __get_ptr_int32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_int64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  */
       break;
       case GSD_TYPE_FLOAT:
 
-      /* "gsd/fl.pyx":845
+      /* "gsd/fl.pyx":815
  *                 data_ptr = __get_ptr_int64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *                 data_ptr = __get_ptr_float32(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *                 data_ptr = __get_ptr_float64(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_float32(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":844
+      /* "gsd/fl.pyx":814
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:
  *                 data_ptr = __get_ptr_int64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_float32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  */
       break;
       case GSD_TYPE_DOUBLE:
 
-      /* "gsd/fl.pyx":847
+      /* "gsd/fl.pyx":817
  *                 data_ptr = __get_ptr_float32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *                 data_ptr = __get_ptr_float64(data_array)             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError("invalid type for chunk: " + name)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_float64(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":846
+      /* "gsd/fl.pyx":816
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *                 data_ptr = __get_ptr_float32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_DOUBLE:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_float64(data_array)
  *             else:
  */
       break;
       default:
 
-      /* "gsd/fl.pyx":849
+      /* "gsd/fl.pyx":819
  *                 data_ptr = __get_ptr_float64(data_array)
  *             else:
  *                 raise ValueError("invalid type for chunk: " + name)             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-      __pyx_t_3 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 849, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 819, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 849, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 819, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 849, __pyx_L1_error)
+      __PYX_ERR(0, 819, __pyx_L1_error)
       break;
     }
 
-    /* "gsd/fl.pyx":851
+    /* "gsd/fl.pyx":821
  *                 raise ValueError("invalid type for chunk: " + name)
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_read_chunk(&self.__handle,
  *                                                data_ptr,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":852
+          /* "gsd/fl.pyx":822
  * 
  *             with nogil:
  *                 retval = libgsd.gsd_read_chunk(&self.__handle,             # <<<<<<<<<<<<<<
  *                                                data_ptr,
  *                                                index_entry)
  */
           __pyx_v_retval = gsd_read_chunk((&__pyx_v_self->__pyx___handle), __pyx_v_data_ptr, __pyx_v_index_entry);
         }
 
-        /* "gsd/fl.pyx":851
+        /* "gsd/fl.pyx":821
  *                 raise ValueError("invalid type for chunk: " + name)
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_read_chunk(&self.__handle,
  *                                                data_ptr,
  */
         /*finally:*/ {
@@ -9280,63 +9051,63 @@
             #endif
             goto __pyx_L13;
           }
           __pyx_L13:;
         }
     }
 
-    /* "gsd/fl.pyx":856
+    /* "gsd/fl.pyx":826
  *                                                index_entry)
  * 
  *             __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *         if index_entry.M == 1:
  */
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 856, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 826, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_v_self->name;
     __Pyx_INCREF(__pyx_t_3);
-    __pyx_t_8 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 856, __pyx_L1_error)
+    __pyx_t_8 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 826, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":827
+    /* "gsd/fl.pyx":797
  * 
  *         # only read chunk if we have data
  *         if index_entry.N != 0 and index_entry.M != 0:             # <<<<<<<<<<<<<<
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:
  *                 data_ptr = __get_ptr_uint8(data_array)
  */
   }
 
-  /* "gsd/fl.pyx":858
+  /* "gsd/fl.pyx":828
  *             __raise_on_error(retval, self.name)
  * 
  *         if index_entry.M == 1:             # <<<<<<<<<<<<<<
  *             return data_array.reshape([index_entry.N])
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_index_entry->M == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "gsd/fl.pyx":859
+    /* "gsd/fl.pyx":829
  * 
  *         if index_entry.M == 1:
  *             return data_array.reshape([index_entry.N])             # <<<<<<<<<<<<<<
  *         else:
  *             return data_array
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_reshape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 859, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_reshape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 829, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 859, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 829, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 859, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 829, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
     __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -9346,45 +9117,45 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 859, __pyx_L1_error)
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 829, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":858
+    /* "gsd/fl.pyx":828
  *             __raise_on_error(retval, self.name)
  * 
  *         if index_entry.M == 1:             # <<<<<<<<<<<<<<
  *             return data_array.reshape([index_entry.N])
  *         else:
  */
   }
 
-  /* "gsd/fl.pyx":861
+  /* "gsd/fl.pyx":831
  *             return data_array.reshape([index_entry.N])
  *         else:
  *             return data_array             # <<<<<<<<<<<<<<
  * 
  *     def find_matching_chunk_names(self, match):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_data_array);
     __pyx_r = __pyx_v_data_array;
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":718
+  /* "gsd/fl.pyx":688
  *         return index_entry != NULL
  * 
  *     def read_chunk(self, frame, name):             # <<<<<<<<<<<<<<
  *         """read_chunk(frame, name)
  * 
  */
 
@@ -9401,37 +9172,37 @@
   __Pyx_XDECREF(__pyx_v_name_e);
   __Pyx_XDECREF(__pyx_v_data_array);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":863
+/* "gsd/fl.pyx":833
  *             return data_array
  * 
  *     def find_matching_chunk_names(self, match):             # <<<<<<<<<<<<<<
  *         """find_matching_chunk_names(match)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_15find_matching_chunk_names(PyObject *__pyx_v_self, PyObject *__pyx_v_match); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_14find_matching_chunk_names[] = "find_matching_chunk_names(match)\n\n        Find all the chunk names in the file that start with the string *match*.\n\n        Args:\n            match (str): Start of the chunk name to match\n\n        Returns:\n            list[str]: Matching chunk names\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='data/chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='data/chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='input/chunk3',\n                                  data=numpy.array([9, 10],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='input/chunk4',\n                                  data=numpy.array([11, 12, 13, 14],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.find_matching_chunk_names('')\n                f.find_matching_chunk_names('data')\n                f.find_matching_chunk_names('input')\n                f.find_matching_chunk_names('other')\n                f.close()\n        ";
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_15find_matching_chunk_names(PyObject *__pyx_v_self, PyObject *__pyx_v_match) {
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_17find_matching_chunk_names(PyObject *__pyx_v_self, PyObject *__pyx_v_match); /*proto*/
+static char __pyx_doc_3gsd_2fl_7GSDFile_16find_matching_chunk_names[] = "find_matching_chunk_names(match)\n\n        Find all the chunk names in the file that start with the string *match*.\n\n        Args:\n            match (str): Start of the chunk name to match\n\n        Returns:\n            list[str]: Matching chunk names\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='data/chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='data/chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='input/chunk3',\n                                  data=numpy.array([9, 10],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='input/chunk4',\n                                  data=numpy.array([11, 12, 13, 14],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.find_matching_chunk_names('')\n                f.find_matching_chunk_names('data')\n                f.find_matching_chunk_names('input')\n                f.find_matching_chunk_names('other')\n                f.close()\n        ";
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_17find_matching_chunk_names(PyObject *__pyx_v_self, PyObject *__pyx_v_match) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find_matching_chunk_names (wrapper)", 0);
-  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_14find_matching_chunk_names(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), ((PyObject *)__pyx_v_match));
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_16find_matching_chunk_names(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), ((PyObject *)__pyx_v_match));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_14find_matching_chunk_names(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_match) {
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_16find_matching_chunk_names(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_match) {
   char const *__pyx_v_c_found;
   char *__pyx_v_c_match;
   PyObject *__pyx_v_match_e = NULL;
   PyObject *__pyx_v_retval = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -9441,121 +9212,121 @@
   char *__pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_matching_chunk_names", 0);
 
-  /* "gsd/fl.pyx":906
+  /* "gsd/fl.pyx":876
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":907
+    /* "gsd/fl.pyx":877
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         cdef const char * c_found
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 907, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 877, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 907, __pyx_L1_error)
+    __PYX_ERR(0, 877, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":906
+    /* "gsd/fl.pyx":876
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":911
+  /* "gsd/fl.pyx":881
  *         cdef const char * c_found
  *         cdef char * c_match
  *         match_e = match.encode('utf-8')             # <<<<<<<<<<<<<<
  *         c_match = match_e
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 911, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_match_e = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":912
+  /* "gsd/fl.pyx":882
  *         cdef char * c_match
  *         match_e = match.encode('utf-8')
  *         c_match = match_e             # <<<<<<<<<<<<<<
  * 
  *         retval = []
  */
-  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_match_e); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 912, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_match_e); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 882, __pyx_L1_error)
   __pyx_v_c_match = __pyx_t_5;
 
-  /* "gsd/fl.pyx":914
+  /* "gsd/fl.pyx":884
  *         c_match = match_e
  * 
  *         retval = []             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 914, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_retval = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":916
+  /* "gsd/fl.pyx":886
  *         retval = []
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,
  *                                                           c_match,
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":917
+        /* "gsd/fl.pyx":887
  * 
  *         with nogil:
  *             c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,             # <<<<<<<<<<<<<<
  *                                                           c_match,
  *                                                           NULL)
  */
         __pyx_v_c_found = gsd_find_matching_chunk_name((&__pyx_v_self->__pyx___handle), __pyx_v_c_match, NULL);
       }
 
-      /* "gsd/fl.pyx":916
+      /* "gsd/fl.pyx":886
  *         retval = []
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,
  *                                                           c_match,
  */
       /*finally:*/ {
@@ -9566,63 +9337,63 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":921
+  /* "gsd/fl.pyx":891
  *                                                           NULL)
  * 
  *         while c_found != NULL:             # <<<<<<<<<<<<<<
  *             retval.append(c_found.decode('utf-8'))
  * 
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_c_found != NULL) != 0);
     if (!__pyx_t_1) break;
 
-    /* "gsd/fl.pyx":922
+    /* "gsd/fl.pyx":892
  * 
  *         while c_found != NULL:
  *             retval.append(c_found.decode('utf-8'))             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_c_found, 0, strlen(__pyx_v_c_found), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 922, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_c_found, 0, strlen(__pyx_v_c_found), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 892, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_retval, __pyx_t_2); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 922, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_retval, __pyx_t_2); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 892, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":924
+    /* "gsd/fl.pyx":894
  *             retval.append(c_found.decode('utf-8'))
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,
  *                                                               c_match,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":925
+          /* "gsd/fl.pyx":895
  * 
  *             with nogil:
  *                 c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,             # <<<<<<<<<<<<<<
  *                                                               c_match,
  *                                                               c_found)
  */
           __pyx_v_c_found = gsd_find_matching_chunk_name((&__pyx_v_self->__pyx___handle), __pyx_v_c_match, __pyx_v_c_found);
         }
 
-        /* "gsd/fl.pyx":924
+        /* "gsd/fl.pyx":894
  *             retval.append(c_found.decode('utf-8'))
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,
  *                                                               c_match,
  */
         /*finally:*/ {
@@ -9634,27 +9405,27 @@
             goto __pyx_L13;
           }
           __pyx_L13:;
         }
     }
   }
 
-  /* "gsd/fl.pyx":929
+  /* "gsd/fl.pyx":899
  *                                                               c_found)
  * 
  *         return retval             # <<<<<<<<<<<<<<
  * 
  *     def upgrade(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_retval);
   __pyx_r = __pyx_v_retval;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":863
+  /* "gsd/fl.pyx":833
  *             return data_array
  * 
  *     def find_matching_chunk_names(self, match):             # <<<<<<<<<<<<<<
  *         """find_matching_chunk_names(match)
  * 
  */
 
@@ -9669,140 +9440,140 @@
   __Pyx_XDECREF(__pyx_v_match_e);
   __Pyx_XDECREF(__pyx_v_retval);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":931
+/* "gsd/fl.pyx":901
  *         return retval
  * 
  *     def upgrade(self):             # <<<<<<<<<<<<<<
  *         """upgrade()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_17upgrade(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_16upgrade[] = "upgrade()\n\n        Upgrade a GSD file to the v2 specification in place. The file must be\n        open in a writable mode.\n\n        ";
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_17upgrade(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_19upgrade(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_3gsd_2fl_7GSDFile_18upgrade[] = "upgrade()\n\n        Upgrade a GSD file to the v2 specification in place. The file must be\n        open in a writable mode.\n\n        ";
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_19upgrade(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("upgrade (wrapper)", 0);
-  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_16upgrade(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_18upgrade(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_16upgrade(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_18upgrade(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   int __pyx_v_retval;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("upgrade", 0);
 
-  /* "gsd/fl.pyx":939
+  /* "gsd/fl.pyx":909
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":940
+    /* "gsd/fl.pyx":910
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         logger.info('upgrading file: ' + self.name)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 940, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 910, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 940, __pyx_L1_error)
+    __PYX_ERR(0, 910, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":939
+    /* "gsd/fl.pyx":909
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":942
+  /* "gsd/fl.pyx":912
  *             raise ValueError("File is not open")
  * 
  *         logger.info('upgrading file: ' + self.name)             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 942, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 912, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 942, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 912, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_upgrading_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 942, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_upgrading_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 912, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 942, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 912, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":944
+  /* "gsd/fl.pyx":914
  *         logger.info('upgrading file: ' + self.name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_upgrade(&self.__handle)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":945
+        /* "gsd/fl.pyx":915
  * 
  *         with nogil:
  *             retval = libgsd.gsd_upgrade(&self.__handle)             # <<<<<<<<<<<<<<
  * 
  *         __raise_on_error(retval, self.name)
  */
         __pyx_v_retval = gsd_upgrade((&__pyx_v_self->__pyx___handle));
       }
 
-      /* "gsd/fl.pyx":944
+      /* "gsd/fl.pyx":914
  *         logger.info('upgrading file: ' + self.name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_upgrade(&self.__handle)
  * 
  */
       /*finally:*/ {
@@ -9813,32 +9584,32 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":947
+  /* "gsd/fl.pyx":917
  *             retval = libgsd.gsd_upgrade(&self.__handle)
  * 
  *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 917, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_4);
-  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 917, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":931
+  /* "gsd/fl.pyx":901
  *         return retval
  * 
  *     def upgrade(self):             # <<<<<<<<<<<<<<
  *         """upgrade()
  * 
  */
 
@@ -9854,78 +9625,78 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":949
+/* "gsd/fl.pyx":919
  *         __raise_on_error(retval, self.name)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_19__enter__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_19__enter__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_21__enter__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_21__enter__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_18__enter__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_20__enter__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_18__enter__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_20__enter__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "gsd/fl.pyx":950
+  /* "gsd/fl.pyx":920
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, exc_type, exc_value, traceback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":949
+  /* "gsd/fl.pyx":919
  *         __raise_on_error(retval, self.name)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":952
+/* "gsd/fl.pyx":922
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_21__exit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_21__exit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_23__exit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_23__exit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_exc_type = 0;
   CYTHON_UNUSED PyObject *__pyx_v_exc_value = 0;
   CYTHON_UNUSED PyObject *__pyx_v_traceback = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -9952,90 +9723,90 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 952, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 922, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_traceback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 952, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 922, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 952, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 922, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_exc_type = values[0];
     __pyx_v_exc_value = values[1];
     __pyx_v_traceback = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 952, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 922, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_20__exit__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_exc_type, __pyx_v_exc_value, __pyx_v_traceback);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_22__exit__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_exc_type, __pyx_v_exc_value, __pyx_v_traceback);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_20__exit__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_type, CYTHON_UNUSED PyObject *__pyx_v_exc_value, CYTHON_UNUSED PyObject *__pyx_v_traceback) {
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_22__exit__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_type, CYTHON_UNUSED PyObject *__pyx_v_exc_value, CYTHON_UNUSED PyObject *__pyx_v_traceback) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "gsd/fl.pyx":953
+  /* "gsd/fl.pyx":923
  * 
  *     def __exit__(self, exc_type, exc_value, traceback):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def __reduce__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 953, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 923, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 953, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 923, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":952
+  /* "gsd/fl.pyx":922
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -10050,37 +9821,37 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":955
+/* "gsd/fl.pyx":925
  *         self.close()
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         """Allows filehandles to be pickled when in read only mode."""
  *         if self.mode not in ['rb', 'r']:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_23__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_22__reduce__[] = "Allows filehandles to be pickled when in read only mode.";
-static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_23__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_25__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_3gsd_2fl_7GSDFile_24__reduce__[] = "Allows filehandles to be pickled when in read only mode.";
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_25__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_22__reduce__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_24__reduce__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_22__reduce__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_24__reduce__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
@@ -10088,114 +9859,114 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce__", 0);
 
-  /* "gsd/fl.pyx":957
+  /* "gsd/fl.pyx":927
  *     def __reduce__(self):
  *         """Allows filehandles to be pickled when in read only mode."""
  *         if self.mode not in ['rb', 'r']:             # <<<<<<<<<<<<<<
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,
  */
   __Pyx_INCREF(__pyx_v_self->mode);
   __pyx_t_1 = __pyx_v_self->mode;
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_rb, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 957, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_rb, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 927, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_r, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 957, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_r, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 927, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":958
+    /* "gsd/fl.pyx":928
  *         """Allows filehandles to be pickled when in read only mode."""
  *         if self.mode not in ['rb', 'r']:
  *             raise PickleError("Only read only GSDFiles can be pickled.")             # <<<<<<<<<<<<<<
  *         return (GSDFile,
  *                 (self.name, self.mode, self.application,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 958, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 928, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_kp_u_Only_read_only_GSDFiles_can_be_p) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_kp_u_Only_read_only_GSDFiles_can_be_p);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 958, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 928, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 958, __pyx_L1_error)
+    __PYX_ERR(0, 928, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":957
+    /* "gsd/fl.pyx":927
  *     def __reduce__(self):
  *         """Allows filehandles to be pickled when in read only mode."""
  *         if self.mode not in ['rb', 'r']:             # <<<<<<<<<<<<<<
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,
  */
   }
 
-  /* "gsd/fl.pyx":959
+  /* "gsd/fl.pyx":929
  *         if self.mode not in ['rb', 'r']:
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,             # <<<<<<<<<<<<<<
  *                 (self.name, self.mode, self.application,
  *                     self.schema, self.schema_version),
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "gsd/fl.pyx":960
+  /* "gsd/fl.pyx":930
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,
  *                 (self.name, self.mode, self.application,             # <<<<<<<<<<<<<<
  *                     self.schema, self.schema_version),
  *                 )
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_application); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 960, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_application); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 930, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "gsd/fl.pyx":961
+  /* "gsd/fl.pyx":931
  *         return (GSDFile,
  *                 (self.name, self.mode, self.application,
  *                     self.schema, self.schema_version),             # <<<<<<<<<<<<<<
  *                 )
  * 
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 961, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema_version); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 961, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema_version); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "gsd/fl.pyx":960
+  /* "gsd/fl.pyx":930
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,
  *                 (self.name, self.mode, self.application,             # <<<<<<<<<<<<<<
  *                     self.schema, self.schema_version),
  *                 )
  */
-  __pyx_t_8 = PyTuple_New(5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 960, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 930, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_v_self->name);
   __Pyx_GIVEREF(__pyx_v_self->name);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_self->name);
   __Pyx_INCREF(__pyx_v_self->mode);
   __Pyx_GIVEREF(__pyx_v_self->mode);
   PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_self->mode);
@@ -10205,34 +9976,34 @@
   PyTuple_SET_ITEM(__pyx_t_8, 3, __pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_8, 4, __pyx_t_7);
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
 
-  /* "gsd/fl.pyx":959
+  /* "gsd/fl.pyx":929
  *         if self.mode not in ['rb', 'r']:
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,             # <<<<<<<<<<<<<<
  *                 (self.name, self.mode, self.application,
  *                     self.schema, self.schema_version),
  */
-  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 959, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 929, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile));
   PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile));
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_8);
   __pyx_t_8 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":955
+  /* "gsd/fl.pyx":925
  *         self.close()
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         """Allows filehandles to be pickled when in read only mode."""
  *         if self.mode not in ['rb', 'r']:
  */
 
@@ -10247,15 +10018,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":965
+/* "gsd/fl.pyx":935
  * 
  *     property name:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.name
  * 
  */
 
@@ -10273,42 +10044,42 @@
 }
 
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4name___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":966
+  /* "gsd/fl.pyx":936
  *     property name:
  *         def __get__(self):
  *             return self.name             # <<<<<<<<<<<<<<
  * 
  *     property mode:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_r = __pyx_v_self->name;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":965
+  /* "gsd/fl.pyx":935
  * 
  *     property name:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.name
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":969
+/* "gsd/fl.pyx":939
  * 
  *     property mode:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.mode
  * 
  */
 
@@ -10326,42 +10097,42 @@
 }
 
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4mode___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":970
+  /* "gsd/fl.pyx":940
  *     property mode:
  *         def __get__(self):
  *             return self.mode             # <<<<<<<<<<<<<<
  * 
  *     property gsd_version:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->mode);
   __pyx_r = __pyx_v_self->mode;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":969
+  /* "gsd/fl.pyx":939
  * 
  *     property mode:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.mode
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":973
+/* "gsd/fl.pyx":943
  * 
  *     property gsd_version:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             cdef uint32_t v = self.__handle.header.gsd_version
  *             return (v >> 16, v & 0xffff)
  */
 
@@ -10387,49 +10158,49 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":974
+  /* "gsd/fl.pyx":944
  *     property gsd_version:
  *         def __get__(self):
  *             cdef uint32_t v = self.__handle.header.gsd_version             # <<<<<<<<<<<<<<
  *             return (v >> 16, v & 0xffff)
  * 
  */
   __pyx_t_1 = __pyx_v_self->__pyx___handle.header.gsd_version;
   __pyx_v_v = __pyx_t_1;
 
-  /* "gsd/fl.pyx":975
+  /* "gsd/fl.pyx":945
  *         def __get__(self):
  *             cdef uint32_t v = self.__handle.header.gsd_version
  *             return (v >> 16, v & 0xffff)             # <<<<<<<<<<<<<<
  * 
  *     property schema_version:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_v >> 16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_v >> 16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_long((__pyx_v_v & 0xffff)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long((__pyx_v_v & 0xffff)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":973
+  /* "gsd/fl.pyx":943
  * 
  *     property gsd_version:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             cdef uint32_t v = self.__handle.header.gsd_version
  *             return (v >> 16, v & 0xffff)
  */
 
@@ -10442,15 +10213,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":978
+/* "gsd/fl.pyx":948
  * 
  *     property schema_version:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             cdef uint32_t v = self.__handle.header.schema_version
  *             return (v >> 16, v & 0xffff)
  */
 
@@ -10476,49 +10247,49 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":979
+  /* "gsd/fl.pyx":949
  *     property schema_version:
  *         def __get__(self):
  *             cdef uint32_t v = self.__handle.header.schema_version             # <<<<<<<<<<<<<<
  *             return (v >> 16, v & 0xffff)
  * 
  */
   __pyx_t_1 = __pyx_v_self->__pyx___handle.header.schema_version;
   __pyx_v_v = __pyx_t_1;
 
-  /* "gsd/fl.pyx":980
+  /* "gsd/fl.pyx":950
  *         def __get__(self):
  *             cdef uint32_t v = self.__handle.header.schema_version
  *             return (v >> 16, v & 0xffff)             # <<<<<<<<<<<<<<
  * 
  *     property schema:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_v >> 16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 980, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_v >> 16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_long((__pyx_v_v & 0xffff)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 980, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long((__pyx_v_v & 0xffff)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 980, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":978
+  /* "gsd/fl.pyx":948
  * 
  *     property schema_version:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             cdef uint32_t v = self.__handle.header.schema_version
  *             return (v >> 16, v & 0xffff)
  */
 
@@ -10531,15 +10302,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":983
+/* "gsd/fl.pyx":953
  * 
  *     property schema:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.__handle.header.schema.decode('utf-8')
  * 
  */
 
@@ -10562,31 +10333,31 @@
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":984
+  /* "gsd/fl.pyx":954
  *     property schema:
  *         def __get__(self):
  *             return self.__handle.header.schema.decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  *     property application:
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->__pyx___handle.header.schema;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 984, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 954, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":983
+  /* "gsd/fl.pyx":953
  * 
  *     property schema:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.__handle.header.schema.decode('utf-8')
  * 
  */
 
@@ -10597,15 +10368,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":987
+/* "gsd/fl.pyx":957
  * 
  *     property application:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.__handle.header.application.decode('utf-8')
  * 
  */
 
@@ -10628,31 +10399,31 @@
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":988
+  /* "gsd/fl.pyx":958
  *     property application:
  *         def __get__(self):
  *             return self.__handle.header.application.decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  *     property nframes:
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->__pyx___handle.header.application;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 988, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 958, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":987
+  /* "gsd/fl.pyx":957
  * 
  *     property application:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.__handle.header.application.decode('utf-8')
  * 
  */
 
@@ -10663,15 +10434,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":991
+/* "gsd/fl.pyx":961
  * 
  *     property nframes:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if not self.__is_open:
  *                 raise ValueError("File is not open")
  */
 
@@ -10694,61 +10465,61 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":992
+  /* "gsd/fl.pyx":962
  *     property nframes:
  *         def __get__(self):
  *             if not self.__is_open:             # <<<<<<<<<<<<<<
  *                 raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":993
+    /* "gsd/fl.pyx":963
  *         def __get__(self):
  *             if not self.__is_open:
  *                 raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *             return libgsd.gsd_get_nframes(&self.__handle)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 993, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 993, __pyx_L1_error)
+    __PYX_ERR(0, 963, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":992
+    /* "gsd/fl.pyx":962
  *     property nframes:
  *         def __get__(self):
  *             if not self.__is_open:             # <<<<<<<<<<<<<<
  *                 raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":995
+  /* "gsd/fl.pyx":965
  *                 raise ValueError("File is not open")
  * 
  *             return libgsd.gsd_get_nframes(&self.__handle)             # <<<<<<<<<<<<<<
  * 
- *     def __dealloc__(self):
+ *     property maximum_write_buffer_size:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(gsd_get_nframes((&__pyx_v_self->__pyx___handle))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 995, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(gsd_get_nframes((&__pyx_v_self->__pyx___handle))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 965, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":991
+  /* "gsd/fl.pyx":961
  * 
  *     property nframes:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if not self.__is_open:
  *                 raise ValueError("File is not open")
  */
 
@@ -10759,113 +10530,537 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":997
- *             return libgsd.gsd_get_nframes(&self.__handle)
+/* "gsd/fl.pyx":968
+ * 
+ *     property maximum_write_buffer_size:
+ *         def __get__(self):             # <<<<<<<<<<<<<<
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_25maximum_write_buffer_size___get__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_25maximum_write_buffer_size___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+
+  /* "gsd/fl.pyx":969
+ *     property maximum_write_buffer_size:
+ *         def __get__(self):
+ *             if not self.__is_open:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("File is not open")
+ * 
+ */
+  __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
+  if (unlikely(__pyx_t_1)) {
+
+    /* "gsd/fl.pyx":970
+ *         def __get__(self):
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")             # <<<<<<<<<<<<<<
+ * 
+ *             return libgsd.gsd_get_maximum_write_buffer_size(&self.__handle)
+ */
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 970, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 970, __pyx_L1_error)
+
+    /* "gsd/fl.pyx":969
+ *     property maximum_write_buffer_size:
+ *         def __get__(self):
+ *             if not self.__is_open:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("File is not open")
+ * 
+ */
+  }
+
+  /* "gsd/fl.pyx":972
+ *                 raise ValueError("File is not open")
+ * 
+ *             return libgsd.gsd_get_maximum_write_buffer_size(&self.__handle)             # <<<<<<<<<<<<<<
+ * 
+ *         def __set__(self, size):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(gsd_get_maximum_write_buffer_size((&__pyx_v_self->__pyx___handle))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 972, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "gsd/fl.pyx":968
+ * 
+ *     property maximum_write_buffer_size:
+ *         def __get__(self):             # <<<<<<<<<<<<<<
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("gsd.fl.GSDFile.maximum_write_buffer_size.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "gsd/fl.pyx":974
+ *             return libgsd.gsd_get_maximum_write_buffer_size(&self.__handle)
+ * 
+ *         def __set__(self, size):             # <<<<<<<<<<<<<<
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")
+ */
+
+/* Python wrapper */
+static int __pyx_pw_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_size); /*proto*/
+static int __pyx_pw_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_size) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_2__set__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), ((PyObject *)__pyx_v_size));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_2__set__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_size) {
+  int __pyx_v_retval;
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  uint64_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+
+  /* "gsd/fl.pyx":975
+ * 
+ *         def __set__(self, size):
+ *             if not self.__is_open:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("File is not open")
+ * 
+ */
+  __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
+  if (unlikely(__pyx_t_1)) {
+
+    /* "gsd/fl.pyx":976
+ *         def __set__(self, size):
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")             # <<<<<<<<<<<<<<
+ * 
+ *             retval = libgsd.gsd_set_maximum_write_buffer_size(&self.__handle, size)
+ */
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 976, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 976, __pyx_L1_error)
+
+    /* "gsd/fl.pyx":975
+ * 
+ *         def __set__(self, size):
+ *             if not self.__is_open:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("File is not open")
+ * 
+ */
+  }
+
+  /* "gsd/fl.pyx":978
+ *                 raise ValueError("File is not open")
+ * 
+ *             retval = libgsd.gsd_set_maximum_write_buffer_size(&self.__handle, size)             # <<<<<<<<<<<<<<
+ *             __raise_on_error(retval, self.name)
+ * 
+ */
+  __pyx_t_3 = __Pyx_PyInt_As_uint64_t(__pyx_v_size); if (unlikely((__pyx_t_3 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 978, __pyx_L1_error)
+  __pyx_v_retval = gsd_set_maximum_write_buffer_size((&__pyx_v_self->__pyx___handle), __pyx_t_3);
+
+  /* "gsd/fl.pyx":979
+ * 
+ *             retval = libgsd.gsd_set_maximum_write_buffer_size(&self.__handle, size)
+ *             __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
+ * 
+ *     property index_entries_to_buffer:
+ */
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 979, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __pyx_v_self->name;
+  __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_5 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 979, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "gsd/fl.pyx":974
+ *             return libgsd.gsd_get_maximum_write_buffer_size(&self.__handle)
+ * 
+ *         def __set__(self, size):             # <<<<<<<<<<<<<<
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("gsd.fl.GSDFile.maximum_write_buffer_size.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "gsd/fl.pyx":982
+ * 
+ *     property index_entries_to_buffer:
+ *         def __get__(self):             # <<<<<<<<<<<<<<
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_23index_entries_to_buffer_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_23index_entries_to_buffer_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_23index_entries_to_buffer___get__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_23index_entries_to_buffer___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+
+  /* "gsd/fl.pyx":983
+ *     property index_entries_to_buffer:
+ *         def __get__(self):
+ *             if not self.__is_open:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("File is not open")
+ * 
+ */
+  __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
+  if (unlikely(__pyx_t_1)) {
+
+    /* "gsd/fl.pyx":984
+ *         def __get__(self):
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")             # <<<<<<<<<<<<<<
+ * 
+ *             return libgsd.gsd_get_index_entries_to_buffer(&self.__handle)
+ */
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 984, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 984, __pyx_L1_error)
+
+    /* "gsd/fl.pyx":983
+ *     property index_entries_to_buffer:
+ *         def __get__(self):
+ *             if not self.__is_open:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("File is not open")
+ * 
+ */
+  }
+
+  /* "gsd/fl.pyx":986
+ *                 raise ValueError("File is not open")
+ * 
+ *             return libgsd.gsd_get_index_entries_to_buffer(&self.__handle)             # <<<<<<<<<<<<<<
+ * 
+ *         def __set__(self, number):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(gsd_get_index_entries_to_buffer((&__pyx_v_self->__pyx___handle))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 986, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "gsd/fl.pyx":982
+ * 
+ *     property index_entries_to_buffer:
+ *         def __get__(self):             # <<<<<<<<<<<<<<
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("gsd.fl.GSDFile.index_entries_to_buffer.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "gsd/fl.pyx":988
+ *             return libgsd.gsd_get_index_entries_to_buffer(&self.__handle)
+ * 
+ *         def __set__(self, number):             # <<<<<<<<<<<<<<
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")
+ */
+
+/* Python wrapper */
+static int __pyx_pw_3gsd_2fl_7GSDFile_23index_entries_to_buffer_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_number); /*proto*/
+static int __pyx_pw_3gsd_2fl_7GSDFile_23index_entries_to_buffer_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_number) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_23index_entries_to_buffer_2__set__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), ((PyObject *)__pyx_v_number));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_3gsd_2fl_7GSDFile_23index_entries_to_buffer_2__set__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_number) {
+  int __pyx_v_retval;
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  uint64_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+
+  /* "gsd/fl.pyx":989
+ * 
+ *         def __set__(self, number):
+ *             if not self.__is_open:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("File is not open")
+ * 
+ */
+  __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
+  if (unlikely(__pyx_t_1)) {
+
+    /* "gsd/fl.pyx":990
+ *         def __set__(self, number):
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")             # <<<<<<<<<<<<<<
+ * 
+ *             retval = libgsd.gsd_set_index_entries_to_buffer(&self.__handle, number)
+ */
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 990, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 990, __pyx_L1_error)
+
+    /* "gsd/fl.pyx":989
+ * 
+ *         def __set__(self, number):
+ *             if not self.__is_open:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("File is not open")
+ * 
+ */
+  }
+
+  /* "gsd/fl.pyx":992
+ *                 raise ValueError("File is not open")
+ * 
+ *             retval = libgsd.gsd_set_index_entries_to_buffer(&self.__handle, number)             # <<<<<<<<<<<<<<
+ *             __raise_on_error(retval, self.name)
+ * 
+ */
+  __pyx_t_3 = __Pyx_PyInt_As_uint64_t(__pyx_v_number); if (unlikely((__pyx_t_3 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 992, __pyx_L1_error)
+  __pyx_v_retval = gsd_set_index_entries_to_buffer((&__pyx_v_self->__pyx___handle), __pyx_t_3);
+
+  /* "gsd/fl.pyx":993
+ * 
+ *             retval = libgsd.gsd_set_index_entries_to_buffer(&self.__handle, number)
+ *             __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
+ * 
+ *     def __dealloc__(self):
+ */
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __pyx_v_self->name;
+  __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_5 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "gsd/fl.pyx":988
+ *             return libgsd.gsd_get_index_entries_to_buffer(&self.__handle)
+ * 
+ *         def __set__(self, number):             # <<<<<<<<<<<<<<
+ *             if not self.__is_open:
+ *                 raise ValueError("File is not open")
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("gsd.fl.GSDFile.index_entries_to_buffer.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "gsd/fl.pyx":995
+ *             __raise_on_error(retval, self.name)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  */
 
 /* Python wrapper */
-static void __pyx_pw_3gsd_2fl_7GSDFile_25__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_3gsd_2fl_7GSDFile_25__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_3gsd_2fl_7GSDFile_27__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_3gsd_2fl_7GSDFile_27__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_3gsd_2fl_7GSDFile_24__dealloc__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
+  __pyx_pf_3gsd_2fl_7GSDFile_26__dealloc__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_3gsd_2fl_7GSDFile_24__dealloc__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
+static void __pyx_pf_3gsd_2fl_7GSDFile_26__dealloc__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "gsd/fl.pyx":998
+  /* "gsd/fl.pyx":996
  * 
  *     def __dealloc__(self):
  *         if self.__is_open:             # <<<<<<<<<<<<<<
  *             logger.info('closing file: ' + self.name)
  *             libgsd.gsd_close(&self.__handle)
  */
   __pyx_t_1 = (__pyx_v_self->__pyx___is_open != 0);
   if (__pyx_t_1) {
 
-    /* "gsd/fl.pyx":999
+    /* "gsd/fl.pyx":997
  *     def __dealloc__(self):
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)             # <<<<<<<<<<<<<<
  *             libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 999, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 997, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 999, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 997, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_closing_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 999, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_closing_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 997, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 999, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 997, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":1000
+    /* "gsd/fl.pyx":998
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  *             libgsd.gsd_close(&self.__handle)             # <<<<<<<<<<<<<<
  *             self.__is_open = False
  */
     (void)(gsd_close((&__pyx_v_self->__pyx___handle)));
 
-    /* "gsd/fl.pyx":1001
+    /* "gsd/fl.pyx":999
  *             logger.info('closing file: ' + self.name)
  *             libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False             # <<<<<<<<<<<<<<
  */
     __pyx_v_self->__pyx___is_open = 0;
 
-    /* "gsd/fl.pyx":998
+    /* "gsd/fl.pyx":996
  * 
  *     def __dealloc__(self):
  *         if self.__is_open:             # <<<<<<<<<<<<<<
  *             logger.info('closing file: ' + self.name)
  *             libgsd.gsd_close(&self.__handle)
  */
   }
 
-  /* "gsd/fl.pyx":997
- *             return libgsd.gsd_get_nframes(&self.__handle)
+  /* "gsd/fl.pyx":995
+ *             __raise_on_error(retval, self.name)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  */
 
   /* function exit code */
@@ -10876,15 +11071,15 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_WriteUnraisable("gsd.fl.GSDFile.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10893,29 +11088,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10926,15 +11121,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10943,29 +11138,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10976,15 +11171,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10993,29 +11188,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -11026,15 +11221,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11043,29 +11238,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11076,15 +11271,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11093,29 +11288,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11126,212 +11321,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11347,15 +11542,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -11363,84 +11558,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11455,15 +11650,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11479,15 +11674,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11495,84 +11690,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11587,15 +11782,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11611,15 +11806,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11627,84 +11822,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11719,176 +11914,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -11919,15 +12114,15 @@
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_3gsd_2fl_7GSDFile_25__dealloc__(o);
+    __pyx_pw_3gsd_2fl_7GSDFile_27__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->mode);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -11956,37 +12151,68 @@
   return __pyx_pw_3gsd_2fl_7GSDFile_11application_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_3gsd_2fl_7GSDFile_nframes(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_3gsd_2fl_7GSDFile_7nframes_1__get__(o);
 }
 
+static PyObject *__pyx_getprop_3gsd_2fl_7GSDFile_maximum_write_buffer_size(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_1__get__(o);
+}
+
+static int __pyx_setprop_3gsd_2fl_7GSDFile_maximum_write_buffer_size(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_3gsd_2fl_7GSDFile_25maximum_write_buffer_size_3__set__(o, v);
+  }
+  else {
+    PyErr_SetString(PyExc_NotImplementedError, "__del__");
+    return -1;
+  }
+}
+
+static PyObject *__pyx_getprop_3gsd_2fl_7GSDFile_index_entries_to_buffer(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_3gsd_2fl_7GSDFile_23index_entries_to_buffer_1__get__(o);
+}
+
+static int __pyx_setprop_3gsd_2fl_7GSDFile_index_entries_to_buffer(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_3gsd_2fl_7GSDFile_23index_entries_to_buffer_3__set__(o, v);
+  }
+  else {
+    PyErr_SetString(PyExc_NotImplementedError, "__del__");
+    return -1;
+  }
+}
+
 static PyMethodDef __pyx_methods_3gsd_2fl_GSDFile[] = {
   {"close", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_3close, METH_NOARGS, __pyx_doc_3gsd_2fl_7GSDFile_2close},
   {"truncate", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_5truncate, METH_NOARGS, __pyx_doc_3gsd_2fl_7GSDFile_4truncate},
   {"end_frame", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_7end_frame, METH_NOARGS, __pyx_doc_3gsd_2fl_7GSDFile_6end_frame},
-  {"write_chunk", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_7GSDFile_9write_chunk, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3gsd_2fl_7GSDFile_8write_chunk},
-  {"chunk_exists", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_7GSDFile_11chunk_exists, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3gsd_2fl_7GSDFile_10chunk_exists},
-  {"read_chunk", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_7GSDFile_13read_chunk, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3gsd_2fl_7GSDFile_12read_chunk},
-  {"find_matching_chunk_names", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_15find_matching_chunk_names, METH_O, __pyx_doc_3gsd_2fl_7GSDFile_14find_matching_chunk_names},
-  {"upgrade", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_17upgrade, METH_NOARGS, __pyx_doc_3gsd_2fl_7GSDFile_16upgrade},
-  {"__enter__", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_19__enter__, METH_NOARGS, 0},
-  {"__exit__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_7GSDFile_21__exit__, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce__", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_23__reduce__, METH_NOARGS, __pyx_doc_3gsd_2fl_7GSDFile_22__reduce__},
+  {"flush", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_9flush, METH_NOARGS, __pyx_doc_3gsd_2fl_7GSDFile_8flush},
+  {"write_chunk", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_7GSDFile_11write_chunk, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3gsd_2fl_7GSDFile_10write_chunk},
+  {"chunk_exists", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_7GSDFile_13chunk_exists, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3gsd_2fl_7GSDFile_12chunk_exists},
+  {"read_chunk", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_7GSDFile_15read_chunk, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3gsd_2fl_7GSDFile_14read_chunk},
+  {"find_matching_chunk_names", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_17find_matching_chunk_names, METH_O, __pyx_doc_3gsd_2fl_7GSDFile_16find_matching_chunk_names},
+  {"upgrade", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_19upgrade, METH_NOARGS, __pyx_doc_3gsd_2fl_7GSDFile_18upgrade},
+  {"__enter__", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_21__enter__, METH_NOARGS, 0},
+  {"__exit__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_7GSDFile_23__exit__, METH_VARARGS|METH_KEYWORDS, 0},
+  {"__reduce__", (PyCFunction)__pyx_pw_3gsd_2fl_7GSDFile_25__reduce__, METH_NOARGS, __pyx_doc_3gsd_2fl_7GSDFile_24__reduce__},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_3gsd_2fl_GSDFile[] = {
   {(char *)"name", __pyx_getprop_3gsd_2fl_7GSDFile_name, 0, (char *)0, 0},
   {(char *)"mode", __pyx_getprop_3gsd_2fl_7GSDFile_mode, 0, (char *)0, 0},
   {(char *)"gsd_version", __pyx_getprop_3gsd_2fl_7GSDFile_gsd_version, 0, (char *)0, 0},
   {(char *)"schema_version", __pyx_getprop_3gsd_2fl_7GSDFile_schema_version, 0, (char *)0, 0},
   {(char *)"schema", __pyx_getprop_3gsd_2fl_7GSDFile_schema, 0, (char *)0, 0},
   {(char *)"application", __pyx_getprop_3gsd_2fl_7GSDFile_application, 0, (char *)0, 0},
   {(char *)"nframes", __pyx_getprop_3gsd_2fl_7GSDFile_nframes, 0, (char *)0, 0},
+  {(char *)"maximum_write_buffer_size", __pyx_getprop_3gsd_2fl_7GSDFile_maximum_write_buffer_size, __pyx_setprop_3gsd_2fl_7GSDFile_maximum_write_buffer_size, (char *)0, 0},
+  {(char *)"index_entries_to_buffer", __pyx_getprop_3gsd_2fl_7GSDFile_index_entries_to_buffer, __pyx_setprop_3gsd_2fl_7GSDFile_index_entries_to_buffer, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_3gsd_2fl_GSDFile = {
   PyVarObject_HEAD_INIT(0, 0)
   "gsd.fl.GSDFile", /*tp_name*/
   sizeof(struct __pyx_obj_3gsd_2fl_GSDFile), /*tp_basicsize*/
@@ -12013,15 +12239,15 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
-  "GSDFile\n\n    GSD file access interface.\n\n    Args:\n\n        name (str): Name of the open file.\n\n        mode (str): Mode of the open file.\n\n        gsd_version (tuple[int, int]): GSD file layer version number\n            (major, minor).\n\n        application (str): Name of the generating application.\n\n        schema (str): Name of the data schema.\n\n        schema_version (tuple[int, int]): Schema version number\n            (major, minor).\n\n        nframes (int): Number of frames.\n\n    :py:class:`GSDFile` implements an object oriented class interface to the GSD\n    file layer. Use :py:func:`open` to open a GSD file and obtain a\n    :py:class:`GSDFile` instance. :py:class:`GSDFile` can be used as a context\n    manager.\n\n    Attributes:\n\n        name (str): Name of the open file.\n\n        mode (str): Mode of the open file.\n\n        gsd_version (tuple[int, int]): GSD file layer version number\n            (major, minor).\n\n        application (str): Name of the generating application.\n\n        schema (str): Name of the data schema.\n\n        schema_version (tuple[int, int]): Schema version number\n            (major, minor).\n\n        nframes (int): Number of frames.\n    ", /*tp_doc*/
+  "GSDFile\n\n    GSD file access interface.\n\n    Args:\n\n        name (str): Name of the open file.\n\n        mode (str): Mode of the open file.\n\n        gsd_version (tuple[int, int]): GSD file layer version number\n            (major, minor).\n\n        application (str): Name of the generating application.\n\n        schema (str): Name of the data schema.\n\n        schema_version (tuple[int, int]): Schema version number\n            (major, minor).\n\n        nframes (int): Number of frames.\n\n    :py:class:`GSDFile` implements an object oriented class interface to the GSD\n    file layer. Use :py:func:`open` to open a GSD file and obtain a\n    :py:class:`GSDFile` instance. :py:class:`GSDFile` can be used as a context\n    manager.\n\n    Attributes:\n\n        name (str): Name of the open file.\n\n        mode (str): Mode of the open file.\n\n        gsd_version (tuple[int, int]): GSD file layer version number\n            (major, minor).\n\n        application (str): Name of the generating application.\n\n        schema (str): Name of the data schema.\n\n        schema_version (tuple[int, int]): Schema version number\n            (major, minor).\n\n        nframes (int): Number of frames.\n\n        maximum_write_buffer_size (int): The Maximum write buffer size (bytes).\n\n        index_entries_to_buffer (int): Number of index entries to buffer before\n            flushing.\n    ", /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_3gsd_2fl_GSDFile, /*tp_methods*/
@@ -12049,15 +12275,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -12104,15 +12330,14 @@
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_Corrupt_GSD_file, __pyx_k_Corrupt_GSD_file, sizeof(__pyx_k_Corrupt_GSD_file), 0, 1, 0, 0},
   {&__pyx_kp_u_File_is_not_open, __pyx_k_File_is_not_open, sizeof(__pyx_k_File_is_not_open), 0, 1, 0, 0},
   {&__pyx_kp_u_File_must_be_readable, __pyx_k_File_must_be_readable, sizeof(__pyx_k_File_must_be_readable), 0, 1, 0, 0},
   {&__pyx_kp_u_File_must_be_writable, __pyx_k_File_must_be_writable, sizeof(__pyx_k_File_must_be_writable), 0, 1, 0, 0},
-  {&__pyx_n_s_FutureWarning, __pyx_k_FutureWarning, sizeof(__pyx_k_FutureWarning), 0, 0, 1, 1},
   {&__pyx_n_s_GSDFile, __pyx_k_GSDFile, sizeof(__pyx_k_GSDFile), 0, 0, 1, 1},
   {&__pyx_kp_u_GSD_can_only_write_1_or_2_dimens, __pyx_k_GSD_can_only_write_1_or_2_dimens, sizeof(__pyx_k_GSD_can_only_write_1_or_2_dimens), 0, 1, 0, 0},
   {&__pyx_kp_u_GSD_namelist_is_full, __pyx_k_GSD_namelist_is_full, sizeof(__pyx_k_GSD_namelist_is_full), 0, 1, 0, 0},
   {&__pyx_n_s_IOError, __pyx_k_IOError, sizeof(__pyx_k_IOError), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_u_Invalid_gsd_argument, __pyx_k_Invalid_gsd_argument, sizeof(__pyx_k_Invalid_gsd_argument), 0, 1, 0, 0},
   {&__pyx_kp_u_Invalid_mode, __pyx_k_Invalid_mode, sizeof(__pyx_k_Invalid_mode), 0, 1, 0, 0},
@@ -12122,27 +12347,19 @@
   {&__pyx_kp_u_Not_a_GSD_file, __pyx_k_Not_a_GSD_file, sizeof(__pyx_k_Not_a_GSD_file), 0, 1, 0, 0},
   {&__pyx_kp_u_Only_read_only_GSDFiles_can_be_p, __pyx_k_Only_read_only_GSDFiles_can_be_p, sizeof(__pyx_k_Only_read_only_GSDFiles_can_be_p), 0, 1, 0, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_kp_u_Provide_application_when_creatin, __pyx_k_Provide_application_when_creatin, sizeof(__pyx_k_Provide_application_when_creatin), 0, 1, 0, 0},
   {&__pyx_kp_u_Provide_schema_version_when_crea, __pyx_k_Provide_schema_version_when_crea, sizeof(__pyx_k_Provide_schema_version_when_crea), 0, 1, 0, 0},
   {&__pyx_kp_u_Provide_schema_when_creating_a_f, __pyx_k_Provide_schema_when_creating_a_f, sizeof(__pyx_k_Provide_schema_when_creating_a_f), 0, 1, 0, 0},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
-  {&__pyx_kp_u_The_ab_mode_is_deprecated_use_r, __pyx_k_The_ab_mode_is_deprecated_use_r, sizeof(__pyx_k_The_ab_mode_is_deprecated_use_r), 0, 1, 0, 0},
-  {&__pyx_kp_u_The_rb_mode_is_deprecated_use_r, __pyx_k_The_rb_mode_is_deprecated_use_r, sizeof(__pyx_k_The_rb_mode_is_deprecated_use_r), 0, 1, 0, 0},
-  {&__pyx_kp_u_The_rb_mode_is_deprecated_use_r_2, __pyx_k_The_rb_mode_is_deprecated_use_r_2, sizeof(__pyx_k_The_rb_mode_is_deprecated_use_r_2), 0, 1, 0, 0},
-  {&__pyx_kp_u_The_wb_mode_is_deprecated_use_w, __pyx_k_The_wb_mode_is_deprecated_use_w, sizeof(__pyx_k_The_wb_mode_is_deprecated_use_w), 0, 1, 0, 0},
-  {&__pyx_kp_u_The_wb_mode_is_deprecated_use_w_2, __pyx_k_The_wb_mode_is_deprecated_use_w_2, sizeof(__pyx_k_The_wb_mode_is_deprecated_use_w_2), 0, 1, 0, 0},
-  {&__pyx_kp_u_The_xb_mode_is_deprecated_use_x, __pyx_k_The_xb_mode_is_deprecated_use_x, sizeof(__pyx_k_The_xb_mode_is_deprecated_use_x), 0, 1, 0, 0},
-  {&__pyx_kp_u_The_xb_mode_is_deprecated_use_x_2, __pyx_k_The_xb_mode_is_deprecated_use_x_2, sizeof(__pyx_k_The_xb_mode_is_deprecated_use_x_2), 0, 1, 0, 0},
   {&__pyx_kp_u_Unknown_error, __pyx_k_Unknown_error, sizeof(__pyx_k_Unknown_error), 0, 1, 0, 0},
   {&__pyx_kp_u_Unsupported_GSD_file_version, __pyx_k_Unsupported_GSD_file_version, sizeof(__pyx_k_Unsupported_GSD_file_version), 0, 1, 0, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-  {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
+  {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
   {&__pyx_n_u_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 1, 0, 1},
-  {&__pyx_n_u_ab, __pyx_k_ab, sizeof(__pyx_k_ab), 0, 1, 0, 1},
   {&__pyx_kp_u_and_schema_version, __pyx_k_and_schema_version, sizeof(__pyx_k_and_schema_version), 0, 1, 0, 0},
   {&__pyx_n_s_application, __pyx_k_application, sizeof(__pyx_k_application), 0, 0, 1, 1},
   {&__pyx_kp_u_application_2, __pyx_k_application_2, sizeof(__pyx_k_application_2), 0, 1, 0, 0},
   {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
   {&__pyx_kp_u_chunk, __pyx_k_chunk, sizeof(__pyx_k_chunk), 0, 1, 0, 0},
   {&__pyx_kp_u_chunk_exists, __pyx_k_chunk_exists, sizeof(__pyx_k_chunk_exists), 0, 1, 0, 0},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
@@ -12156,14 +12373,15 @@
   {&__pyx_kp_u_end_frame, __pyx_k_end_frame, sizeof(__pyx_k_end_frame), 0, 1, 0, 0},
   {&__pyx_n_s_exc_type, __pyx_k_exc_type, sizeof(__pyx_k_exc_type), 0, 0, 1, 1},
   {&__pyx_n_s_exc_value, __pyx_k_exc_value, sizeof(__pyx_k_exc_value), 0, 0, 1, 1},
   {&__pyx_n_s_exists, __pyx_k_exists, sizeof(__pyx_k_exists), 0, 0, 1, 1},
   {&__pyx_kp_u_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 1, 0, 0},
   {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
   {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
+  {&__pyx_kp_u_flush, __pyx_k_flush, sizeof(__pyx_k_flush), 0, 1, 0, 0},
   {&__pyx_n_s_frame, __pyx_k_frame, sizeof(__pyx_k_frame), 0, 0, 1, 1},
   {&__pyx_kp_u_frame_2, __pyx_k_frame_2, sizeof(__pyx_k_frame_2), 0, 1, 0, 0},
   {&__pyx_n_s_getLogger, __pyx_k_getLogger, sizeof(__pyx_k_getLogger), 0, 0, 1, 1},
   {&__pyx_n_s_gsd_fl, __pyx_k_gsd_fl, sizeof(__pyx_k_gsd_fl), 0, 0, 1, 1},
   {&__pyx_kp_u_gsd_fl, __pyx_k_gsd_fl, sizeof(__pyx_k_gsd_fl), 0, 1, 0, 0},
   {&__pyx_kp_s_gsd_fl_pyx, __pyx_k_gsd_fl_pyx, sizeof(__pyx_k_gsd_fl_pyx), 0, 0, 1, 0},
   {&__pyx_kp_u_has_incorrect_schema, __pyx_k_has_incorrect_schema, sizeof(__pyx_k_has_incorrect_schema), 0, 1, 0, 0},
@@ -12190,15 +12408,14 @@
   {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
   {&__pyx_kp_u_overwriting_file, __pyx_k_overwriting_file, sizeof(__pyx_k_overwriting_file), 0, 1, 0, 0},
   {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
   {&__pyx_kp_u_r_2, __pyx_k_r_2, sizeof(__pyx_k_r_2), 0, 1, 0, 0},
   {&__pyx_n_u_rb, __pyx_k_rb, sizeof(__pyx_k_rb), 0, 1, 0, 1},
-  {&__pyx_kp_u_rb_2, __pyx_k_rb_2, sizeof(__pyx_k_rb_2), 0, 1, 0, 0},
   {&__pyx_kp_u_read_chunk, __pyx_k_read_chunk, sizeof(__pyx_k_read_chunk), 0, 1, 0, 0},
   {&__pyx_n_s_reshape, __pyx_k_reshape, sizeof(__pyx_k_reshape), 0, 0, 1, 1},
   {&__pyx_n_s_schema, __pyx_k_schema, sizeof(__pyx_k_schema), 0, 0, 1, 1},
   {&__pyx_kp_u_schema_2, __pyx_k_schema_2, sizeof(__pyx_k_schema_2), 0, 1, 0, 0},
   {&__pyx_n_s_schema_version, __pyx_k_schema_version, sizeof(__pyx_k_schema_version), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
@@ -12210,208 +12427,125 @@
   {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
   {&__pyx_n_s_uint64, __pyx_k_uint64, sizeof(__pyx_k_uint64), 0, 0, 1, 1},
   {&__pyx_n_s_uint8, __pyx_k_uint8, sizeof(__pyx_k_uint8), 0, 0, 1, 1},
   {&__pyx_kp_u_upgrading_file, __pyx_k_upgrading_file, sizeof(__pyx_k_upgrading_file), 0, 1, 0, 0},
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
   {&__pyx_n_u_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 1, 0, 1},
-  {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
   {&__pyx_n_s_warning, __pyx_k_warning, sizeof(__pyx_k_warning), 0, 0, 1, 1},
   {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
-  {&__pyx_n_u_wb, __pyx_k_wb, sizeof(__pyx_k_wb), 0, 1, 0, 1},
-  {&__pyx_kp_u_wb_2, __pyx_k_wb_2, sizeof(__pyx_k_wb_2), 0, 1, 0, 0},
   {&__pyx_kp_u_with_mode, __pyx_k_with_mode, sizeof(__pyx_k_with_mode), 0, 1, 0, 0},
   {&__pyx_kp_u_write_chunk, __pyx_k_write_chunk, sizeof(__pyx_k_write_chunk), 0, 1, 0, 0},
   {&__pyx_n_u_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 1, 0, 1},
-  {&__pyx_n_u_xb, __pyx_k_xb, sizeof(__pyx_k_xb), 0, 1, 0, 1},
-  {&__pyx_kp_u_xb_2, __pyx_k_xb_2, sizeof(__pyx_k_xb_2), 0, 1, 0, 0},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_IOError = __Pyx_GetBuiltinName(__pyx_n_s_IOError); if (!__pyx_builtin_IOError) __PYX_ERR(0, 43, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 45, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 51, __pyx_L1_error)
-  __pyx_builtin_FutureWarning = __Pyx_GetBuiltinName(__pyx_n_s_FutureWarning); if (!__pyx_builtin_FutureWarning) __PYX_ERR(0, 318, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 360, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 783, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 753, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "gsd/fl.pyx":317
- *         if mode == 'wb':
- *             mode = 'w'
- *             warnings.warn("The 'wb' mode is deprecated, use 'w'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'wb+':
- */
-  __pyx_tuple_ = PyTuple_Pack(2, __pyx_kp_u_The_wb_mode_is_deprecated_use_w, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 317, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
-
-  /* "gsd/fl.pyx":321
- *         elif mode == 'wb+':
- *             mode = 'w'
- *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'rb':
- */
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_kp_u_The_wb_mode_is_deprecated_use_w_2, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 321, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "gsd/fl.pyx":325
- *         elif mode == 'rb':
- *             mode = 'r'
- *             warnings.warn("The 'rb' mode is deprecated, use 'r'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'rb+':
- */
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_kp_u_The_rb_mode_is_deprecated_use_r, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 325, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-
-  /* "gsd/fl.pyx":329
- *         elif mode == 'rb+':
- *             mode = 'r+'
- *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'xb':
- */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_kp_u_The_rb_mode_is_deprecated_use_r_2, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 329, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
-  /* "gsd/fl.pyx":333
- *         elif mode == 'xb':
- *             mode = 'x'
- *             warnings.warn("The 'xb' mode is deprecated, use 'x'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'xb+':
- */
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_kp_u_The_xb_mode_is_deprecated_use_x, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 333, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-
-  /* "gsd/fl.pyx":337
- *         elif mode == 'xb+':
- *             mode = 'x'
- *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- *         elif mode == 'ab':
- */
-  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_kp_u_The_xb_mode_is_deprecated_use_x_2, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 337, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-
-  /* "gsd/fl.pyx":341
- *         elif mode == 'ab':
- *             mode = 'r+'
- *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",             # <<<<<<<<<<<<<<
- *                            FutureWarning)
- * 
- */
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_kp_u_The_ab_mode_is_deprecated_use_r, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 341, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-
-  /* "gsd/fl.pyx":372
+  /* "gsd/fl.pyx":326
  *         if overwrite:
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")             # <<<<<<<<<<<<<<
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Provide_application_when_creatin); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 372, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Provide_application_when_creatin); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "gsd/fl.pyx":374
+  /* "gsd/fl.pyx":328
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")             # <<<<<<<<<<<<<<
  *             if schema_version is None:
  *                 raise ValueError("Provide schema_version when creating a file")
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Provide_schema_when_creating_a_f); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 374, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Provide_schema_when_creating_a_f); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "gsd/fl.pyx":376
+  /* "gsd/fl.pyx":330
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:
  *                 raise ValueError("Provide schema_version when creating a file")             # <<<<<<<<<<<<<<
  * 
  *             # create a new file or overwrite an existing one
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Provide_schema_version_when_crea); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 376, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Provide_schema_version_when_crea); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "gsd/fl.pyx":491
+  /* "gsd/fl.pyx":445
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         logger.info('truncating file: ' + self.name)
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_File_is_not_open); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 491, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_File_is_not_open); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 445, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "gsd/fl.pyx":26
  * cimport numpy
  * 
  * logger = logging.getLogger('gsd.fl')             # <<<<<<<<<<<<<<
  * 
  * ####################
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_gsd_fl); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_gsd_fl); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "gsd/fl.pyx":149
  * 
  * 
  * def open(name, mode, application=None, schema=None, schema_version=None):             # <<<<<<<<<<<<<<
  *     """open(name, mode, application=None, schema=None, schema_version=None)
  * 
  */
-  __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_name, __pyx_n_s_mode, __pyx_n_s_application, __pyx_n_s_schema, __pyx_n_s_schema_version); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gsd_fl_pyx, __pyx_n_s_open, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_name, __pyx_n_s_mode, __pyx_n_s_application, __pyx_n_s_schema, __pyx_n_s_schema_version); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gsd_fl_pyx, __pyx_n_s_open, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -12459,22 +12593,22 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_3gsd_2fl_GSDFile) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_3gsd_2fl_GSDFile) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_3gsd_2fl_GSDFile.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_3gsd_2fl_GSDFile.tp_dictoffset && __pyx_type_3gsd_2fl_GSDFile.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_3gsd_2fl_GSDFile.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_GSDFile, (PyObject *)&__pyx_type_3gsd_2fl_GSDFile) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_GSDFile, (PyObject *)&__pyx_type_3gsd_2fl_GSDFile) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
   __pyx_ptype_3gsd_2fl_GSDFile = &__pyx_type_3gsd_2fl_GSDFile;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -12485,70 +12619,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -12848,15 +12951,15 @@
  * ####################
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_logger, __pyx_t_2) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "gsd/fl.pyx":149
  * 
@@ -12876,15 +12979,15 @@
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -14873,18 +14976,18 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -14930,22 +15033,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -15783,15 +15886,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15979,15 +16082,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16175,15 +16278,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16371,15 +16474,15 @@
                         } else if (8 * sizeof(int64_t) >= 4 * PyLong_SHIFT) {
                             return (int64_t) (((((((((int64_t)digits[3]) << PyLong_SHIFT) | (int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16643,15 +16746,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16839,15 +16942,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `gsd-2.9.0/gsd/fl.pyx` & `gsd-3.0.0/gsd/fl.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -191,36 +191,14 @@
     ``application`` and ``schema_version`` are ignored and may be ``None``.
     When ``schema`` is not ``None``, :py:func:`open` throws an exception if the
     file's schema does not match ``schema``.
 
     When opening a file for writing (``'w'``, ``'x'``, or ``'a'`` modes): The
     given ``application``, ``schema``, and ``schema_version`` must not be None.
 
-    .. deprecated:: 2.9.0
-
-        The following values to ``mode`` are deprecated:
-
-        +------------------+---------------------------------------------+
-        | mode             | description                                 |
-        +==================+=============================================+
-        | ``'rb'``         | Equivalent to ``'r'``                       |
-        +------------------+---------------------------------------------+
-        | ``'rb+'``        | Equivalent to ``'r+'``                      |
-        +------------------+---------------------------------------------+
-        | ``'wb'``         | Equivalent to ``'w'``                       |
-        +------------------+---------------------------------------------+
-        | ``'wb+'``        | Equivalent to ``'w'``                       |
-        +------------------+---------------------------------------------+
-        | ``'xb'``         | Equivalent to ``'x'``                       |
-        +------------------+---------------------------------------------+
-        | ``'xb+'``        | Equivalent to ``'x'``                       |
-        +------------------+---------------------------------------------+
-        | ``'ab'``         | Equivalent to ``'r+'``                      |
-        +------------------+---------------------------------------------+
-
     Example:
 
         .. ipython:: python
 
             with gsd.fl.open(name='file.gsd', mode='w',
                              application="My application", schema="My Schema",
                              schema_version=[1,0]) as f:
@@ -289,14 +267,19 @@
 
         schema (str): Name of the data schema.
 
         schema_version (tuple[int, int]): Schema version number
             (major, minor).
 
         nframes (int): Number of frames.
+
+        maximum_write_buffer_size (int): The Maximum write buffer size (bytes).
+
+        index_entries_to_buffer (int): Number of index entries to buffer before
+            flushing.
     """
 
     cdef libgsd.gsd_handle __handle
     cdef bint __is_open
     cdef str mode
     cdef str name
 
@@ -308,43 +291,14 @@
                  schema_version):
         cdef libgsd.gsd_open_flag c_flags
         cdef int exclusive_create = 0
         cdef int overwrite = 0
 
         self.mode = mode
 
-        if mode == 'wb':
-            mode = 'w'
-            warnings.warn("The 'wb' mode is deprecated, use 'w'",
-                           FutureWarning)
-        elif mode == 'wb+':
-            mode = 'w'
-            warnings.warn("The 'wb+' mode is deprecated, use 'w'",
-                           FutureWarning)
-        elif mode == 'rb':
-            mode = 'r'
-            warnings.warn("The 'rb' mode is deprecated, use 'r'",
-                           FutureWarning)
-        elif mode == 'rb+':
-            mode = 'r+'
-            warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
-                           FutureWarning)
-        elif mode == 'xb':
-            mode = 'x'
-            warnings.warn("The 'xb' mode is deprecated, use 'x'",
-                           FutureWarning)
-        elif mode == 'xb+':
-            mode = 'x'
-            warnings.warn("The 'xb+' mode is deprecated, use 'x'",
-                           FutureWarning)
-        elif mode == 'ab':
-            mode = 'r+'
-            warnings.warn("The 'ab' mode is deprecated, use 'r+'",
-                           FutureWarning)
-
         if mode == 'w':
             c_flags = libgsd.GSD_OPEN_READWRITE
             overwrite = 1
         elif mode == 'r':
             c_flags = libgsd.GSD_OPEN_READONLY
         elif mode == 'r+':
             c_flags = libgsd.GSD_OPEN_READWRITE
@@ -538,14 +492,30 @@
         logger.debug('end frame: ' + self.name)
 
         with nogil:
             retval = libgsd.gsd_end_frame(&self.__handle)
 
         __raise_on_error(retval, self.name)
 
+    def flush(self):
+        """flush()
+
+        Flush all buffered frames to the file.
+        """
+
+        if not self.__is_open:
+            raise ValueError("File is not open")
+
+        logger.debug('flush: ' + self.name)
+
+        with nogil:
+            retval = libgsd.gsd_flush(&self.__handle)
+
+        __raise_on_error(retval, self.name)
+
     def write_chunk(self, name, data):
         """write_chunk(name, data)
 
         Write a data chunk to the file. After writing all chunks in the
         current frame, call :py:meth:`end_frame()`.
 
         Args:
@@ -990,12 +960,40 @@
     property nframes:
         def __get__(self):
             if not self.__is_open:
                 raise ValueError("File is not open")
 
             return libgsd.gsd_get_nframes(&self.__handle)
 
+    property maximum_write_buffer_size:
+        def __get__(self):
+            if not self.__is_open:
+                raise ValueError("File is not open")
+
+            return libgsd.gsd_get_maximum_write_buffer_size(&self.__handle)
+
+        def __set__(self, size):
+            if not self.__is_open:
+                raise ValueError("File is not open")
+
+            retval = libgsd.gsd_set_maximum_write_buffer_size(&self.__handle, size)
+            __raise_on_error(retval, self.name)
+
+    property index_entries_to_buffer:
+        def __get__(self):
+            if not self.__is_open:
+                raise ValueError("File is not open")
+
+            return libgsd.gsd_get_index_entries_to_buffer(&self.__handle)
+
+        def __set__(self, number):
+            if not self.__is_open:
+                raise ValueError("File is not open")
+
+            retval = libgsd.gsd_set_index_entries_to_buffer(&self.__handle, number)
+            __raise_on_error(retval, self.name)
+
     def __dealloc__(self):
         if self.__is_open:
             logger.info('closing file: ' + self.name)
             libgsd.gsd_close(&self.__handle)
             self.__is_open = False
```

### Comparing `gsd-2.9.0/gsd/gsd.c` & `gsd-3.0.0/gsd/gsd.c`

 * *Files 4% similar despite different names*

```diff
@@ -60,24 +60,24 @@
 
 /// Initial size of write buffer
 enum
     {
     GSD_INITIAL_WRITE_BUFFER_SIZE = 1024
     };
 
-/// Maximum size of write buffer
+/// Default maximum size of write buffer
 enum
     {
-    GSD_MAXIMUM_WRITE_BUFFER_SIZE = 16 * 1024 * 1024
+    GSD_DEFAULT_MAXIMUM_WRITE_BUFFER_SIZE = 64 * 1024 * 1024
     };
 
-/// Size of copy buffer
+/// Default number of index entries to buffer
 enum
     {
-    GSD_COPY_BUFFER_SIZE = 128 * 1024
+    GSD_DEFAULT_INDEX_ENTRIES_TO_BUFFER = 256 * 1024
     };
 
 /// Size of hash map
 enum
     {
     GSD_NAME_MAP_SIZE = 57557
     };
@@ -961,25 +961,31 @@
     int retval = gsd_index_buffer_free(&handle->file_index);
     if (retval != 0)
         {
         return retval;
         }
 
     // allocate the copy buffer
-    char* buf = malloc(GSD_COPY_BUFFER_SIZE);
+    uint64_t copy_buffer_size
+        = GSD_DEFAULT_INDEX_ENTRIES_TO_BUFFER * sizeof(struct gsd_index_entry);
+    if (copy_buffer_size > size_old * sizeof(struct gsd_index_entry))
+        {
+        copy_buffer_size = size_old * sizeof(struct gsd_index_entry);
+        }
+    char* buf = malloc(copy_buffer_size);
 
     // write the current index to the end of the file
     int64_t new_index_location = lseek(handle->fd, 0, SEEK_END);
     int64_t old_index_location = handle->header.index_location;
     size_t total_bytes_written = 0;
     size_t old_index_bytes = size_old * sizeof(struct gsd_index_entry);
     while (total_bytes_written < old_index_bytes)
         {
-        size_t bytes_to_copy = GSD_COPY_BUFFER_SIZE;
-        if (old_index_bytes - total_bytes_written < GSD_COPY_BUFFER_SIZE)
+        size_t bytes_to_copy = copy_buffer_size;
+        if (old_index_bytes - total_bytes_written < copy_buffer_size)
             {
             bytes_to_copy = old_index_bytes - total_bytes_written;
             }
 
         ssize_t bytes_read = gsd_io_pread_retry(handle->fd,
                                                 buf,
                                                 bytes_to_copy,
@@ -1002,21 +1008,21 @@
             return GSD_ERROR_IO;
             }
 
         total_bytes_written += bytes_written;
         }
 
     // fill the new index space with 0s
-    gsd_util_zero_memory(buf, GSD_COPY_BUFFER_SIZE);
+    gsd_util_zero_memory(buf, copy_buffer_size);
 
     size_t new_index_bytes = size_new * sizeof(struct gsd_index_entry);
     while (total_bytes_written < new_index_bytes)
         {
-        size_t bytes_to_copy = GSD_COPY_BUFFER_SIZE;
-        if (new_index_bytes - total_bytes_written < GSD_COPY_BUFFER_SIZE)
+        size_t bytes_to_copy = copy_buffer_size;
+        if (new_index_bytes - total_bytes_written < copy_buffer_size)
             {
             bytes_to_copy = new_index_bytes - total_bytes_written;
             }
 
         ssize_t bytes_written = gsd_io_pwrite_retry(handle->fd,
                                                     buf,
                                                     bytes_to_copy,
@@ -1116,15 +1122,15 @@
         }
 
     handle->file_size += handle->write_buffer.size;
 
     // reset write_buffer for new data
     handle->write_buffer.size = 0;
 
-    // move buffer_index entries to file_index
+    // Move buffer_index entries to frame_index.
     size_t i;
     for (i = 0; i < handle->buffer_index.size; i++)
         {
         struct gsd_index_entry* new_index;
         int retval = gsd_index_buffer_add(&handle->frame_index, &new_index);
         if (retval != GSD_SUCCESS)
             {
@@ -1586,14 +1592,18 @@
         retval = gsd_byte_buffer_allocate(&handle->frame_names.data, GSD_NAME_SIZE);
         if (retval != GSD_SUCCESS)
             {
             return retval;
             }
         }
 
+    handle->pending_index_entries = 0;
+    handle->maximum_write_buffer_size = GSD_DEFAULT_MAXIMUM_WRITE_BUFFER_SIZE;
+    handle->index_entries_to_buffer = GSD_DEFAULT_INDEX_ENTRIES_TO_BUFFER;
+
     return GSD_SUCCESS;
     }
 
 uint32_t gsd_make_version(unsigned int major, unsigned int minor)
     {
     return major << (sizeof(uint32_t) * 4) | minor;
     }
@@ -1796,18 +1806,29 @@
 int gsd_close(struct gsd_handle* handle)
     {
     if (handle == NULL)
         {
         return GSD_ERROR_INVALID_ARGUMENT;
         }
 
+    int retval;
+
+    if (handle->open_flags != GSD_OPEN_READONLY)
+        {
+        retval = gsd_flush(handle);
+        if (retval != GSD_SUCCESS)
+            {
+            return retval;
+            }
+        }
+
     // save the fd so we can use it after freeing the handle
     int fd = handle->fd;
 
-    int retval = gsd_index_buffer_free(&handle->file_index);
+    retval = gsd_index_buffer_free(&handle->file_index);
     if (retval != GSD_SUCCESS)
         {
         return retval;
         }
 
     if (handle->frame_index.reserved > 0)
         {
@@ -1879,16 +1900,35 @@
         return GSD_ERROR_INVALID_ARGUMENT;
         }
     if (handle->open_flags == GSD_OPEN_READONLY)
         {
         return GSD_ERROR_FILE_MUST_BE_WRITABLE;
         }
 
-    // increment the frame counter
     handle->cur_frame++;
+    handle->pending_index_entries = 0;
+
+    if (handle->frame_index.size > 0 || handle->buffer_index.size > handle->index_entries_to_buffer)
+        {
+        return gsd_flush(handle);
+        }
+
+    return GSD_SUCCESS;
+    }
+
+int gsd_flush(struct gsd_handle* handle)
+    {
+    if (handle == NULL)
+        {
+        return GSD_ERROR_INVALID_ARGUMENT;
+        }
+    if (handle->open_flags == GSD_OPEN_READONLY)
+        {
+        return GSD_ERROR_FILE_MUST_BE_WRITABLE;
+        }
 
     // flush the namelist buffer
     int retval = gsd_flush_name_buffer(handle);
     if (retval != GSD_SUCCESS)
         {
         return retval;
         }
@@ -1903,55 +1943,72 @@
     // sync the data before writing the index
     retval = fsync(handle->fd);
     if (retval != 0)
         {
         return GSD_ERROR_IO;
         }
 
-    // write the frame index to the file
-    if (handle->frame_index.size > 0)
+    // Write the frame index to the file, excluding the index entries that are part of the current
+    // frame.
+    if (handle->pending_index_entries > handle->frame_index.size)
+        {
+        return GSD_ERROR_INVALID_ARGUMENT;
+        }
+    uint64_t index_entries_to_write = handle->frame_index.size - handle->pending_index_entries;
+
+    if (index_entries_to_write > 0)
         {
         // ensure there is enough space in the index
-        if ((handle->file_index.size + handle->frame_index.size) > handle->file_index.reserved)
+        if ((handle->file_index.size + index_entries_to_write) > handle->file_index.reserved)
             {
-            gsd_expand_file_index(handle, handle->file_index.size + handle->frame_index.size);
+            gsd_expand_file_index(handle, handle->file_index.size + index_entries_to_write);
             }
 
         // sort the index before writing
         retval = gsd_index_buffer_sort(&handle->frame_index);
         if (retval != 0)
             {
             return retval;
             }
 
         // write the frame index entries to the file
         int64_t write_pos = handle->header.index_location
                             + sizeof(struct gsd_index_entry) * handle->file_index.size;
 
-        size_t bytes_to_write = sizeof(struct gsd_index_entry) * handle->frame_index.size;
+        size_t bytes_to_write = sizeof(struct gsd_index_entry) * index_entries_to_write;
         ssize_t bytes_written
             = gsd_io_pwrite_retry(handle->fd, handle->frame_index.data, bytes_to_write, write_pos);
 
         if (bytes_written == -1 || bytes_written != bytes_to_write)
             {
             return GSD_ERROR_IO;
             }
 
 #if !GSD_USE_MMAP
         // add the entries to the file index
         memcpy(handle->file_index.data + handle->file_index.size,
                handle->frame_index.data,
-               sizeof(struct gsd_index_entry) * handle->frame_index.size);
+               sizeof(struct gsd_index_entry) * index_entries_to_write);
 #endif
 
         // update size of file index
-        handle->file_index.size += handle->frame_index.size;
+        handle->file_index.size += index_entries_to_write;
 
-        // clear the frame index
-        handle->frame_index.size = 0;
+        // Clear the frame index, keeping those in the current unfinished frame.
+        if (handle->pending_index_entries > 0)
+            {
+            for (uint64_t i = 0; i < handle->pending_index_entries; i++)
+                {
+                handle->frame_index.data[i]
+                    = handle->frame_index
+                          .data[handle->frame_index.size - handle->pending_index_entries];
+                }
+            }
+
+        handle->frame_index.size = handle->pending_index_entries;
         }
 
     return GSD_SUCCESS;
     }
 
 int gsd_write_chunk(struct gsd_handle* handle,
                     const char* name,
@@ -2003,18 +2060,18 @@
     entry.id = id;
     entry.type = (uint8_t)type;
     entry.N = N;
     entry.M = M;
     size_t size = N * M * gsd_sizeof_type(type);
 
     // decide whether to write this chunk to the buffer or straight to disk
-    if (size < GSD_MAXIMUM_WRITE_BUFFER_SIZE / 2)
+    if (size < handle->maximum_write_buffer_size)
         {
         // flush the buffer if this entry won't fit
-        if (size > (GSD_MAXIMUM_WRITE_BUFFER_SIZE - handle->write_buffer.size))
+        if (size > (handle->maximum_write_buffer_size - handle->write_buffer.size))
             {
             gsd_flush_write_buffer(handle);
             }
 
         entry.location = handle->write_buffer.size;
 
         // add an entry to the buffer index
@@ -2059,14 +2116,15 @@
             return GSD_ERROR_IO;
             }
 
         // update the file_size in the handle
         handle->file_size += bytes_written;
         }
 
+    handle->pending_index_entries++;
     return GSD_SUCCESS;
     }
 
 uint64_t gsd_get_nframes(struct gsd_handle* handle)
     {
     if (handle == NULL)
         {
@@ -2086,14 +2144,22 @@
         {
         return NULL;
         }
     if (frame >= gsd_get_nframes(handle))
         {
         return NULL;
         }
+    if (handle->open_flags != GSD_OPEN_READONLY)
+        {
+        int retval = gsd_flush(handle);
+        if (retval != GSD_SUCCESS)
+            {
+            return NULL;
+            }
+        }
 
     // find the id for the given name
     uint16_t match_id = gsd_name_id_map_find(&handle->name_map, name);
     if (match_id == UINT16_MAX)
         {
         return NULL;
         }
@@ -2176,14 +2242,22 @@
         {
         return GSD_ERROR_INVALID_ARGUMENT;
         }
     if (chunk == NULL)
         {
         return GSD_ERROR_INVALID_ARGUMENT;
         }
+    if (handle->open_flags != GSD_OPEN_READONLY)
+        {
+        int retval = gsd_flush(handle);
+        if (retval != GSD_SUCCESS)
+            {
+            return retval;
+            }
+        }
 
     size_t size = chunk->N * chunk->M * gsd_sizeof_type((enum gsd_type)chunk->type);
     if (size == 0)
         {
         return GSD_ERROR_FILE_CORRUPT;
         }
     if (chunk->location == 0)
@@ -2267,14 +2341,22 @@
         {
         return NULL;
         }
     if (handle->file_names.n_names == 0)
         {
         return NULL;
         }
+    if (handle->open_flags != GSD_OPEN_READONLY)
+        {
+        int retval = gsd_flush(handle);
+        if (retval != GSD_SUCCESS)
+            {
+            return NULL;
+            }
+        }
 
     // return nothing found if the name buffer is corrupt
     if (handle->file_names.data.data[handle->file_names.data.reserved - 1] != 0)
         {
         return NULL;
         }
 
@@ -2484,14 +2566,56 @@
             return retval;
             }
         }
 
     return GSD_SUCCESS;
     }
 
+uint64_t gsd_get_maximum_write_buffer_size(struct gsd_handle* handle)
+    {
+    if (handle == NULL)
+        {
+        return 0;
+        }
+    return handle->maximum_write_buffer_size;
+    }
+
+int gsd_set_maximum_write_buffer_size(struct gsd_handle* handle, uint64_t size)
+    {
+    if (handle == NULL || size == 0)
+        {
+        return GSD_ERROR_INVALID_ARGUMENT;
+        }
+
+    handle->maximum_write_buffer_size = size;
+
+    return GSD_SUCCESS;
+    }
+
+uint64_t gsd_get_index_entries_to_buffer(struct gsd_handle* handle)
+    {
+    if (handle == NULL)
+        {
+        return 0;
+        }
+    return handle->index_entries_to_buffer;
+    }
+
+int gsd_set_index_entries_to_buffer(struct gsd_handle* handle, uint64_t number)
+    {
+    if (handle == NULL || number == 0)
+        {
+        return GSD_ERROR_INVALID_ARGUMENT;
+        }
+
+    handle->index_entries_to_buffer = number;
+
+    return GSD_SUCCESS;
+    }
+
 // undefine windows wrapper macros
 #ifdef _WIN32
 #undef lseek
 #undef write
 #undef read
 #undef open
 #undef ftruncate
```

### Comparing `gsd-2.9.0/gsd/gsd.h` & `gsd-3.0.0/gsd/gsd.h`

 * *Files 12% similar despite different names*

```diff
@@ -310,26 +310,35 @@
         int64_t file_size;
 
         /// Flags passed to gsd_open() when opening this handle
         enum gsd_open_flag open_flags;
 
         /// Access the names in the namelist
         struct gsd_name_id_map name_map;
+
+        /// Number of index entries pending in the current frame.
+        uint64_t pending_index_entries;
+
+        /// Maximum write buffer size (bytes).
+        uint64_t maximum_write_buffer_size;
+
+        /// Number of index entries to buffer before flushing.
+        uint64_t index_entries_to_buffer;
         };
 
-    /** Specify a version
+    /** Specify a version.
 
         @param major major version
         @param minor minor version
 
         @return a packed version number aaaa.bbbb suitable for storing in a gsd file version entry.
     */
     uint32_t gsd_make_version(unsigned int major, unsigned int minor);
 
-    /** Create a GSD file
+    /** Create a GSD file.
 
         @param fname File name (UTF-8 encoded).
         @param application Generating application name (truncated to 63 chars).
         @param schema Schema name for data to be written in this GSD file (truncated to 63 chars).
         @param schema_version Version of the scheme data to be written (make with
         gsd_make_version()).
 
@@ -343,15 +352,15 @@
           - GSD_ERROR_IO: IO error (check errno).
     */
     int gsd_create(const char* fname,
                    const char* application,
                    const char* schema,
                    uint32_t schema_version);
 
-    /** Create and open a GSD file
+    /** Create and open a GSD file.
 
         @param handle Handle to open.
         @param fname File name (UTF-8 encoded).
         @param application Generating application name (truncated to 63 chars).
         @param schema Schema name for data to be written in this GSD file (truncated to 63 chars).
         @param schema_version Version of the scheme data to be written (make with
             gsd_make_version()).
@@ -377,15 +386,15 @@
                             const char* fname,
                             const char* application,
                             const char* schema,
                             uint32_t schema_version,
                             enum gsd_open_flag flags,
                             int exclusive_create);
 
-    /** Open a GSD file
+    /** Open a GSD file.
 
         @param handle Handle to open.
         @param fname File name to open (UTF-8 encoded).
         @param flags Either GSD_OPEN_READWRITE, GSD_OPEN_READONLY, or GSD_OPEN_APPEND.
 
         @pre The file name *fname* is a GSD file.
 
@@ -399,15 +408,15 @@
           - GSD_ERROR_NOT_A_GSD_FILE: Not a GSD file.
           - GSD_ERROR_INVALID_GSD_FILE_VERSION: Invalid GSD file version.
           - GSD_ERROR_FILE_CORRUPT: Corrupt file.
           - GSD_ERROR_MEMORY_ALLOCATION_FAILED: Unable to allocate memory.
     */
     int gsd_open(struct gsd_handle* handle, const char* fname, enum gsd_open_flag flags);
 
-    /** Truncate a GSD file
+    /** Truncate a GSD file.
 
         @param handle Open GSD file to truncate.
 
         After truncating, a file will have no frames and no data chunks. The file size will be that
         of a newly created gsd file. The application, schema, and schema version metadata will be
         kept. Truncate does not close and reopen the file, so it is suitable for writing restart
         files on Lustre file systems without any metadata access.
@@ -418,68 +427,89 @@
           - GSD_ERROR_NOT_A_GSD_FILE: Not a GSD file.
           - GSD_ERROR_INVALID_GSD_FILE_VERSION: Invalid GSD file version.
           - GSD_ERROR_FILE_CORRUPT: Corrupt file.
           - GSD_ERROR_MEMORY_ALLOCATION_FAILED: Unable to allocate memory.
     */
     int gsd_truncate(struct gsd_handle* handle);
 
-    /** Close a GSD file
+    /** Close a GSD file.
 
         @param handle GSD file to close.
 
         @pre *handle* was opened by gsd_open().
-        @pre gsd_end_frame() has been called since the last call to gsd_write_chunk().
 
+        @post Writable files: All data and index entries buffered before the previous call to
+              gsd_end_frame() is written to the file (see gsd_flush()).
         @post The file is closed.
         @post *handle* is freed and can no longer be used.
 
-        @warning Ensure that all gsd_write_chunk() calls are committed with gsd_end_frame() before
+        @warning Ensure that all gsd_write_chunk() calls are completed with gsd_end_frame() before
         closing the file.
 
         @return
           - GSD_SUCCESS (0) on success. Negative value on failure:
           - GSD_ERROR_IO: IO error (check errno).
           - GSD_ERROR_INVALID_ARGUMENT: *handle* is NULL.
     */
     int gsd_close(struct gsd_handle* handle);
 
-    /** Commit the current frame and increment the frame counter.
+    /** Complete the current frame.
 
         @param handle Handle to an open GSD file
 
         @pre *handle* was opened by gsd_open().
-        @pre gsd_write_chunk() has been called at least once since the last call to gsd_end_frame().
 
-        @post The current frame counter is increased by 1 and cached indexes are written to disk.
+        @post The current frame counter is increased by 1.
+        @post Flush the write buffer if it has overflowed. See gsd_flush().
 
         @return
           - GSD_SUCCESS (0) on success. Negative value on failure:
           - GSD_ERROR_IO: IO error (check errno).
           - GSD_ERROR_INVALID_ARGUMENT: *handle* is NULL.
           - GSD_ERROR_FILE_MUST_BE_WRITABLE: The file was opened read-only.
           - GSD_ERROR_MEMORY_ALLOCATION_FAILED: Unable to allocate memory.
     */
     int gsd_end_frame(struct gsd_handle* handle);
 
-    /** Write a data chunk to the current frame
+    /** Flush the write buffer.
+
+        @param handle Handle to an open GSD file
+
+        @pre *handle* was opened by gsd_open().
+
+        @post All data buffered by gsd_write_chunk() are present in the file.
+        @post All index entries buffered by gsd_write_chunk() prior to the last call to
+              gsd_end_frame() are present in the file.
+
+        @return
+          - GSD_SUCCESS (0) on success. Negative value on failure:
+          - GSD_ERROR_IO: IO error (check errno).
+          - GSD_ERROR_INVALID_ARGUMENT: *handle* is NULL.
+          - GSD_ERROR_FILE_MUST_BE_WRITABLE: The file was opened read-only.
+          - GSD_ERROR_MEMORY_ALLOCATION_FAILED: Unable to allocate memory.
+    */
+    int gsd_flush(struct gsd_handle* handle);
+
+    /** Add a data chunk to the current frame.
 
         @param handle Handle to an open GSD file.
         @param name Name of the data chunk.
         @param type type ID that identifies the type of data in *data*.
         @param N Number of rows in the data.
         @param M Number of columns in the data.
         @param flags set to 0, non-zero values reserved for future use.
         @param data Data buffer.
 
         @pre *handle* was opened by gsd_open().
         @pre *name* is a unique name for data chunks in the given frame.
         @pre data is allocated and contains at least `N * M * gsd_sizeof_type(type)` bytes.
 
-        @post The given data chunk is written to the end of the file and its location is updated in
-        the in-memory index.
+        @post When there is space in the buffer: The given data is present in the write buffer.
+              Otherwise, the data is present at the end of the file.
+        @post The index is present in the buffer.
 
         @note If the GSD file is version 1.0, the chunk name is truncated to 63 bytes. GSD version
         2.0 files support arbitrarily long names.
 
         @note *N* == 0 is allowed. When *N* is 0, *data* may be NULL.
 
         @return
@@ -495,31 +525,33 @@
                         const char* name,
                         enum gsd_type type,
                         uint64_t N,
                         uint32_t M,
                         uint8_t flags,
                         const void* data);
 
-    /** Find a chunk in the GSD file
+    /** Find a chunk in the GSD file.
 
         @param handle Handle to an open GSD file
         @param frame Frame to look for chunk
         @param name Name of the chunk to find
 
         @pre *handle* was opened by gsd_open() in read or readwrite mode.
 
         The found entry contains size and type metadata and can be passed to gsd_read_chunk() to
         read the data.
 
         @return A pointer to the found chunk, or NULL if not found.
+
+        @note gsd_find_chunk() calls gsd_flush() when the file is writable.
     */
     const struct gsd_index_entry*
     gsd_find_chunk(struct gsd_handle* handle, uint64_t frame, const char* name);
 
-    /** Read a chunk from the GSD file
+    /** Read a chunk from the GSD file.
 
         @param handle Handle to an open GSD file.
         @param data Data buffer to read into.
         @param chunk Chunk to read.
 
         @pre *handle* was opened in read or readwrite mode.
         @pre *chunk* was found by gsd_find_chunk().
@@ -528,18 +560,20 @@
 
         @return
           - GSD_SUCCESS (0) on success. Negative value on failure:
           - GSD_ERROR_IO: IO error (check errno).
           - GSD_ERROR_INVALID_ARGUMENT: *handle* is NULL, *data* is NULL, or *chunk* is NULL.
           - GSD_ERROR_FILE_MUST_BE_READABLE: The file was opened in append mode.
           - GSD_ERROR_FILE_CORRUPT: The GSD file is corrupt.
+
+        @note gsd_read_chunk() calls gsd_flush() when the file is writable.
     */
     int gsd_read_chunk(struct gsd_handle* handle, void* data, const struct gsd_index_entry* chunk);
 
-    /** Get the number of frames in the GSD file
+    /** Get the number of frames in the GSD file.
 
         @param handle Handle to an open GSD file
 
         @pre *handle* was opened by gsd_open().
 
         @return The number of frames in the file, or 0 on error.
     */
@@ -564,14 +598,16 @@
 
         To find the first matching chunk name, pass NULL for prev. Pass in the previous found string
         to find the next after that, and so on. Chunk names match if they begin with the string in
         *match*. Chunk names returned by this function may be present in at least one frame.
 
         @return Pointer to a string, NULL if no more matching chunks are found found, or NULL if
         *prev* is invalid
+
+        @note  gsd_find_matching_chunk_name() calls gsd_flush() when the file is writable.
     */
     const char*
     gsd_find_matching_chunk_name(struct gsd_handle* handle, const char* match, const char* prev);
 
     /** Upgrade a GSD file to the latest specification.
 
         @param handle Handle to an open GSD file
@@ -583,12 +619,65 @@
           - GSD_SUCCESS (0) on success. Negative value on failure:
           - GSD_ERROR_IO: IO error (check errno).
           - GSD_ERROR_INVALID_ARGUMENT: *handle* is NULL
           - GSD_ERROR_FILE_MUST_BE_WRITABLE: The file was opened in read-only mode.
     */
     int gsd_upgrade(struct gsd_handle* handle);
 
+    /** Get the maximum write buffer size.
+
+        @param handle Handle to an open GSD file
+
+        @pre *handle* was opened by gsd_open().
+
+        @return The maximum write buffer size in bytes, or 0 on error.
+    */
+    uint64_t gsd_get_maximum_write_buffer_size(struct gsd_handle* handle);
+
+    /** Set the maximum write buffer size.
+
+        @param handle Handle to an open GSD file
+        @param size Maximum number of bytes to allocate in the write buffer (must be greater than
+        0).
+
+        @pre *handle* was opened by gsd_open().
+
+        @return
+          - GSD_SUCCESS (0) on success. Negative value on failure:
+          - GSD_ERROR_INVALID_ARGUMENT: *handle* is NULL
+          - GSD_ERROR_INVALID_ARGUMENT: size == 0
+    */
+    int gsd_set_maximum_write_buffer_size(struct gsd_handle* handle, uint64_t size);
+
+    /** Get the number of index entries to buffer.
+
+        @param handle Handle to an open GSD file
+
+        @pre *handle* was opened by gsd_open().
+
+        @return The number of index entries to buffer, or 0 on error.
+    */
+    uint64_t gsd_get_index_entries_to_buffer(struct gsd_handle* handle);
+
+    /** Set the number of index entries to buffer.
+
+        @param handle Handle to an open GSD file
+        @param number Number of index entries to buffer before automatically flushing in
+        `gsd_end_frame()` (must be greater than 0).
+
+        @pre *handle* was opened by gsd_open().
+
+        @note GSD may allocate more than this number of entries in the buffer, as needed to store
+        all index entries for the already buffered frames and the current frame.
+
+        @return
+          - GSD_SUCCESS (0) on success. Negative value on failure:
+          - GSD_ERROR_INVALID_ARGUMENT: *handle* is NULL
+          - GSD_ERROR_INVALID_ARGUMENT: number == 0
+    */
+    int gsd_set_index_entries_to_buffer(struct gsd_handle* handle, uint64_t number);
+
 #ifdef __cplusplus
     }
 #endif
 
 #endif // #ifndef GSD_H
```

### Comparing `gsd-2.9.0/gsd/hoomd.py` & `gsd-3.0.0/gsd/hoomd.py`

 * *Files 6% similar despite different names*

```diff
@@ -403,26 +403,41 @@
                                                  dtype=numpy.float32)
             self.value = self.value.reshape([self.N])
         if self.group is not None:
             self.group = numpy.ascontiguousarray(self.group, dtype=numpy.int32)
             self.group = self.group.reshape([self.N, self.M])
 
 
-class Snapshot(object):
+class Frame:
     """System state at one point in time.
 
-    .. deprecated:: 2.8.0
+    Attributes:
+        configuration (`ConfigurationData`): Configuration data.
+
+        particles (`ParticleData`): Particles.
+
+        bonds (`BondData`): Bonds.
+
+        angles (`BondData`): Angles.
+
+        dihedrals (`BondData`): Dihedrals.
+
+        impropers (`BondData`): Impropers.
+
+        pairs (`BondData`): Special pair.
 
-        Replaced by `Frame`.
+        constraints (`ConstraintData`): Distance constraints.
+
+        state (dict): State data.
+
+        log (dict): Logged data (values must be `numpy.ndarray` or
+            `array_like`)
     """
 
     def __init__(self):
-        if not isinstance(self, Frame):
-            warnings.warn("Snapshot is deprecated, use Frame", FutureWarning)
-
         self.configuration = ConfigurationData()
         self.particles = ParticleData()
         self.bonds = BondData(2)
         self.angles = BondData(3)
         self.dihedrals = BondData(4)
         self.impropers = BondData(4)
         self.constraints = ConstraintData()
@@ -613,44 +628,14 @@
                     'hpmc/simple_polygon/vertices'].reshape([sumN, 2])
 
         for k in self.state:
             if k not in self._valid_state:
                 raise RuntimeError('Not a valid state: ' + k)
 
 
-class Frame(Snapshot):
-    """System state at one point in time.
-
-    Attributes:
-        configuration (`ConfigurationData`): Configuration data.
-
-        particles (`ParticleData`): Particles.
-
-        bonds (`BondData`): Bonds.
-
-        angles (`BondData`): Angles.
-
-        dihedrals (`BondData`): Dihedrals.
-
-        impropers (`BondData`): Impropers.
-
-        pairs (`BondData`): Special pair.
-
-        constraints (`ConstraintData`): Distance constraints.
-
-        state (dict): State data.
-
-        log (dict): Logged data (values must be `numpy.ndarray` or
-            `array_like`)
-    """
-
-    def __init__(self):
-        super().__init__()
-
-
 class _HOOMDTrajectoryIterable(object):
     """Iterable over a HOOMDTrajectory object."""
 
     def __init__(self, trajectory, indices):
         self._trajectory = trajectory
         self._indices = indices
         self._indices_iterator = iter(indices)
@@ -854,35 +839,28 @@
             iterable: An iterable object the provides :py:class:`Frame`
                 instances. This could be another HOOMDTrajectory, a generator
                 that modifies frames, or a list of frames.
         """
         for item in iterable:
             self.append(item)
 
-    def read_frame(self, idx):
+    def _read_frame(self, idx):
         """Read the frame at the given index from the file.
 
         Args:
             idx (int): Frame index to read.
 
         Returns:
             `Frame` with the frame data
 
         Replace any data chunks not present in the given frame with either data
         from frame 0, or initialize from default values if not in frame 0. Cache
         frame 0 data to avoid file read overhead. Return any default data as
         non-writable numpy arrays.
-
-        .. deprecated:: v2.5
         """
-        warnings.warn("Deprecated, trajectory[idx]", FutureWarning)
-        return self._read_frame(idx)
-
-    def _read_frame(self, idx):
-        """Implements read_frame."""
         if idx >= len(self):
             raise IndexError
 
         logger.debug('reading frame ' + str(idx) + ' from: ' + str(self.file))
 
         if self._initial_frame is None and idx != 0:
             self._read_frame(0)
@@ -1091,44 +1069,23 @@
     |                  | Raise :py:exc:`FileExistsError`             |
     |                  | if it already exists.                       |
     +------------------+---------------------------------------------+
     | ``'a'``          | Open a file for reading and writing.        |
     |                  | Creates the file if it doesn't exist.       |
     +------------------+---------------------------------------------+
 
-    .. deprecated:: 2.9.0
-
-        The following values to ``mode`` are deprecated:
-
-        +------------------+---------------------------------------------+
-        | mode             | description                                 |
-        +==================+=============================================+
-        | ``'rb'``         | Equivalent to ``'r'``                       |
-        +------------------+---------------------------------------------+
-        | ``'rb+'``        | Equivalent to ``'r+'``                      |
-        +------------------+---------------------------------------------+
-        | ``'wb'``         | Equivalent to ``'w'``                       |
-        +------------------+---------------------------------------------+
-        | ``'wb+'``        | Equivalent to ``'w'``                       |
-        +------------------+---------------------------------------------+
-        | ``'xb'``         | Equivalent to ``'x'``                       |
-        +------------------+---------------------------------------------+
-        | ``'xb+'``        | Equivalent to ``'x'``                       |
-        +------------------+---------------------------------------------+
-        | ``'ab'``         | Equivalent to ``'r+'``                      |
-        +------------------+---------------------------------------------+
     """
     if fl is None:
         raise RuntimeError("file layer module is not available")
     if gsd is None:
         raise RuntimeError("gsd module is not available")
 
     gsdfileobj = fl.open(name=str(name),
                          mode=mode,
-                         application='gsd.hoomd ' + gsd.__version__,
+                         application='gsd.hoomd ' + gsd.version.version,
                          schema='hoomd',
                          schema_version=[1, 4])
 
     return HOOMDTrajectory(gsdfileobj)
 
 
 def read_log(name, scalar_only=False):
@@ -1167,15 +1124,15 @@
     if fl is None:
         raise RuntimeError("file layer module is not available")
     if gsd is None:
         raise RuntimeError("gsd module is not available")
 
     with fl.open(name=str(name),
                  mode='r',
-                 application='gsd.hoomd ' + gsd.__version__,
+                 application='gsd.hoomd ' + gsd.version.version,
                  schema='hoomd',
                  schema_version=[1, 4]) as gsdfileobj:
 
         logged_data_names = gsdfileobj.find_matching_chunk_names('log/')
         # Always log timestep associated with each log entry
         logged_data_names.insert(0, 'configuration/step')
         if len(logged_data_names) == 1:
```

### Comparing `gsd-2.9.0/gsd/libgsd.pxd` & `gsd-3.0.0/gsd/libgsd.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,15 @@
                             const gsd_open_flag flags,
                             int exclusive_create)
     int gsd_open(gsd_handle* handle, const char *fname,
                  const gsd_open_flag flags)
     int gsd_truncate(gsd_handle* handle)
     int gsd_close(gsd_handle* handle)
     int gsd_end_frame(gsd_handle* handle)
+    int gsd_flush(gsd_handle* handle)
     int gsd_write_chunk(gsd_handle* handle,
                         const char *name,
                         gsd_type type,
                         uint64_t N,
                         uint8_t M,
                         uint8_t flags,
                         const void *data)
@@ -120,7 +121,11 @@
                        const gsd_index_entry* chunk)
     uint64_t gsd_get_nframes(gsd_handle* handle)
     size_t gsd_sizeof_type(gsd_type type)
     const char *gsd_find_matching_chunk_name(gsd_handle* handle,
                                              const char *match,
                                              const char *prev)
     int gsd_upgrade(gsd_handle *handle)
+    uint64_t gsd_get_maximum_write_buffer_size(gsd_handle* handle)
+    int gsd_set_maximum_write_buffer_size(gsd_handle* handle, uint64_t size)
+    uint64_t gsd_get_index_entries_to_buffer(gsd_handle* handle)
+    int gsd_set_index_entries_to_buffer(gsd_handle* handle, uint64_t number)
```

### Comparing `gsd-2.9.0/gsd/pygsd.py` & `gsd-3.0.0/gsd/pygsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from __future__ import division
 import logging
 import numpy
 import struct
 from collections import namedtuple
 import sys
 
-__version__ = "2.9.0"
+version = "3.0.0"
 
 logger = logging.getLogger('gsd.pygsd')
 
 gsd_header = namedtuple(
     'gsd_header',
     'magic index_location index_allocated_entries '
     'namelist_location namelist_allocated_entries '
```

### Comparing `gsd-2.9.0/gsd/pytest_plugin_validate.py` & `gsd-3.0.0/gsd/pytest_plugin_validate.py`

 * *Files identical despite different names*

### Comparing `gsd-2.9.0/gsd/test/conftest.py` & `gsd-3.0.0/gsd/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gsd-2.9.0/gsd/test/test_fl.py` & `gsd-3.0.0/gsd/test/test_fl.py`

 * *Files 2% similar despite different names*

```diff
@@ -954,7 +954,79 @@
             f.end_frame()
 
         for i in range(nframes):
             data1 = f.read_chunk(frame=i, name='data1')
             data10 = f.read_chunk(frame=i, name='data10')
             assert data1[0] == i
             assert data10[0] == i * 10
+
+
+@pytest.mark.parametrize('n_flush', [0, 1, 2])
+def test_flush(tmp_path, open_mode, n_flush):
+    """Test flush."""
+    data = numpy.array([1, 2, 3, 4, 5, 10012], dtype=numpy.int64)
+    with gsd.fl.open(name=tmp_path / 'test_flush.gsd',
+                     mode=open_mode.write,
+                     application='test_flush',
+                     schema='none',
+                     schema_version=[1, 2]) as f:
+        f.write_chunk(name='chunk1', data=data)
+        f.end_frame()
+        f.write_chunk(name='chunk2', data=data)
+        f.end_frame()
+        f.write_chunk(name='chunk3', data=data)
+
+        # Ensure that the data is buffered by opening the file with a 2nd
+        # handle read-only and checking it.
+        with gsd.fl.open(name=tmp_path / 'test_flush.gsd',
+                         mode='r') as f_readonly:
+            assert not f_readonly.chunk_exists(frame=0, name='chunk1')
+            assert not f_readonly.chunk_exists(frame=1, name='chunk2')
+            assert f_readonly.nframes == 0
+
+        # 0 calls to flush tests the implicit flush on close, 2 calls to flush
+        # tests that repeated calls are handled properly.
+        for i in range(n_flush):
+            f.flush()
+
+    with gsd.fl.open(name=tmp_path / 'test_flush.gsd',
+                     mode=open_mode.read) as f:
+        assert f.chunk_exists(frame=0, name='chunk1')
+        assert f.chunk_exists(frame=1, name='chunk2')
+
+        # The third chunk is not written because end_frame is not called a
+        # third time.
+
+        assert not f.chunk_exists(frame=2, name='chunk3')
+        assert f.nframes == 2
+
+
+def test_maximum_write_buffer_size(tmp_path, open_mode):
+    """Test maximum_write_buffer_size."""
+    with gsd.fl.open(name=tmp_path / 'test_maximum_write_buffer_size.gsd',
+                     mode=open_mode.write,
+                     application='test_maximum_write_buffer_size',
+                     schema='none',
+                     schema_version=[1, 2]) as f:
+
+        assert f.maximum_write_buffer_size > 0
+        f.maximum_write_buffer_size = 1024
+        assert f.maximum_write_buffer_size == 1024
+
+        with pytest.raises(RuntimeError):
+            f.maximum_write_buffer_size = 0
+
+
+def test_index_entries_to_buffer(tmp_path, open_mode):
+    """Test index_entries_to_buffer."""
+    with gsd.fl.open(name=tmp_path / 'test_index_entries_to_buffer.gsd',
+                     mode=open_mode.write,
+                     application='test_index_entries_to_buffer',
+                     schema='none',
+                     schema_version=[1, 2]) as f:
+
+        assert f.index_entries_to_buffer > 0
+        f.index_entries_to_buffer = 1024
+        assert f.index_entries_to_buffer == 1024
+
+        with pytest.raises(RuntimeError):
+            f.index_entries_to_buffer = 0
```

### Comparing `gsd-2.9.0/gsd/test/test_gsd_v1.gsd` & `gsd-3.0.0/gsd/test/test_gsd_v1.gsd`

 * *Files identical despite different names*

### Comparing `gsd-2.9.0/gsd/test/test_hoomd.py` & `gsd-3.0.0/gsd/test/test_hoomd.py`

 * *Files identical despite different names*

### Comparing `gsd-2.9.0/gsd/test/test_largefile.py` & `gsd-3.0.0/gsd/test/test_largefile.py`

 * *Files identical despite different names*

### Comparing `gsd-2.9.0/gsd.egg-info/PKG-INFO` & `gsd-3.0.0/gsd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 2.9.0
+Version: 3.0.0
 Summary: General simulation data file format.
 Author-email: "Joshua A. Anderson" <joaander@umich.edu>
 License: BSD-2-Clause
 Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v2.9.0/gsd-v2.9.0.tar.gz
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.0.0/gsd-3.0.0.tar.gz
 Project-URL: Source, https://github.com/glotzerlab/gsd
 Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
@@ -58,15 +58,15 @@
 ```python
 >>> def create_frame(i):
 ...     s = gsd.hoomd.Frame();
 ...     s.configuration.step = i;
 ...     s.particles.N = 4+i;
 ...     s.particles.position = numpy.random.random(size=(4+i,3))
 ...     return s;
->>> with gsd.hoomd.open('test.gsd', 'ab') as t:
+>>> with gsd.hoomd.open('test.gsd', 'a') as t:
 ...     t.extend( (create_frame(i) for i in range(10)) )
 ...     print(len(t))
 11
 ```
 
 Randomly index frames:
 ```python
```

### Comparing `gsd-2.9.0/gsd.egg-info/SOURCES.txt` & `gsd-3.0.0/gsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gsd-2.9.0/pyproject.toml` & `gsd-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 requires-python = ">=3.6"
 name = "gsd"
-version = "2.9.0"
+version = "3.0.0"
 description = "General simulation data file format."
 readme = "README.md"
 license = {text = "BSD-2-Clause"}
 authors = [
     {name = "Joshua A. Anderson", email = "joaander@umich.edu"},
 ]
 classifiers=[
@@ -21,15 +21,15 @@
 
 [project.scripts]
 gsd = "gsd.__main__:main"
 
 [project.urls]
 Homepage = "https://gsd.readthedocs.io"
 Documentation = "https://gsd.readthedocs.io"
-Download = "https://github.com/glotzerlab/gsd/releases/download/v2.9.0/gsd-v2.9.0.tar.gz"
+Download = "https://github.com/glotzerlab/gsd/releases/download/v3.0.0/gsd-3.0.0.tar.gz"
 Source = "https://github.com/glotzerlab/gsd"
 Issues = "https://github.com/glotzerlab/gsd/issues"
 
 [tool.setuptools]
 packages = ["gsd", "gsd.test"]
 
 [build-system]
```

### Comparing `gsd-2.9.0/setup.cfg` & `gsd-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gsd-2.9.0/setup.py` & `gsd-3.0.0/setup.py`

 * *Files identical despite different names*

