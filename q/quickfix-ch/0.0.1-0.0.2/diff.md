# Comparing `tmp/quickfix-ch-0.0.1.tar.gz` & `tmp/quickfix-ch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfix-ch-0.0.1.tar", last modified: Fri Jun 16 08:25:01 2023, max compression
+gzip compressed data, was "quickfix-ch-0.0.2.tar", last modified: Fri Jun 16 09:04:36 2023, max compression
```

## Comparing `quickfix-ch-0.0.1.tar` & `quickfix-ch-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 08:25:01.464609 quickfix-ch-0.0.1/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 08:25:01.464298 quickfix-ch-0.0.1/PKG-INFO
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 08:25:01.462123 quickfix-ch-0.0.1/quickfix/
--rw-r--r--   0 javierphon   (503) staff       (20)        0 2023-06-16 08:14:55.000000 quickfix-ch-0.0.1/quickfix/__init__.py
--rw-r--r--   0 javierphon   (503) staff       (20)  2064364 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix.py
--rw-r--r--   0 javierphon   (503) staff       (20)     4825 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix40.py
--rw-r--r--   0 javierphon   (503) staff       (20)     6232 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix41.py
--rw-r--r--   0 javierphon   (503) staff       (20)    21580 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix42.py
--rw-r--r--   0 javierphon   (503) staff       (20)    64741 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix43.py
--rw-r--r--   0 javierphon   (503) staff       (20)   262984 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix44.py
--rw-r--r--   0 javierphon   (503) staff       (20)   379998 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix50.py
--rw-r--r--   0 javierphon   (503) staff       (20)   449402 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix50sp1.py
--rw-r--r--   0 javierphon   (503) staff       (20)   532344 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfix50sp2.py
--rw-r--r--   0 javierphon   (503) staff       (20)     1223 2023-06-16 07:59:37.000000 quickfix-ch-0.0.1/quickfix/quickfixt11.py
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 08:25:01.463660 quickfix-ch-0.0.1/quickfix_ch.egg-info/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 08:25:01.000000 quickfix-ch-0.0.1/quickfix_ch.egg-info/PKG-INFO
--rw-r--r--   0 javierphon   (503) staff       (20)      404 2023-06-16 08:25:01.000000 quickfix-ch-0.0.1/quickfix_ch.egg-info/SOURCES.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 08:25:01.000000 quickfix-ch-0.0.1/quickfix_ch.egg-info/dependency_links.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        9 2023-06-16 08:25:01.000000 quickfix-ch-0.0.1/quickfix_ch.egg-info/top_level.txt
--rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 08:25:01.464963 quickfix-ch-0.0.1/setup.cfg
--rw-r--r--   0 javierphon   (503) staff       (20)      859 2023-06-16 08:24:44.000000 quickfix-ch-0.0.1/setup.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 09:04:36.306913 quickfix-ch-0.0.2/
+-rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 09:04:36.306408 quickfix-ch-0.0.2/PKG-INFO
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 09:04:36.301699 quickfix-ch-0.0.2/quickfix/
+-rw-r--r--   0 javierphon   (503) staff       (20)        0 2023-06-16 08:14:55.000000 quickfix-ch-0.0.2/quickfix/__init__.py
+-rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.2/quickfix/_quickfix.13.so
+-rwxr-xr-x   0 javierphon   (503) staff       (20)     1000 2023-06-16 07:59:51.000000 quickfix-ch-0.0.2/quickfix/_quickfix.la
+-rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.2/quickfix/_quickfix.so
+-rw-r--r--   0 javierphon   (503) staff       (20)  2064364 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     4825 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix40.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     6232 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix41.py
+-rw-r--r--   0 javierphon   (503) staff       (20)    21580 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix42.py
+-rw-r--r--   0 javierphon   (503) staff       (20)    64741 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix43.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   262984 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix44.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   379998 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix50.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   449402 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix50sp1.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   532344 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfix50sp2.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     1223 2023-06-16 07:59:37.000000 quickfix-ch-0.0.2/quickfix/quickfixt11.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 09:04:36.305348 quickfix-ch-0.0.2/quickfix_ch.egg-info/
+-rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 09:04:36.000000 quickfix-ch-0.0.2/quickfix_ch.egg-info/PKG-INFO
+-rw-r--r--   0 javierphon   (503) staff       (20)      473 2023-06-16 09:04:36.000000 quickfix-ch-0.0.2/quickfix_ch.egg-info/SOURCES.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 09:04:36.000000 quickfix-ch-0.0.2/quickfix_ch.egg-info/dependency_links.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)        9 2023-06-16 09:04:36.000000 quickfix-ch-0.0.2/quickfix_ch.egg-info/top_level.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 09:04:36.307366 quickfix-ch-0.0.2/setup.cfg
+-rw-r--r--   0 javierphon   (503) staff       (20)      943 2023-06-16 09:04:22.000000 quickfix-ch-0.0.2/setup.py
```

### Comparing `quickfix-ch-0.0.1/PKG-INFO` & `quickfix-ch-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-ch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python FIX library that supports ARM Macs
 Author: Coinhako (Javier)
 Author-email: <javier.phon@coinhako.com>
 Keywords: python,FIX,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix.py` & `quickfix-ch-0.0.2/quickfix/quickfix.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix40.py` & `quickfix-ch-0.0.2/quickfix/quickfix40.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix41.py` & `quickfix-ch-0.0.2/quickfix/quickfix41.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix42.py` & `quickfix-ch-0.0.2/quickfix/quickfix42.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix43.py` & `quickfix-ch-0.0.2/quickfix/quickfix43.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix44.py` & `quickfix-ch-0.0.2/quickfix/quickfix44.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix50.py` & `quickfix-ch-0.0.2/quickfix/quickfix50.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix50sp1.py` & `quickfix-ch-0.0.2/quickfix/quickfix50sp1.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfix50sp2.py` & `quickfix-ch-0.0.2/quickfix/quickfix50sp2.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix/quickfixt11.py` & `quickfix-ch-0.0.2/quickfix/quickfixt11.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.1/quickfix_ch.egg-info/PKG-INFO` & `quickfix-ch-0.0.2/quickfix_ch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-ch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python FIX library that supports ARM Macs
 Author: Coinhako (Javier)
 Author-email: <javier.phon@coinhako.com>
 Keywords: python,FIX,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quickfix-ch-0.0.1/setup.py` & `quickfix-ch-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
-DESCRIPTION = 'A python FIX library that supports ARM Macs'
-LONG_DESCRIPTION = 'A python FIX library that supports ARM Macs'
+VERSION = "0.0.2"
+DESCRIPTION = "A python FIX library that supports ARM Macs"
+LONG_DESCRIPTION = "A python FIX library that supports ARM Macs"
 
 # Setting up
 setup(
     name="quickfix-ch",
     version=VERSION,
     author="Coinhako (Javier)",
     author_email="<javier.phon@coinhako.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION  ,
-    packages=find_packages(),     install_requires=[ ],
-    keywords=['python', 'FIX', 'finance'],
+    packages=find_packages(),
+    package_data={
+        "": ["_quickfix.*"]
+    },
+    include_package_data=True,
+    install_requires=[],
+    keywords=["python", "FIX", "finance"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

