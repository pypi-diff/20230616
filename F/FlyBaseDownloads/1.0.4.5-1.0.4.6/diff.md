# Comparing `tmp/FlyBaseDownloads-1.0.4.5.tar.gz` & `tmp/FlyBaseDownloads-1.0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyBaseDownloads-1.0.4.5.tar", last modified: Thu Jun 15 23:09:12 2023, max compression
+gzip compressed data, was "FlyBaseDownloads-1.0.4.6.tar", last modified: Thu Jun 15 23:25:32 2023, max compression
```

## Comparing `FlyBaseDownloads-1.0.4.5.tar` & `FlyBaseDownloads-1.0.4.6.tar`

### file list

```diff
@@ -1,15 +1,29 @@
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 23:09:12.304954 FlyBaseDownloads-1.0.4.5/
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 23:09:12.300954 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     4787 2023-06-15 22:18:16.000000 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads/Downloads.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1497 2023-06-15 22:52:26.000000 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads/FBD.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      616 2023-06-15 23:09:00.000000 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 23:09:12.304954 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads.egg-info/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 23:09:12.000000 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      310 2023-06-15 23:09:12.000000 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-15 23:09:12.000000 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-15 23:09:12.000000 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-15 23:09:12.000000 FlyBaseDownloads-1.0.4.5/FlyBaseDownloads.egg-info/top_level.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 23:09:12.304954 FlyBaseDownloads-1.0.4.5/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.4.5/README.md
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-15 23:09:12.304954 FlyBaseDownloads-1.0.4.5/setup.cfg
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      919 2023-06-15 23:08:56.000000 FlyBaseDownloads-1.0.4.5/setup.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 23:25:32.524129 FlyBaseDownloads-1.0.4.6/
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 23:25:32.520130 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     4787 2023-06-15 22:18:16.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/Downloads.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1497 2023-06-15 22:52:26.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/FBD.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      616 2023-06-15 23:09:00.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 23:25:32.524129 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1163 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Alleles_Stocks.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      782 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Clones.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1216 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Gene_Ontology_annotation.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      890 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Gene_groups.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     3621 2023-06-15 22:55:14.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Genes.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      761 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Homologs.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      821 2023-06-15 21:36:31.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Human_disease.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      798 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Insertions.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1277 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Ontology_Terms.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      522 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Organisms.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      572 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/References.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      513 2023-06-15 21:30:18.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/Synonyms.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       10 2023-06-15 23:11:35.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/classes/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 23:25:32.520130 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads.egg-info/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 23:25:32.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      827 2023-06-15 23:25:32.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-15 23:25:32.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-15 23:25:32.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-15 23:25:32.000000 FlyBaseDownloads-1.0.4.6/FlyBaseDownloads.egg-info/top_level.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 23:25:32.524129 FlyBaseDownloads-1.0.4.6/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.4.6/README.md
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-15 23:25:32.524129 FlyBaseDownloads-1.0.4.6/setup.cfg
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      947 2023-06-15 23:23:29.000000 FlyBaseDownloads-1.0.4.6/setup.py
```

### Comparing `FlyBaseDownloads-1.0.4.5/FlyBaseDownloads/Downloads.py` & `FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/Downloads.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4.5/FlyBaseDownloads/FBD.py` & `FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/FBD.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4.5/FlyBaseDownloads/__init__.py` & `FlyBaseDownloads-1.0.4.6/FlyBaseDownloads/__init__.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4.5/FlyBaseDownloads.egg-info/PKG-INFO` & `FlyBaseDownloads-1.0.4.6/FlyBaseDownloads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.4.5
+Version: 1.0.4.6
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FlyBaseDownloads-1.0.4.5/PKG-INFO` & `FlyBaseDownloads-1.0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.4.5
+Version: 1.0.4.6
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FlyBaseDownloads-1.0.4.5/README.md` & `FlyBaseDownloads-1.0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4.5/setup.py` & `FlyBaseDownloads-1.0.4.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 @author: javiera.quiroz
 """
 
 from setuptools import setup
 
 setup(
     name='FlyBaseDownloads',
-    version='1.0.4.5',
+    version='1.0.4.6',
     license='MIT',
     author='Javiera Quiroz Olave',
     url= 'https://github.com/JavieraQuirozO/FlyBaseDownloads',
     author_email='javiera.quiroz@biomedica.udec.cl',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=open('requirements.txt').readlines(),
     description='Package to download Flybase data in Python, easily and quickly.',
-    packages=['FlyBaseDownloads'],
+    packages=['FlyBaseDownloads', 'FlyBaseDownloads.classes'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Healthcare Industry',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
```

