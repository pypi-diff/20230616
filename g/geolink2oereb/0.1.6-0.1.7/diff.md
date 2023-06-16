# Comparing `tmp/geolink2oereb-0.1.6.tar.gz` & `tmp/geolink2oereb-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink2oereb-0.1.6.tar", last modified: Fri Jun 16 13:06:46 2023, max compression
+gzip compressed data, was "geolink2oereb-0.1.7.tar", last modified: Fri Jun 16 15:25:19 2023, max compression
```

## Comparing `geolink2oereb-0.1.6.tar` & `geolink2oereb-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.549759 geolink2oereb-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.557759 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-16 13:06:05.000000 geolink2oereb-0.1.6/src/geolink2oereb/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:46.553759 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 13:06:46.000000 geolink2oereb-0.1.6/src/geolink2oereb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.897179 geolink2oereb-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 15:25:19.897179 geolink2oereb-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 15:25:19.901179 geolink2oereb-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.893179 geolink2oereb-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.893179 geolink2oereb-0.1.7/src/geolink2oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.897179 geolink2oereb-0.1.7/src/geolink2oereb/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.897179 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.897179 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.897179 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.897179 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-16 15:24:30.000000 geolink2oereb-0.1.7/src/geolink2oereb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:19.897179 geolink2oereb-0.1.7/src/geolink2oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 15:25:19.000000 geolink2oereb-0.1.7/src/geolink2oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 15:25:19.000000 geolink2oereb-0.1.7/src/geolink2oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:25:19.000000 geolink2oereb-0.1.7/src/geolink2oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 15:25:19.000000 geolink2oereb-0.1.7/src/geolink2oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:25:19.000000 geolink2oereb-0.1.7/src/geolink2oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 15:25:19.000000 geolink2oereb-0.1.7/src/geolink2oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 15:25:19.000000 geolink2oereb-0.1.7/src/geolink2oereb.egg-info/top_level.txt
```

### Comparing `geolink2oereb-0.1.6/LICENSE` & `geolink2oereb-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.6/PKG-INFO` & `geolink2oereb-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.6
+Version: 0.1.7
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.6/README.md` & `geolink2oereb-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.6/setup.py` & `geolink2oereb-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'WebTest >= 1.3.1',  # py3 compat
     'pytest',  # includes virtualenv
     'pytest-cov'
 ]
 
 setup(
     name='geolink2oereb',
-    version='0.1.6',
+    version='0.1.7',
     description='Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities',
     license='BSD',
     long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `geolink2oereb-0.1.6/src/geolink2oereb/cli.py` & `geolink2oereb-0.1.7/src/geolink2oereb/cli.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py` & `geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py` & `geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 from geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes import (
     OeREBKRM_V2_0_Dokumente_Dokument,
     LocalisationCH_V1_MultilingualText,
     LocalisationCH_V1_LocalisedText,
     LocalisedTextType,
     OeREBKRM_V2_0_Amt_Amt,
-    ZustaendigeStelleType
+    ZustaendigeStelleType,
+    TitelType,
+    LocalisedTextType86,
+    OeREBKRM_V2_0_LocalisedUri,
+    TextImWebType,
+    OeREBKRM_V2_0_MultilingualUri
 )
 
 
 def multilingual_text_from_dict(multilingual_dict):
     if multilingual_dict is None:
         return multilingual_dict
     localized_texts = LocalisedTextType()
     for language in multilingual_dict:
         localized_texts.LocalisationCH_V1_LocalisedText.append(
             LocalisationCH_V1_LocalisedText(language, multilingual_dict[language])
         )
-    return LocalisationCH_V1_MultilingualText(localized_texts)
+    return TitelType(LocalisationCH_V1_MultilingualText(localized_texts))
+
+
+def multilingual_uri_from_dict(multilingual_dict):
+    if multilingual_dict is None:
+        return multilingual_dict
+    localized_texts = LocalisedTextType86()
+    for language in multilingual_dict:
+        localized_texts.OeREBKRM_V2_0_LocalisedUri.append(
+            OeREBKRM_V2_0_LocalisedUri(language, multilingual_dict[language])
+        )
+    return TextImWebType(OeREBKRM_V2_0_MultilingualUri(localized_texts))
 
 
 def office_record_to_oerebkrmtrsfr(office_record):
     """
 
     Args:
         office_record (pyramid_oereb.core.records.office.OfficeRecord): The office record to translate.
     Returns:
         geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes.OeREBKRM_V2_0_Amt_Amt
     """
     amt = OeREBKRM_V2_0_Amt_Amt(
         Name=multilingual_text_from_dict(office_record.name),
-        AmtImWeb=multilingual_text_from_dict(office_record.office_at_web),
+        AmtImWeb=multilingual_uri_from_dict(office_record.office_at_web),
         UID=office_record.uid,
         Zeile1=office_record.line1,
         Zeile2=office_record.line2,
         Strasse=office_record.street,
         Hausnr=office_record.number,
         PLZ=office_record.postal_code,
         Ort=office_record.city,
@@ -54,15 +70,15 @@
     amt = office_record_to_oerebkrmtrsfr(document_record.responsible_office)
     dokument = OeREBKRM_V2_0_Dokumente_Dokument(
         Typ=document_record.document_type.code,
         Titel=multilingual_text_from_dict(document_record.title),
         Abkuerzung=multilingual_text_from_dict(document_record.abbreviation),
         OffizielleNr=multilingual_text_from_dict(document_record.official_number),
         NurInGemeinde=document_record.only_in_municipality,
-        TextImWeb=multilingual_text_from_dict(document_record.text_at_web),
+        TextImWeb=multilingual_uri_from_dict(document_record.text_at_web),
         # Dokument=multilingual_text_from_dict(document_record.file),
         AuszugIndex=document_record.index,
         Rechtsstatus=document_record.law_status.code,
         publiziertAb=document_record.published_from,
         publiziertBis=document_record.published_until,
         ZustaendigeStelle=ZustaendigeStelleType(REF=str(amt))
     )
```

### Comparing `geolink2oereb-0.1.6/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py` & `geolink2oereb-0.1.7/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 logging.basicConfig(level="DEBUG", format="%(asctime)s [%(levelname)s] %(message)s")
 
 __version__ = "1.0.0"
 
 
 class OEREBlexSourceCustom(OEREBlexSource):
+    # comletely skip federal documents because they should be added via official
+    # sources: https://models.geo.admin.ch/V_D/OeREB/OeREBKRM_V2_0_Gesetze.xml
+    # TODO: add french identifier of federal docs
+    filter_federal_documents = ['Bund', 'Cancelleria federale', 'Confederaziun']
+
     def _get_document_title(self, document, current_file, language):
         """
         Starting with V2, pyramid_oereb uses the file title instead of the document title by default.
         In this project, we always want to use the document title, so this overrides that.
         return {language: u'{title} ({file_name})'.format(title=document.title, file_name=current_file.title)}
         file_name=current_file.title
 
@@ -35,14 +40,35 @@
         if document.doctype == "decree":
             user_title = document.title + " (" + current_file._title + ")"
         else:
             user_title = document.title
 
         return {language: "{user_title}".format(user_title=user_title)}
 
+    def _get_document_records(self, document, language):
+        """
+        Converts the received documents into records. This subclass filters configured objects.
+
+        Args:
+            document (geolink_formatter.entity.Document): The geoLink document to be returned as document
+                record.
+            language (str): The language of the returned documents.
+
+        Returns:
+            list of pyramid_oereb.core.records.documents.DocumentRecord: The converted record.
+        """
+        if document.federal_level:
+            if document.federal_level in self.filter_federal_documents:
+                logging.info(
+                    f'filtering {document} because its federal level is '
+                    f'in the filter list {self.filter_federal_documents}'
+                )
+                return []
+        return super(OEREBlexSourceCustom, self)._get_document_records(document, language)
+
 
 def oerebkrm_v2_0_dokument_typ_2_document_type_records():
     """
     Returns: list of pyramid_oereb.core.records.document_types.DocumentTypeRecord
     """
     document_type_records = []
     for document_type_enum in list(OeREBKRM_V2_0_DokumentTyp):
```

### Comparing `geolink2oereb-0.1.6/src/geolink2oereb/transform.py` & `geolink2oereb-0.1.7/src/geolink2oereb/transform.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.6/src/geolink2oereb.egg-info/PKG-INFO` & `geolink2oereb-0.1.7/src/geolink2oereb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.6
+Version: 0.1.7
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.6/src/geolink2oereb.egg-info/SOURCES.txt` & `geolink2oereb-0.1.7/src/geolink2oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

