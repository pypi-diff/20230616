# Comparing `tmp/git2vec-0.1.3.tar.gz` & `tmp/git2vec-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2vec-0.1.3.tar", last modified: Fri Jun  9 14:01:50 2023, max compression
+gzip compressed data, was "git2vec-0.1.4.tar", last modified: Fri Jun 16 17:59:31 2023, max compression
```

## Comparing `git2vec-0.1.3.tar` & `git2vec-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 14:01:50.107738 git2vec-0.1.3/
--rw-rw-rw-   0        0        0     2805 2023-06-09 14:01:50.106736 git2vec-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2151 2023-06-03 12:01:57.000000 git2vec-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 14:01:50.091687 git2vec-0.1.3/git2vec/
--rw-rw-rw-   0        0        0        0 2023-06-03 12:01:57.000000 git2vec-0.1.3/git2vec/__init__.py
--rw-rw-rw-   0        0        0     4805 2023-06-09 14:01:22.000000 git2vec-0.1.3/git2vec/loader.py
--rw-rw-rw-   0        0        0     3996 2023-06-03 12:01:57.000000 git2vec-0.1.3/git2vec/vectordb.py
-drwxrwxrwx   0        0        0        0 2023-06-09 14:01:50.103737 git2vec-0.1.3/git2vec.egg-info/
--rw-rw-rw-   0        0        0     2805 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 14:01:50.108740 git2vec-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-06-09 14:01:33.000000 git2vec-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:59:31.218937 git2vec-0.1.4/
+-rw-rw-rw-   0        0        0     2805 2023-06-16 17:59:31.216941 git2vec-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2151 2023-06-09 14:25:12.000000 git2vec-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 17:59:31.191349 git2vec-0.1.4/git2vec/
+-rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2vec-0.1.4/git2vec/__init__.py
+-rw-rw-rw-   0        0        0     7697 2023-06-16 17:49:11.000000 git2vec-0.1.4/git2vec/loader.py
+-rw-rw-rw-   0        0        0     3996 2023-06-09 14:25:12.000000 git2vec-0.1.4/git2vec/vectordb.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:59:31.214921 git2vec-0.1.4/git2vec.egg-info/
+-rw-rw-rw-   0        0        0     2805 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 17:59:31.218937 git2vec-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2023-06-16 17:59:23.000000 git2vec-0.1.4/setup.py
```

### Comparing `git2vec-0.1.3/PKG-INFO` & `git2vec-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.3
+Version: 0.1.4
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2vec-0.1.3/README.md` & `git2vec-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.3/git2vec/vectordb.py` & `git2vec-0.1.4/git2vec/vectordb.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.3/git2vec.egg-info/PKG-INFO` & `git2vec-0.1.4/git2vec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.3
+Version: 0.1.4
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2vec-0.1.3/setup.py` & `git2vec-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2vec',
-    version='0.1.3',
+    version='0.1.4',
     description='A useful module for handling Git data.',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2vec',
     packages=find_packages(),
     install_requires=[
         'langchain',
         'pinecone-client',
         'tiktoken',
         'gitpython'
+        "python-dotenv",
+        "pandas",
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',  
         'Intended Audience :: Developers',  
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  
         'Programming Language :: Python :: 3.6',
```

