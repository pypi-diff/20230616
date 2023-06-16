# Comparing `tmp/geolink2oereb-0.1.5.tar.gz` & `tmp/geolink2oereb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink2oereb-0.1.5.tar", last modified: Fri Jun 16 12:27:27 2023, max compression
+gzip compressed data, was "geolink2oereb-0.1.6.tar", last modified: Fri Jun 16 13:06:46 2023, max compression
```

## Comparing `geolink2oereb-0.1.5.tar` & `geolink2oereb-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.549759 geolink2oereb-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/top_level.txt
```

### Comparing `geolink2oereb-0.1.5/LICENSE` & `geolink2oereb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.5/PKG-INFO` & `geolink2oereb-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.5
+Version: 0.1.6
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.5/README.md` & `geolink2oereb-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.5/setup.py` & `geolink2oereb-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'WebTest >= 1.3.1',  # py3 compat
     'pytest',  # includes virtualenv
     'pytest-cov'
 ]
 
 setup(
     name='geolink2oereb',
-    version='0.1.5',
+    version='0.1.6',
     description='Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities',
     license='BSD',
     long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `geolink2oereb-0.1.5/src/geolink2oereb/cli.py` & `geolink2oereb-0.1.6/src/geolink2oereb/cli.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py` & `geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py` & `geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py` & `geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.5/src/geolink2oereb/transform.py` & `geolink2oereb-0.1.6/src/geolink2oereb/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,10 +120,11 @@
     uuid_dokumente = []
     for amt in unique_aemter:
         new_amt_uuid = str(uuid4())
         for dokument in unique_dokumente:
             if dokument.ZustaendigeStelle.REF == str(amt):
                 dokument.ZustaendigeStelle.set_REF(new_amt_uuid)
                 uuid_dokumente.append(dokument)
+                dokument.set_TID(str(uuid4()))
         amt.set_TID(new_amt_uuid)
         uuid_aemter.append(amt)
     return uuid_dokumente, uuid_aemter
```

### Comparing `geolink2oereb-0.1.5/src/geolink2oereb.egg-info/PKG-INFO` & `geolink2oereb-0.1.6/src/geolink2oereb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.5
+Version: 0.1.6
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.5/src/geolink2oereb.egg-info/SOURCES.txt` & `geolink2oereb-0.1.6/src/geolink2oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

