# Comparing `tmp/pysmo-0.8.2.tar.gz` & `tmp/pysmo-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmo-0.8.2.tar", max compression
+gzip compressed data, was "pysmo-0.8.3.tar", max compression
```

## Comparing `pysmo-0.8.2.tar` & `pysmo-0.8.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35147 2022-05-19 23:31:41.963627 pysmo-0.8.2/LICENSE
--rw-r--r--   0        0        0     1587 2023-06-12 17:13:12.657529 pysmo-0.8.2/README.md
--rw-r--r--   0        0        0      990 2023-06-13 16:10:38.276560 pysmo-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      501 2023-06-12 17:13:13.238522 pysmo-0.8.2/pysmo/__init__.py
--rw-r--r--   0        0        0      380 2023-06-12 17:13:13.283522 pysmo-0.8.2/pysmo/core/__init__.py
--rw-r--r--   0        0        0      285 2023-06-12 17:13:13.327521 pysmo-0.8.2/pysmo/core/sac/__init__.py
--rw-r--r--   0        0        0     8500 2023-06-12 17:13:13.360521 pysmo-0.8.2/pysmo/core/sac/sacfunc.py
--rw-r--r--   0        0        0    10074 2023-06-13 16:07:20.048885 pysmo-0.8.2/pysmo/core/sac/sacheader.py
--rw-r--r--   0        0        0    18220 2023-06-12 17:13:13.428520 pysmo-0.8.2/pysmo/core/sac/sacheader.yml
--rw-r--r--   0        0        0    16547 2023-06-12 17:13:13.462520 pysmo-0.8.2/pysmo/core/sac/sacio.py
--rw-r--r--   0        0        0      113 2023-06-12 17:13:13.507519 pysmo-0.8.2/pysmo/tools/__init__.py
--rw-r--r--   0        0        0      417 2022-05-19 23:31:41.969627 pysmo-0.8.2/pysmo/tools/noise/__init__.py
--rw-r--r--   0        0        0     4122 2023-06-12 17:13:13.553519 pysmo-0.8.2/pysmo/tools/noise/peterson.py
--rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 pysmo-0.8.2/setup.py
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 pysmo-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-05-19 23:31:41.963627 pysmo-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1587 2023-06-16 15:42:23.000208 pysmo-0.8.3/README.md
+-rw-r--r--   0        0        0      990 2023-06-16 15:46:08.199543 pysmo-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-06-16 15:42:23.604201 pysmo-0.8.3/pysmo/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-16 15:42:23.671200 pysmo-0.8.3/pysmo/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-06-16 15:42:23.704200 pysmo-0.8.3/pysmo/core/sac/__init__.py
+-rw-r--r--   0        0        0     8500 2023-06-16 15:42:23.738200 pysmo-0.8.3/pysmo/core/sac/sacfunc.py
+-rw-r--r--   0        0        0    10302 2023-06-16 15:44:36.766625 pysmo-0.8.3/pysmo/core/sac/sacheader.py
+-rw-r--r--   0        0        0    18220 2023-06-16 15:42:23.838198 pysmo-0.8.3/pysmo/core/sac/sacheader.yml
+-rw-r--r--   0        0        0    16547 2023-06-16 15:42:23.872198 pysmo-0.8.3/pysmo/core/sac/sacio.py
+-rw-r--r--   0        0        0      113 2023-06-16 15:42:23.917197 pysmo-0.8.3/pysmo/tools/__init__.py
+-rw-r--r--   0        0        0      417 2022-05-19 23:31:41.969627 pysmo-0.8.3/pysmo/tools/noise/__init__.py
+-rw-r--r--   0        0        0     4122 2023-06-16 15:42:23.962197 pysmo-0.8.3/pysmo/tools/noise/peterson.py
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 pysmo-0.8.3/setup.py
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 pysmo-0.8.3/PKG-INFO
```

### Comparing `pysmo-0.8.2/LICENSE` & `pysmo-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.2/README.md` & `pysmo-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.2/pyproject.toml` & `pysmo-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysmo"
-version = "0.8.2"
+version = "0.8.3"
 description = "Python module to read/write/manipulate SAC (Seismic Analysis Code) files"
 readme = "README.md"
 authors = ["Simon M. Lloyd <simon@slloyd.net>"]
 license = "GPL-3.0-or-later"
 documentation = "https://pysmo.readthedocs.io"
 classifiers = [
     "Intended Audience :: Science/Research",
```

### Comparing `pysmo-0.8.2/pysmo/core/sac/sacfunc.py` & `pysmo-0.8.3/pysmo/core/sac/sacfunc.py`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.2/pysmo/core/sac/sacheader.py` & `pysmo-0.8.3/pysmo/core/sac/sacheader.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,18 @@
 
         # Save headers of type 'k' as a string. Also check length is not
         # exceeded. Strings are also padded with spaces to match the sac
         # header length.
         elif self.header_type == 'k':
             if isinstance(value, bool):
                 raise ValueError('Value for %s may not be a bool.' % self.name)
+            # fix for aimbat returning bytes instead of strings. Should really be
+            # fixed there, but I don't know what is causing it...
+            if isinstance(value, bytes):
+                value = value.decode()
             try:
                 value = str(value).rstrip()
             except ValueError:
                 raise ValueError('Unable to set %s to %s - must be of type\
                                  str.' % (self.name, value))
             if len(value) > self.length:
                 raise ValueError('%s is too long - maximum length is %s' %
```

### Comparing `pysmo-0.8.2/pysmo/core/sac/sacheader.yml` & `pysmo-0.8.3/pysmo/core/sac/sacheader.yml`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.2/pysmo/core/sac/sacio.py` & `pysmo-0.8.3/pysmo/core/sac/sacio.py`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.2/pysmo/tools/noise/peterson.py` & `pysmo-0.8.3/pysmo/tools/noise/peterson.py`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.2/setup.py` & `pysmo-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'numpy>=1.19.4,<2.0.0',
  'pyproj>=3.0.0,<4.0.0',
  'requests>=2.25.1,<3.0.0',
  'scipy>=1.5.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pysmo',
-    'version': '0.8.2',
+    'version': '0.8.3',
     'description': 'Python module to read/write/manipulate SAC (Seismic Analysis Code) files',
     'long_description': "\n![Test Status](https://github.com/pysmo/pysmo/actions/workflows/run-tests.yml/badge.svg)\n![Build Status](https://github.com/pysmo/pysmo/actions/workflows/build.yml/badge.svg)\n[![Documentation Status](https://readthedocs.org/projects/pysmo/badge/?version=latest)](https://pysmo.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/pysmo/pysmo/branch/master/graph/badge.svg?token=ZsHTBN4rxF)](https://codecov.io/gh/pysmo/pysmo)\n[![PyPI](https://img.shields.io/pypi/v/pysmo)](https://pypi.org/project/pysmo/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pysmo)\n\nPysmo\n=====\n\nPython package to read/write/manipulate SAC (Seismic Analysis Code) files.\n\n\nQuickstart\n----------\nTo install the stable version of pysmo run the following command in a terminal:\n\n```shell\n$ pip install pysmo\n```\n\nPre-release versions of pysmo can be installed by running:\n\n```shell\n$ pip install pysmo --pre\n```\n\nFinally, to install the current ``master`` branch directly from Github run:\n\n```shell\n$ pip install git+https://github.com/pysmo/pysmo\n```\n\nPysmo can then be used in a python script or the python shell directly:\n\n\n```python\n>>> from pysmo import SacIO\n>>> seismogram = SacIO.from_file('file.sac')\n>>> print(seismogram.delta)\n0.02500000037252903\n>>> print(seismogram.data)\n[-2.987490077543953e-08, -2.983458813332618e-08, ...\n>>> help(seismogram)\nHelp on SacIO in module pysmo.core.sac.sacio object:\n\n...\n```\nDocumentation\n-------------\n\nThe complete pysmo documentation is available at https://pysmo.readthedocs.io/\n\nContributors\n------------\n\n- Helio Tejedor\n",
     'author': 'Simon M. Lloyd',
     'author_email': 'simon@slloyd.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pysmo-0.8.2/PKG-INFO` & `pysmo-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmo
-Version: 0.8.2
+Version: 0.8.3
 Summary: Python module to read/write/manipulate SAC (Seismic Analysis Code) files
 License: GPL-3.0-or-later
 Author: Simon M. Lloyd
 Author-email: simon@slloyd.net
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

