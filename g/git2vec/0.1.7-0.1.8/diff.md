# Comparing `tmp/git2vec-0.1.7.tar.gz` & `tmp/git2vec-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2vec-0.1.7.tar", last modified: Fri Jun 16 19:32:47 2023, max compression
+gzip compressed data, was "git2vec-0.1.8.tar", last modified: Fri Jun 16 19:47:20 2023, max compression
```

## Comparing `git2vec-0.1.7.tar` & `git2vec-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 19:32:47.226318 git2vec-0.1.7/
--rw-rw-rw-   0        0        0     2701 2023-06-16 19:32:47.224950 git2vec-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2047 2023-06-16 18:53:23.000000 git2vec-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 19:32:47.198232 git2vec-0.1.7/git2vec/
--rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2vec-0.1.7/git2vec/__init__.py
--rw-rw-rw-   0        0        0     7607 2023-06-16 19:31:59.000000 git2vec-0.1.7/git2vec/loader.py
--rw-rw-rw-   0        0        0     3996 2023-06-09 14:25:12.000000 git2vec-0.1.7/git2vec/vectordb.py
-drwxrwxrwx   0        0        0        0 2023-06-16 19:32:47.221435 git2vec-0.1.7/git2vec.egg-info/
--rw-rw-rw-   0        0        0     2701 2023-06-16 19:32:47.000000 git2vec-0.1.7/git2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-16 19:32:47.000000 git2vec-0.1.7/git2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 19:32:47.000000 git2vec-0.1.7/git2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-06-16 19:32:47.000000 git2vec-0.1.7/git2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 19:32:47.000000 git2vec-0.1.7/git2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 19:32:47.227314 git2vec-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-06-16 19:32:10.000000 git2vec-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:47:20.861891 git2vec-0.1.8/
+-rw-rw-rw-   0        0        0     2701 2023-06-16 19:47:20.860895 git2vec-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2023-06-16 18:53:23.000000 git2vec-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 19:47:20.846494 git2vec-0.1.8/git2vec/
+-rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2vec-0.1.8/git2vec/__init__.py
+-rw-rw-rw-   0        0        0     7581 2023-06-16 19:45:41.000000 git2vec-0.1.8/git2vec/loader.py
+-rw-rw-rw-   0        0        0     3996 2023-06-09 14:25:12.000000 git2vec-0.1.8/git2vec/vectordb.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:47:20.856882 git2vec-0.1.8/git2vec.egg-info/
+-rw-rw-rw-   0        0        0     2701 2023-06-16 19:47:20.000000 git2vec-0.1.8/git2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-16 19:47:20.000000 git2vec-0.1.8/git2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:47:20.000000 git2vec-0.1.8/git2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-16 19:47:20.000000 git2vec-0.1.8/git2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 19:47:20.000000 git2vec-0.1.8/git2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 19:47:20.861891 git2vec-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-06-16 19:46:46.000000 git2vec-0.1.8/setup.py
```

### Comparing `git2vec-0.1.7/PKG-INFO` & `git2vec-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.7
+Version: 0.1.8
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2vec-0.1.7/README.md` & `git2vec-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.7/git2vec/loader.py` & `git2vec-0.1.8/git2vec/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     :return: The document or None if the file should be skipped.
     """
     if not isinstance(item, Blob):
         return None
 
     file_path = os.path.join(output_path, item.path)
 
-    if not map(lambda x: not any([x.endswith(t) for t in UNWANTED_TYPES]), file_path):
+    if any([file_path.endswith(t) for t in UNWANTED_TYPES]):
         return None
 
     rel_file_path = os.path.relpath(file_path, output_path)
     try:
         with open(file_path, "rb") as f:
             content = f.read()
             file_type = os.path.splitext(item.name)[1]
```

### Comparing `git2vec-0.1.7/git2vec/vectordb.py` & `git2vec-0.1.8/git2vec/vectordb.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.7/git2vec.egg-info/PKG-INFO` & `git2vec-0.1.8/git2vec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.7
+Version: 0.1.8
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2vec-0.1.7/setup.py` & `git2vec-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2vec',
-    version='0.1.7',
+    version='0.1.8',
     description='A useful module for handling Git data.',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2vec',
     packages=find_packages(),
     install_requires=[
         'langchain',
```

