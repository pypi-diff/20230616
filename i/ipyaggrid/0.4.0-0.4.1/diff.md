# Comparing `tmp/ipyaggrid-0.4.0.tar.gz` & `tmp/ipyaggrid-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ipyaggrid-0.4.0.tar", last modified: Mon Apr  3 11:25:02 2023, max compression
+gzip compressed data, was "ipyaggrid-0.4.1.tar", last modified: Fri Jun 16 14:13:48 2023, max compression
```

## Comparing `ipyaggrid-0.4.0.tar` & `ipyaggrid-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/builder_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid/flexbox/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/flexbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/flexbox/flexbox_css.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/flexbox/flexbox_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/ipyaggrid.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/js/helpersBuiltin.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   200433 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/137.ff8524eacb40847460e4.js
--rw-r--r--   0 runner    (1001) docker     (123)  1118282 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/461.54206acb00b733358b0e.js
--rw-r--r--   0 runner    (1001) docker     (123)    70486 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  4076714 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/590.76db7a0e38bda319cef5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/590.76db7a0e38bda319cef5.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    44259 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/591.746a48cdbfb965edc0b2.js
--rw-r--r--   0 runner    (1001) docker     (123)   251279 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/716.2ca2ae9f2a4d362ee4d3.js
--rw-r--r--   0 runner    (1001) docker     (123)  1089059 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/731.4c18aa787877929491e8.js
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/731.4c18aa787877929491e8.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1281803 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/remoteEntry.04bb4f50742cd4b84a6c.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-03 11:24:20.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)   177445 2023-04-03 11:25:01.000000 ipyaggrid-0.4.0/ipyaggrid/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid/magics/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/magics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/magics/custom_magics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-03 11:23:32.000000 ipyaggrid-0.4.0/ipyaggrid/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)  4089693 2023-04-03 11:24:13.000000 ipyaggrid-0.4.0/ipyaggrid/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123) 11439714 2023-04-03 11:24:13.000000 ipyaggrid-0.4.0/ipyaggrid/nbextension/index.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    21419 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/ipyaggrid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/ipyaggrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-03 11:25:02.000000 ipyaggrid-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-03 11:22:52.000000 ipyaggrid-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.937531 ipyaggrid-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-16 14:13:48.937531 ipyaggrid-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.909531 ipyaggrid-0.4.1/ipyaggrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/builder_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.913531 ipyaggrid-0.4.1/ipyaggrid/flexbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/flexbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/flexbox/flexbox_css.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/flexbox/flexbox_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/ipyaggrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.913531 ipyaggrid-0.4.1/ipyaggrid/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/js/helpersBuiltin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.913531 ipyaggrid-0.4.1/ipyaggrid/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.921531 ipyaggrid-0.4.1/ipyaggrid/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   200433 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/137.ba3ca1a8cae12f94c800.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1118282 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/461.54206acb00b733358b0e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    70486 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  4076714 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/590.4932d69c73f82d65d630.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/590.4932d69c73f82d65d630.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    44259 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/591.746a48cdbfb965edc0b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   251279 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/716.2ca2ae9f2a4d362ee4d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1089059 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/731.4c18aa787877929491e8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/731.4c18aa787877929491e8.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1281803 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/remoteEntry.d473f2ede13b01cc16fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 14:12:48.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)   177445 2023-06-16 14:13:30.000000 ipyaggrid-0.4.1/ipyaggrid/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.921531 ipyaggrid-0.4.1/ipyaggrid/magics/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/magics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/magics/custom_magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.925531 ipyaggrid-0.4.1/ipyaggrid/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-16 14:13:31.000000 ipyaggrid-0.4.1/ipyaggrid/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4089693 2023-06-16 14:13:47.000000 ipyaggrid-0.4.1/ipyaggrid/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123) 11439714 2023-06-16 14:13:47.000000 ipyaggrid-0.4.1/ipyaggrid/nbextension/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    21419 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/ipyaggrid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:13:48.913531 ipyaggrid-0.4.1/ipyaggrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-16 14:13:48.000000 ipyaggrid-0.4.1/ipyaggrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-16 14:13:48.000000 ipyaggrid-0.4.1/ipyaggrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:13:48.000000 ipyaggrid-0.4.1/ipyaggrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:13:48.000000 ipyaggrid-0.4.1/ipyaggrid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 14:13:48.000000 ipyaggrid-0.4.1/ipyaggrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 14:13:48.000000 ipyaggrid-0.4.1/ipyaggrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 14:13:48.937531 ipyaggrid-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-16 14:11:23.000000 ipyaggrid-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ipyaggrid-0.4.0/LICENSE` & `ipyaggrid-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/PKG-INFO` & `ipyaggrid-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ipyaggrid
-Version: 0.4.0
+Version: 0.4.1
 Summary: Jupyter widget - ag-grid in the notebook
