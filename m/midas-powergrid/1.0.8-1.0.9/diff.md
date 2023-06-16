# Comparing `tmp/midas-powergrid-1.0.8.tar.gz` & `tmp/midas-powergrid-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-powergrid-1.0.8.tar", last modified: Tue Aug  9 11:12:41 2022, max compression
+gzip compressed data, was "midas-powergrid-1.0.9.tar", last modified: Thu Aug 11 10:40:03 2022, max compression
```

## Comparing `midas-powergrid-1.0.8.tar` & `midas-powergrid-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.266848 midas-powergrid-1.0.8/
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     7648 2022-03-31 13:27:18.000000 midas-powergrid-1.0.8/LICENSE
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3946 2022-08-09 11:12:41.266848 midas-powergrid-1.0.8/PKG-INFO
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     3009 2022-04-27 11:57:16.000000 midas-powergrid-1.0.8/README.md
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.260182 midas-powergrid-1.0.8/midas/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.260182 midas-powergrid-1.0.8/midas/modules/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.263515 midas-powergrid-1.0.8/midas/modules/powergrid/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 06:28:22.000000 midas-powergrid-1.0.8/midas/modules/powergrid/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.263515 midas-powergrid-1.0.8/midas/modules/powergrid/analysis/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-05-04 06:31:55.000000 midas-powergrid-1.0.8/midas/modules/powergrid/analysis/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5277 2022-05-04 06:31:55.000000 midas-powergrid-1.0.8/midas/modules/powergrid/analysis/bus.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5597 2022-05-04 06:31:55.000000 midas-powergrid-1.0.8/midas/modules/powergrid/analysis/grid.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3960 2022-06-21 08:34:45.000000 midas-powergrid-1.0.8/midas/modules/powergrid/analysis/power.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.263515 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-08 13:16:58.000000 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      679 2022-06-29 08:19:34.000000 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/base.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      512 2022-04-08 13:16:58.000000 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/line_loading.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      568 2022-04-08 13:16:58.000000 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/load_voltage_change.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      563 2022-04-08 13:16:58.000000 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/sgen_voltage_change.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1036 2022-04-08 13:16:58.000000 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/tap_changes.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1067 2022-06-29 08:19:34.000000 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/voltage_band.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1469 2022-06-29 08:19:34.000000 midas-powergrid-1.0.8/midas/modules/powergrid/constraints/voltage_change.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.263515 midas-powergrid-1.0.8/midas/modules/powergrid/custom/
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)        0 2022-03-31 13:27:18.000000 midas-powergrid-1.0.8/midas/modules/powergrid/custom/__init__.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)    83955 2022-03-31 13:27:18.000000 midas-powergrid-1.0.8/midas/modules/powergrid/custom/bhv.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     2050 2022-03-31 13:27:18.000000 midas-powergrid-1.0.8/midas/modules/powergrid/custom/midaslv.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2999 2022-06-29 08:19:34.000000 midas-powergrid-1.0.8/midas/modules/powergrid/custom/midasmv.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.263515 midas-powergrid-1.0.8/midas/modules/powergrid/elements/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-08 13:16:58.000000 midas-powergrid-1.0.8/midas/modules/powergrid/elements/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2094 2022-04-08 13:16:58.000000 midas-powergrid-1.0.8/midas/modules/powergrid/elements/base.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3305 2022-07-05 09:06:41.000000 midas-powergrid-1.0.8/midas/modules/powergrid/elements/bus.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1432 2022-07-05 09:10:05.000000 midas-powergrid-1.0.8/midas/modules/powergrid/elements/line.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1959 2022-07-05 09:10:05.000000 midas-powergrid-1.0.8/midas/modules/powergrid/elements/load.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1958 2022-07-05 09:10:05.000000 midas-powergrid-1.0.8/midas/modules/powergrid/elements/sgen.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      570 2022-04-08 13:16:58.000000 midas-powergrid-1.0.8/midas/modules/powergrid/elements/switch.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      758 2022-04-08 13:18:33.000000 midas-powergrid-1.0.8/midas/modules/powergrid/elements/transformer.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     5021 2022-04-08 13:11:59.000000 midas-powergrid-1.0.8/midas/modules/powergrid/meta.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.263515 midas-powergrid-1.0.8/midas/modules/powergrid/model/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2022-05-09 06:28:22.000000 midas-powergrid-1.0.8/midas/modules/powergrid/model/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3847 2022-06-29 08:19:34.000000 midas-powergrid-1.0.8/midas/modules/powergrid/model/constrainted.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    14257 2022-07-07 16:59:40.000000 midas-powergrid-1.0.8/midas/modules/powergrid/model/static.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    10192 2022-07-07 16:59:40.000000 midas-powergrid-1.0.8/midas/modules/powergrid/module.py
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     6575 2022-03-31 13:27:44.000000 midas-powergrid-1.0.8/midas/modules/powergrid/plotter.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    10410 2022-08-09 11:01:27.000000 midas-powergrid-1.0.8/midas/modules/powergrid/simulator.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-09 11:12:41.263515 midas-powergrid-1.0.8/midas_powergrid.egg-info/
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     3946 2022-08-09 11:12:41.000000 midas-powergrid-1.0.8/midas_powergrid.egg-info/PKG-INFO
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     1614 2022-08-09 11:12:41.000000 midas-powergrid-1.0.8/midas_powergrid.egg-info/SOURCES.txt
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)        1 2022-08-09 11:12:41.000000 midas-powergrid-1.0.8/midas_powergrid.egg-info/dependency_links.txt
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)      128 2022-08-09 11:12:41.000000 midas-powergrid-1.0.8/midas_powergrid.egg-info/requires.txt
--rwxrwxrwx   0 sbalduin  (1000) wheel      (998)        6 2022-08-09 11:12:41.000000 midas-powergrid-1.0.8/midas_powergrid.egg-info/top_level.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2022-08-09 11:12:41.266848 midas-powergrid-1.0.8/setup.cfg
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1835 2022-05-04 06:31:55.000000 midas-powergrid-1.0.8/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.856681 midas-powergrid-1.0.9/
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     7648 2022-03-31 13:27:18.000000 midas-powergrid-1.0.9/LICENSE
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3946 2022-08-11 10:40:03.856681 midas-powergrid-1.0.9/PKG-INFO
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     3009 2022-04-27 11:57:16.000000 midas-powergrid-1.0.9/README.md
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.850014 midas-powergrid-1.0.9/midas/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.850014 midas-powergrid-1.0.9/midas/modules/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.850014 midas-powergrid-1.0.9/midas/modules/powergrid/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-05-09 06:28:22.000000 midas-powergrid-1.0.9/midas/modules/powergrid/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.853347 midas-powergrid-1.0.9/midas/modules/powergrid/analysis/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-05-04 06:31:55.000000 midas-powergrid-1.0.9/midas/modules/powergrid/analysis/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     5277 2022-05-04 06:31:55.000000 midas-powergrid-1.0.9/midas/modules/powergrid/analysis/bus.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     5597 2022-05-04 06:31:55.000000 midas-powergrid-1.0.9/midas/modules/powergrid/analysis/grid.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3960 2022-06-21 08:34:45.000000 midas-powergrid-1.0.9/midas/modules/powergrid/analysis/power.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.853347 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-08 13:16:58.000000 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      679 2022-06-29 08:19:34.000000 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/base.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      512 2022-04-08 13:16:58.000000 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/line_loading.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      568 2022-04-08 13:16:58.000000 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/load_voltage_change.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      563 2022-04-08 13:16:58.000000 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/sgen_voltage_change.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1036 2022-04-08 13:16:58.000000 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/tap_changes.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1067 2022-06-29 08:19:34.000000 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/voltage_band.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1469 2022-06-29 08:19:34.000000 midas-powergrid-1.0.9/midas/modules/powergrid/constraints/voltage_change.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.853347 midas-powergrid-1.0.9/midas/modules/powergrid/custom/
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)        0 2022-03-31 13:27:18.000000 midas-powergrid-1.0.9/midas/modules/powergrid/custom/__init__.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)    83955 2022-03-31 13:27:18.000000 midas-powergrid-1.0.9/midas/modules/powergrid/custom/bhv.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     2050 2022-03-31 13:27:18.000000 midas-powergrid-1.0.9/midas/modules/powergrid/custom/midaslv.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2999 2022-06-29 08:19:34.000000 midas-powergrid-1.0.9/midas/modules/powergrid/custom/midasmv.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.856681 midas-powergrid-1.0.9/midas/modules/powergrid/elements/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-08 13:16:58.000000 midas-powergrid-1.0.9/midas/modules/powergrid/elements/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2094 2022-04-08 13:16:58.000000 midas-powergrid-1.0.9/midas/modules/powergrid/elements/base.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3305 2022-07-05 09:06:41.000000 midas-powergrid-1.0.9/midas/modules/powergrid/elements/bus.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1432 2022-07-05 09:10:05.000000 midas-powergrid-1.0.9/midas/modules/powergrid/elements/line.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1959 2022-07-05 09:10:05.000000 midas-powergrid-1.0.9/midas/modules/powergrid/elements/load.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1958 2022-07-05 09:10:05.000000 midas-powergrid-1.0.9/midas/modules/powergrid/elements/sgen.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      570 2022-04-08 13:16:58.000000 midas-powergrid-1.0.9/midas/modules/powergrid/elements/switch.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      758 2022-04-08 13:18:33.000000 midas-powergrid-1.0.9/midas/modules/powergrid/elements/transformer.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     5021 2022-04-08 13:11:59.000000 midas-powergrid-1.0.9/midas/modules/powergrid/meta.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.856681 midas-powergrid-1.0.9/midas/modules/powergrid/model/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2022-05-09 06:28:22.000000 midas-powergrid-1.0.9/midas/modules/powergrid/model/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3847 2022-06-29 08:19:34.000000 midas-powergrid-1.0.9/midas/modules/powergrid/model/constrainted.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    14399 2022-08-10 13:28:54.000000 midas-powergrid-1.0.9/midas/modules/powergrid/model/static.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    10192 2022-07-07 16:59:40.000000 midas-powergrid-1.0.9/midas/modules/powergrid/module.py
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     6575 2022-03-31 13:27:44.000000 midas-powergrid-1.0.9/midas/modules/powergrid/plotter.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    10359 2022-08-11 10:38:27.000000 midas-powergrid-1.0.9/midas/modules/powergrid/simulator.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-08-11 10:40:03.856681 midas-powergrid-1.0.9/midas_powergrid.egg-info/
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     3946 2022-08-11 10:40:03.000000 midas-powergrid-1.0.9/midas_powergrid.egg-info/PKG-INFO
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)     1614 2022-08-11 10:40:03.000000 midas-powergrid-1.0.9/midas_powergrid.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)        1 2022-08-11 10:40:03.000000 midas-powergrid-1.0.9/midas_powergrid.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)      128 2022-08-11 10:40:03.000000 midas-powergrid-1.0.9/midas_powergrid.egg-info/requires.txt
+-rwxrwxrwx   0 sbalduin  (1000) wheel      (998)        6 2022-08-11 10:40:03.000000 midas-powergrid-1.0.9/midas_powergrid.egg-info/top_level.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2022-08-11 10:40:03.856681 midas-powergrid-1.0.9/setup.cfg
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1835 2022-05-04 06:31:55.000000 midas-powergrid-1.0.9/setup.py
```

### Comparing `midas-powergrid-1.0.8/LICENSE` & `midas-powergrid-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/PKG-INFO` & `midas-powergrid-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-powergrid
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simulator for pandapower grids.
 Home-page: https://gitlab.com/midas-mosaik/midas-powergrid
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `midas-powergrid-1.0.8/README.md` & `midas-powergrid-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/analysis/bus.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/analysis/bus.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/analysis/grid.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/analysis/grid.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/analysis/power.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/analysis/power.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/constraints/base.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/constraints/base.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/constraints/line_loading.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/constraints/line_loading.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/constraints/load_voltage_change.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/constraints/load_voltage_change.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/constraints/sgen_voltage_change.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/constraints/sgen_voltage_change.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/constraints/tap_changes.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/constraints/tap_changes.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/constraints/voltage_band.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/constraints/voltage_band.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/constraints/voltage_change.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/constraints/voltage_change.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/custom/bhv.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/custom/bhv.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/custom/midaslv.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/custom/midaslv.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/custom/midasmv.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/custom/midasmv.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/elements/base.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/elements/base.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/elements/bus.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/elements/bus.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/elements/line.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/elements/line.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/elements/load.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/elements/load.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/elements/sgen.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/elements/sgen.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/elements/switch.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/elements/switch.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/elements/transformer.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/elements/transformer.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/meta.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/meta.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/model/constrainted.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/model/constrainted.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/model/static.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/model/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,17 @@
         etype = etype.lower()
         if etype not in ["load", "sgen", "trafo", "switch", "storage"]:
             LOG.info("Invalid etype %s. Skipping.", etype)
             return False
 
         for name, value in data.items():
             # Add try/except
+            if etype == "switch" and name == "closed":
+                if not isinstance(value, bool):
+                    value = value != 0
             self.grid[etype].at[idx, name] = value
 
     def run_powerflow(self, time):
         """Run the powerflow calculation."""
         try:
             pp.runpp(self.grid)
             self.lf_converged = True
```

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/module.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/module.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/plotter.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/plotter.py`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/midas/modules/powergrid/simulator.py` & `midas-powergrid-1.0.9/midas/modules/powergrid/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,17 +175,15 @@
         Returns
         -------
         int
             The next step this simulator wants to be stepped.
 
         """
         self._sim_time = time
-        if self.key_value_logs:
-            LOG.info(json.dumps(inputs))
-        else:
+        if not self.key_value_logs:
             LOG.debug("At step %d received inputs %s", time, mformat(inputs))
 
         for eid, attrs in inputs.items():
             gidx = eid.split("-")[0]
             grid = self.models.get(f"Grid-{gidx}", None)
 
             if grid is None:
```

### Comparing `midas-powergrid-1.0.8/midas_powergrid.egg-info/PKG-INFO` & `midas-powergrid-1.0.9/midas_powergrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-powergrid
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simulator for pandapower grids.
 Home-page: https://gitlab.com/midas-mosaik/midas-powergrid
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `midas-powergrid-1.0.8/midas_powergrid.egg-info/SOURCES.txt` & `midas-powergrid-1.0.9/midas_powergrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midas-powergrid-1.0.8/setup.py` & `midas-powergrid-1.0.9/setup.py`

 * *Files identical despite different names*

