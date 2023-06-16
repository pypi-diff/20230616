# Comparing `tmp/jaaql-monitor-1.2.69.tar.gz` & `tmp/jaaql-monitor-1.2.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.69.tar", last modified: Fri Jun 16 15:07:45 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.70.tar", last modified: Fri Jun 16 15:25:55 2023, max compression
```

## Comparing `jaaql-monitor-1.2.69.tar` & `jaaql-monitor-1.2.70.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 15:07:45.762393 jaaql-monitor-1.2.69/
--rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.69/LICENSE.txt
--rw-rw-rw-   0        0        0     1454 2023-06-16 15:07:45.762393 jaaql-monitor-1.2.69/PKG-INFO
--rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.69/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 15:07:45.757388 jaaql-monitor-1.2.69/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1454 2023-06-16 15:07:45.000000 jaaql-monitor-1.2.69/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-16 15:07:45.000000 jaaql-monitor-1.2.69/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 15:07:45.000000 jaaql-monitor-1.2.69/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-16 15:07:45.000000 jaaql-monitor-1.2.69/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 15:07:45.000000 jaaql-monitor-1.2.69/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 15:07:45.757388 jaaql-monitor-1.2.69/monitor/
--rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.69/monitor/__init__.py
--rw-rw-rw-   0        0        0    31356 2023-06-16 14:59:07.000000 jaaql-monitor-1.2.69/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-06-16 15:07:38.000000 jaaql-monitor-1.2.69/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-06-16 15:07:45.762393 jaaql-monitor-1.2.69/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.69/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:25:55.993157 jaaql-monitor-1.2.70/
+-rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.70/LICENSE.txt
+-rw-rw-rw-   0        0        0     1454 2023-06-16 15:25:55.993157 jaaql-monitor-1.2.70/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.70/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 15:25:55.993157 jaaql-monitor-1.2.70/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1454 2023-06-16 15:25:55.000000 jaaql-monitor-1.2.70/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-16 15:25:55.000000 jaaql-monitor-1.2.70/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 15:25:55.000000 jaaql-monitor-1.2.70/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-16 15:25:55.000000 jaaql-monitor-1.2.70/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 15:25:55.000000 jaaql-monitor-1.2.70/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 15:25:55.993157 jaaql-monitor-1.2.70/monitor/
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.70/monitor/__init__.py
+-rw-rw-rw-   0        0        0    31356 2023-06-16 14:59:07.000000 jaaql-monitor-1.2.70/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-06-16 15:25:48.000000 jaaql-monitor-1.2.70/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 15:25:55.993157 jaaql-monitor-1.2.70/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.70/setup.py
```

### Comparing `jaaql-monitor-1.2.69/LICENSE.txt` & `jaaql-monitor-1.2.70/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.69/PKG-INFO` & `jaaql-monitor-1.2.70/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.69
+Version: 1.2.70
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.69/README.md` & `jaaql-monitor-1.2.70/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.69/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.70/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.69
+Version: 1.2.70
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.69/monitor/main.py` & `jaaql-monitor-1.2.70/monitor/main.py`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.69/setup.py` & `jaaql-monitor-1.2.70/setup.py`

 * *Files identical despite different names*

