# Comparing `tmp/TapisCL-ICICLE-0.0.52.tar.gz` & `tmp/TapisCL-ICICLE-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.52.tar", last modified: Mon May 22 23:32:10 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.60.tar", last modified: Fri Jun 16 03:35:09 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.52.tar` & `TapisCL-ICICLE-0.0.60.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 23:32:10.836639 TapisCL-ICICLE-0.0.52/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.52/LICENSE
--rw-rw-rw-   0        0        0    44553 2023-05-22 23:32:10.836639 TapisCL-ICICLE-0.0.52/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-05-06 23:32:02.000000 TapisCL-ICICLE-0.0.52/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 23:32:10.812633 TapisCL-ICICLE-0.0.52/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      186 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:32:10.816639 TapisCL-ICICLE-0.0.52/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0        0 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0     5345 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0     4514 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/client/connectionInitializer.py
--rw-rw-rw-   0        0        0     1223 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/client/formatters.py
--rw-rw-rw-   0        0        0     2854 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/client/handlers.py
--rw-rw-rw-   0        0        0      895 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/client/parsers.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:32:10.823639 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3420 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/appCommands.py
--rw-rw-rw-   0        0        0     8167 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0     5271 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2977 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     2189 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     4429 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:32:10.825639 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1401 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      845 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     1997 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0     4479 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/systemCommands.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:32:10.826640 TapisCL-ICICLE-0.0.52/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0     8718 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      527 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/server/serverConnection.py
--rw-rw-rw-   0        0        0      161 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:32:10.831639 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/args.py
--rw-rw-rw-   0        0        0     8565 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/decorators.py
--rw-rw-rw-   0        0        0     2141 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1201 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0      925 2023-04-29 17:45:39.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/logger.py
--rw-rw-rw-   0        0        0     2127 2023-04-29 18:53:15.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/schemas.py
--rw-rw-rw-   0        0        0     2504 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:32:10.835639 TapisCL-ICICLE-0.0.52/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44553 2023-05-22 23:32:10.000000 TapisCL-ICICLE-0.0.52/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-05-22 23:32:10.000000 TapisCL-ICICLE-0.0.52/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 23:32:10.000000 TapisCL-ICICLE-0.0.52/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-22 23:32:10.000000 TapisCL-ICICLE-0.0.52/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-05-22 23:32:10.000000 TapisCL-ICICLE-0.0.52/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 23:32:10.000000 TapisCL-ICICLE-0.0.52/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-05-22 23:31:30.000000 TapisCL-ICICLE-0.0.52/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 23:32:10.836639 TapisCL-ICICLE-0.0.52/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.499647 TapisCL-ICICLE-0.0.60/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.60/LICENSE
+-rw-rw-rw-   0        0        0    44549 2023-06-16 03:35:09.498647 TapisCL-ICICLE-0.0.60/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-05-06 23:32:02.000000 TapisCL-ICICLE-0.0.60/README.md
+-rw-rw-rw-   0        0        0     1225 2023-06-16 03:35:00.000000 TapisCL-ICICLE-0.0.60/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 03:35:09.499647 TapisCL-ICICLE-0.0.60/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.475143 TapisCL-ICICLE-0.0.60/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.476143 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.477143 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0     9614 2023-06-16 03:29:32.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0     8443 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.483645 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/appCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.485647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0    14578 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0     6867 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     3159 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4900 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    11391 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7537 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.486647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1453 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     2210 2023-06-16 03:18:11.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0    10602 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/systemCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.489647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0     9976 2023-06-16 03:30:19.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0     7659 2023-06-16 02:40:58.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      462 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/serviceCheck.py
+-rw-rw-rw-   0        0        0      171 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.490647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4384 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.493647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     1436 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.497647 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44549 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      316 2023-06-06 01:10:45.000000 TapisCL-ICICLE-0.0.60/src/__main__.py
```

### Comparing `TapisCL-ICICLE-0.0.52/LICENSE` & `TapisCL-ICICLE-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.52/PKG-INFO` & `TapisCL-ICICLE-0.0.60/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.52
+Version: 0.0.60
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
-Author-email: Michael Ray <ahumanbeing189@gmail.com>
+Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE
+Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE
 Keywords: Tapis,CLI,Agave,HPC,Tapis Pods,TACC
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `TapisCL-ICICLE-0.0.52/README.md` & `TapisCL-ICICLE-0.0.60/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/decorators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,131 +1,119 @@
-#!/usr/bin/python3
-import socket
-import argparse
-from argparse import SUPPRESS
-import sys
-import pyfiglet
-from getpass import getpass
-import os
+"""
+DECORATORS
+These decorators are used in the tapisObjectWrappers.py file to standardize special functions. Allows for increased code reusability
+"""
+import typing
 import time
-from client.handlers import Handlers
+import abc
+import socket
+from functools import update_wrapper, partial
+
 try:
-    from ..utilities import schemas
-    from ..utilities import socketOpts as SO
-    from ..utilities import killableThread
-    from ..utilities import decorators
-    from ..utilities import args
-    from ..utilities import logger
-    from . import formatters
-    from . import handlers
-    from . import parsers
-    from . import connectionInitializer
+    from socketopts import schemas
+    from utilities import exceptions, killableThread
+    from commands.arguments import argument
 except:
-    import utilities.schemas as schemas
-    import utilities.socketOpts as SO
-    import utilities.killableThread as killableThread
-    import utilities.decorators as decorators
-    import utilities.args as args
-    import utilities.logger as logger
-    import client.formatters as formatters
-    import client.handlers as handlers
-    import client.parsers as parsers
-    import client.connectionInitializer as connectionInitializer
+    from ..socketopts import schemas
+    from ..utilities import exceptions, killableThread
+    from ..commands.arguments import argument
+
 
+class BaseRequirementDecorator(abc.ABC):
+    username: typing.Optional[str] = None
+    password: typing.Optional[str] = None
 
-__location__ = os.path.realpath(
-    os.path.join(os.getcwd(), os.path.dirname(__file__)))
-server_path = os.path.join(__location__, r'..\server\server.py')
+    @abc.abstractmethod
+    async def __call__(self, command: typing.Type[object], connection: socket.socket, *args, **kwargs):
+        pass
 
 
-class CLI(SO.ClientSocketOpts, decorators.DecoratorSetup, formatters.Formatters, args.Args, parsers.Parsers, connectionInitializer.ConnectionInitilializer):
+class Auth(BaseRequirementDecorator):
     """
-    Receive user input, either direct from bash environment or from the custom interface, then parse these commands and send them to the server to be executed. 
+    used for secure authentication from the client. Requires that the function has a username and password parameter for credentials. sends request for credentials from 
+    the client, and checks those credentials against the stored credentials in the server.
     """
-    def __init__(self, IP: str, PORT: int):
-        super().__init__()
+    async def __call__(self, command, *args, **kwargs):
+        connection = kwargs['connection']
+        requires_username = True
+        if connection:
+            auth_request = schemas.FormRequest(request_content=argument.Form('auth', [
+                        argument.Argument('username'),
+                        argument.Argument('password', arg_type='secure')
+                    ]).json(),
+                    message={"message":"Password is required to continue. If you logged in using TACC password login, use that. Otherwise use the session password\nYour username was returned during initial login"})
+            await connection.send(auth_request)
+            auth_data = await connection.receive()
+            if auth_data.request_content['password'] != self.password:
+                raise ValueError("The provided password does not match the stored password")
+            if auth_data.request_content['username'] != self.username:
+                raise ValueError("The provided username does not match the stored username")
+            return await command.run(**kwargs)
+        return await command.run(**kwargs)
 
-        self.ip, self.port = IP, PORT
-        self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM) 
 
-        # sets up connection with the server
-        self.username = None
-        self.password = None
-
-        # set up argparse
-        self.parser = argparse.ArgumentParser(description="Command Line Argument Parser", exit_on_error=False, usage=SUPPRESS, conflict_handler='resolve')
-        self.parser.add_argument('command')
+class NeedsConfirmation(BaseRequirementDecorator):
+    """
+    add to functions that you want user confirmation to exit. If you accidentally enter a command to delete a pod, this will not let you until you confirm
+    """
+    async def __call__(self, command, *args, **kwargs):
+        connection = kwargs['connection']
+        if connection:
+            connection = connection
+            confirmation_request = schemas.FormRequest(message={"message":f"YOU REQUESTED TO {command.__class__.__name__.upper()}. THIS MIGHT CAUSE DATA LOSS! Please confirm (y/n)"},
+                                                       request_content={"confirmation":argument.Argument('confirm', arg_type='confirmation')})
+            await connection.send(confirmation_request)
+            confirmation_reply: schemas.FormResponse = await connection.receive()
+            confirmed = confirmation_reply.request_content['confirmation']
+            if not confirmed:
+                raise exceptions.NoConfirmationError(command)
+        return await command.run(**kwargs)
+
+
+DECORATOR_LIST = [
+    NeedsConfirmation,
+    Auth
+]
+    
+class DecoratorSetup:
+    """
+    for instantiation of the tapis wrappers, and the server, to set up decorators with user credentials and the socket connection. If you want to use the decorators in your class
+    YOU WILL NEED TO USE THIS!
+    """
+    def configure_decorators(self, username, password):
+        self.username = username
+        self.password = password
 
-        self.message_handlers = {
-            'FormRequest':self.form_handler,
-            'AuthRequest':self.auth_handler,
-            'ConfirmationRequest':self.confirmation_handler,
-        }
 
-        for parameters in self.argparser_args.values():
-            self.parser.add_argument(*parameters["args"], **parameters["kwargs"])
+class AnimatedLoading:
+    """
+    Add this if you want to print a loading animation while a function is executing
+    """
+    def __init__(self, func: typing.Callable):
+        update_wrapper(self, func)
+        self.func = func
+        self.__code__ = func.__code__
+        self.animation_frames = ['|','/','-','\\']
+
+    def __get__(self, obj, objtype):
+        """Support instance methods."""
+        return partial(self.__call__, obj)
 
-        print(r"If you find any issues, please create a new issue here: https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/issues")
+    def __repr__(self):
+        return self.func
+    
+    def __str__(self):
+        return str(self.func)
     
-    def special_forms_ops(self):
-        """
-        handle special form requests sent by the server
-        """
+    def animation(self):
         while True:
-            message = self.schema_unpack_explicit(self.connection)
-            message_type = message.schema_type
-            if message_type in self.message_handlers.keys():
-                filled_form = self.message_handlers[message_type](message)
-            else:
-                return message
-            self.json_send_explicit(self.connection, filled_form.dict())
-
-    def terminal_cli(self):
-        self.username, self.url = self.connect()
-        try:
-            kwargs = self.parser.parse_args()
-        except:
-            print("Invalid Arguments")
-            os._exit(0)
-        kwargs = vars(kwargs)
-        command = self.command_input_parser(kwargs, exit_=1) # operate with args, send them over
-        self.json_send_explicit(self.connection, command.dict())
-        response = self.special_forms_ops()
-        if response.schema_type == 'ResponseData':
-            self.print_response(response.response_message)
-        os._exit(0)
-
-    def environment_cli(self):
-        self.username, self.url = self.connect()
-        title = pyfiglet.figlet_format("-----------\nTapisCLICICLE\n-----------", font="slant") # print the title when CLI is accessed
-        print(title)
-        
-        while True: # open the CLI if no arguments provided on startup
-            try:
-                time.sleep(0.01)
-                kwargs = self.process_command(str(input(f"[{self.username}@{self.url}] "))) # ask for and process user input
-                try:
-                    command = self.command_input_parser(kwargs) # run operations
-                except:
-                    continue
-                if not command:
-                    continue
-                self.json_send_explicit(self.connection, command.dict())
-                response = self.special_forms_ops()
-                self.environment_cli_response_stream_handler(response)
-            except KeyboardInterrupt:
-                pass # keyboard interrupts mess with the server, dont do it! it wont work anyway, hahahaha
-            except WindowsError: # if connection error with the server (there wont be any connection errors)
-                print("[-] Connection was dropped. Exiting")
-                os._exit(0)
-            except Exception as e: # if something else happens
-                print(e)
-
-    def main(self):
-        if len(sys.argv) > 1: # checks if any command line arguments were provided. Does not open CLI
-            self.terminal_cli()
-        self.environment_cli()
-
-
-if __name__ == "__main__":
-    client = CLI(socket.gethostbyname(socket.gethostname()), 30000)
-    client.main()
+            for frame in self.animation_frames:
+                print(f"loading {frame}", end='', flush=True)
+                time.sleep(0.5)
+    
+    def __call__(self, obj, *args, **kwargs):
+        animation_thread = killableThread.KillableThread(target=self.animation)
+        animation_thread.start()
+        result = self.func(obj, *args, **kwargs)
+        animation_thread.kill()
+        print("", end='', flush=True)
+        return result
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/appCommands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from tapipy import tapis
-import pyperclip
 import json
-try:
-    from . import baseCommand
-    from ..utilities import decorators
-except:
-    import commands.baseCommand as baseCommand
-    import utilities.decorators as decorators
+
+
+if __name__ != "__main__":
+    from . import baseCommand, decorators
 
 
 class create_app(baseCommand.BaseCommand):
     """
     @help: create an app. You must have a properly configured app config file. 
     See a template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/app-config.json
     @todo: add a system where the class can say whether or not the config file of the app exists, and if it does not, open up a form to get system information. Maybe
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from tapipy.tapis import TapisResult
 
 
 HANDLED_TYPES = (TapisResult)
 JSON_SERIALIZABLE = (str, int, dict, list, set, tuple)
     
 
@@ -44,33 +46,42 @@
                 if name in desired_data:
                     filled_data[name] = data
             return filled_data
         return return_data
     
     @staticmethod
     def pod_formatter(self, return_data, verbose):
-        if not verbose:
+        if return_data:
             return_data = DataFormatters.json_serializer(return_data)
-            return DataFormatters.base_formatter(self, return_data, desired_data=DataFormatters.pod_data)
-        return str(return_data)
+            if not verbose:
+                return DataFormatters.base_formatter(self, return_data, desired_data=DataFormatters.pod_data)
+            return return_data
+        return "No data found"
     
     @staticmethod
     def system_formatter(self, return_data, verbose):
-        if not verbose:
+        if return_data:
             return_data = DataFormatters.json_serializer(return_data)
-            return DataFormatters.base_formatter(self, return_data, desired_data=DataFormatters.system_data)
-        return str(return_data)
+            if not verbose:
+                return DataFormatters.base_formatter(self, return_data, desired_data=DataFormatters.system_data)
+            return return_data
+        return "No data found"
     
     @staticmethod
     def app_formatter(self, return_data, verbose):
-        if not verbose:
+        if return_data:
             return_data = DataFormatters.json_serializer(return_data)
-            return DataFormatters.base_formatter(self, return_data, desired_data=DataFormatters.app_data)
-        return str(return_data)
+            if not verbose:
+                return DataFormatters.base_formatter(self, return_data, desired_data=DataFormatters.app_data)
+            return return_data
+        return "No data found"
     
     @staticmethod
     def server_formatter(self, return_data, verbose):
-        if not verbose:
-            return_data = DataFormatters.json_serializer(return_data)
-            return DataFormatters.base_formatter(self, return_data, desired_data=DataFormatters.server_data)
-        return str(return_data)
+        if return_data:
+            try:
+                json.dumps(return_data)
+                return return_data
+            except:
+                return str(return_data)
+        return "No data found"
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from py2neo import Graph
-try:
-    from ...utilities import decorators
-    from .. import baseCommand
-except:
-    import utilities.decorators as decorators
-    import commands.baseCommand as baseCommand
 
 
+if __name__ != "__main__":
+    from .. import baseCommand, decorators
+    from ..arguments import argument
+
 
 class neo4j(baseCommand.BaseQuery):
     """
     @help: integrated CLI to interface with Neo4j pods
     """
-    decorator=decorators.RequiresExpression()
-    async def run(self, id: str, expression: str = None, *args, **kwargs) -> str: # function to submit queries to a Neo4j knowledge graph
-        uname, pword = self.get_pod_credentials(id)
-        graph = Graph(f"bolt+ssc://{id}.pods.{self.t.base_url.split('https://')[1]}:443", auth=(uname, pword), secure=True, verify=True)
+    required_arguments = [
+        argument.Argument('id'),
+        argument.Argument('expression', arg_type='expression')
+    ]
+    async def run(self, *args, **kwargs) -> str: # function to submit queries to a Neo4j knowledge graph
+        uname, pword = self.get_pod_credentials(kwargs["id"])
+        graph = Graph(f"bolt+ssc://{kwargs['id']}.pods.{self.t.base_url.split('https://')[1]}:443", auth=(uname, pword), secure=True, verify=True)
 
         try:
-            return_value = graph.run(expression)
+            return_value = graph.run(kwargs['expression'])
             print(type(return_value))
-            if str(return_value) == '(No data)' and 'create' in expression.lower(): # if no data is returned (mostly if something is created) then just say 'success'
-                return f'[+][{id}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
+            if str(return_value) == '(No data)' and 'create' in kwargs['expression'].lower(): # if no data is returned (mostly if something is created) then just say 'success'
+                return f'[+][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
             elif str(return_value) == '(No data)':
-                return f'[-][{id}@pods.{self.t.base_url.split("https://")[1]}:443] KG is empty'
+                return f'[-][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] KG is empty'
 
             print(return_value)
             print(type(return_value))
-            return str(f'[+][{id}] {return_value}')
+            return str(f'[+][{kwargs["id"]}] {return_value}')
         except Exception as e:
             return str(e)
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import sys
-import time
-import re
-from tapipy.tapis import Tapis
-import os
 import typing
 
-try:
-    from ..utilities import exceptions
-    from ..utilities import decorators
-    from ..utilities import args as Args
-    from ..utilities import schemas
-    from ..utilities import killableThread
-    from . import baseCommand
-except:
-    import utilities.killableThread as killableThread
-    import utilities.exceptions as exceptions
-    import utilities.decorators as decorators
-    import utilities.args as Args
-    import utilities.decorators as decorators
-    import utilities.schemas as schemas
-    import commands.baseCommand as baseCommand
+from tapipy.tapis import Tapis
+
+
+if __name__ != "__main__":
+    from . import baseCommand, decorators
+    from utilities import exceptions
+    from commands.arguments.argument import Argument
 
 
 class switch_service(baseCommand.BaseCommand):
     """
     @help: switch the connected tapis service
     @todo: upgrade to federated auth
     """
-    decorator = decorators.Auth()
-    async def run(self, link: str, username: str=None, password=None, *args, **kwargs) -> tuple[typing.Any, str, str] | None:  # link is the baseURL
-        results = kwargs['server'].switch_session(username, password, link)
+    required_arguments=[
+        Argument('link', size_limit=80),
+        Argument('auth', choices=['password', 'device_code', 'federated'])
+    ]
+    async def run(self, *args, **kwargs):  # link is the baseURL
+        auth = kwargs['auth']
+        link = kwargs['link']
+        self.server.auth_type = auth
+        if auth == "password":
+            results = await self.server.password_grant(link, kwargs['connection'])
+        elif auth == "device_code":
+            results = await self.server.device_code_grant(link, kwargs['connection'])
+        elif auth == "federated":
+            results = await self.server.federated_grant(link, kwargs['connection'])
+        else:
+            results = None
         return results
       
 
 class exit(baseCommand.BaseCommand):
     """
     @help: exit the CLI without shutting down the service
     """
@@ -45,22 +45,31 @@
     """
     @help: exit the CLI and shutdown the service
     """
     decorator = decorators.NeedsConfirmation()
     async def run(self, *args, **kwargs):
         raise exceptions.Shutdown
     
+    
 class whoami(baseCommand.BaseCommand):
     """
     @help: returns the username of the current user
     """
     async def run(self, *args, **kwargs) -> str:
         user_info = self.t.authenticator.get_userinfo()
         return user_info
     
 
 class get_args(baseCommand.BaseCommand):
     """
     @help: get the list of possible arguments 
     """
     async def run(self, *args, **kwargs):
-        return Args.Args.argparser_args
+        return kwargs['server'].arguments
+    
+
+class whereami(baseCommand.BaseCommand):
+    """
+    @help: get the URI of current tapis tenant
+    """
+    async def run(self, *args, **kwargs):
+        return kwargs['server'].url
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,159 +1,134 @@
 import sys
-from getpass import getpass
 import time
-import re
-from tapipy.tapis import Tapis
 import socket
 import os
-import logging
-import typing
 import asyncio
 import traceback
 
-try:
-    from ..utilities import exceptions
-    from ..utilities import logger
-    from ..utilities import socketOpts as SO
-    from ..utilities import killableThread
-    from ..utilities import schemas
-    from . import serverConnection
-    from ..commands.query import neo4j, postgres
-    from ..commands import baseCommand
-    from ..commands import commandMap
-    from ..utilities import decorators
-except ImportError:
-    import utilities.decorators as decorators
-    import utilities.exceptions as exceptions
-    import utilities.logger as logger
-    import utilities.socketOpts as SO
-    import utilities.killableThread as killableThread
-    import utilities.schemas as schemas
-    import server.serverConnection as serverConnection
-    import commands.baseCommand as baseCommand
+from tapipy.tapis import Tapis
+
+if __name__ != "__main__":
+    from commands import commandMap, decorators
+    from utilities import logger, exceptions
+    from socketopts import schemas, socketOpts
+    from server import auth
+else:
     import commands.commandMap as commandMap
 
 
-class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup):
+class ServerConnection(socketOpts.ServerSocketOpts):
+    """
+    connection object to wrap around async reader and writer to make work easier
+    """
+    def __init__(self, name, reader, writer, debug=False):
+        super().__init__(name, debug=debug)
+        self.name = name
+        self.reader = reader
+        self.writer = writer
+
+    async def close(self):
+        self.writer.close()
+        await self.writer.wait_closed()
+        
+
+class TaskCallback:
+    def __init__(self, logger, task: asyncio.Task):
+        self.logger, self.task = logger, task
+        print("DOING THE INIT")
+
+    def __call__(self, result):
+        print(result)
+        result = self.task.result()
+        self.logger.info(result)
+
+
+class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup, auth.ServerSideAuth):
     """
     Receives commands from the client and executes Tapis operations
     """
+    SESSION_TIME = 1200
     def __init__(self, IP: str, PORT: int):
         super().__init__()
         self.initial = True
 
         self.t = None
         self.url = None
         self.access_token = None
         self.username = None
         self.password = None
+        self.auth_type = None
 
         self.__name__ = "Server"
         self.initialize_logger(self.__name__)
         # setting up socket server
         self.ip, self.port = IP, PORT
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.sock.setblocking(False)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.bind((self.ip, self.port))
         self.sock.listen(1)
-        self.end_time = time.time() + 300  # start the countdown on the timeout
+        self.end_time = time.time() + self.SESSION_TIME # start the countdown on the timeout
+
+        self.task_list = []
 
         self.server = None
+        self.num_connections = 0
 
         self.logger.info('initialization complete')
 
-    def switch_session(self, username: str, password, link: str, *args, **kwargs):
-        start = time.time()
-        try:
-            t = Tapis(base_url=f"https://{link}",
-                    username=username,
-                    password=password)
-            t.get_tokens()
-        except Exception as e:
-            self.logger.warning(e)
-            raise ValueError(f"Invalid tapis auth credentials")
-        
-        self.username = username
-        self.password = password
-        self.t = t
-        self.url = link
-        self.access_token = self.t.access_token
-
-        self.configure_decorators(self.username, self.password)
-        self.update_credentials(t, username, password)
-        # V3 Headers
-        header_dat = {"X-Tapis-token": t.access_token.access_token,
-                      "Content-Type": "application/json"}
-        # create authenticator for tapis systems
-        authenticator = t.access_token
-        # extract the access token from the authenticator
-        
-        if 'win' in sys.platform:
-            os.system(f"set JWT={self.access_token}")
-        else: # unix based
-            os.system(f"export JWT={self.access_token}")
-
-        self.logger.info(f"initiated in {time.time()-start}")
-
-        return f"Successfully initialized tapis service on {self.url}"
-
     async def handshake(self, connection):
         self.logger.info("Handshake starting")
         if self.initial:  # if this is the first time in the session that the cli is connecting
             startup_data = schemas.StartupData(initial = self.initial)
             await connection.send(startup_data)
-            self.logger.info("send the initial status update")
-
-            for attempt in range(1, 4):
-                url: schemas.StartupData = await connection.receive()
-                self.logger.info("received the link")
-                try:
-                    #await self.run_command(connection, {'command':'switch_service', 'link':url.url, 'verbose':False})
-                    await self.aggregate_command_map['switch_service'](link=url.url, connection=connection, server=self, verbose=False)
-                    self.logger.info("Verification success")
-                    break
-                except ValueError as e:
-                    login_failure_data = schemas.ResponseData(response_message = (str(e), attempt))
-                    await connection.send(login_failure_data)
-                    self.logger.warning(f"Verification failure, {e}")
-                    if attempt == 3:  
-                        self.logger.error(
-                            "Attempted verification too many times. Exiting")
-                        raise ValueError("auth failure")
-                    continue
+            await self.auth_startup(connection)
         else:
-            self.configure_decorators(self.username, self.password)
+            startup_result = schemas.StartupData(initial = self.initial, username = self.username, url = self.url)
+            await connection.send(startup_result)
         self.initial = False
-        startup_result = schemas.StartupData(initial = self.initial, username = self.username, url = self.url)
-        self.logger.info("Connection success")
-        await connection.send(startup_result)
         self.logger.info("Final connection data sent")
 
     async def accept(self, reader, writer):
         """
         accept connection request and initialize communication with the client
         """  
-        connection = serverConnection.ServerConnection(reader=reader, writer=writer)
+        self.num_connections += 1
+        connection = ServerConnection(f"CON-{self.num_connections}", reader=reader, writer=writer, debug=True)
         self.timeout_handler()
         ip, port= writer.transport.get_extra_info('socket').getsockname()
         if ip != socket.gethostbyname(socket.gethostname()):
             raise exceptions.UnauthorizedAccessError(ip)
         self.logger.info("Received connection request")
         try:
             await self.handshake(connection)
-        except ValueError:
+        except exceptions.InvalidCredentialsReceived as e:
             self.logger.warning("invalid credentials entered too many times. Cancelling request")
             await connection.close()
             return
-
+        except exceptions.ClientSideError as e:
+            self.logger.warning(f"Encountered client side error during startup handshake. {e}")
+            await connection.close()
+            return
+        except Exception as e:
+            self.logger.warning(e)
+            await connection.close()
+            return
         self.logger.info("connection is running now")
-        loop = asyncio.get_event_loop()
-        await loop.create_task(self.receive_and_execute(connection))
+        await connection.send(schemas.ResponseData(request_content={name:argument.json() for name, argument in self.arguments.items()}))
+        
+        setup_response: schemas.ResponseData = await connection.receive()
+        if not setup_response.request_content['setup_success']:
+            self.logger.warning(f"The setup of the connection {connection.name} failed")
+            return
 
+        loop = asyncio.get_event_loop()
+        task: asyncio.Task = loop.create_task(self.receive_and_execute(connection))
+        callback = TaskCallback(self.logger, task)
+        task.add_done_callback(callback)
 
     def timeout_handler(self):  
         """
         checks if the timeout has been exceeded
         """
         if time.time() > self.end_time: 
             raise exceptions.TimeoutError
@@ -162,47 +137,54 @@
         """
         receive and process commands
         """
         while True:
             try:
                 message = await connection.receive()
                 self.timeout_handler()  
-                kwargs, exit_status = message.kwargs, message.exit_status
+                kwargs = message.request_content
                 result = await self.run_command(connection, kwargs)
-                response = schemas.ResponseData(response_message = result, url = self.url, active_username = self.username)
-                self.end_time = time.time() + 300 
+                response = schemas.ResponseData(message={"message":result}, url=self.url, active_username=self.username)
+                self.end_time = time.time() + self.SESSION_TIME 
                 await connection.send(response)
                 self.logger.info(message.schema_type)
+            except exceptions.ClientSideError as e:
+                self.logger.warning(e)
+                continue
             except (exceptions.TimeoutError, exceptions.Shutdown) as e:
-                error_response = schemas.ResponseData(response_message = str(e), exit_status=1)
+                error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
                 await connection.send(error_response)
                 self.logger.warning(str(e))
                 self.server.close()
                 loop = asyncio.get_event_loop()
                 loop.stop()
                 loop.close()
                 sys.exit(0)
             except exceptions.Exit as e:
                 self.logger.info("user exit initiated")
-                error_response = schemas.ResponseData(response_message = str(e), exit_status=1)
+                error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
                 await connection.send(error_response)
                 await connection.close()
                 return
                 #self.accept()  # wait for CLI to reconnect
             except OSError:
                 self.logger.info("connection was lost, waiting to reconnect")
                 await connection.close()
             except (exceptions.CommandNotFoundError, exceptions.NoConfirmationError, exceptions.InvalidCredentialsReceived, Exception) as e:
                 error_str = traceback.format_exc()
-                error_response = schemas.ResponseData(response_message = f"{str(e)}")
+                error_response = schemas.ResponseData(error=str(e), url=self.url, active_username=self.username)
                 await connection.send(error_response)
                 self.logger.warning(f"{error_str}")
     
     async def main(self):
         self.server = await asyncio.start_server(self.accept, sock=self.sock)
-        async with self.server:
-            await self.server.serve_forever()
+        try:
+            async with self.server:
+                await self.server.serve_forever()
+        except KeyboardInterrupt:
+            self.server.close()
+            sys.exit(0)
 
 
 if __name__ == '__main__':
     server = Server(socket.gethostbyname(socket.gethostname()), 30000)
     asyncio.run(server.main())
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         super().__init__(f"Confirmation was not given to the function {function.__class__.__name__}")
 
 
 class InvalidCredentialsReceived(Exception):
     """
     raise error when the provided credentials fail
     """
-    def __init__(self, function: typing.Callable, cred_type: str):
-        super().__init__(f"The {cred_type} provided for the command {function.__class__.__name__} was invalid")
+    def __init__(self, *args):
+        super().__init__(*args)
 
 
 class HelpDoesNotExist(AttributeError):
     """
     raise error when the program tries to extract help information from a method, but help is not found
     """
     def __init__(self, command_name):
@@ -59,8 +59,24 @@
 
 
 class UnauthorizedAccessError(Exception):
     """
     raise error when an unauthorized IP tries to connect to the server
     """
     def __init__(self, ip):
-        super().__init__(f"DANGER! UNAUTHORIZED IP {ip} TRIED TO CONNECT TO THE SERVER. SOMEONE IS TRYING TO PIGGYBACK ON THE TAPIS APPLICATION, AND ATTEMPTING TO STEAL YOUR DATA.")
+        super().__init__(f"DANGER! UNAUTHORIZED IP {ip} TRIED TO CONNECT TO THE SERVER. SOMEONE IS TRYING TO PIGGYBACK ON THE TAPIS APPLICATION, AND ATTEMPTING TO STEAL YOUR DATA.")
+
+
+class ClientSideError(ConnectionError):
+    """
+    raise error when problem is on client side
+    """
+    def __init__(self, error_message):
+        super().__init__(f"CLIENT SIDE ERROR: {error_message}")
+
+
+class NoTenantClient(AttributeError):
+    """
+    raise error when no client for tenant for auth
+    """
+    def __init__(self, tenant):
+        super().__init__(f"No client found for the tenant {tenant}")
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 """
 HELPERS
 Aggregation of helper functions and classes
 """
-import typing
 import sys
 import threading
-import re
-try:
-    from . import exceptions
-    from . import args
-except:
-    import exceptions as exceptions
-    import args as args
 
 
 class KillableThread(threading.Thread):
     """
     Extends the threading.Thread class from python threading library. Used for the loading animation
     """
     def __init__(self, *args, **keywords):
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,8 +22,21 @@
         stream_handler.setFormatter(stream_format)
         file_handler.setFormatter(file_format)
 
         # add the handlers
         self.logger.addHandler(stream_handler)
         self.logger.addHandler(file_handler)
 
+        self.logger.disabled = False
+
+
+class ConnectionLogger:
+    def initialize_logger(self, name):
+        self.logger = logging.getLogger(name)
+        self.logger.setLevel(logging.INFO)
+        stream_handler = logging.StreamHandler(stream=sys.stdout)
+        stream_handler.setLevel(logging.INFO)
+        stream_format = logging.Formatter(
+            '%(name)s - %(levelname)s - %(message)s')
+        stream_handler.setFormatter(stream_format)
+        self.logger.addHandler(stream_handler)
         self.logger.disabled = False
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCLICICLE/utilities/schemas.py` & `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,81 @@
 '''
 SCHEMAS
 These are standardized JSON serializable data formats to make socket operations on the localhost client-server smoother.
 '''
-from typing import Any, Optional
-from pydantic import BaseModel
+from typing import Any, Optional, Literal
 
+from pydantic import BaseModel, Field, validator
 
-class CommandData(BaseModel):
+
+class BaseSchema(BaseModel):
+    schema_type: str
+    request_content: dict = dict()
+    message: dict = dict()
+    error: str = str()
+    system: str = str()
+    pwd: str = str()
+
+
+class CommandData(BaseSchema):
     """
     Command execution request sent from the client to the server to execute a specified command
     """
-    schema_type: str = 'CommandData'
-    kwargs: Optional[dict]
-    expression: Optional[str] 
-    exit_status: int = 0
+    schema_type = 'CommandData'
 
 
-class AuthData(BaseModel):
+class PasswordAuthData(BaseSchema):
     """
     Sends credentials from the client to the server for auth to Tapis services
     """
-    schema_type: str = 'AuthData'
+    schema_type: str = 'PasswordAuthData'
     username: Optional[str]
     password: Optional[str]
 
 
-class StartupData(BaseModel):
+class StartupData(BaseSchema):
     """
     used only during connection inintialization between the client and server to transmit startup data
     """
     schema_type: str = 'StartupData'
     initial: bool = False
     username: Optional[str]
     url: Optional[str]
 
 
-class ResponseData(BaseModel):
+class ResponseData(BaseSchema):
     """
     data from the server to the client with return data from commands, as well as errors
     """
     schema_type: str = 'ResponseData'
-    response_message: Any
-    exit_status: int = 0
-    url: str | None = None
-    active_username: str | None = None
-
+    url: str = str()
+    active_username: str = str()
+    exit_status = 0
+    
 
-class FormRequest(BaseModel):
+class FormRequest(BaseSchema):
     """
     Request seperate input for some command parameters. If the arguments_list is empty, this will be interpreted as an expression request for something like neo4j
     """
     schema_type: str = 'FormRequest'
-    arguments_list: list
 
 
-class FormResponse(BaseModel):
+class FormResponse(BaseSchema):
     """
     respond to a form request with proper data
     """
     schema_type: str = 'FormResponse'
-    arguments_list: dict | str
 
 
-class AuthRequest(BaseModel):
+class AuthRequest(BaseSchema):
     """
     Request auth credentials from the client
     """
     schema_type: str = 'AuthRequest'
-    requires_username: bool = True
-    secure_input: bool = False
+    auth_request_type: Literal["password", "device_code", "federated", "requested", "success"]
 
 
-class ConfirmationRequest(BaseModel):
+class ConfirmationRequest(BaseSchema):
     """
     ask the client for confirmation to carry out an action
     """
-    schema_type: str = 'ConfirmationRequest'
-    message: str
+    schema_type: str = 'ConfirmationRequest'
```

### Comparing `TapisCL-ICICLE-0.0.52/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.52
+Version: 0.0.60
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
-Author-email: Michael Ray <ahumanbeing189@gmail.com>
+Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE
+Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE
 Keywords: Tapis,CLI,Agave,HPC,Tapis Pods,TACC
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `TapisCL-ICICLE-0.0.52/pyproject.toml` & `TapisCL-ICICLE-0.0.60/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,36 +2,43 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.52"
+version = "0.0.60"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
-authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
+authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Tapis", "CLI", "Agave", "HPC", "Tapis Pods", "TACC"]
 dependencies = [
     "pydantic",
     "pyfiglet",
     "tapipy",
     "pyperclip",
     "py2neo",
-    "psycopg"
+    "psycopg",
+    "blessed",
+    "prompt_toolkit",
+    "TapisFederatedAuthClientAPI",
+    "requests"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
-Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE"
+Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE"
 
 [project.entry-points."TapisCLICICLE.__main__"]
-tomatoes = "TapisCLICICLE:__main__"
+TapisCLICICLE = "src:__main__"
+
+[tool.poetry.scripts]
+TapisCLICICLE = "src.__main__"
```

