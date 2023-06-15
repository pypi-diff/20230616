# Comparing `tmp/FlyBaseDownloads-1.0.4.1.tar.gz` & `tmp/FlyBaseDownloads-1.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyBaseDownloads-1.0.4.1.tar", last modified: Thu Jun 15 22:32:44 2023, max compression
+gzip compressed data, was "FlyBaseDownloads-1.0.4.2.tar", last modified: Thu Jun 15 22:43:43 2023, max compression
```

## Comparing `FlyBaseDownloads-1.0.4.1.tar` & `FlyBaseDownloads-1.0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:32:44.407765 FlyBaseDownloads-1.0.4.1/
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:32:44.403765 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     4787 2023-06-15 22:18:16.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/Downloads.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1689 2023-06-15 21:50:47.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/FBD.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      616 2023-06-15 21:50:54.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:32:44.407765 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      310 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/top_level.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:32:44.407765 FlyBaseDownloads-1.0.4.1/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.4.1/README.md
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-15 22:32:44.407765 FlyBaseDownloads-1.0.4.1/setup.cfg
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      919 2023-06-15 22:32:05.000000 FlyBaseDownloads-1.0.4.1/setup.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:43:43.412738 FlyBaseDownloads-1.0.4.2/
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:43:43.412738 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     4787 2023-06-15 22:18:16.000000 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads/Downloads.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1502 2023-06-15 22:42:40.000000 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads/FBD.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      612 2023-06-15 22:40:21.000000 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:43:43.412738 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads.egg-info/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:43:43.000000 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      310 2023-06-15 22:43:43.000000 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-15 22:43:43.000000 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-15 22:43:43.000000 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-15 22:43:43.000000 FlyBaseDownloads-1.0.4.2/FlyBaseDownloads.egg-info/top_level.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:43:43.412738 FlyBaseDownloads-1.0.4.2/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.4.2/README.md
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-15 22:43:43.416738 FlyBaseDownloads-1.0.4.2/setup.cfg
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      919 2023-06-15 22:38:26.000000 FlyBaseDownloads-1.0.4.2/setup.py
```

### Comparing `FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/Downloads.py` & `FlyBaseDownloads-1.0.4.2/FlyBaseDownloads/Downloads.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/FBD.py` & `FlyBaseDownloads-1.0.4.2/FlyBaseDownloads/FBD.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 """
 Created on Mon Jun 12 12:42:17 2023
 
 @author: javiera.quiroz
 """
 
 from FlyBaseDownloads.classes.Synonyms import Synonyms
-from FlyBaseDownloads.classes.Genes import Genes
-from FlyBaseDownloads.classes.Gene_Ontology_annotation import Gene_Ontology_annotation
-from FlyBaseDownloads.classes.Gene_groups import Gene_groups
-from FlyBaseDownloads.classes.Homologs import Homologs
-from FlyBaseDownloads.classes.Ontology_Terms import Ontology_Terms
-from FlyBaseDownloads.classes.Organisms import Organisms
-from FlyBaseDownloads.classes.Insertions import Insertions
-from FlyBaseDownloads.classes.Clones import Clones
-from FlyBaseDownloads.classes.References import References
-from FlyBaseDownloads.classes.Alleles_Stocks import Alleles_Stocks
-from FlyBaseDownloads.classes.Human_disease import Human_disease
+from classes.Genes import Genes
+from classes.Gene_Ontology_annotation import Gene_Ontology_annotation
+from classes.Gene_groups import Gene_groups
+from classes.Homologs import Homologs
+from classes.Ontology_Terms import Ontology_Terms
+from classes.Organisms import Organisms
+from classes.Insertions import Insertions
+from classes.Clones import Clones
+from classes.References import References
+from classes.Alleles_Stocks import Alleles_Stocks
+from classes.Human_disease import Human_disease
 
 
 
 class FBD():
     
     def __name__(self):
         self.__name__ = 'FlyBase Downloads'
```

### Comparing `FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/__init__.py` & `FlyBaseDownloads-1.0.4.2/FlyBaseDownloads/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Jun 13 17:35:44 2023
 
 @author: javiera.quiroz
 """
 
-from FlyBaseDownloads.FBD import FBD 
+from FlyBaseDownloads import FBD 
 
 db = FBD()
 
 #Synonyms
 Synonyms = db.Synonyms
 
 #Genes
```

### Comparing `FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/PKG-INFO` & `FlyBaseDownloads-1.0.4.2/FlyBaseDownloads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.4.1
+Version: 1.0.4.2
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FlyBaseDownloads-1.0.4.1/PKG-INFO` & `FlyBaseDownloads-1.0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.4.1
+Version: 1.0.4.2
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FlyBaseDownloads-1.0.4.1/README.md` & `FlyBaseDownloads-1.0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4.1/setup.py` & `FlyBaseDownloads-1.0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: javiera.quiroz
 """
 
 from setuptools import setup
 
 setup(
     name='FlyBaseDownloads',
-    version='1.0.4.1',
+    version='1.0.4.2',
     license='MIT',
     author='Javiera Quiroz Olave',
     url= 'https://github.com/JavieraQuirozO/FlyBaseDownloads',
     author_email='javiera.quiroz@biomedica.udec.cl',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=open('requirements.txt').readlines(),
```