-Home-page: https://gitlab.com/DGothrek/ipyaggrid
-Author: DGothrek
-Author-email: louisraison1@gmail.com
+Home-page: https://github.com/widgetti/ipyaggrid
+Author: Mario Buikhuizen, Maarten Breddels, DGothrek
+Author-email: mariobuikhuizen@gmail.com, maartenbreddels@gmail.com
 License: MIT
-Download-URL: https://gitlab.com/DGothrek/ipyaggrid/repository/archive.tar.gz?ref=0.4.0
+Download-URL: https://github.com/widgetti/ipyaggrid/archive/refs/tags/v0.4.1.zip
 Description: # ipyaggrid
         
         [![Latest Version](https://img.shields.io/pypi/v/ipyaggrid.svg)](https://pypi.python.org/pypi/ipyaggrid/)
         [![Downloads](https://img.shields.io/pypi/dm/ipyaggrid.svg)](https://pypi.python.org/pypi/ipyaggrid/)
         [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gl/DGothrek%2Fipyaggrid/binder-demo)
         
         ### Doc
@@ -30,7 +30,9 @@
 Keywords: ipywidget,javascript,ag-grid
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Provides-Extra: unit-test
+Provides-Extra: ui-test
```

### Comparing `ipyaggrid-0.4.0/README.md` & `ipyaggrid-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/__init__.py` & `ipyaggrid-0.4.1/ipyaggrid/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/__meta__.py` & `ipyaggrid-0.4.1/ipyaggrid/__meta__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,28 +16,27 @@
     return version
 
 
 # meta data
 
 __name__ = 'ipyaggrid'
 name_url = __name__.replace('_', '-')
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 __version_js__ = __version__
 
 
 __description__ = 'Jupyter widget - ag-grid in the notebook'
 __long_description__ = 'See repo README'
-__author__ = 'DGothrek'
-__author_email__ = 'louisraison1@gmail.com'
+__author__ = 'Mario Buikhuizen, Maarten Breddels, DGothrek'
+__author_email__ = 'mariobuikhuizen@gmail.com, maartenbreddels@gmail.com'
 
 # gitlab template
-__url__ = 'https://gitlab.com/{}/{}'.format(__author__, name_url)
-__download_url__ = 'https://gitlab.com/{}/{}/repository/archive.tar.gz?ref={}'.format(__author__,
-                                                                                      name_url,
-                                                                                      __version__)
+__url__ = 'https://github.com/widgetti/ipyaggrid'
+
+__download_url__ = 'https://github.com/widgetti/ipyaggrid/archive/refs/tags/v{}.zip'.format(__version__)
 
 __keywords__ = ['ipywidget',
                 'javascript',
                 'ag-grid',
                 ]
 __license__ = 'MIT'
 __classifiers__ = ['Development Status :: 4 - Beta',
```

### Comparing `ipyaggrid-0.4.0/ipyaggrid/builder_params.py` & `ipyaggrid-0.4.1/ipyaggrid/builder_params.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/display.py` & `ipyaggrid-0.4.1/ipyaggrid/display.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/flexbox/flexbox_css.py` & `ipyaggrid-0.4.1/ipyaggrid/flexbox/flexbox_css.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/flexbox/flexbox_standard.py` & `ipyaggrid-0.4.1/ipyaggrid/flexbox/flexbox_standard.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/grid.py` & `ipyaggrid-0.4.1/ipyaggrid/grid.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/js/helpersBuiltin.js` & `ipyaggrid-0.4.1/ipyaggrid/js/helpersBuiltin.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 helpersBuiltin = {
     dateFormatter: function(node) {
         // make sure date is not undefined
-        if (node && node.value) {
+        if (node && node.value && node.value !== "NaT") {
             let d = new Date(node.value);
             let h = d.getHours();
             let m = d.getMinutes();
             let s = d.getSeconds();
             const offset = d.getTimezoneOffset() * 60000;
             d = new Date(d.getTime() - offset);
             const ymd = d.toISOString().substring(0, 10);
```

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/package.json` & `ipyaggrid-0.4.1/ipyaggrid/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603365384615384%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.d473f2ede13b01cc16fa.js'}}",*

 * * "'version'": "'0.4.1'"}*

```diff
@@ -43,15 +43,15 @@
         "dist/*.js",
         "src/styles/**/*.css",
         "src/styles/icons/*.svg"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.04bb4f50742cd4b84a6c.js"
+            "load": "static/remoteEntry.d473f2ede13b01cc16fa.js"
         },
         "extension": "src/labplugin",
         "outputDir": "../ipyaggrid/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -80,9 +80,9 @@
         "dev": "webpack --mode=development && npm run build:labextension:dev",
         "format": "prettier --write '**/*.{js,jsx}'",
         "lint": "eslint '**/*.{js,jsx}' --quiet",
         "prepare": "webpack --mode production",
         "test": "echo \"Error: no test specified\"",
         "watch": "watch 'webpack --mode development' src/"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/137.ff8524eacb40847460e4.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/137.ba3ca1a8cae12f94c800.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -345,15 +345,15 @@
             t.r(i), t.d(i, {
                 AgGridModel: () => g,
                 AgGridView: () => p
             });
             var a = t(2390),
                 o = (t(8174), t(9336), t(1611), t(3960), t(8999), t(2455), t(3704), t(521), t(8276), t(194)),
                 r = t(5106);
-            const l = "0.4.0";
+            const l = "0.4.1";
             t(4329), t(9966), t(4027), t(9339), t(7064);
             const d = `~${l}`;
             class g extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "AgGridModel",
```

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/461.54206acb00b733358b0e.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/461.54206acb00b733358b0e.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/590.76db7a0e38bda319cef5.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/590.4932d69c73f82d65d630.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 590.76db7a0e38bda319cef5.js.LICENSE.txt */
+/*! For license information please see 590.4932d69c73f82d65d630.js.LICENSE.txt */
 (self.webpackChunkipyaggrid = self.webpackChunkipyaggrid || []).push([
     [590], {
         5590: (module, exports, __webpack_require__) => {
             var __WEBPACK_AMD_DEFINE_ARRAY__, __WEBPACK_AMD_DEFINE_RESULT__;
             __WEBPACK_AMD_DEFINE_ARRAY__ = [__webpack_require__(2390)], __WEBPACK_AMD_DEFINE_RESULT__ = function(__WEBPACK_EXTERNAL_MODULE__9__) {
                 return function(e) {
                     var t = {};
@@ -44,15 +44,15 @@
                             return e.default
                         } : function() {
                             return e
                         };
                         return n.d(t, "a", t), t
                     }, n.o = function(e, t) {
                         return Object.prototype.hasOwnProperty.call(e, t)
-                    }, n.p = "https://unpkg.com/ipyaggrid@0.4.0/dist/", n(n.s = 112)
+                    }, n.p = "https://unpkg.com/ipyaggrid@0.4.1/dist/", n(n.s = 112)
                 }([function(e, t, n) {
                     "use strict";
                     (function(e) {
                         function r(e) {
                             return null == e || "" === e ? null : e
                         }
 
@@ -30320,15 +30320,15 @@
                         },
                         uncompressBase64ToStr: function(e, t) {
                             const n = atob(e);
                             return o.uncompress(n, t)
                         }
                     }
                 }, function(e) {
-                    e.exports = JSON.parse('{"a":"0.4.0"}')
+                    e.exports = JSON.parse('{"a":"0.4.1"}')
                 }, function(e, t, n) {
                     "use strict";
                     n.r(t), n.d(t, "version", (function() {
                         return r
                     })), n.d(t, "bisect", (function() {
                         return g
                     })), n.d(t, "bisectRight", (function() {
```

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/590.76db7a0e38bda319cef5.js.LICENSE.txt` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/590.4932d69c73f82d65d630.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/591.746a48cdbfb965edc0b2.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/591.746a48cdbfb965edc0b2.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/716.2ca2ae9f2a4d362ee4d3.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/716.2ca2ae9f2a4d362ee4d3.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/731.4c18aa787877929491e8.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/731.4c18aa787877929491e8.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/remoteEntry.04bb4f50742cd4b84a6c.js` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/remoteEntry.d473f2ede13b01cc16fa.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -43,31 +43,31 @@
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        137: "ff8524eacb40847460e4",
+        137: "ba3ca1a8cae12f94c800",
         324: "afe7407c89fce3ffc72d",
         390: "cdc0ebfd32eb6ac143e8",
         461: "54206acb00b733358b0e",
         486: "9a102cac74aa3af2b7b8",
-        590: "76db7a0e38bda319cef5",
+        590: "4932d69c73f82d65d630",
         591: "746a48cdbfb965edc0b2",
         716: "2ca2ae9f2a4d362ee4d3",
         731: "4c18aa787877929491e8",
         906: "95bbf22d029b842482b2"
     } [e] + ".js?v=" + {
-        137: "ff8524eacb40847460e4",
+        137: "ba3ca1a8cae12f94c800",
         324: "afe7407c89fce3ffc72d",
         390: "cdc0ebfd32eb6ac143e8",
         461: "54206acb00b733358b0e",
         486: "9a102cac74aa3af2b7b8",
-        590: "76db7a0e38bda319cef5",
+        590: "4932d69c73f82d65d630",
         591: "746a48cdbfb965edc0b2",
         716: "2ca2ae9f2a4d362ee4d3",
         731: "4c18aa787877929491e8",
         906: "95bbf22d029b842482b2"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
@@ -123,15 +123,15 @@
                         (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (d("ag-grid-community", "28.1.1", (() => w.e(731).then((() => () => w(1731))))), d("ag-grid-enterprise", "28.1.1", (() => Promise.all([w.e(906), w.e(324)]).then((() => () => w(1906))))), d("d3", "5.16.0", (() => w.e(716).then((() => () => w(2716))))), d("ipyaggrid", "0.4.0", (() => Promise.all([w.e(390), w.e(590)]).then((() => () => w(5590))))), d("lodash", "4.17.21", (() => w.e(486).then((() => () => w(6486))))), d("pako", "1.0.11", (() => w.e(591).then((() => () => w(9591)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("ag-grid-community", "28.1.1", (() => w.e(731).then((() => () => w(1731))))), d("ag-grid-enterprise", "28.1.1", (() => Promise.all([w.e(906), w.e(324)]).then((() => () => w(1906))))), d("d3", "5.16.0", (() => w.e(716).then((() => () => w(2716))))), d("ipyaggrid", "0.4.1", (() => Promise.all([w.e(390), w.e(590)]).then((() => () => w(5590))))), d("lodash", "4.17.21", (() => w.e(486).then((() => () => w(6486))))), d("pako", "1.0.11", (() => w.e(591).then((() => () => w(9591)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `ipyaggrid-0.4.0/ipyaggrid/labextension/static/third-party-licenses.json` & `ipyaggrid-0.4.1/ipyaggrid/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/magics/custom_magics.py` & `ipyaggrid-0.4.1/ipyaggrid/magics/custom_magics.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/nbextension/extension.js` & `ipyaggrid-0.4.1/ipyaggrid/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/nbextension/index.js` & `ipyaggrid-0.4.1/ipyaggrid/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -30805,15 +30805,15 @@
             },
             uncompressBase64ToStr: function(e, t) {
                 const n = atob(e);
                 return o.uncompress(n, t)
             }
         }
     }, function(e) {
-        e.exports = JSON.parse('{"a":"0.4.0"}')
+        e.exports = JSON.parse('{"a":"0.4.1"}')
     }, function(e, t, n) {
         "use strict";
         n.r(t), n.d(t, "version", (function() {
             return r
         })), n.d(t, "bisect", (function() {
             return g
         })), n.d(t, "bisectRight", (function() {
```

### Comparing `ipyaggrid-0.4.0/ipyaggrid/nbextension/index.js.map` & `ipyaggrid-0.4.1/ipyaggrid/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid/util.py` & `ipyaggrid-0.4.1/ipyaggrid/util.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.4.0/ipyaggrid.egg-info/PKG-INFO` & `ipyaggrid-0.4.1/ipyaggrid.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ipyaggrid
-Version: 0.4.0
+Version: 0.4.1
 Summary: Jupyter widget - ag-grid in the notebook
-Home-page: https://gitlab.com/DGothrek/ipyaggrid
-Author: DGothrek
-Author-email: louisraison1@gmail.com
+Home-page: https://github.com/widgetti/ipyaggrid
+Author: Mario Buikhuizen, Maarten Breddels, DGothrek
+Author-email: mariobuikhuizen@gmail.com, maartenbreddels@gmail.com
 License: MIT
-Download-URL: https://gitlab.com/DGothrek/ipyaggrid/repository/archive.tar.gz?ref=0.4.0
+Download-URL: https://github.com/widgetti/ipyaggrid/archive/refs/tags/v0.4.1.zip
 Description: # ipyaggrid
         
         [![Latest Version](https://img.shields.io/pypi/v/ipyaggrid.svg)](https://pypi.python.org/pypi/ipyaggrid/)
         [![Downloads](https://img.shields.io/pypi/dm/ipyaggrid.svg)](https://pypi.python.org/pypi/ipyaggrid/)
         [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gl/DGothrek%2Fipyaggrid/binder-demo)
         
         ### Doc
@@ -30,7 +30,9 @@
 Keywords: ipywidget,javascript,ag-grid
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Provides-Extra: unit-test
+Provides-Extra: ui-test
```

### Comparing `ipyaggrid-0.4.0/ipyaggrid.egg-info/SOURCES.txt` & `ipyaggrid-0.4.1/ipyaggrid.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 ipyaggrid.egg-info/requires.txt
 ipyaggrid.egg-info/top_level.txt
 ipyaggrid/flexbox/__init__.py
 ipyaggrid/flexbox/flexbox_css.py
 ipyaggrid/flexbox/flexbox_standard.py
 ipyaggrid/js/helpersBuiltin.js
 ipyaggrid/labextension/package.json
-ipyaggrid/labextension/static/137.ff8524eacb40847460e4.js
+ipyaggrid/labextension/static/137.ba3ca1a8cae12f94c800.js
 ipyaggrid/labextension/static/461.54206acb00b733358b0e.js
 ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js
 ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js.LICENSE.txt
-ipyaggrid/labextension/static/590.76db7a0e38bda319cef5.js
-ipyaggrid/labextension/static/590.76db7a0e38bda319cef5.js.LICENSE.txt
+ipyaggrid/labextension/static/590.4932d69c73f82d65d630.js
+ipyaggrid/labextension/static/590.4932d69c73f82d65d630.js.LICENSE.txt
 ipyaggrid/labextension/static/591.746a48cdbfb965edc0b2.js
 ipyaggrid/labextension/static/716.2ca2ae9f2a4d362ee4d3.js
 ipyaggrid/labextension/static/731.4c18aa787877929491e8.js
 ipyaggrid/labextension/static/731.4c18aa787877929491e8.js.LICENSE.txt
 ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js
 ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js.LICENSE.txt
-ipyaggrid/labextension/static/remoteEntry.04bb4f50742cd4b84a6c.js
+ipyaggrid/labextension/static/remoteEntry.d473f2ede13b01cc16fa.js
 ipyaggrid/labextension/static/style.js
 ipyaggrid/labextension/static/third-party-licenses.json
 ipyaggrid/magics/__init__.py
 ipyaggrid/magics/custom_magics.py
 ipyaggrid/nbextension/extension.js
 ipyaggrid/nbextension/index.js
 ipyaggrid/nbextension/index.js.map
```

### Comparing `ipyaggrid-0.4.0/setup.py` & `ipyaggrid-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,13 +64,21 @@
     url=url,
     download_url=download_url,
     keywords=keywords,
     license=license,
     classifiers=classifiers,
     packages=packages,
     install_requires=install_requires,
+    extras_require={
+        "unit-test": [
+            "pytest",
+        ],
+        "ui-test": [
+            "solara[pytest]",
+        ]
+    },
     include_package_data=include_package_data,
     package_data=package_data,
     data_files=data_files,
     zip_safe=zip_safe,
     entry_points=entry_points
 )
```

