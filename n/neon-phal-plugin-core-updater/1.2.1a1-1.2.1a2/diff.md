# Comparing `tmp/neon-phal-plugin-core-updater-1.2.1a1.tar.gz` & `tmp/neon-phal-plugin-core-updater-1.2.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-core-updater-1.2.1a1.tar", last modified: Thu Jun 15 23:53:08 2023, max compression
+gzip compressed data, was "neon-phal-plugin-core-updater-1.2.1a2.tar", last modified: Fri Jun 16 00:00:19 2023, max compression
```

## Comparing `neon-phal-plugin-core-updater-1.2.1a1.tar` & `neon-phal-plugin-core-updater-1.2.1a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:53:08.182339 neon-phal-plugin-core-updater-1.2.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-15 23:53:01.000000 neon-phal-plugin-core-updater-1.2.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-15 23:53:08.182339 neon-phal-plugin-core-updater-1.2.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-15 23:53:01.000000 neon-phal-plugin-core-updater-1.2.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:53:08.182339 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater/
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-15 23:53:01.000000 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:53:08.182339 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-15 23:53:08.000000 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 23:53:08.000000 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:53:08.000000 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 23:53:08.000000 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 23:53:08.000000 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 23:53:08.000000 neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 23:53:08.182339 neon-phal-plugin-core-updater-1.2.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-15 23:53:01.000000 neon-phal-plugin-core-updater-1.2.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-16 00:00:12.000000 neon-phal-plugin-core-updater-1.2.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-16 00:00:12.000000 neon-phal-plugin-core-updater-1.2.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater/
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-16 00:00:12.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-16 00:00:12.000000 neon-phal-plugin-core-updater-1.2.1a2/setup.py
```

### Comparing `neon-phal-plugin-core-updater-1.2.1a1/LICENSE.md` & `neon-phal-plugin-core-updater-1.2.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-core-updater-1.2.1a1/PKG-INFO` & `neon-phal-plugin-core-updater-1.2.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.2.1a1
+Version: 1.2.1a2
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-core-updater-1.2.1a1/README.md` & `neon-phal-plugin-core-updater-1.2.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater/__init__.py` & `neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-core-updater-1.2.1a1/neon_phal_plugin_core_updater.egg-info/PKG-INFO` & `neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.2.1a1
+Version: 1.2.1a2
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-core-updater-1.2.1a1/setup.py` & `neon-phal-plugin-core-updater-1.2.1a2/setup.py`

 * *Files identical despite different names*

