# Comparing `tmp/bio-pypage-0.1.0.tar.gz` & `tmp/bio-pypage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-pypage-0.1.0.tar", last modified: Fri Jun 16 08:21:46 2023, max compression
+gzip compressed data, was "bio-pypage-0.1.1.tar", last modified: Fri Jun 16 08:26:13 2023, max compression
```

## Comparing `bio-pypage-0.1.0.tar` & `bio-pypage-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-16 08:21:46.781952 bio-pypage-0.1.0/
--rw-r--r--   0 workspace   (502) staff       (20)     1070 2022-06-09 10:36:48.000000 bio-pypage-0.1.0/LICENSE
--rw-r--r--   0 workspace   (502) staff       (20)     5125 2023-06-16 08:21:46.781525 bio-pypage-0.1.0/PKG-INFO
--rw-r--r--   0 workspace   (502) staff       (20)     4642 2023-06-15 23:18:47.000000 bio-pypage-0.1.0/README.md
-drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-16 08:21:46.775397 bio-pypage-0.1.0/bio_pypage.egg-info/
--rw-r--r--   0 workspace   (502) staff       (20)     5125 2023-06-16 08:21:46.000000 bio-pypage-0.1.0/bio_pypage.egg-info/PKG-INFO
--rw-r--r--   0 workspace   (502) staff       (20)      300 2023-06-16 08:21:46.000000 bio-pypage-0.1.0/bio_pypage.egg-info/SOURCES.txt
--rw-r--r--   0 workspace   (502) staff       (20)        1 2023-06-16 08:21:46.000000 bio-pypage-0.1.0/bio_pypage.egg-info/dependency_links.txt
--rw-r--r--   0 workspace   (502) staff       (20)      119 2023-06-16 08:21:46.000000 bio-pypage-0.1.0/bio_pypage.egg-info/requires.txt
--rw-r--r--   0 workspace   (502) staff       (20)        7 2023-06-16 08:21:46.000000 bio-pypage-0.1.0/bio_pypage.egg-info/top_level.txt
-drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-16 08:21:46.780593 bio-pypage-0.1.0/pypage/
--rw-r--r--   0 workspace   (502) staff       (20)      132 2023-06-15 22:20:27.000000 bio-pypage-0.1.0/pypage/__init__.py
--rw-r--r--   0 workspace   (502) staff       (20)     9455 2023-06-15 14:51:03.000000 bio-pypage-0.1.0/pypage/heatmap.py
--rw-r--r--   0 workspace   (502) staff       (20)     3657 2022-06-09 10:36:48.000000 bio-pypage-0.1.0/pypage/hist.py
--rw-r--r--   0 workspace   (502) staff       (20)    12550 2022-06-29 13:50:11.000000 bio-pypage-0.1.0/pypage/information.py
--rw-r--r--   0 workspace   (502) staff       (20)    15280 2023-06-15 21:49:50.000000 bio-pypage-0.1.0/pypage/page.py
--rw-r--r--   0 workspace   (502) staff       (20)     3909 2022-06-09 13:50:18.000000 bio-pypage-0.1.0/pypage/utils.py
--rw-r--r--   0 workspace   (502) staff       (20)       38 2023-06-16 08:21:46.782106 bio-pypage-0.1.0/setup.cfg
--rw-r--r--   0 workspace   (502) staff       (20)      889 2023-06-16 08:21:36.000000 bio-pypage-0.1.0/setup.py
+drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-16 08:26:13.555509 bio-pypage-0.1.1/
+-rw-r--r--   0 workspace   (502) staff       (20)     1070 2022-06-09 10:36:48.000000 bio-pypage-0.1.1/LICENSE
+-rw-r--r--   0 workspace   (502) staff       (20)     5125 2023-06-16 08:26:13.555146 bio-pypage-0.1.1/PKG-INFO
+-rw-r--r--   0 workspace   (502) staff       (20)     4642 2023-06-16 08:24:17.000000 bio-pypage-0.1.1/README.md
+drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-16 08:26:13.552225 bio-pypage-0.1.1/bio_pypage.egg-info/
+-rw-r--r--   0 workspace   (502) staff       (20)     5125 2023-06-16 08:26:12.000000 bio-pypage-0.1.1/bio_pypage.egg-info/PKG-INFO
+-rw-r--r--   0 workspace   (502) staff       (20)      300 2023-06-16 08:26:13.000000 bio-pypage-0.1.1/bio_pypage.egg-info/SOURCES.txt
+-rw-r--r--   0 workspace   (502) staff       (20)        1 2023-06-16 08:26:13.000000 bio-pypage-0.1.1/bio_pypage.egg-info/dependency_links.txt
+-rw-r--r--   0 workspace   (502) staff       (20)      119 2023-06-16 08:26:13.000000 bio-pypage-0.1.1/bio_pypage.egg-info/requires.txt
+-rw-r--r--   0 workspace   (502) staff       (20)        7 2023-06-16 08:26:13.000000 bio-pypage-0.1.1/bio_pypage.egg-info/top_level.txt
+drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-16 08:26:13.554667 bio-pypage-0.1.1/pypage/
+-rw-r--r--   0 workspace   (502) staff       (20)      132 2023-06-15 22:20:27.000000 bio-pypage-0.1.1/pypage/__init__.py
+-rw-r--r--   0 workspace   (502) staff       (20)     9455 2023-06-15 14:51:03.000000 bio-pypage-0.1.1/pypage/heatmap.py
+-rw-r--r--   0 workspace   (502) staff       (20)     3657 2022-06-09 10:36:48.000000 bio-pypage-0.1.1/pypage/hist.py
+-rw-r--r--   0 workspace   (502) staff       (20)    12550 2022-06-29 13:50:11.000000 bio-pypage-0.1.1/pypage/information.py
+-rw-r--r--   0 workspace   (502) staff       (20)    15280 2023-06-15 21:49:50.000000 bio-pypage-0.1.1/pypage/page.py
+-rw-r--r--   0 workspace   (502) staff       (20)     3909 2022-06-09 13:50:18.000000 bio-pypage-0.1.1/pypage/utils.py
+-rw-r--r--   0 workspace   (502) staff       (20)       38 2023-06-16 08:26:13.555657 bio-pypage-0.1.1/setup.cfg
+-rw-r--r--   0 workspace   (502) staff       (20)      889 2023-06-16 08:25:49.000000 bio-pypage-0.1.1/setup.py
```

### Comparing `bio-pypage-0.1.0/LICENSE` & `bio-pypage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.0/PKG-INFO` & `bio-pypage-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-pypage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of the PAGE algorithm
 Home-page: https://github.com/noamteyssier/pypage
 Author: Artemy Bakulin, Noam Teyssier
 Author-email: logic2000.bakulin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -141,15 +141,15 @@
     hm.show(show_reg=True)
     
     return results
 ```
 
 ## Manual
 
-For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/noamteyssier/pypage/MANUAL.md).
+For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/noamteyssier/pyPAGE/MANUAL.md).
 
 ## License
 MIT license
 
 ## Citing
 See the paper
```

