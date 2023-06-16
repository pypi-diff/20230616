# Comparing `tmp/jianglab-0.4.5.tar.gz` & `tmp/jianglab-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.4.5.tar", last modified: Fri Jun 16 19:57:28 2023, max compression
+gzip compressed data, was "jianglab-0.4.6.tar", last modified: Fri Jun 16 20:01:45 2023, max compression
```

## Comparing `jianglab-0.4.5.tar` & `jianglab-0.4.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 19:57:28.244739 jianglab-0.4.5/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-16 19:57:28.244407 jianglab-0.4.5/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.5/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 19:57:28.240438 jianglab-0.4.5/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.5/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    21177 2023-06-16 19:57:08.000000 jianglab-0.4.5/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.5/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 19:57:28.243736 jianglab-0.4.5/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-16 19:57:28.000000 jianglab-0.4.5/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-16 19:57:28.000000 jianglab-0.4.5/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-16 19:57:28.000000 jianglab-0.4.5/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-16 19:57:28.000000 jianglab-0.4.5/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-16 19:57:28.000000 jianglab-0.4.5/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-16 19:57:28.244856 jianglab-0.4.5/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-16 19:57:16.000000 jianglab-0.4.5/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 20:01:45.856291 jianglab-0.4.6/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-16 20:01:45.855954 jianglab-0.4.6/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.6/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 20:01:45.852220 jianglab-0.4.6/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.6/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    21183 2023-06-16 20:01:41.000000 jianglab-0.4.6/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.6/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 20:01:45.855354 jianglab-0.4.6/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-16 20:01:45.856420 jianglab-0.4.6/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-16 20:01:38.000000 jianglab-0.4.6/setup.py
```

### Comparing `jianglab-0.4.5/PKG-INFO` & `jianglab-0.4.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.5
+Version: 0.4.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.5/README.md` & `jianglab-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.4.5/jianglab/common_functions.py` & `jianglab-0.4.6/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
     return pickle.load(open(filename, "rb", -1))
 
 def get_bad_lanes(cmcr_file_path):
     gsheet = import_gsheet()
     bad_lanes = cmcr_file_path.split("\\")[-1].replace("-",".").split(".")[:6]
     bad_lanes = ".".join(bad_lanes)
     bad_lanes = gsheet[gsheet.File_name.str.contains(bad_lanes)]["Bad_lanes"]
-    if pd.isna(bad_lanes):
+    if pd.isna(bad_lanes).any():
         bad_lanes = []
         print("No bad lanes found")
     elif len(bad_lanes) == 1:
         bad_lanes = bad_lanes
     else:                      
         bad_lanes = [int(x) for x in list(bad_lanes)[0].split(",")]
     return bad_lanes
```

### Comparing `jianglab-0.4.5/jianglab.egg-info/PKG-INFO` & `jianglab-0.4.6/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.5
+Version: 0.4.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.5/setup.py` & `jianglab-0.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.4.5',
+    version='0.4.6',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

