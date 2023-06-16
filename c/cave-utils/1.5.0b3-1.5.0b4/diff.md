# Comparing `tmp/cave_utils-1.5.0b3.tar.gz` & `tmp/cave_utils-1.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-1.5.0b3.tar", last modified: Thu Jun 15 19:05:09 2023, max compression
+gzip compressed data, was "cave_utils-1.5.0b4.tar", last modified: Fri Jun 16 14:33:38 2023, max compression
```

## Comparing `cave_utils-1.5.0b3.tar` & `cave_utils-1.5.0b4.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b3/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b3/NOTICE.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b3/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 19:05:09.664970 cave_utils-1.5.0b3/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-06-13 15:24:05.000000 cave_utils-1.5.0b3/cave_utils/__init__ .py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-13 15:24:47.000000 cave_utils-1.5.0b3/cave_utils/socket.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    55892 2023-06-15 19:04:19.000000 cave_utils-1.5.0b3/cave_utils/validator.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/cave_utils.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      319 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b3/pyproject.toml
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      997 2023-06-15 19:03:56.000000 cave_utils-1.5.0b3/setup.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       46 2023-06-13 15:19:05.000000 cave_utils-1.5.0b3/test/test_import.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-16 14:33:38.003865 cave_utils-1.5.0b4/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b4/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b4/NOTICE.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-16 14:33:38.003865 cave_utils-1.5.0b4/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b4/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-16 14:33:38.003865 cave_utils-1.5.0b4/cave_utils.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-16 14:33:37.000000 cave_utils-1.5.0b4/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      250 2023-06-16 14:33:37.000000 cave_utils-1.5.0b4/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-06-16 14:33:37.000000 cave_utils-1.5.0b4/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-06-16 14:33:37.000000 cave_utils-1.5.0b4/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-06-16 14:33:37.000000 cave_utils-1.5.0b4/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b4/pyproject.toml
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-06-16 14:33:38.003865 cave_utils-1.5.0b4/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      997 2023-06-16 14:30:29.000000 cave_utils-1.5.0b4/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-16 14:33:38.003865 cave_utils-1.5.0b4/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       45 2023-06-16 14:29:05.000000 cave_utils-1.5.0b4/test/test_import.py
```

### Comparing `cave_utils-1.5.0b3/LICENSE` & `cave_utils-1.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b3/NOTICE.md` & `cave_utils-1.5.0b4/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b3/PKG-INFO` & `cave_utils-1.5.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 1.5.0b3
+Version: 1.5.0b4
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b3.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b4.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b3/README.md` & `cave_utils-1.5.0b4/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b3/cave_utils.egg-info/PKG-INFO` & `cave_utils-1.5.0b4/cave_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave-utils
-Version: 1.5.0b3
+Version: 1.5.0b4
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b3.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b4.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b3/setup.py` & `cave_utils-1.5.0b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'cave_utils',
   packages=['cave_utils'],
-  version = '1.5.0b3',
+  version = '1.5.0b4',
   license='MIT',
   description = 'Cave utilities for the CAVE App at the MIT',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/mit-cave/cave_utils',
-  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b3.tar.gz',
+  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b4.tar.gz',
   keywords = [],
   install_requires=[
     'pamda>=2.1.2',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

