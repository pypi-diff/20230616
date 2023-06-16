# Comparing `tmp/geolink2oereb-0.1.8.tar.gz` & `tmp/geolink2oereb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink2oereb-0.1.8.tar", last modified: Fri Jun 16 15:48:21 2023, max compression
+gzip compressed data, was "geolink2oereb-0.1.9.tar", last modified: Fri Jun 16 16:04:11 2023, max compression
```

## Comparing `geolink2oereb-0.1.8.tar` & `geolink2oereb-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.818105 geolink2oereb-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 15:48:21.818105 geolink2oereb-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 15:48:21.818105 geolink2oereb-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.814105 geolink2oereb-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.814105 geolink2oereb-0.1.8/src/geolink2oereb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.814105 geolink2oereb-0.1.8/src/geolink2oereb/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.814105 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.814105 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.818105 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.818105 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-16 15:47:47.000000 geolink2oereb-0.1.8/src/geolink2oereb/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:48:21.814105 geolink2oereb-0.1.8/src/geolink2oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 15:48:21.000000 geolink2oereb-0.1.8/src/geolink2oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 15:48:21.000000 geolink2oereb-0.1.8/src/geolink2oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:48:21.000000 geolink2oereb-0.1.8/src/geolink2oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 15:48:21.000000 geolink2oereb-0.1.8/src/geolink2oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:48:21.000000 geolink2oereb-0.1.8/src/geolink2oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 15:48:21.000000 geolink2oereb-0.1.8/src/geolink2oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 15:48:21.000000 geolink2oereb-0.1.8/src/geolink2oereb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.108221 geolink2oereb-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/src/geolink2oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/src/geolink2oereb/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-16 16:03:37.000000 geolink2oereb-0.1.9/src/geolink2oereb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:11.112221 geolink2oereb-0.1.9/src/geolink2oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 16:04:11.000000 geolink2oereb-0.1.9/src/geolink2oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 16:04:11.000000 geolink2oereb-0.1.9/src/geolink2oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:04:11.000000 geolink2oereb-0.1.9/src/geolink2oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 16:04:11.000000 geolink2oereb-0.1.9/src/geolink2oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:04:11.000000 geolink2oereb-0.1.9/src/geolink2oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 16:04:11.000000 geolink2oereb-0.1.9/src/geolink2oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 16:04:11.000000 geolink2oereb-0.1.9/src/geolink2oereb.egg-info/top_level.txt
```

### Comparing `geolink2oereb-0.1.8/LICENSE` & `geolink2oereb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.8/PKG-INFO` & `geolink2oereb-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.8
+Version: 0.1.9
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.8/README.md` & `geolink2oereb-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.8/setup.py` & `geolink2oereb-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'WebTest >= 1.3.1',  # py3 compat
     'pytest',  # includes virtualenv
     'pytest-cov'
 ]
 
 setup(
     name='geolink2oereb',
-    version='0.1.8',
+    version='0.1.9',
     description='Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities',
     license='BSD',
     long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `geolink2oereb-0.1.8/src/geolink2oereb/cli.py` & `geolink2oereb-0.1.9/src/geolink2oereb/cli.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py` & `geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py` & `geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+import logging
 from geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes import (
     OeREBKRM_V2_0_Dokumente_Dokument,
     LocalisationCH_V1_MultilingualText,
     LocalisationCH_V1_LocalisedText,
     LocalisedTextType,
     OeREBKRM_V2_0_Amt_Amt,
     ZustaendigeStelleType,
     TitelType,
     LocalisedTextType86,
     OeREBKRM_V2_0_LocalisedUri,
     TextImWebType,
     OeREBKRM_V2_0_MultilingualUri
 )
 
+logging.basicConfig(level="DEBUG", format="%(asctime)s [%(levelname)s] %(message)s")
+
+
+def fix_url(url):
+    if not url.startswith('http'):
+        new_url = 'https://{}'.format(url)
+        logging.info(f"Fixing url from {url} to {new_url}")
+        return new_url
+    return url
+
 
 def multilingual_text_from_dict(multilingual_dict):
     if multilingual_dict is None:
         return multilingual_dict
     localized_texts = LocalisedTextType()
     for language in multilingual_dict:
         localized_texts.LocalisationCH_V1_LocalisedText.append(
@@ -26,15 +37,15 @@
 
 def multilingual_uri_from_dict(multilingual_dict):
     if multilingual_dict is None:
         return multilingual_dict
     localized_texts = LocalisedTextType86()
     for language in multilingual_dict:
         localized_texts.OeREBKRM_V2_0_LocalisedUri.append(
-            OeREBKRM_V2_0_LocalisedUri(language, multilingual_dict[language])
+            OeREBKRM_V2_0_LocalisedUri(language, fix_url(multilingual_dict[language]))
         )
     return TextImWebType(OeREBKRM_V2_0_MultilingualUri(localized_texts))
 
 
 def office_record_to_oerebkrmtrsfr(office_record):
     """
```

### Comparing `geolink2oereb-0.1.8/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py` & `geolink2oereb-0.1.9/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.8/src/geolink2oereb/transform.py` & `geolink2oereb-0.1.9/src/geolink2oereb/transform.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.8/src/geolink2oereb.egg-info/PKG-INFO` & `geolink2oereb-0.1.9/src/geolink2oereb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.8
+Version: 0.1.9
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.8/src/geolink2oereb.egg-info/SOURCES.txt` & `geolink2oereb-0.1.9/src/geolink2oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

