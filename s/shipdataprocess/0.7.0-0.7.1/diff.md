# Comparing `tmp/shipdataprocess-0.7.0-py2.py3-none-any.whl.zip` & `tmp/shipdataprocess-0.7.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18351 bytes, number of entries: 11
--rw-r--r--  2.0 unx      855 b- defN 22-Jan-26 12:37 shipdataprocess/__init__.py
--rw-r--r--  2.0 unx     5154 b- defN 22-Jan-26 12:24 shipdataprocess/collapse.py
--rw-r--r--  2.0 unx     9128 b- defN 22-Jan-26 11:35 shipdataprocess/normalize.py
--rw-r--r--  2.0 unx    17757 b- defN 22-Jan-25 23:59 shipdataprocess/shiptype.py
--rw-r--r--  2.0 unx    19311 b- defN 22-Jan-26 12:24 shipdataprocess/standardize.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Jan-26 12:39 shipdataprocess-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1840 b- defN 22-Jan-26 12:39 shipdataprocess-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Jan-26 12:39 shipdataprocess-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 22-Jan-26 12:39 shipdataprocess-0.7.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 19-Jul-28 12:11 shipdataprocess-0.7.0.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      947 b- defN 22-Jan-26 12:39 shipdataprocess-0.7.0.dist-info/RECORD
-11 files, 66476 bytes uncompressed, 16737 bytes compressed:  74.8%
+Zip file size: 18315 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      855 b- defN 22-Jan-26 22:27 shipdataprocess/__init__.py
+-rw-r--r--  2.0 unx     5154 b- defN 22-Jan-26 13:08 shipdataprocess/collapse.py
+-rw-r--r--  2.0 unx     8940 b- defN 22-Jan-26 16:27 shipdataprocess/normalize.py
+-rw-r--r--  2.0 unx    17757 b- defN 22-Jan-26 13:08 shipdataprocess/shiptype.py
+-rw-r--r--  2.0 unx    19311 b- defN 22-Jan-27 00:16 shipdataprocess/standardize.py
+-rw-r--r--  2.0 unx    11357 b- defN 22-Jan-27 23:21 shipdataprocess-0.7.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1840 b- defN 22-Jan-27 23:21 shipdataprocess-0.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-Jan-27 23:21 shipdataprocess-0.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 22-Jan-27 23:21 shipdataprocess-0.7.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 19-Jul-28 12:11 shipdataprocess-0.7.1.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      947 b- defN 22-Jan-27 23:21 shipdataprocess-0.7.1.dist-info/RECORD
+11 files, 66288 bytes uncompressed, 16701 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: shipdataprocess/shiptype.py
 Comment: 
 
 Filename: shipdataprocess/standardize.py
 Comment: 
 
-Filename: shipdataprocess-0.7.0.dist-info/LICENSE
+Filename: shipdataprocess-0.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: shipdataprocess-0.7.0.dist-info/METADATA
+Filename: shipdataprocess-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: shipdataprocess-0.7.0.dist-info/WHEEL
+Filename: shipdataprocess-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: shipdataprocess-0.7.0.dist-info/top_level.txt
+Filename: shipdataprocess-0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: shipdataprocess-0.7.0.dist-info/zip-safe
+Filename: shipdataprocess-0.7.1.dist-info/zip-safe
 Comment: 
 
-Filename: shipdataprocess-0.7.0.dist-info/RECORD
+Filename: shipdataprocess-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shipdataprocess/__init__.py

```diff
@@ -1,13 +1,13 @@
 """
 Useful modules to process vessel data
 """
 
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 __author__ = "Jaeyoon Park"
 __email__ = "jaeyoon@globalfishingwatch.org"
 __source__ = "https://github.com/GlobalFishingWatch/shipdataprocess"
 __license__ = """
 Copyright 2017 Global Fishing Watch Inc.
 Authors:
```

## shipdataprocess/normalize.py

```diff
@@ -18,34 +18,29 @@
 
     :param name: String, an original vessel name
     :return: String, a normalized vessel name
     """
 
     if (name is None) | (name != name) | (name == ""):
         return None
-    print(name)
+
     #
     # Remove nasty characters and white spaces
-    # try:
-    #     name = unidecode(str(name.decode("utf-8")))
-    # except UnicodeDecodeError:
-    #     name = unidecode(str(name.decode("iso_8859-1")))
-
     if issubclass(type(name), str):
         name = unidecode(name)
     elif isinstance(name, bytes):
         try:
             name = unidecode(str(name, "utf-8", "strict"))
         except UnicodeDecodeError:
             name = unidecode(str(name, "iso-8859-1", "strict"))
     elif isinstance(name, int):
         name = str(name)
     else:
         return None
-    print(name)
+
     #
     # Turn to upper cases
     name = name.upper()
 
     name = re.sub(r"\s+", " ", name)
     name = name.strip()
     name = name.replace("\n", "").replace("\r", "")
```

## Comparing `shipdataprocess-0.7.0.dist-info/LICENSE` & `shipdataprocess-0.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shipdataprocess-0.7.0.dist-info/METADATA` & `shipdataprocess-0.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipdataprocess
-Version: 0.7.0
+Version: 0.7.1
 Summary: Useful modules to process vessel data
 Home-page: https://github.com/GlobalFishingWatch/shipdataprocess
 Author: Jaeyoon Park
 Author-email: jaeyoon@globalfishingwatch.org
 License: Apache 2.0
 Keywords: ship,vessel,fishing,normalization
 Platform: UNKNOWN
```

