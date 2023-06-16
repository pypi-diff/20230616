# Comparing `tmp/geolink2oereb-0.1.3.tar.gz` & `tmp/geolink2oereb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink2oereb-0.1.3.tar", last modified: Fri Jun 16 06:01:04 2023, max compression
+gzip compressed data, was "geolink2oereb-0.1.4.tar", last modified: Fri Jun 16 06:32:44 2023, max compression
```

## Comparing `geolink2oereb-0.1.3.tar` & `geolink2oereb-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.022047 geolink2oereb-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.030047 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-16 06:00:21.000000 geolink2oereb-0.1.3/src/geolink2oereb/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:01:04.026047 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 06:01:04.000000 geolink2oereb-0.1.3/src/geolink2oereb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.933644 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-16 06:32:02.000000 geolink2oereb-0.1.4/src/geolink2oereb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:32:44.929644 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 06:32:44.000000 geolink2oereb-0.1.4/src/geolink2oereb.egg-info/top_level.txt
```

### Comparing `geolink2oereb-0.1.3/LICENSE` & `geolink2oereb-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.3/PKG-INFO` & `geolink2oereb-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.3/README.md` & `geolink2oereb-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.3/setup.py` & `geolink2oereb-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'WebTest >= 1.3.1',  # py3 compat
     'pytest',  # includes virtualenv
     'pytest-cov'
 ]
 
 setup(
     name='geolink2oereb',
-    version='0.1.3',
+    version='0.1.4',
     description='Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities',
     license='BSD',
     long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `geolink2oereb-0.1.3/src/geolink2oereb/cli.py` & `geolink2oereb-0.1.4/src/geolink2oereb/cli.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py` & `geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py` & `geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
     LocalisationCH_V1_LocalisedText,
     LocalisedTextType,
     OeREBKRM_V2_0_Amt_Amt,
 )
 
 
 def multilingual_text_from_dict(multilingual_dict):
+    if multilingual_dict is None:
+        return multilingual_dict
     localized_texts = LocalisedTextType()
     for language in multilingual_dict:
         localized_texts.LocalisationCH_V1_LocalisedText.append(
             LocalisationCH_V1_LocalisedText(language, multilingual_dict[language])
         )
     return LocalisationCH_V1_MultilingualText(localized_texts)
```

### Comparing `geolink2oereb-0.1.3/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py` & `geolink2oereb-0.1.4/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.3/src/geolink2oereb/transform.py` & `geolink2oereb-0.1.4/src/geolink2oereb/transform.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.3/src/geolink2oereb.egg-info/PKG-INFO` & `geolink2oereb-0.1.4/src/geolink2oereb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.3/src/geolink2oereb.egg-info/SOURCES.txt` & `geolink2oereb-0.1.4/src/geolink2oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

