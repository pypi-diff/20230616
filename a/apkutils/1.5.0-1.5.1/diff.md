# Comparing `tmp/apkutils-1.5.0-py3-none-any.whl.zip` & `tmp/apkutils-1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 473032 bytes, number of entries: 53
+Zip file size: 473027 bytes, number of entries: 53
 -rw-r--r--  2.0 unx       97 b- defN 80-Jan-01 00:00 apkutils/__init__.py
 -rw-r--r--  2.0 unx       90 b- defN 80-Jan-01 00:00 apkutils/__main__.py
 -rw-r--r--  2.0 unx    21423 b- defN 80-Jan-01 00:00 apkutils/apk.py
 -rw-r--r--  2.0 unx    74581 b- defN 80-Jan-01 00:00 apkutils/apkfile.py
 -rw-r--r--  2.0 unx   116716 b- defN 80-Jan-01 00:00 apkutils/axml/__init__.py
 -rw-r--r--  2.0 unx     7039 b- defN 80-Jan-01 00:00 apkutils/axml/bytecode.py
 -rw-r--r--  2.0 unx     2115 b- defN 80-Jan-01 00:00 apkutils/axml/public.py
@@ -43,13 +43,13 @@
 -rw-r--r--  2.0 unx    11171 b- defN 80-Jan-01 00:00 apkutils/dex/typeinference/typeinference.py
 -rw-r--r--  2.0 unx     1158 b- defN 80-Jan-01 00:00 apkutils/dex/util.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 apkutils/elf/__init__.py
 -rw-r--r--  2.0 unx     6655 b- defN 80-Jan-01 00:00 apkutils/elf/elfparser.py
 -rwxr-xr-x  2.0 unx    69313 b- defN 80-Jan-01 00:00 apkutils/gdiff.py
 -rw-r--r--  2.0 unx    16570 b- defN 80-Jan-01 00:00 apkutils/intersection.py
 -rw-r--r--  2.0 unx     6155 b- defN 80-Jan-01 00:00 apkutils/wildcard.py
--rw-r--r--  2.0 unx     1065 b- defN 80-Jan-01 00:00 apkutils-1.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2719 b- defN 80-Jan-01 00:00 apkutils-1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 apkutils-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 apkutils-1.5.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     4457 b- defN 16-Jan-01 00:00 apkutils-1.5.0.dist-info/RECORD
-53 files, 2476218 bytes uncompressed, 465994 bytes compressed:  81.2%
+-rw-r--r--  2.0 unx     1065 b- defN 80-Jan-01 00:00 apkutils-1.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2711 b- defN 80-Jan-01 00:00 apkutils-1.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 apkutils-1.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 apkutils-1.5.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     4457 b- defN 16-Jan-01 00:00 apkutils-1.5.1.dist-info/RECORD
+53 files, 2476210 bytes uncompressed, 465989 bytes compressed:  81.2%
```

## zipnote {}

```diff
@@ -138,23 +138,23 @@
 
 Filename: apkutils/intersection.py
 Comment: 
 
 Filename: apkutils/wildcard.py
 Comment: 
 
-Filename: apkutils-1.5.0.dist-info/LICENSE
+Filename: apkutils-1.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: apkutils-1.5.0.dist-info/METADATA
+Filename: apkutils-1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: apkutils-1.5.0.dist-info/WHEEL
+Filename: apkutils-1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: apkutils-1.5.0.dist-info/entry_points.txt
+Filename: apkutils-1.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: apkutils-1.5.0.dist-info/RECORD
+Filename: apkutils-1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## apkutils/__init__.py

```diff
@@ -1,5 +1,5 @@
 from apkutils.apk import APK
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 
 __all__ = ["APK", "__version__", "apkfile"]
```

