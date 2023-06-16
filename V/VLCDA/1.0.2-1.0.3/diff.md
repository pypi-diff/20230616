# Comparing `tmp/VLCDA-1.0.2.tar.gz` & `tmp/VLCDA-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VLCDA-1.0.2.tar", last modified: Fri Jun 16 00:32:04 2023, max compression
+gzip compressed data, was "VLCDA-1.0.3.tar", last modified: Fri Jun 16 00:39:44 2023, max compression
```

## Comparing `VLCDA-1.0.2.tar` & `VLCDA-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 00:32:04.093872 VLCDA-1.0.2/
--rw-rw-rw-   0        0        0     1077 2023-06-16 00:19:36.000000 VLCDA-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      592 2023-06-16 00:32:04.100401 VLCDA-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2023-06-16 00:30:13.000000 VLCDA-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 00:32:04.062755 VLCDA-1.0.2/VLCDA/
--rw-rw-rw-   0        0        0    19570 2023-06-16 00:20:07.000000 VLCDA-1.0.2/VLCDA/Logic_Circuits_Evolution.py
--rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 VLCDA-1.0.2/VLCDA/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:32:04.089866 VLCDA-1.0.2/VLCDA.egg-info/
--rw-rw-rw-   0        0        0      592 2023-06-16 00:32:03.000000 VLCDA-1.0.2/VLCDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-06-16 00:32:03.000000 VLCDA-1.0.2/VLCDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 00:32:03.000000 VLCDA-1.0.2/VLCDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 00:32:03.000000 VLCDA-1.0.2/VLCDA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-16 00:32:04.103396 VLCDA-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      654 2023-06-16 00:31:56.000000 VLCDA-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:39:44.281137 VLCDA-1.0.3/
+-rw-rw-rw-   0        0        0     1077 2023-06-16 00:19:36.000000 VLCDA-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-16 00:39:44.280138 VLCDA-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1406 2023-06-16 00:33:20.000000 VLCDA-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 00:39:44.250584 VLCDA-1.0.3/VLCDA/
+-rw-rw-rw-   0        0        0    19570 2023-06-16 00:20:07.000000 VLCDA-1.0.3/VLCDA/Logic_Circuits_Evolution.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 VLCDA-1.0.3/VLCDA/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:39:44.277127 VLCDA-1.0.3/VLCDA.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-16 00:39:42.000000 VLCDA-1.0.3/VLCDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-16 00:39:44.000000 VLCDA-1.0.3/VLCDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 00:39:43.000000 VLCDA-1.0.3/VLCDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 00:39:43.000000 VLCDA-1.0.3/VLCDA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 00:39:44.281137 VLCDA-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-06-16 00:39:39.000000 VLCDA-1.0.3/setup.py
```

### Comparing `VLCDA-1.0.2/LICENSE.txt` & `VLCDA-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.2/README.md` & `VLCDA-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.2/VLCDA/Logic_Circuits_Evolution.py` & `VLCDA-1.0.3/VLCDA/Logic_Circuits_Evolution.py`

 * *Files identical despite different names*

