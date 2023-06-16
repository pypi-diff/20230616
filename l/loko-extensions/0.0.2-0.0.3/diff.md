# Comparing `tmp/loko-extensions-0.0.2.tar.gz` & `tmp/loko-extensions-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loko-extensions-0.0.2.tar", last modified: Thu Oct 27 15:04:51 2022, max compression
+gzip compressed data, was "loko-extensions-0.0.3.tar", last modified: Fri Jun 16 08:49:04 2023, max compression
```

## Comparing `loko-extensions-0.0.2.tar` & `loko-extensions-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       57 2022-10-27 15:00:31.000000 loko-extensions-0.0.2/MANIFEST.in
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      325 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/PKG-INFO
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1961 2022-10-27 13:07:29.000000 loko-extensions-0.0.2/README.md
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/apps/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/apps/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/business/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/business/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1453 2022-09-16 11:59:10.000000 loko-extensions-0.0.2/loko_extensions/business/decorators.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/config/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/config/AppConfig.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/config/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/dao/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/dao/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/examples/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/examples/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/model/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/model/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)    17534 2022-10-27 09:42:12.000000 loko-extensions-0.0.2/loko_extensions/model/components.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/resources/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/resources/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/services/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/services/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/services/services.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/test/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/test/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions/utils/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/utils/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      252 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/loko_extensions/utils/pathutils.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/loko_extensions.egg-info/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      325 2022-10-27 15:04:51.000000 loko-extensions-0.0.2/loko_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      774 2022-10-27 15:04:51.000000 loko-extensions-0.0.2/loko_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        1 2022-10-27 15:04:51.000000 loko-extensions-0.0.2/loko_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       16 2022-10-27 15:04:51.000000 loko-extensions-0.0.2/loko_extensions.egg-info/top_level.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      282 2022-10-27 14:36:27.000000 loko-extensions-0.0.2/ppom.json
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.2/requirements.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       38 2022-10-27 15:04:51.214034 loko-extensions-0.0.2/setup.cfg
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      740 2022-10-27 14:38:56.000000 loko-extensions-0.0.2/setup.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       57 2022-10-27 15:00:31.000000 loko-extensions-0.0.3/MANIFEST.in
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2329 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/PKG-INFO
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1961 2022-10-27 13:07:29.000000 loko-extensions-0.0.3/README.md
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/apps/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/apps/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/business/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/business/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1510 2023-06-16 08:33:47.000000 loko-extensions-0.0.3/loko_extensions/business/decorator_fastapi.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1453 2022-09-16 11:59:10.000000 loko-extensions-0.0.3/loko_extensions/business/decorators.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/config/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/config/AppConfig.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/config/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/dao/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/dao/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/examples/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/examples/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/model/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/model/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)    17534 2022-10-27 09:42:12.000000 loko-extensions-0.0.3/loko_extensions/model/components.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/resources/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/resources/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/services/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/services/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/services/services.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/test/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/test/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions/utils/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/utils/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      252 2022-09-06 10:49:17.000000 loko-extensions-0.0.3/loko_extensions/utils/pathutils.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/loko_extensions.egg-info/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2329 2023-06-16 08:49:04.000000 loko-extensions-0.0.3/loko_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      858 2023-06-16 08:49:04.000000 loko-extensions-0.0.3/loko_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        1 2023-06-16 08:49:04.000000 loko-extensions-0.0.3/loko_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        7 2023-06-16 08:49:04.000000 loko-extensions-0.0.3/loko_extensions.egg-info/requires.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       16 2023-06-16 08:49:04.000000 loko-extensions-0.0.3/loko_extensions.egg-info/top_level.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      282 2023-06-16 08:33:47.000000 loko-extensions-0.0.3/ppom.json
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        7 2023-06-16 08:35:54.000000 loko-extensions-0.0.3/requirements.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       38 2023-06-16 08:49:04.158381 loko-extensions-0.0.3/setup.cfg
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      963 2023-06-16 08:41:47.000000 loko-extensions-0.0.3/setup.py
```

### Comparing `loko-extensions-0.0.2/README.md` & `loko-extensions-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `loko-extensions-0.0.2/loko_extensions/business/decorators.py` & `loko-extensions-0.0.3/loko_extensions/business/decorators.py`

 * *Files identical despite different names*

### Comparing `loko-extensions-0.0.2/loko_extensions/model/components.py` & `loko-extensions-0.0.3/loko_extensions/model/components.py`

 * *Files identical despite different names*

### Comparing `loko-extensions-0.0.2/loko_extensions.egg-info/SOURCES.txt` & `loko-extensions-0.0.3/loko_extensions.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 ppom.json
 requirements.txt
 setup.py
 loko_extensions/__init__.py
 loko_extensions.egg-info/PKG-INFO
 loko_extensions.egg-info/SOURCES.txt
 loko_extensions.egg-info/dependency_links.txt
+loko_extensions.egg-info/requires.txt
 loko_extensions.egg-info/top_level.txt
 loko_extensions/apps/__init__.py
 loko_extensions/business/__init__.py
+loko_extensions/business/decorator_fastapi.py
 loko_extensions/business/decorators.py
 loko_extensions/config/AppConfig.py
 loko_extensions/config/__init__.py
 loko_extensions/dao/__init__.py
 loko_extensions/examples/__init__.py
 loko_extensions/model/__init__.py
 loko_extensions/model/components.py
```

### Comparing `loko-extensions-0.0.2/setup.py` & `loko-extensions-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import setuptools,os
 
 def get_requirements():
     return [x for x in open("./requirements.txt").read().split("\n") if not x.startswith("pkg_resources")]
 
+def get_long_description() -> str:
+
+    readme_filepath = os.path.join(os.path.dirname(__file__), "README.md")
+    with open(readme_filepath) as f:
+        return f.read()
+
 import json
 ppom=json.load(open("./ppom.json"))
 version=ppom['version']
 
 setuptools.setup(
     name="loko-extensions",
     version=version,
     author="Live Tech",
     author_email="f.dantonio@ilivetech.it",
-    description="",
-    long_description="",
+    description="A framework for Loko extensions",
+    long_description=get_long_description(),
     python_requires='>3.5.0',
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=get_requirements()
 
-)
+)
```

