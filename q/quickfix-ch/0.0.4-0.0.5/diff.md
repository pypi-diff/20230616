# Comparing `tmp/quickfix-ch-0.0.4.tar.gz` & `tmp/quickfix-ch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfix-ch-0.0.4.tar", last modified: Fri Jun 16 15:26:18 2023, max compression
+gzip compressed data, was "quickfix-ch-0.0.5.tar", last modified: Fri Jun 16 15:30:36 2023, max compression
```

## Comparing `quickfix-ch-0.0.4.tar` & `quickfix-ch-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:26:18.608514 quickfix-ch-0.0.4/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 15:26:18.608337 quickfix-ch-0.0.4/PKG-INFO
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:26:18.605049 quickfix-ch-0.0.4/py-quickfix/
--rw-r--r--   0 javierphon   (503) staff       (20)        0 2023-06-16 08:14:55.000000 quickfix-ch-0.0.4/py-quickfix/__init__.py
--rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.4/py-quickfix/_quickfix.13.so
--rwxr-xr-x   0 javierphon   (503) staff       (20)     1000 2023-06-16 07:59:51.000000 quickfix-ch-0.0.4/py-quickfix/_quickfix.la
--rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.4/py-quickfix/_quickfix.so
--rw-r--r--   0 javierphon   (503) staff       (20)  2064364 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix.py
--rw-r--r--   0 javierphon   (503) staff       (20)     4825 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix40.py
--rw-r--r--   0 javierphon   (503) staff       (20)     6232 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix41.py
--rw-r--r--   0 javierphon   (503) staff       (20)    21580 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix42.py
--rw-r--r--   0 javierphon   (503) staff       (20)    64741 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix43.py
--rw-r--r--   0 javierphon   (503) staff       (20)   262984 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix44.py
--rw-r--r--   0 javierphon   (503) staff       (20)   379998 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix50.py
--rw-r--r--   0 javierphon   (503) staff       (20)   449402 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix50sp1.py
--rw-r--r--   0 javierphon   (503) staff       (20)   532344 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfix50sp2.py
--rw-r--r--   0 javierphon   (503) staff       (20)     1223 2023-06-16 07:59:37.000000 quickfix-ch-0.0.4/py-quickfix/quickfixt11.py
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:26:18.607965 quickfix-ch-0.0.4/quickfix_ch.egg-info/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 15:26:18.000000 quickfix-ch-0.0.4/quickfix_ch.egg-info/PKG-INFO
--rw-r--r--   0 javierphon   (503) staff       (20)      515 2023-06-16 15:26:18.000000 quickfix-ch-0.0.4/quickfix_ch.egg-info/SOURCES.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 15:26:18.000000 quickfix-ch-0.0.4/quickfix_ch.egg-info/dependency_links.txt
--rw-r--r--   0 javierphon   (503) staff       (20)       12 2023-06-16 15:26:18.000000 quickfix-ch-0.0.4/quickfix_ch.egg-info/top_level.txt
--rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 15:26:18.608736 quickfix-ch-0.0.4/setup.cfg
--rw-r--r--   0 javierphon   (503) staff       (20)      954 2023-06-16 15:26:11.000000 quickfix-ch-0.0.4/setup.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:30:36.162297 quickfix-ch-0.0.5/
+-rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 15:30:36.162093 quickfix-ch-0.0.5/PKG-INFO
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:30:36.158113 quickfix-ch-0.0.5/quickfixCH/
+-rw-r--r--   0 javierphon   (503) staff       (20)        0 2023-06-16 08:14:55.000000 quickfix-ch-0.0.5/quickfixCH/__init__.py
+-rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.5/quickfixCH/_quickfix.13.so
+-rwxr-xr-x   0 javierphon   (503) staff       (20)     1000 2023-06-16 07:59:51.000000 quickfix-ch-0.0.5/quickfixCH/_quickfix.la
+-rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.5/quickfixCH/_quickfix.so
+-rw-r--r--   0 javierphon   (503) staff       (20)  2064364 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     4825 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix40.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     6232 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix41.py
+-rw-r--r--   0 javierphon   (503) staff       (20)    21580 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix42.py
+-rw-r--r--   0 javierphon   (503) staff       (20)    64741 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix43.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   262984 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix44.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   379998 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix50.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   449402 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix50sp1.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   532344 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfix50sp2.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     1223 2023-06-16 07:59:37.000000 quickfix-ch-0.0.5/quickfixCH/quickfixt11.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:30:36.161684 quickfix-ch-0.0.5/quickfix_ch.egg-info/
+-rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 15:30:36.000000 quickfix-ch-0.0.5/quickfix_ch.egg-info/PKG-INFO
+-rw-r--r--   0 javierphon   (503) staff       (20)      501 2023-06-16 15:30:36.000000 quickfix-ch-0.0.5/quickfix_ch.egg-info/SOURCES.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 15:30:36.000000 quickfix-ch-0.0.5/quickfix_ch.egg-info/dependency_links.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)       11 2023-06-16 15:30:36.000000 quickfix-ch-0.0.5/quickfix_ch.egg-info/top_level.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 15:30:36.162515 quickfix-ch-0.0.5/setup.cfg
+-rw-r--r--   0 javierphon   (503) staff       (20)      953 2023-06-16 15:30:32.000000 quickfix-ch-0.0.5/setup.py
```

### Comparing `quickfix-ch-0.0.4/PKG-INFO` & `quickfix-ch-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-ch
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python FIX library that supports ARM Macs
 Author: Coinhako (Javier)
 Author-email: <javier.phon@coinhako.com>
 Keywords: python,FIX,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quickfix-ch-0.0.4/py-quickfix/_quickfix.13.so` & `quickfix-ch-0.0.5/quickfixCH/_quickfix.13.so`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/_quickfix.la` & `quickfix-ch-0.0.5/quickfixCH/_quickfix.la`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/_quickfix.so` & `quickfix-ch-0.0.5/quickfixCH/_quickfix.so`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix40.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix40.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix41.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix41.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix42.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix42.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix43.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix43.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix44.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix44.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix50.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix50.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix50sp1.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix50sp1.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfix50sp2.py` & `quickfix-ch-0.0.5/quickfixCH/quickfix50sp2.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/py-quickfix/quickfixt11.py` & `quickfix-ch-0.0.5/quickfixCH/quickfixt11.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.4/quickfix_ch.egg-info/PKG-INFO` & `quickfix-ch-0.0.5/quickfix_ch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-ch
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python FIX library that supports ARM Macs
 Author: Coinhako (Javier)
 Author-email: <javier.phon@coinhako.com>
 Keywords: python,FIX,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quickfix-ch-0.0.4/setup.py` & `quickfix-ch-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "A python FIX library that supports ARM Macs"
 LONG_DESCRIPTION = "A python FIX library that supports ARM Macs"
 
 # Setting up
 setup(
     name="quickfix-ch",
     version=VERSION,
     author="Coinhako (Javier)",
     author_email="<javier.phon@coinhako.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION  ,
     packages=find_packages(),
     package_data={
-        "py-quickfix": ["_quickfix.*"]
+        "quickfixCH": ["_quickfix.*"]
     },
     include_package_data=True,
     install_requires=[],
     keywords=["python", "FIX", "finance"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

