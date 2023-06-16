# Comparing `tmp/Pyara-0.1.19.tar.gz` & `tmp/Pyara-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pyara-0.1.19.tar", last modified: Wed Jun 14 09:04:27 2023, max compression
+gzip compressed data, was "dist\Pyara-0.1.25.tar", last modified: Fri Jun 16 10:58:59 2023, max compression
```

## Comparing `Pyara-0.1.19.tar` & `Pyara-0.1.25.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:04:27.000000 Pyara-0.1.19/
--rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.19/LICENSE
--rw-rw-rw-   0        0        0      539 2023-06-14 09:04:27.000000 Pyara-0.1.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/
--rw-rw-rw-   0        0        0      539 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.19/Pyara.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.19/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 09:04:27.000000 Pyara-0.1.19/pyara/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:04:27.000000 Pyara-0.1.19/pyara/Model/
--rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.19/pyara/Model/__init__.py
--rw-rw-rw-   0        0        0     3989 2023-06-14 08:53:51.000000 Pyara-0.1.19/pyara/Model/model.py
--rw-rw-rw-   0        0        0      350 2023-06-14 09:04:25.000000 Pyara-0.1.19/pyara/__init__.py
--rw-rw-rw-   0        0        0     6412 2023-06-14 08:53:51.000000 Pyara-0.1.19/pyara/audio_prepare.py
--rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.19/pyara/config.py
--rw-rw-rw-   0        0        0      836 2023-06-14 08:53:51.000000 Pyara-0.1.19/pyara/main.py
--rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.19/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 09:04:27.000000 Pyara-0.1.19/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-06-14 09:04:25.000000 Pyara-0.1.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:58:59.000000 Pyara-0.1.25/
+-rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.25/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-06-16 10:56:25.000000 Pyara-0.1.25/MANIFEST.in
+-rw-rw-rw-   0        0        0      539 2023-06-16 10:58:59.000000 Pyara-0.1.25/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 10:58:59.000000 Pyara-0.1.25/Pyara.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-16 10:58:59.000000 Pyara-0.1.25/Pyara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-06-16 10:58:59.000000 Pyara-0.1.25/Pyara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 10:58:59.000000 Pyara-0.1.25/Pyara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.25/Pyara.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-06-16 10:58:59.000000 Pyara-0.1.25/Pyara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 10:58:59.000000 Pyara-0.1.25/Pyara.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.25/README.md
+-rw-rw-rw-   0        0        0      950 2023-06-11 12:54:48.000000 Pyara-0.1.25/instruct.txt
+-rw-rw-rw-   0        0        0    92204 2023-03-28 18:31:37.000000 Pyara-0.1.25/mozila11_1.wav
+-rw-rw-rw-   0        0        0   164396 2023-03-28 18:37:21.000000 Pyara-0.1.25/mozila11_2.wav
+drwxrwxrwx   0        0        0        0 2023-06-16 10:58:59.000000 Pyara-0.1.25/pyara/
+drwxrwxrwx   0        0        0        0 2023-06-16 10:58:59.000000 Pyara-0.1.25/pyara/Model/
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.25/pyara/Model/__init__.py
+-rw-rw-rw-   0        0        0     3989 2023-06-14 08:53:51.000000 Pyara-0.1.25/pyara/Model/model.py
+-rw-rw-rw-   0        0        0  1075221 2023-04-03 12:30:41.000000 Pyara-0.1.25/pyara/Model_weights.bin
+-rw-rw-rw-   0        0        0      350 2023-06-14 09:04:25.000000 Pyara-0.1.25/pyara/__init__.py
+-rw-rw-rw-   0        0        0     6412 2023-06-14 08:53:51.000000 Pyara-0.1.25/pyara/audio_prepare.py
+-rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.25/pyara/config.py
+-rw-rw-rw-   0        0        0      836 2023-06-14 08:53:51.000000 Pyara-0.1.25/pyara/main.py
+-rw-rw-rw-   0        0        0   184364 2023-03-28 18:31:37.000000 Pyara-0.1.25/pyara/mozila11_0.wav
+-rw-rw-rw-   0        0        0       28 2023-06-14 09:11:56.000000 Pyara-0.1.25/pyara/some.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.25/pyproject.toml
+-rw-rw-rw-   0        0        0      276 2023-05-28 20:41:04.000000 Pyara-0.1.25/requirements.txt
+-rw-rw-rw-   0        0        0      131 2023-05-30 08:51:00.000000 Pyara-0.1.25/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 10:58:59.000000 Pyara-0.1.25/setup.cfg
+-rw-rw-rw-   0        0        0     1116 2023-06-16 10:58:49.000000 Pyara-0.1.25/setup.py
```

### Comparing `Pyara-0.1.19/LICENSE` & `Pyara-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.19/PKG-INFO` & `Pyara-0.1.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.19
+Version: 0.1.25
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.19/Pyara.egg-info/PKG-INFO` & `Pyara-0.1.25/Pyara.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.19
+Version: 0.1.25
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.19/pyara/Model/model.py` & `Pyara-0.1.25/pyara/Model/model.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.19/pyara/audio_prepare.py` & `Pyara-0.1.25/pyara/audio_prepare.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.19/pyara/config.py` & `Pyara-0.1.25/pyara/config.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.19/pyara/main.py` & `Pyara-0.1.25/pyara/main.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.19/setup.py` & `Pyara-0.1.25/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Metadata of package"""
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages   # ,  pkg_resources
 
 requirements = ['torch>=1.13.1',
                 'torchaudio>=0.13.1'
                 ]
 
 # Создаст библиотеку для загрузки на PyPI
 setup(name='Pyara',
-      version='0.1.19',
+      version='0.1.25',
       url='https://github.com/Millcool/Pyara.git',
       license='MIT',
       author='Ilya Mironov',
       author_email='ilyamironov210202@gmail.com',
       description='Library for audio classification',
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
-      packages=find_packages( exclude=['tests']), #where='src', include=['pyara*'],
+      packages=find_packages(exclude=['tests']), #where='src', include=['pyara*'],
+      #package_dir={"":"src"},
+      package_data={"pyara": ["*.bin"]},
+      include_package_data=True,
       zip_safe=False,
       install_requires=requirements,
       platform='Any',
       classifiers=[
           "Programming Language :: Python :: 3.7",
           "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
           "Operating System :: OS Independent"
```

