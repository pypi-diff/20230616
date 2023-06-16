# Comparing `tmp/jianglab-0.4.2.tar.gz` & `tmp/jianglab-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.4.2.tar", last modified: Thu Jun 15 18:59:55 2023, max compression
+gzip compressed data, was "jianglab-0.4.3.tar", last modified: Thu Jun 15 19:43:12 2023, max compression
```

## Comparing `jianglab-0.4.2.tar` & `jianglab-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 18:59:55.395607 jianglab-0.4.2/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 18:59:55.395166 jianglab-0.4.2/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.2/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 18:59:55.391517 jianglab-0.4.2/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.2/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    21156 2023-06-15 18:59:38.000000 jianglab-0.4.2/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.2/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 18:59:55.394366 jianglab-0.4.2/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 18:59:55.000000 jianglab-0.4.2/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-15 18:59:55.000000 jianglab-0.4.2/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-15 18:59:55.000000 jianglab-0.4.2/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-15 18:59:55.000000 jianglab-0.4.2/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-15 18:59:55.000000 jianglab-0.4.2/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-15 18:59:55.395815 jianglab-0.4.2/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-15 18:59:46.000000 jianglab-0.4.2/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 19:43:12.565489 jianglab-0.4.3/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 19:43:12.564902 jianglab-0.4.3/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.3/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 19:43:12.560383 jianglab-0.4.3/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.3/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    21129 2023-06-15 19:42:52.000000 jianglab-0.4.3/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.3/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 19:43:12.563980 jianglab-0.4.3/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 19:43:12.000000 jianglab-0.4.3/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-15 19:43:12.000000 jianglab-0.4.3/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-15 19:43:12.000000 jianglab-0.4.3/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-15 19:43:12.000000 jianglab-0.4.3/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-15 19:43:12.000000 jianglab-0.4.3/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-15 19:43:12.566061 jianglab-0.4.3/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-15 19:43:01.000000 jianglab-0.4.3/setup.py
```

### Comparing `jianglab-0.4.2/PKG-INFO` & `jianglab-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.2/README.md` & `jianglab-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.4.2/jianglab/common_functions.py` & `jianglab-0.4.3/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
     return pickle.load(open(filename, "rb", -1))
 
 def get_bad_lanes(cmcr_file_path):
     gsheet = import_gsheet()
     bad_lanes = cmcr_file_path.split("\\")[-1].replace("-",".").split(".")[:6]
     bad_lanes = ".".join(bad_lanes)
     bad_lanes = gsheet[gsheet.File_name.str.contains(bad_lanes)]["Bad_lanes"]
-    if len(bad_lanes) != 0 and bad_lanes[0] != "None":                                 
+    if len(bad_lanes) != 0:                                 
         bad_lanes = [int(x) for x in list(bad_lanes)[0].split(",")]
     else:
         bad_lanes = []
         print("No bad lanes found")
     return bad_lanes
 
 def clean_centers_all_process(arr, neighbour_size = (6,6,6)):
```

### Comparing `jianglab-0.4.2/jianglab.egg-info/PKG-INFO` & `jianglab-0.4.3/jianglab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.2/setup.py` & `jianglab-0.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.4.2',
+    version='0.4.3',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

