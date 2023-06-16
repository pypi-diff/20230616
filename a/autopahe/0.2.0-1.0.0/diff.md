# Comparing `tmp/autopahe-0.2.0.tar.gz` & `tmp/autopahe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopahe-0.2.0.tar", last modified: Fri Jun 16 08:16:52 2023, max compression
+gzip compressed data, was "autopahe-1.0.0.tar", last modified: Fri Jun 16 07:42:43 2023, max compression
```

## Comparing `autopahe-0.2.0.tar` & `autopahe-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 08:16:52.189743 autopahe-0.2.0/
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-0.2.0/MANIFEST.in
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6400 2023-06-16 08:16:52.185743 autopahe-0.2.0/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5747 2023-06-16 07:52:43.000000 autopahe-0.2.0/README.md
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 08:16:52.177743 autopahe-0.2.0/autopahe/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       24 2023-06-16 07:36:17.000000 autopahe-0.2.0/autopahe/__init__.py
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    28017 2023-06-16 08:15:19.000000 autopahe-0.2.0/autopahe/auto_pahe.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      211 2023-06-13 23:06:59.000000 autopahe-0.2.0/autopahe/test.py
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 08:16:52.185743 autopahe-0.2.0/autopahe.egg-info/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6400 2023-06-16 08:16:51.000000 autopahe-0.2.0/autopahe.egg-info/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      316 2023-06-16 08:16:51.000000 autopahe-0.2.0/autopahe.egg-info/SOURCES.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-16 08:16:51.000000 autopahe-0.2.0/autopahe.egg-info/dependency_links.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       56 2023-06-16 08:16:51.000000 autopahe-0.2.0/autopahe.egg-info/entry_points.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-16 08:16:51.000000 autopahe-0.2.0/autopahe.egg-info/requires.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-16 08:16:51.000000 autopahe-0.2.0/autopahe.egg-info/top_level.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-0.2.0/pyproject.toml
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-0.2.0/requirements.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-16 08:16:52.189743 autopahe-0.2.0/setup.cfg
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)     1374 2023-06-16 08:16:40.000000 autopahe-0.2.0/setup.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 07:42:43.423442 autopahe-1.0.0/
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-1.0.0/MANIFEST.in
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6409 2023-06-16 07:42:43.423442 autopahe-1.0.0/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5756 2023-06-16 07:38:04.000000 autopahe-1.0.0/README.md
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 07:42:43.419442 autopahe-1.0.0/autopahe/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       24 2023-06-16 07:36:17.000000 autopahe-1.0.0/autopahe/__init__.py
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    27910 2023-06-16 06:58:12.000000 autopahe-1.0.0/autopahe/auto_pahe.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      211 2023-06-13 23:06:59.000000 autopahe-1.0.0/autopahe/test.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 07:42:43.423442 autopahe-1.0.0/autopahe.egg-info/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6409 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      301 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/SOURCES.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/dependency_links.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       56 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/entry_points.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/requires.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/top_level.txt
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-1.0.0/requirements.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-16 07:42:43.423442 autopahe-1.0.0/setup.cfg
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)     1374 2023-06-16 07:39:23.000000 autopahe-1.0.0/setup.py
```

### Comparing `autopahe-0.2.0/PKG-INFO` & `autopahe-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 0.2.0
+Version: 1.0.0
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 <!-- Badges -->
-[![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/)
+<!-- [![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/) -->
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/autopahe/)
 [![License](https://img.shields.io/github/license/haxsysgit/autopahe?color=brightgreen)](https://github.com/haxsysgit/autopahe/blob/main/license.md)
 [![OpenIssues](https://img.shields.io/github/issues/haxsysgit/autopahe?color=important)](https://github.com/haxsysgit/autopahe/issues)
 <!--LineBreak-->
 [![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/autopahe/)
 [![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/autopahe/)
 <!-- Badges -->
```

### Comparing `autopahe-0.2.0/README.md` & `autopahe-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 <!-- Badges -->
-[![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/)
+<!-- [![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/) -->
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/autopahe/)
 [![License](https://img.shields.io/github/license/haxsysgit/autopahe?color=brightgreen)](https://github.com/haxsysgit/autopahe/blob/main/license.md)
 [![OpenIssues](https://img.shields.io/github/issues/haxsysgit/autopahe?color=important)](https://github.com/haxsysgit/autopahe/issues)
 <!--LineBreak-->
 [![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/autopahe/)
 [![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/autopahe/)
 <!-- Badges -->
```

### Comparing `autopahe-0.2.0/autopahe/auto_pahe.py` & `autopahe-1.0.0/autopahe/auto_pahe.py`

 * *Files 1% similar despite different names*

```diff
@@ -776,24 +776,14 @@
         
     if mdcarg:
         multi_download_classic(mdcarg)
         
     if mdarg:
         multi_download_optimized(mdarg)
 
-def data_report(data = None,filepath = "autopahe_data.json",):
-    if data:
-        # Read existing JSON data from file
-        with open(filepath, 'r') as json_file:
-            existing_data = load(json_file)
-
-        existing_data.update(data)
-            
-        with open(filepath,"w") as st:
-            dump(existing_data,st)
         
 
 def main():
     # ===================================== Handling Arguments and other involved function============================================
     parser = argparse.ArgumentParser()
 
     # Adding all the required arguments
@@ -833,29 +823,37 @@
     
     if any(vars(args).values()):
         # Command line arguments are present
         command_main(args)
     else:
         # No command line arguments, run interactive mode
         interactive_main()
-        
-    if search_response_dict and jsonpage_dict:
-        final_data = {**search_response_dict,**jsonpage_dict}
-        data_report(data=final_data)
-
 
 
 
 
 if __name__ == '__main__':
     # INTRO BANNER
     Banners.header() 
     main()
-    
+
+
+final_data = {**search_response_dict,**jsonpage_dict}
 
 n()
+def data_report(filepath = "autopahe_data.json",data = None):
+    if data:
+        # Read existing JSON data from file
+        with open(filepath, 'r') as json_file:
+            existing_data = load(json_file)
+
+        existing_data.update(data)
+            
+        with open(filepath,"w") as st:
+            dump(existing_data,st)
+
 
 finish = time.perf_counter()
 
 print(f'Finish time is {round(finish-start,2)}\n')
```

### Comparing `autopahe-0.2.0/autopahe.egg-info/PKG-INFO` & `autopahe-1.0.0/autopahe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 0.2.0
+Version: 1.0.0
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 <!-- Badges -->
-[![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/)
+<!-- [![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/) -->
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/autopahe/)
 [![License](https://img.shields.io/github/license/haxsysgit/autopahe?color=brightgreen)](https://github.com/haxsysgit/autopahe/blob/main/license.md)
 [![OpenIssues](https://img.shields.io/github/issues/haxsysgit/autopahe?color=important)](https://github.com/haxsysgit/autopahe/issues)
 <!--LineBreak-->
 [![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/autopahe/)
 [![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/autopahe/)
 <!-- Badges -->
```

### Comparing `autopahe-0.2.0/setup.py` & `autopahe-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = 'autopahe',
-    version = '0.2.0',
+    version = '1.0.0',
     author_email="pentacker@gmail.com",
     description = "A python script to automate downloads from animepahe",
     url = "https://github.com/haxsysgit/autopahe",
     author = "Elenasulu Arinze",
     license = "MIT",
     py_modules = [
         'autopahe',
```

