# Comparing `tmp/jobmanager-0.4.1.tar.gz` & `tmp/jobmanager-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobmanager-0.4.1.tar", max compression
+gzip compressed data, was "jobmanager-0.4.2.tar", max compression
```

## Comparing `jobmanager-0.4.1.tar` & `jobmanager-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2016-09-27 20:39:36.170516 jobmanager-0.4.1/LICENSE
--rw-r--r--   0        0        0      702 2023-06-15 21:52:01.363989 jobmanager-0.4.1/README.md
--rw-r--r--   0        0        0      851 2016-09-29 18:55:19.118543 jobmanager-0.4.1/jobmanager/__init__.py
--rw-r--r--   0        0        0     6633 2023-06-15 21:32:12.814108 jobmanager-0.4.1/jobmanager/clients.py
--rw-r--r--   0        0        0    99780 2023-06-15 21:34:26.912639 jobmanager-0.4.1/jobmanager/jobmanager.py
--rw-r--r--   0        0        0    10228 2023-06-15 21:36:19.606765 jobmanager-0.4.1/jobmanager/ode_wrapper.py
--rw-r--r--   0        0        0     2049 2023-06-15 21:34:26.916639 jobmanager-0.4.1/jobmanager/servers.py
--rw-r--r--   0        0        0     3357 2021-11-01 21:25:44.466676 jobmanager-0.4.1/jobmanager/signalDelay.py
--rw-r--r--   0        0        0      928 2023-06-15 21:52:49.604874 jobmanager-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 jobmanager-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2016-09-27 20:39:36.170516 jobmanager-0.4.2/LICENSE
+-rw-r--r--   0        0        0      702 2023-06-15 21:52:01.363989 jobmanager-0.4.2/README.md
+-rw-r--r--   0        0        0      814 2023-06-15 21:55:26.991770 jobmanager-0.4.2/jobmanager/__init__.py
+-rw-r--r--   0        0        0     6633 2023-06-15 21:32:12.814108 jobmanager-0.4.2/jobmanager/clients.py
+-rw-r--r--   0        0        0    99780 2023-06-15 21:34:26.912639 jobmanager-0.4.2/jobmanager/jobmanager.py
+-rw-r--r--   0        0        0    10228 2023-06-15 21:36:19.606765 jobmanager-0.4.2/jobmanager/ode_wrapper.py
+-rw-r--r--   0        0        0     2049 2023-06-15 21:34:26.916639 jobmanager-0.4.2/jobmanager/servers.py
+-rw-r--r--   0        0        0     3357 2021-11-01 21:25:44.466676 jobmanager-0.4.2/jobmanager/signalDelay.py
+-rw-r--r--   0        0        0      928 2023-06-15 21:56:20.272753 jobmanager-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 jobmanager-0.4.2/PKG-INFO
```

### Comparing `jobmanager-0.4.1/LICENSE` & `jobmanager-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.1/README.md` & `jobmanager-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.1/jobmanager/__init__.py` & `jobmanager-0.4.2/jobmanager/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,12 @@
 
 Fork `jobmanager on GitHib <https://github.com/cimatosa/jobmanager/>`_.
 
 """
 
 import warnings
 
-from .jm_version import __version__
-
 from .jobmanager import *
 
 from . import clients
 from . import servers
 from . import ode_wrapper
```

### Comparing `jobmanager-0.4.1/jobmanager/clients.py` & `jobmanager-0.4.2/jobmanager/clients.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.1/jobmanager/jobmanager.py` & `jobmanager-0.4.2/jobmanager/jobmanager.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.1/jobmanager/ode_wrapper.py` & `jobmanager-0.4.2/jobmanager/ode_wrapper.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.1/jobmanager/servers.py` & `jobmanager-0.4.2/jobmanager/servers.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.1/jobmanager/signalDelay.py` & `jobmanager-0.4.2/jobmanager/signalDelay.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.1/pyproject.toml` & `jobmanager-0.4.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobmanager"
-version = "0.4.1"
+version = "0.4.2"
 description = "a facility for distributed computing"
 authors = ["Richard Hartmann", "Paul Müller"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cimatosa/jobmanager"
 repository = "https://github.com/cimatosa/jobmanager"
 keywords =[
```

### Comparing `jobmanager-0.4.1/PKG-INFO` & `jobmanager-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobmanager
-Version: 0.4.1
+Version: 0.4.2
 Summary: a facility for distributed computing
 Home-page: https://github.com/cimatosa/jobmanager
 License: MIT
 Keywords: multiprocessing,queue,parallel,distributed,computing,progress,manager,job,persistent data,scheduler
 Author: Richard Hartmann
 Requires-Python: >=3.6,<4.0
 Classifier: Intended Audience :: Science/Research
```

