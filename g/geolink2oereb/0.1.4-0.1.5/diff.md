# Comparing `tmp/geolink2oereb-0.1.4.tar.gz` & `tmp/geolink2oereb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink2oereb-0.1.4.tar", last modified: Fri Jun 16 06:32:44 2023, max compression
+gzip compressed data, was "geolink2oereb-0.1.5.tar", last modified: Fri Jun 16 12:27:27 2023, max compression
```

## Comparing `geolink2oereb-0.1.4.tar` & `geolink2oereb-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.275359 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-16 12:26:47.000000 geolink2oereb-0.1.5/src/geolink2oereb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:27:27.271359 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 12:27:27.000000 geolink2oereb-0.1.5/src/geolink2oereb.egg-info/top_level.txt
```

### Comparing `geolink2oereb-0.1.4/LICENSE` & `geolink2oereb-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.4/PKG-INFO` & `geolink2oereb-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.4
+Version: 0.1.5
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.4/README.md` & `geolink2oereb-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.4/setup.py` & `geolink2oereb-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'WebTest >= 1.3.1',  # py3 compat
     'pytest',  # includes virtualenv
     'pytest-cov'
 ]
 
 setup(
     name='geolink2oereb',
-    version='0.1.4',
+    version='0.1.5',
     description='Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities',
     license='BSD',
     long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `geolink2oereb-0.1.4/src/geolink2oereb/cli.py` & `geolink2oereb-0.1.5/src/geolink2oereb/cli.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py` & `geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py` & `geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes import (
     OeREBKRM_V2_0_Dokumente_Dokument,
     LocalisationCH_V1_MultilingualText,
     LocalisationCH_V1_LocalisedText,
     LocalisedTextType,
     OeREBKRM_V2_0_Amt_Amt,
+    ZustaendigeStelleType
 )
 
 
 def multilingual_text_from_dict(multilingual_dict):
     if multilingual_dict is None:
         return multilingual_dict
     localized_texts = LocalisedTextType()
@@ -22,44 +23,48 @@
     """
 
     Args:
         office_record (pyramid_oereb.core.records.office.OfficeRecord): The office record to translate.
     Returns:
         geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes.OeREBKRM_V2_0_Amt_Amt
     """
-    return OeREBKRM_V2_0_Amt_Amt(
+    amt = OeREBKRM_V2_0_Amt_Amt(
         Name=multilingual_text_from_dict(office_record.name),
         AmtImWeb=multilingual_text_from_dict(office_record.office_at_web),
         UID=office_record.uid,
         Zeile1=office_record.line1,
         Zeile2=office_record.line2,
         Strasse=office_record.street,
         Hausnr=office_record.number,
         PLZ=office_record.postal_code,
         Ort=office_record.city,
     )
+    return amt
 
 
 def document_record_to_oerebkrmtrsfr(document_record):
     """
 
     Args:
         document_record (pyramid_oereb.core.records.documents.DocumentRecord): The record to translate.
 
     Returns:
-        geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes.OeREBKRM_V2_0_Dokumente_Dokument
+        (geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes.OeREBKRM_V2_0_Amt_Amt,
+            geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes.OeREBKRM_V2_0_Dokumente_Dokument)
     """
-
-    return OeREBKRM_V2_0_Dokumente_Dokument(
+    amt = office_record_to_oerebkrmtrsfr(document_record.responsible_office)
+    dokument = OeREBKRM_V2_0_Dokumente_Dokument(
         Typ=document_record.document_type.code,
         Titel=multilingual_text_from_dict(document_record.title),
         Abkuerzung=multilingual_text_from_dict(document_record.abbreviation),
         OffizielleNr=multilingual_text_from_dict(document_record.official_number),
         NurInGemeinde=document_record.only_in_municipality,
         TextImWeb=multilingual_text_from_dict(document_record.text_at_web),
         # Dokument=multilingual_text_from_dict(document_record.file),
         AuszugIndex=document_record.index,
         Rechtsstatus=document_record.law_status.code,
         publiziertAb=document_record.published_from,
         publiziertBis=document_record.published_until,
-        ZustaendigeStelle=office_record_to_oerebkrmtrsfr(document_record.responsible_office),
+        ZustaendigeStelle=ZustaendigeStelleType(REF=str(amt))
     )
+    dokument.set_TID(str(dokument))
+    return dokument, amt
```

### Comparing `geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py` & `geolink2oereb-0.1.5/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.4/src/geolink2oereb.egg-info/PKG-INFO` & `geolink2oereb-0.1.5/src/geolink2oereb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.4
+Version: 0.1.5
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.4/src/geolink2oereb.egg-info/SOURCES.txt` & `geolink2oereb-0.1.5/src/geolink2oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