### Comparing `bio-pypage-0.1.0/README.md` & `bio-pypage-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     hm.show(show_reg=True)
     
     return results
 ```
 
 ## Manual
 
-For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/noamteyssier/pypage/MANUAL.md).
+For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/noamteyssier/pyPAGE/MANUAL.md).
 
 ## License
 MIT license
 
 ## Citing
 See the paper
```

### Comparing `bio-pypage-0.1.0/bio_pypage.egg-info/PKG-INFO` & `bio-pypage-0.1.1/bio_pypage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-pypage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of the PAGE algorithm
 Home-page: https://github.com/noamteyssier/pypage
 Author: Artemy Bakulin, Noam Teyssier
 Author-email: logic2000.bakulin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -141,15 +141,15 @@
     hm.show(show_reg=True)
     
     return results
 ```
 
 ## Manual
 
-For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/noamteyssier/pypage/MANUAL.md).
+For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/noamteyssier/pyPAGE/MANUAL.md).
 
 ## License
 MIT license
 
 ## Citing
 See the paper
```

### Comparing `bio-pypage-0.1.0/pypage/heatmap.py` & `bio-pypage-0.1.1/pypage/heatmap.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.0/pypage/hist.py` & `bio-pypage-0.1.1/pypage/hist.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.0/pypage/information.py` & `bio-pypage-0.1.1/pypage/information.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.0/pypage/page.py` & `bio-pypage-0.1.1/pypage/page.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.0/pypage/utils.py` & `bio-pypage-0.1.1/pypage/utils.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.0/setup.py` & `bio-pypage-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
    name='bio-pypage',
-   version='0.1.0',
+   version='0.1.1',
    description='Python implementation of the PAGE algorithm',
    author='Artemy Bakulin, Noam Teyssier',
    long_description=long_description,
    long_description_content_type="text/markdown",
    url='https://github.com/noamteyssier/pypage',
    author_email="logic2000.bakulin@gmail.com",
    packages=['pypage'],
```

