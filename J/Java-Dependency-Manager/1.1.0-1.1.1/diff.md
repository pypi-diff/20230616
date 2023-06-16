# Comparing `tmp/Java Dependency Manager-1.1.0.tar.gz` & `tmp/Java Dependency Manager-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Java Dependency Manager-1.1.0.tar", last modified: Thu Jun 15 13:45:05 2023, max compression
+gzip compressed data, was "Java Dependency Manager-1.1.1.tar", last modified: Fri Jun 16 04:01:50 2023, max compression
```

## Comparing `Java Dependency Manager-1.1.0.tar` & `Java Dependency Manager-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 13:45:05.308557 Java Dependency Manager-1.1.0/
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 13:45:05.307716 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/PKG-INFO
--rw-r--r--   0 nagarajurepala   (501) staff       (20)      360 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)        1 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       58 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/entry_points.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       17 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/requires.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       16 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/top_level.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1035 2023-06-15 12:49:38.000000 Java Dependency Manager-1.1.0/LICENSE
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-15 13:45:05.308407 Java Dependency Manager-1.1.0/PKG-INFO
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 13:45:05.307970 Java Dependency Manager-1.1.0/javadepsmanager/
--rw-r--r--   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 07:45:23.000000 Java Dependency Manager-1.1.0/javadepsmanager/__init__.py
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     9755 2023-06-15 13:16:10.000000 Java Dependency Manager-1.1.0/javadepsmanager/command_line.py
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       38 2023-06-15 13:45:05.308599 Java Dependency Manager-1.1.0/setup.cfg
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1015 2023-06-15 13:44:01.000000 Java Dependency Manager-1.1.0/setup.py
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:01:50.075690 Java Dependency Manager-1.1.1/
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:01:50.075124 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)      360 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)        1 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       58 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       17 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/requires.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       16 2023-06-16 04:01:50.000000 Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/top_level.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1035 2023-06-15 12:49:38.000000 Java Dependency Manager-1.1.1/LICENSE
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-16 04:01:50.075546 Java Dependency Manager-1.1.1/PKG-INFO
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-16 04:01:50.075345 Java Dependency Manager-1.1.1/javadepsmanager/
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 07:45:23.000000 Java Dependency Manager-1.1.1/javadepsmanager/__init__.py
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)    10090 2023-06-16 03:57:53.000000 Java Dependency Manager-1.1.1/javadepsmanager/command_line.py
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       38 2023-06-16 04:01:50.075730 Java Dependency Manager-1.1.1/setup.cfg
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1015 2023-06-16 04:01:08.000000 Java Dependency Manager-1.1.1/setup.py
```

### Comparing `Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/PKG-INFO` & `Java Dependency Manager-1.1.1/Java_Dependency_Manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Java-Dependency-Manager
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generates Dependency tree for any java project also compares dependencies between two versions, use jdm in commandline to use this tool
 Home-page: https://github.com/Nagaraju6242/javadepsmanager
 Author: Repala Nagaraju
 Author-email: nagarajrepala@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Nagaraju6242/javadepsmanager
 Project-URL: Tracker, https://github.com/Nagaraju6242/javadepsmanager/issues
```

### Comparing `Java Dependency Manager-1.1.0/LICENSE` & `Java Dependency Manager-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Java Dependency Manager-1.1.0/PKG-INFO` & `Java Dependency Manager-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Java Dependency Manager
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generates Dependency tree for any java project also compares dependencies between two versions, use jdm in commandline to use this tool
 Home-page: https://github.com/Nagaraju6242/javadepsmanager
 Author: Repala Nagaraju
 Author-email: nagarajrepala@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Nagaraju6242/javadepsmanager
 Project-URL: Tracker, https://github.com/Nagaraju6242/javadepsmanager/issues
```

### Comparing `Java Dependency Manager-1.1.0/javadepsmanager/command_line.py` & `Java Dependency Manager-1.1.1/javadepsmanager/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,17 @@
     with open(pom_path,"w") as f:
         f.write(xml)
 
 def main():
     keeppom = False
     compare_versions = False
     version = None
+    version2 = None
+    choice = None
+    results = None
     if(len(sys.argv) > 1 and sys.argv[1] == "keeppom"):
         keeppom = True
     
     print_in_color("Welcome to Java Dependency Manager", "green")
     if not os.path.exists(DEPENDENCIES_DIR):
         os.makedirs(DEPENDENCIES_DIR)
 
@@ -166,14 +169,15 @@
             sys.exit()
         for i,result in enumerate(results, start=1):
             print(f"{i}. {result['namespace']} >> {result['name']} -- {result['latestVersionInfo']['version']}(latest)")
         print_in_color("\nIf you cannot find the required artifact, try using the pom.xml url option\n", "magenta")
         choice = input("Select an option to proceed (or pom.xml url): ")
         if(choice.startswith("https://repo1.maven.org/maven2/")):
             group_id, artifact_id, version = parse_pom_link(choice)
+            choice = None
             print(f"Selected {group_id} >> {artifact_id} >> {version}")
         else:
             if(choice == ""):
                 choice = 0
             else:
                 try:
                     choice = int(choice) - 1
@@ -195,17 +199,22 @@
 
     if not version:
         version = input(f"Enter the required version or leave empty to use latest version: ").strip()
         if(version == ""):
             version = results[choice]['latestVersionInfo']['version']
     
     if(compare_versions):
-        version2 = input(f"Enter the second version to compare with or leave empty to use latest version: ").strip()
-        if(version2 == ""):
-            version2 = results[choice]['latestVersionInfo']['version']
+        if choice:
+            version2 = input(f"Enter the second version to compare with or leave empty to use latest version: ").strip()
+            if(version2 == ""):
+                version2 = results[choice]['latestVersionInfo']['version']
+        else:
+            version2 = input(f"Enter the second version to compare with: ").strip()
+            while(version2 == ""):
+                version2 = input(f"Enter the second version to compare with: ").strip()
         print_in_color(f"Comparing {version} and {version2}", "magenta")
 
     save_dependency_tree(group_id, artifact_id, version)
     if(compare_versions):
         save_dependencies_list(group_id, artifact_id, version, nopom=True)
         dependencies1 = parse_dependencies_list(f"{artifact_id}-{version}-list.txt")
         save_dependency_tree(group_id, artifact_id, version2)
```

### Comparing `Java Dependency Manager-1.1.0/setup.py` & `Java Dependency Manager-1.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Java Dependency Manager',
-    version='1.1.0',
+    version='1.1.1',
     packages=['javadepsmanager'],
     entry_points={
         'console_scripts': [
             'jdm=javadepsmanager.command_line:main'
         ]
     },
     install_requires=[
```

