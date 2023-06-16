# Comparing `tmp/Java Dependency Manager-1.1.1.tar.gz` & `tmp/Java Dependency Manager-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Java Dependency Manager-1.1.1.tar", last modified: Fri Jun 16 04:01:50 2023, max compression
+gzip compressed data, was "Java Dependency Manager-1.1.2.tar", last modified: Fri Jun 16 04:10:51 2023, max compression
```

## Comparing `Java Dependency Manager-1.1.1.tar` & `Java Dependency Manager-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:01:50.075690 Java Dependency Manager-1.1.1/
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:01:50.075124 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/PKG-INFO
--rw-r--r--   0 nagarajurepala   (501) staff       (20)      360 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)        1 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       58 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/entry_points.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       17 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/requires.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       16 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/top_level.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1035 2023-06-15 12:49:38.000000 Java Dependency Manager-1.1.1/LICENSE
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-16 04:01:50.075546 Java Dependency Manager-1.1.1/PKG-INFO
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:01:50.075345 Java Dependency Manager-1.1.1/javadepsmanager/
--rw-r--r--   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 07:45:23.000000 Java Dependency Manager-1.1.1/javadepsmanager/__init__.py
--rw-r--r--   0 nagarajurepala   (501) staff       (20)    10090 2023-06-16 03:57:53.000000 Java Dependency Manager-1.1.1/javadepsmanager/command_line.py
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       38 2023-06-16 04:01:50.075730 Java Dependency Manager-1.1.1/setup.cfg
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1015 2023-06-16 04:01:08.000000 Java Dependency Manager-1.1.1/setup.py
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:10:51.711515 Java Dependency Manager-1.1.2/
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:10:51.710934 Java Dependency Manager-1.1.2/Java_Dependency_Manager.egg-info/
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-16 04:10:51.000000 Java Dependency Manager-1.1.2/Java_Dependency_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)      360 2023-06-16 04:10:51.000000 Java Dependency Manager-1.1.2/Java_Dependency_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)        1 2023-06-16 04:10:51.000000 Java Dependency Manager-1.1.2/Java_Dependency_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       58 2023-06-16 04:10:51.000000 Java Dependency Manager-1.1.2/Java_Dependency_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       17 2023-06-16 04:10:51.000000 Java Dependency Manager-1.1.2/Java_Dependency_Manager.egg-info/requires.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       16 2023-06-16 04:10:51.000000 Java Dependency Manager-1.1.2/Java_Dependency_Manager.egg-info/top_level.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1035 2023-06-15 12:49:38.000000 Java Dependency Manager-1.1.2/LICENSE
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-16 04:10:51.711384 Java Dependency Manager-1.1.2/PKG-INFO
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:10:51.711184 Java Dependency Manager-1.1.2/javadepsmanager/
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 07:45:23.000000 Java Dependency Manager-1.1.2/javadepsmanager/__init__.py
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)    10102 2023-06-16 04:10:27.000000 Java Dependency Manager-1.1.2/javadepsmanager/command_line.py
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       38 2023-06-16 04:10:51.711563 Java Dependency Manager-1.1.2/setup.cfg
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1015 2023-06-16 04:10:49.000000 Java Dependency Manager-1.1.2/setup.py
```

### Comparing `Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/PKG-INFO` & `Java Dependency Manager-1.1.2/Java_Dependency_Manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Java-Dependency-Manager
-Version: 1.1.1
+Version: 1.1.2
 Summary: Generates Dependency tree for any java project also compares dependencies between two versions, use jdm in commandline to use this tool
 Home-page: https://github.com/Nagaraju6242/javadepsmanager
 Author: Repala Nagaraju
 Author-email: nagarajrepala@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Nagaraju6242/javadepsmanager
 Project-URL: Tracker, https://github.com/Nagaraju6242/javadepsmanager/issues
```

### Comparing `Java Dependency Manager-1.1.1/LICENSE` & `Java Dependency Manager-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Java Dependency Manager-1.1.1/PKG-INFO` & `Java Dependency Manager-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Java Dependency Manager
-Version: 1.1.1
+Version: 1.1.2
 Summary: Generates Dependency tree for any java project also compares dependencies between two versions, use jdm in commandline to use this tool
 Home-page: https://github.com/Nagaraju6242/javadepsmanager
 Author: Repala Nagaraju
 Author-email: nagarajrepala@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Nagaraju6242/javadepsmanager
 Project-URL: Tracker, https://github.com/Nagaraju6242/javadepsmanager/issues
```

### Comparing `Java Dependency Manager-1.1.1/javadepsmanager/command_line.py` & `Java Dependency Manager-1.1.2/javadepsmanager/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
     if not version:
         version = input(f"Enter the required version or leave empty to use latest version: ").strip()
         if(version == ""):
             version = results[choice]['latestVersionInfo']['version']
     
     if(compare_versions):
-        if choice:
+        if choice == None:
             version2 = input(f"Enter the second version to compare with or leave empty to use latest version: ").strip()
             if(version2 == ""):
                 version2 = results[choice]['latestVersionInfo']['version']
         else:
             version2 = input(f"Enter the second version to compare with: ").strip()
             while(version2 == ""):
                 version2 = input(f"Enter the second version to compare with: ").strip()
@@ -222,17 +222,17 @@
         dependencies2 = parse_dependencies_list(f"{artifact_id}-{version2}-list.txt")
         dependencies1, dependencies2 = process_dependencies(dependencies1, dependencies2)
         print()
         print_in_color(f"Dependencies in version {version} but not in version {version2}:\n", "yellow")
         deps_in_version1 = list(set(dependencies1) - set(dependencies2))
         deps_in_version2 = list(set(dependencies2) - set(dependencies1))
         if(len(deps_in_version1) == 0):
-            print_in_color("None", "red")
+            print_in_color("None", "green")
         else:
-            print_in_color("\n".join(deps_in_version1), "red")
+            print_in_color("\n".join(deps_in_version1), "green")
         print("\n----------------------------------------\n")
         print_in_color(f"Dependencies in version {version2} but not in version {version}:\n", "yellow")
         if(len(deps_in_version2) == 0):
             print_in_color("None", "red")
         else:
             print_in_color("\n".join(deps_in_version2), "red")
         print()
```

### Comparing `Java Dependency Manager-1.1.1/setup.py` & `Java Dependency Manager-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Java Dependency Manager',
-    version='1.1.1',
+    version='1.1.2',
     packages=['javadepsmanager'],
     entry_points={
         'console_scripts': [
             'jdm=javadepsmanager.command_line:main'
         ]
     },
     install_requires=[
```

