# Comparing `tmp/kanglib-0.3.tar.gz` & `tmp/kanglib-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanglib-0.3.tar", last modified: Thu Jun 15 15:40:50 2023, max compression
+gzip compressed data, was "kanglib-0.4.tar", last modified: Thu Jun 15 22:16:56 2023, max compression
```

## Comparing `kanglib-0.3.tar` & `kanglib-0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:40:50.938034 kanglib-0.3/
--rw-r--r--   0 kang       (501) staff       (20)      401 2023-06-15 15:40:50.937931 kanglib-0.3/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      163 2023-06-15 15:40:46.000000 kanglib-0.3/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:40:50.937240 kanglib-0.3/kanglib/
--rw-r--r--   0 kang       (501) staff       (20)      121 2023-06-15 15:35:23.000000 kanglib-0.3/kanglib/__init__.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:40:50.937808 kanglib-0.3/kanglib.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      401 2023-06-15 15:40:50.000000 kanglib-0.3/kanglib.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      162 2023-06-15 15:40:50.000000 kanglib-0.3/kanglib.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-15 15:40:50.000000 kanglib-0.3/kanglib.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)        8 2023-06-15 15:40:50.000000 kanglib-0.3/kanglib.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-15 15:40:50.938066 kanglib-0.3/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      525 2023-06-15 15:37:59.000000 kanglib-0.3/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:16:56.743924 kanglib-0.4/
+-rw-r--r--   0 kang       (501) staff       (20)     1809 2023-06-15 22:16:56.743820 kanglib-0.4/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     1531 2023-06-15 22:12:18.000000 kanglib-0.4/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:16:56.743120 kanglib-0.4/kanglib/
+-rw-r--r--   0 kang       (501) staff       (20)      121 2023-06-15 15:35:23.000000 kanglib-0.4/kanglib/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      658 2023-06-15 22:09:31.000000 kanglib-0.4/kanglib/calculations.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:16:56.743691 kanglib-0.4/kanglib.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)     1809 2023-06-15 22:16:56.000000 kanglib-0.4/kanglib.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      186 2023-06-15 22:16:56.000000 kanglib-0.4/kanglib.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-15 22:16:56.000000 kanglib-0.4/kanglib.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)        8 2023-06-15 22:16:56.000000 kanglib-0.4/kanglib.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-15 22:16:56.743952 kanglib-0.4/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      595 2023-06-15 22:16:48.000000 kanglib-0.4/setup.py
```

### Comparing `kanglib-0.3/setup.py` & `kanglib-0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kanglib',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     description='Kang lib of Python package: calculate my math function',
     long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',  # 添加这一行
     url='https://github.com/williampolicy/code_pypi',
     author='xiaowen kang',
     author_email='kangxiaowen@gmail.com',
     license='MIT',
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