## Comparing `apkutils-1.5.0.dist-info/LICENSE` & `apkutils-1.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `apkutils-1.5.0.dist-info/METADATA` & `apkutils-1.5.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkutils
-Version: 1.5.0
+Version: 1.5.1
 Summary: 一个APK解析库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Pygments (>=2.12.0,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
-Requires-Dist: cryptography (>=35.0.0,<36.0.0)
+Requires-Dist: cryptography (>=39.0.1)
 Requires-Dist: lxml (>=4.6.4,<5.0.0)
 Requires-Dist: pyelftools (>=0.27,<0.28)
 Requires-Dist: pyftype (>=1.2.4,<2.0.0)
 Project-URL: Repository, https://gitee.com/kin9-0rz/apkutils
 Description-Content-Type: text/markdown
 
 # apkutils
```

## Comparing `apkutils-1.5.0.dist-info/RECORD` & `apkutils-1.5.1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-apkutils/__init__.py,sha256=kKpXFez2OzQyu-hS8OwwOWNyCWm3YX7ttJkaJvoaHe4,97
+apkutils/__init__.py,sha256=vnjJfvMqVfjuRrNBFR3dn7nljuO-md2yN7v6lPHXDZs,97
 apkutils/__main__.py,sha256=OzXl4K9fgDRZkTcNLXJ9QeM-3fhYDzwHL4ufMQoeNC4,90
 apkutils/apk.py,sha256=UBRiHYs6TJSaVnUoFoSYnsFykDv-x9HAvp_Tq3AbsNY,21423
 apkutils/apkfile.py,sha256=DPBewHUeEHc3b7_E6aIEsy_3PlHxAUORvpNrXdK1EqI,74581
 apkutils/axml/__init__.py,sha256=Clj5xyhe1fyLjaPuUjmaj6rZh30hpoxFqDC6mz7qJ_E,116716
 apkutils/axml/bytecode.py,sha256=W6LlIRRA7QUzLwTmbA6X4qLZpvHIjUfkn0EMLbbVIwQ,7039
 apkutils/axml/public.py,sha256=3OBHD1ebcZS2vK-MwImjU2QoR5h-K6cnTiMrUz4RkZ4,2115
 apkutils/axml/public.xml,sha256=5AkrYjynoMAFavwQ10Ue_ybXF68eFdcJGVSI15RwiMs,191132
@@ -42,12 +42,12 @@
 apkutils/dex/typeinference/typeinference.py,sha256=mGAPdZEvVP9FdoXGUzpOc7VwAA_dkFNt0UNcbPEXhY0,11171
 apkutils/dex/util.py,sha256=sGq4Vs86P5Q1Sql_Ox88m_yln94WGmIGPQ8CSqVzg1E,1158
 apkutils/elf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 apkutils/elf/elfparser.py,sha256=qePx0dGlsW_WZ8bI_haFKbxyTA-m-xjXOpf_OvzzbdU,6655
 apkutils/gdiff.py,sha256=sRlYt-elMgF_AVuQEwVEgCA3ZpP6X--YtNqA73raDhk,69313
 apkutils/intersection.py,sha256=zoautoRj-e7L46jC8jP1cvlx-lqX_IVc6xxhuSxayE8,16570
 apkutils/wildcard.py,sha256=woYxOenEWrtDroJspdZsqaz60UTAHCYBhoRJcbwjDTE,6155
-apkutils-1.5.0.dist-info/LICENSE,sha256=F2ornjxonXB1RZRczJWEucKZ2ASoCr2dmcane5Q-BDc,1065
-apkutils-1.5.0.dist-info/METADATA,sha256=hLwTcbxuqHruM9yhdiNlI0NYCELqMBtZRKD5m9jJeb0,2719
-apkutils-1.5.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-apkutils-1.5.0.dist-info/entry_points.txt,sha256=dYqfsOj8NPSIBA9O3RWB-ld8mzyYMCipfCLgcrbI1fY,46
-apkutils-1.5.0.dist-info/RECORD,,
+apkutils-1.5.1.dist-info/LICENSE,sha256=F2ornjxonXB1RZRczJWEucKZ2ASoCr2dmcane5Q-BDc,1065
+apkutils-1.5.1.dist-info/METADATA,sha256=gpTVlLa-F26YP3ddPOg7-yMK7iTsecjcDi55Cfh1DRc,2711
+apkutils-1.5.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+apkutils-1.5.1.dist-info/entry_points.txt,sha256=dYqfsOj8NPSIBA9O3RWB-ld8mzyYMCipfCLgcrbI1fY,46
+apkutils-1.5.1.dist-info/RECORD,,
```

