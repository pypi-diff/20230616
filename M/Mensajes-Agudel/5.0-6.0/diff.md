# Comparing `tmp/Mensajes-Agudel-5.0.tar.gz` & `tmp/Mensajes-Agudel-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-Agudel-5.0.tar", last modified: Fri Jun 16 01:46:31 2023, max compression
+gzip compressed data, was "Mensajes-Agudel-6.0.tar", last modified: Fri Jun 16 01:57:08 2023, max compression
```

## Comparing `Mensajes-Agudel-5.0.tar` & `Mensajes-Agudel-6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 01:46:31.692604 Mensajes-Agudel-5.0/
--rw-rw-rw-   0        0        0      823 2023-06-16 01:25:50.000000 Mensajes-Agudel-5.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-06-16 01:26:31.000000 Mensajes-Agudel-5.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-16 01:46:31.676652 Mensajes-Agudel-5.0/Mensajes_Agudel.egg-info/
--rw-rw-rw-   0        0        0      707 2023-06-16 01:46:31.000000 Mensajes-Agudel-5.0/Mensajes_Agudel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-06-16 01:46:31.000000 Mensajes-Agudel-5.0/Mensajes_Agudel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 01:46:31.000000 Mensajes-Agudel-5.0/Mensajes_Agudel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-16 01:46:31.000000 Mensajes-Agudel-5.0/Mensajes_Agudel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-16 01:46:31.000000 Mensajes-Agudel-5.0/Mensajes_Agudel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      707 2023-06-16 01:46:31.691633 Mensajes-Agudel-5.0/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-16 01:21:58.000000 Mensajes-Agudel-5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 01:46:31.678653 Mensajes-Agudel-5.0/mensajes/
--rw-rw-rw-   0        0        0       37 2023-06-01 13:46:37.000000 Mensajes-Agudel-5.0/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:46:31.682661 Mensajes-Agudel-5.0/mensajes/adios/
--rw-rw-rw-   0        0        0       46 2023-06-01 13:53:46.000000 Mensajes-Agudel-5.0/mensajes/adios/__init__.py
--rw-rw-rw-   0        0        0      183 2023-06-01 13:52:31.000000 Mensajes-Agudel-5.0/mensajes/adios/despedidas.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:46:31.686647 Mensajes-Agudel-5.0/mensajes/hola/
--rw-rw-rw-   0        0        0       45 2023-06-01 13:48:45.000000 Mensajes-Agudel-5.0/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-15 23:07:53.000000 Mensajes-Agudel-5.0/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       13 2023-06-15 23:12:09.000000 Mensajes-Agudel-5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 01:46:31.692604 Mensajes-Agudel-5.0/setup.cfg
--rw-rw-rw-   0        0        0      977 2023-06-16 01:45:54.000000 Mensajes-Agudel-5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:46:31.689638 Mensajes-Agudel-5.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-15 23:34:42.000000 Mensajes-Agudel-5.0/tests/__init__.py
--rw-rw-rw-   0        0        0      645 2023-06-15 23:35:59.000000 Mensajes-Agudel-5.0/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:57:08.670393 Mensajes-Agudel-6.0/
+-rw-rw-rw-   0        0        0      823 2023-06-16 01:25:50.000000 Mensajes-Agudel-6.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-06-16 01:26:31.000000 Mensajes-Agudel-6.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-16 01:57:08.652856 Mensajes-Agudel-6.0/Mensajes_Agudel.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-06-16 01:57:08.000000 Mensajes-Agudel-6.0/Mensajes_Agudel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-06-16 01:57:08.000000 Mensajes-Agudel-6.0/Mensajes_Agudel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 01:57:08.000000 Mensajes-Agudel-6.0/Mensajes_Agudel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-16 01:57:08.000000 Mensajes-Agudel-6.0/Mensajes_Agudel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-16 01:57:08.000000 Mensajes-Agudel-6.0/Mensajes_Agudel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      707 2023-06-16 01:57:08.669420 Mensajes-Agudel-6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-16 01:21:58.000000 Mensajes-Agudel-6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 01:57:08.654853 Mensajes-Agudel-6.0/mensajes/
+-rw-rw-rw-   0        0        0       37 2023-06-01 13:46:37.000000 Mensajes-Agudel-6.0/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:57:08.658842 Mensajes-Agudel-6.0/mensajes/adios/
+-rw-rw-rw-   0        0        0       46 2023-06-01 13:53:46.000000 Mensajes-Agudel-6.0/mensajes/adios/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-06-01 13:52:31.000000 Mensajes-Agudel-6.0/mensajes/adios/despedidas.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:57:08.663413 Mensajes-Agudel-6.0/mensajes/hola/
+-rw-rw-rw-   0        0        0       45 2023-06-01 13:48:45.000000 Mensajes-Agudel-6.0/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      426 2023-06-16 01:56:08.000000 Mensajes-Agudel-6.0/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       13 2023-06-15 23:12:09.000000 Mensajes-Agudel-6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 01:57:08.670393 Mensajes-Agudel-6.0/setup.cfg
+-rw-rw-rw-   0        0        0      977 2023-06-16 01:56:20.000000 Mensajes-Agudel-6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:57:08.667401 Mensajes-Agudel-6.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-15 23:34:42.000000 Mensajes-Agudel-6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      645 2023-06-15 23:35:59.000000 Mensajes-Agudel-6.0/tests/test_hola.py
```

### Comparing `Mensajes-Agudel-5.0/LICENSE` & `Mensajes-Agudel-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-Agudel-5.0/Mensajes_Agudel.egg-info/PKG-INFO` & `Mensajes-Agudel-6.0/Mensajes_Agudel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-Agudel
-Version: 5.0
+Version: 6.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.hektor.dev
 Author: Agustin Delgue
 Author-email: hola@hektor.dev
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Mensajes-Agudel-5.0/PKG-INFO` & `Mensajes-Agudel-6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-Agudel
-Version: 5.0
+Version: 6.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.hektor.dev
 Author: Agustin Delgue
 Author-email: hola@hektor.dev
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Mensajes-Agudel-5.0/setup.py` & `Mensajes-Agudel-6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Mensajes-Agudel',
-    version='5.0',
+    version='6.0',
     description='Un paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Agustin Delgue',
     author_email='hola@hektor.dev',
     url='https://www.hektor.dev',
     license_files=['LICENSE'],
```

### Comparing `Mensajes-Agudel-5.0/tests/test_hola.py` & `Mensajes-Agudel-6.0/tests/test_hola.py`

 * *Files identical despite different names*

