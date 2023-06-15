# Comparing `tmp/hveto-2.1.1.tar.gz` & `tmp/hveto-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hveto-2.1.1.tar", last modified: Tue Jun 13 21:56:20 2023, max compression
+gzip compressed data, was "hveto-2.1.2.tar", last modified: Thu Jun 15 23:31:21 2023, max compression
```

## Comparing `hveto-2.1.1.tar` & `hveto-2.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-13 21:56:20.236428 hveto-2.1.1/
--rw-r--r--   0 areeda     (501) staff       (20)    35147 2022-09-06 21:22:40.000000 hveto-2.1.1/LICENSE
--rw-r--r--   0 areeda     (501) staff       (20)       64 2022-09-06 21:22:40.000000 hveto-2.1.1/MANIFEST.in
--rw-r--r--   0 areeda     (501) staff       (20)     3623 2023-06-13 21:56:20.236552 hveto-2.1.1/PKG-INFO
--rw-r--r--   0 areeda     (501) staff       (20)     2361 2022-09-06 21:22:40.000000 hveto-2.1.1/README.rst
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-13 21:56:20.237454 hveto-2.1.1/hveto/
--rw-r--r--   0 areeda     (501) staff       (20)      971 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)    36486 2023-06-13 21:50:49.000000 hveto-2.1.1/hveto/__main__.py
--rw-r--r--   0 areeda     (501) staff       (20)      471 2023-06-13 21:56:20.237509 hveto-2.1.1/hveto/_version.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-13 21:56:20.229650 hveto-2.1.1/hveto/cli/
--rw-r--r--   0 areeda     (501) staff       (20)      896 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/cli/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)    14377 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/cli/cache_events.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-13 21:56:20.231268 hveto-2.1.1/hveto/cli/tests/
--rw-r--r--   0 areeda     (501) staff       (20)      811 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/cli/tests/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)     3063 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/cli/tests/test_trace.py
--rw-r--r--   0 areeda     (501) staff       (20)     3976 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/cli/trace.py
--rw-r--r--   0 areeda     (501) staff       (20)    11142 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/config.py
--rw-r--r--   0 areeda     (501) staff       (20)     1698 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/const.py
--rw-r--r--   0 areeda     (501) staff       (20)    10767 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/core.py
--rw-r--r--   0 areeda     (501) staff       (20)    14792 2023-06-13 21:50:49.000000 hveto-2.1.1/hveto/html.py
--rw-r--r--   0 areeda     (501) staff       (20)    18808 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/plot.py
--rw-r--r--   0 areeda     (501) staff       (20)     2681 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/segments.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-13 21:56:20.236009 hveto-2.1.1/hveto/tests/
--rw-r--r--   0 areeda     (501) staff       (20)      749 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/tests/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)     1266 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/tests/test_core.py
--rw-r--r--   0 areeda     (501) staff       (20)     3861 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/tests/test_html.py
--rw-r--r--   0 areeda     (501) staff       (20)     1731 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/tests/test_plot.py
--rw-r--r--   0 areeda     (501) staff       (20)     2710 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/tests/test_segments.py
--rw-r--r--   0 areeda     (501) staff       (20)     1896 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/tests/test_triggers.py
--rw-r--r--   0 areeda     (501) staff       (20)     2149 2022-09-06 21:22:40.000000 hveto-2.1.1/hveto/tests/test_utils.py
--rw-r--r--   0 areeda     (501) staff       (20)    11255 2023-06-13 21:50:49.000000 hveto-2.1.1/hveto/triggers.py
--rw-r--r--   0 areeda     (501) staff       (20)     4878 2023-06-13 21:50:49.000000 hveto-2.1.1/hveto/utils.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-13 21:56:20.226812 hveto-2.1.1/hveto.egg-info/
--rw-r--r--   0 areeda     (501) staff       (20)     3623 2023-06-13 21:56:20.000000 hveto-2.1.1/hveto.egg-info/PKG-INFO
--rw-r--r--   0 areeda     (501) staff       (20)      753 2023-06-13 21:56:20.000000 hveto-2.1.1/hveto.egg-info/SOURCES.txt
--rw-r--r--   0 areeda     (501) staff       (20)        1 2023-06-13 21:56:20.000000 hveto-2.1.1/hveto.egg-info/dependency_links.txt
--rw-r--r--   0 areeda     (501) staff       (20)      130 2023-06-13 21:56:20.000000 hveto-2.1.1/hveto.egg-info/entry_points.txt
--rw-r--r--   0 areeda     (501) staff       (20)        1 2022-09-06 21:34:21.000000 hveto-2.1.1/hveto.egg-info/not-zip-safe
--rw-r--r--   0 areeda     (501) staff       (20)      205 2023-06-13 21:56:20.000000 hveto-2.1.1/hveto.egg-info/requires.txt
--rw-r--r--   0 areeda     (501) staff       (20)        6 2023-06-13 21:56:20.000000 hveto-2.1.1/hveto.egg-info/top_level.txt
--rw-r--r--   0 areeda     (501) staff       (20)     2107 2023-06-13 21:56:20.237142 hveto-2.1.1/setup.cfg
--rw-r--r--   0 areeda     (501) staff       (20)     1184 2022-09-06 21:22:40.000000 hveto-2.1.1/setup.py
--rw-r--r--   0 areeda     (501) staff       (20)    65747 2022-09-06 21:22:40.000000 hveto-2.1.1/versioneer.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-15 23:31:21.839918 hveto-2.1.2/
+-rw-r--r--   0 areeda     (501) staff       (20)    35147 2022-09-06 21:22:40.000000 hveto-2.1.2/LICENSE
+-rw-r--r--   0 areeda     (501) staff       (20)       64 2022-09-06 21:22:40.000000 hveto-2.1.2/MANIFEST.in
+-rw-r--r--   0 areeda     (501) staff       (20)     3623 2023-06-15 23:31:21.840035 hveto-2.1.2/PKG-INFO
+-rw-r--r--   0 areeda     (501) staff       (20)     2361 2022-09-06 21:22:40.000000 hveto-2.1.2/README.rst
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-15 23:31:21.859412 hveto-2.1.2/hveto/
+-rw-r--r--   0 areeda     (501) staff       (20)      971 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)    36486 2023-06-13 21:50:49.000000 hveto-2.1.2/hveto/__main__.py
+-rw-r--r--   0 areeda     (501) staff       (20)      471 2023-06-15 23:31:21.859482 hveto-2.1.2/hveto/_version.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-15 23:31:21.835550 hveto-2.1.2/hveto/cli/
+-rw-r--r--   0 areeda     (501) staff       (20)      896 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/cli/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)    14377 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/cli/cache_events.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-15 23:31:21.836461 hveto-2.1.2/hveto/cli/tests/
+-rw-r--r--   0 areeda     (501) staff       (20)      811 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/cli/tests/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3063 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/cli/tests/test_trace.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3976 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/cli/trace.py
+-rw-r--r--   0 areeda     (501) staff       (20)    11142 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/config.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1698 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/const.py
+-rw-r--r--   0 areeda     (501) staff       (20)    10767 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/core.py
+-rw-r--r--   0 areeda     (501) staff       (20)    14792 2023-06-13 21:50:49.000000 hveto-2.1.2/hveto/html.py
+-rw-r--r--   0 areeda     (501) staff       (20)    18808 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/plot.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2681 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/segments.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-15 23:31:21.839507 hveto-2.1.2/hveto/tests/
+-rw-r--r--   0 areeda     (501) staff       (20)      749 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/tests/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1266 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/tests/test_core.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3861 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/tests/test_html.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1731 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/tests/test_plot.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2710 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/tests/test_segments.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1896 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/tests/test_triggers.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2149 2022-09-06 21:22:40.000000 hveto-2.1.2/hveto/tests/test_utils.py
+-rw-r--r--   0 areeda     (501) staff       (20)    11255 2023-06-13 21:50:49.000000 hveto-2.1.2/hveto/triggers.py
+-rw-r--r--   0 areeda     (501) staff       (20)     4878 2023-06-13 21:50:49.000000 hveto-2.1.2/hveto/utils.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-15 23:31:21.834349 hveto-2.1.2/hveto.egg-info/
+-rw-r--r--   0 areeda     (501) staff       (20)     3623 2023-06-15 23:31:21.000000 hveto-2.1.2/hveto.egg-info/PKG-INFO
+-rw-r--r--   0 areeda     (501) staff       (20)      753 2023-06-15 23:31:21.000000 hveto-2.1.2/hveto.egg-info/SOURCES.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        1 2023-06-15 23:31:21.000000 hveto-2.1.2/hveto.egg-info/dependency_links.txt
+-rw-r--r--   0 areeda     (501) staff       (20)      130 2023-06-15 23:31:21.000000 hveto-2.1.2/hveto.egg-info/entry_points.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        1 2022-09-06 21:34:21.000000 hveto-2.1.2/hveto.egg-info/not-zip-safe
+-rw-r--r--   0 areeda     (501) staff       (20)      205 2023-06-15 23:31:21.000000 hveto-2.1.2/hveto.egg-info/requires.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        6 2023-06-15 23:31:21.000000 hveto-2.1.2/hveto.egg-info/top_level.txt
+-rw-r--r--   0 areeda     (501) staff       (20)     2107 2023-06-15 23:31:21.859026 hveto-2.1.2/setup.cfg
+-rw-r--r--   0 areeda     (501) staff       (20)     1184 2022-09-06 21:22:40.000000 hveto-2.1.2/setup.py
+-rw-r--r--   0 areeda     (501) staff       (20)    65747 2022-09-06 21:22:40.000000 hveto-2.1.2/versioneer.py
```

### Comparing `hveto-2.1.1/LICENSE` & `hveto-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/PKG-INFO` & `hveto-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hveto
-Version: 2.1.1
+Version: 2.1.2
 Summary: A python implementation of the HierarchicalVeto (hveto) algorithm.
 Home-page: https://github.com/gwdetchar/hveto/
 Author: Joshua Smith
 Author-email: joshua.smith@ligo.org
 License: GPL-3.0-or-later
 Keywords: physics,astronomy,gravitational-waves,ligo
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hveto-2.1.1/README.rst` & `hveto-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/__init__.py` & `hveto-2.1.2/hveto/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/__main__.py` & `hveto-2.1.2/hveto/__main__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/cli/__init__.py` & `hveto-2.1.2/hveto/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/cli/cache_events.py` & `hveto-2.1.2/hveto/cli/cache_events.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/cli/tests/__init__.py` & `hveto-2.1.2/hveto/cli/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/cli/tests/test_trace.py` & `hveto-2.1.2/hveto/cli/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/cli/trace.py` & `hveto-2.1.2/hveto/cli/trace.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/config.py` & `hveto-2.1.2/hveto/config.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/const.py` & `hveto-2.1.2/hveto/const.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/core.py` & `hveto-2.1.2/hveto/core.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/html.py` & `hveto-2.1.2/hveto/html.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/plot.py` & `hveto-2.1.2/hveto/plot.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/segments.py` & `hveto-2.1.2/hveto/segments.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/tests/__init__.py` & `hveto-2.1.2/hveto/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/tests/test_core.py` & `hveto-2.1.2/hveto/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/tests/test_html.py` & `hveto-2.1.2/hveto/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/tests/test_plot.py` & `hveto-2.1.2/hveto/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/tests/test_segments.py` & `hveto-2.1.2/hveto/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/tests/test_triggers.py` & `hveto-2.1.2/hveto/tests/test_triggers.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/tests/test_utils.py` & `hveto-2.1.2/hveto/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/triggers.py` & `hveto-2.1.2/hveto/triggers.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto/utils.py` & `hveto-2.1.2/hveto/utils.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/hveto.egg-info/PKG-INFO` & `hveto-2.1.2/hveto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hveto
-Version: 2.1.1
+Version: 2.1.2
 Summary: A python implementation of the HierarchicalVeto (hveto) algorithm.
 Home-page: https://github.com/gwdetchar/hveto/
 Author: Joshua Smith
 Author-email: joshua.smith@ligo.org
 License: GPL-3.0-or-later
 Keywords: physics,astronomy,gravitational-waves,ligo
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hveto-2.1.1/hveto.egg-info/SOURCES.txt` & `hveto-2.1.2/hveto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/setup.cfg` & `hveto-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/setup.py` & `hveto-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.1/versioneer.py` & `hveto-2.1.2/versioneer.py`

 * *Files identical despite different names*

