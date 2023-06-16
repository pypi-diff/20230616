# Comparing `tmp/geolink2oereb-0.1.2.tar.gz` & `tmp/geolink2oereb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink2oereb-0.1.2.tar", last modified: Thu Jun  1 14:22:15 2023, max compression
+gzip compressed data, was "geolink2oereb-0.1.3.tar", last modified: Fri Jun 16 06:01:04 2023, max compression
```

## Comparing `geolink2oereb-0.1.2.tar` & `geolink2oereb-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.940505 geolink2oereb-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.940505 geolink2oereb-0.1.2/src/geolink2oereb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.022047 geolink2oereb-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/top_level.txt
```

### Comparing `geolink2oereb-0.1.2/LICENSE` & `geolink2oereb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.2/PKG-INFO` & `geolink2oereb-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.2/README.md` & `geolink2oereb-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.2/setup.py` & `geolink2oereb-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'WebTest >= 1.3.1',  # py3 compat
     'pytest',  # includes virtualenv
     'pytest-cov'
 ]
 
 setup(
     name='geolink2oereb',
-    version='0.1.2',
+    version='0.1.3',
     description='Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities',
     license='BSD',
     long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `geolink2oereb-0.1.2/src/geolink2oereb/cli.py` & `geolink2oereb-0.1.3/src/geolink2oereb/cli.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py` & `geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py` & `geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Returns:
         geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes.OeREBKRM_V2_0_Dokumente_Dokument
     """
 
     return OeREBKRM_V2_0_Dokumente_Dokument(
         Typ=document_record.document_type.code,
         Titel=multilingual_text_from_dict(document_record.title),
-        Abkuerzung=document_record.abbreviation,
+        Abkuerzung=multilingual_text_from_dict(document_record.abbreviation),
         OffizielleNr=multilingual_text_from_dict(document_record.official_number),
         NurInGemeinde=document_record.only_in_municipality,
         TextImWeb=multilingual_text_from_dict(document_record.text_at_web),
         # Dokument=multilingual_text_from_dict(document_record.file),
         AuszugIndex=document_record.index,
         Rechtsstatus=document_record.law_status.code,
         publiziertAb=document_record.published_from,
```

### Comparing `geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py` & `geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.2/src/geolink2oereb/transform.py` & `geolink2oereb-0.1.3/src/geolink2oereb/transform.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.2/src/geolink2oereb.egg-info/PKG-INFO` & `geolink2oereb-0.1.3/src/geolink2oereb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.2/src/geolink2oereb.egg-info/SOURCES.txt` & `geolink2oereb-0.1.3/src/geolink2oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

