# Comparing `tmp/FlyBaseDownloads-1.0.4.3.tar.gz` & `tmp/FlyBaseDownloads-1.0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyBaseDownloads-1.0.4.3.tar", last modified: Thu Jun 15 22:45:45 2023, max compression
+gzip compressed data, was "FlyBaseDownloads-1.0.4.4.tar", last modified: Thu Jun 15 22:56:11 2023, max compression
```

## Comparing `FlyBaseDownloads-1.0.4.3.tar` & `FlyBaseDownloads-1.0.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:45:45.126484 FlyBaseDownloads-1.0.4.3/
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:45:45.126484 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     4787 2023-06-15 22:18:16.000000 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads/Downloads.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1502 2023-06-15 22:45:23.000000 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads/FBD.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      612 2023-06-15 22:40:21.000000 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:45:45.126484 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads.egg-info/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:45:45.000000 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      310 2023-06-15 22:45:45.000000 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-15 22:45:45.000000 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-15 22:45:45.000000 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-15 22:45:45.000000 FlyBaseDownloads-1.0.4.3/FlyBaseDownloads.egg-info/top_level.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:45:45.130484 FlyBaseDownloads-1.0.4.3/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.4.3/README.md
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-15 22:45:45.130484 FlyBaseDownloads-1.0.4.3/setup.cfg
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      919 2023-06-15 22:45:31.000000 FlyBaseDownloads-1.0.4.3/setup.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:56:11.965438 FlyBaseDownloads-1.0.4.4/
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:56:11.965438 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     4787 2023-06-15 22:18:16.000000 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads/Downloads.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1497 2023-06-15 22:52:26.000000 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads/FBD.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      616 2023-06-15 22:52:52.000000 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:56:11.965438 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads.egg-info/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:56:11.000000 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      310 2023-06-15 22:56:11.000000 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-15 22:56:11.000000 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-15 22:56:11.000000 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-15 22:56:11.000000 FlyBaseDownloads-1.0.4.4/FlyBaseDownloads.egg-info/top_level.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:56:11.965438 FlyBaseDownloads-1.0.4.4/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.4.4/README.md
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-15 22:56:11.969438 FlyBaseDownloads-1.0.4.4/setup.cfg
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      919 2023-06-15 22:55:22.000000 FlyBaseDownloads-1.0.4.4/setup.py
```

### Comparing `FlyBaseDownloads-1.0.4.3/FlyBaseDownloads/Downloads.py` & `FlyBaseDownloads-1.0.4.4/FlyBaseDownloads/Downloads.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4.3/FlyBaseDownloads/FBD.py` & `FlyBaseDownloads-1.0.4.4/FlyBaseDownloads/FBD.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Jun 12 12:42:17 2023
 
 @author: javiera.quiroz
 """
 
-from classes.Synonyms import Synonyms
-from FlyBaseDownloads.classes.Genes import Genes
-from classes.Gene_Ontology_annotation import Gene_Ontology_annotation
-from classes.Gene_groups import Gene_groups
-from classes.Homologs import Homologs
-from classes.Ontology_Terms import Ontology_Terms
-from classes.Organisms import Organisms
-from classes.Insertions import Insertions
-from classes.Clones import Clones
-from classes.References import References
-from classes.Alleles_Stocks import Alleles_Stocks
-from classes.Human_disease import Human_disease
+from .classes.Synonyms import Synonyms
+from .classes.Genes import Genes
+from .classes.Gene_Ontology_annotation import Gene_Ontology_annotation
+from .classes.Gene_groups import Gene_groups
+from .classes.Homologs import Homologs
+from .classes.Ontology_Terms import Ontology_Terms
+from .classes.Organisms import Organisms
+from .classes.Insertions import Insertions
+from .classes.Clones import Clones
+from .classes.References import References
+from .classes.Alleles_Stocks import Alleles_Stocks
+from .classes.Human_disease import Human_disease
 
 
 
 class FBD():
     
     def __name__(self):
         self.__name__ = 'FlyBase Downloads'
```

### Comparing `FlyBaseDownloads-1.0.4.3/FlyBaseDownloads/__init__.py` & `FlyBaseDownloads-1.0.4.4/FlyBaseDownloads/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Jun 13 17:35:44 2023
 
 @author: javiera.quiroz
 """
 
-from FlyBaseDownloads import FBD 
+from FlyBaseDownloads.FBD import FBD 
 
 db = FBD()
 
 #Synonyms
 Synonyms = db.Synonyms
 
 #Genes
```

### Comparing `FlyBaseDownloads-1.0.4.3/FlyBaseDownloads.egg-info/PKG-INFO` & `FlyBaseDownloads-1.0.4.4/FlyBaseDownloads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.4.3
+Version: 1.0.4.4
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FlyBaseDownloads-1.0.4.3/PKG-INFO` & `FlyBaseDownloads-1.0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.4.3
+Version: 1.0.4.4
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FlyBaseDownloads-1.0.4.3/README.md` & `FlyBaseDownloads-1.0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4.3/setup.py` & `FlyBaseDownloads-1.0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: javiera.quiroz
 """
 
 from setuptools import setup
 
 setup(
     name='FlyBaseDownloads',
-    version='1.0.4.3',
+    version='1.0.4.4',
     license='MIT',
     author='Javiera Quiroz Olave',
     url= 'https://github.com/JavieraQuirozO/FlyBaseDownloads',
     author_email='javiera.quiroz@biomedica.udec.cl',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=open('requirements.txt').readlines(),
```

