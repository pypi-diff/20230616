# Comparing `tmp/pymca-5.8.5-py2.py3-none-any.whl.zip` & `tmp/pymca-5.8.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5499 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     5930 b- defN 23-Jun-13 10:31 pymca-5.8.5.data/scripts/pymca_launcher
--rw-rw-rw-  2.0 fat       31 b- defN 23-May-16 09:38 pymca-5.8.5.data/scripts/pymca_launcher.bat
--rw-rw-rw-  2.0 fat     1817 b- defN 23-Jun-13 10:31 pymca-5.8.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1775 b- defN 23-Jun-13 10:31 pymca-5.8.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-13 10:31 pymca-5.8.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-13 10:31 pymca-5.8.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      570 b- defN 23-Jun-13 10:31 pymca-5.8.5.dist-info/RECORD
-7 files, 10239 bytes uncompressed, 4483 bytes compressed:  56.2%
+Zip file size: 5501 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-Jun-16 17:06 pymca-5.8.7.data/scripts/pymca_launcher
+-rw-rw-rw-  2.0 fat       31 b- defN 23-May-16 09:38 pymca-5.8.7.data/scripts/pymca_launcher.bat
+-rw-rw-rw-  2.0 fat     1817 b- defN 23-Jun-16 17:06 pymca-5.8.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1775 b- defN 23-Jun-16 17:06 pymca-5.8.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-16 17:06 pymca-5.8.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-16 17:06 pymca-5.8.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      570 b- defN 23-Jun-16 17:06 pymca-5.8.7.dist-info/RECORD
+7 files, 10239 bytes uncompressed, 4485 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: pymca-5.8.5.data/scripts/pymca_launcher
+Filename: pymca-5.8.7.data/scripts/pymca_launcher
 Comment: 
 
-Filename: pymca-5.8.5.data/scripts/pymca_launcher.bat
+Filename: pymca-5.8.7.data/scripts/pymca_launcher.bat
 Comment: 
 
-Filename: pymca-5.8.5.dist-info/LICENSE
+Filename: pymca-5.8.7.dist-info/LICENSE
 Comment: 
 
-Filename: pymca-5.8.5.dist-info/METADATA
+Filename: pymca-5.8.7.dist-info/METADATA
 Comment: 
 
-Filename: pymca-5.8.5.dist-info/WHEEL
+Filename: pymca-5.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: pymca-5.8.5.dist-info/top_level.txt
+Filename: pymca-5.8.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pymca-5.8.5.dist-info/RECORD
+Filename: pymca-5.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pymca-5.8.5.data/scripts/pymca_launcher` & `pymca-5.8.7.data/scripts/pymca_launcher`

 * *Files identical despite different names*

## Comparing `pymca-5.8.5.dist-info/LICENSE` & `pymca-5.8.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymca-5.8.5.dist-info/METADATA` & `pymca-5.8.7.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymca
-Version: 5.8.5
+Version: 5.8.7
 Summary: pymca
 Author: V.A. Sole - ESRF
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Education
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
-Requires-Dist: PyMca5 (>=5.8.5)
+Requires-Dist: PyMca5 (>=5.8.7)
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 pymca
 =====
```

## Comparing `pymca-5.8.5.dist-info/RECORD` & `pymca-5.8.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pymca-5.8.5.data/scripts/pymca_launcher,sha256=Fb--wx4LLVczNN-YP2lGd1GwsrsDI8UKC6RLQaPNfN4,5930
-pymca-5.8.5.data/scripts/pymca_launcher.bat,sha256=Lm_Zznk2TPd-cGs5zg26n3C0tapiGFMiX3N8_y8t1uY,31
-pymca-5.8.5.dist-info/LICENSE,sha256=0xSm7j4zKlKb7GhoOA15734tylOyDqlhp7blkZSg8fo,1817
-pymca-5.8.5.dist-info/METADATA,sha256=xdnExqmxhq0F2hXvb6-StgygfINdq6XGo7mgZW0-HbU,1775
-pymca-5.8.5.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-pymca-5.8.5.dist-info/top_level.txt,sha256=LsnUUUmmL7eZNziV16X2GG0U6S4iV2i58f5XXOiq8DU,6
-pymca-5.8.5.dist-info/RECORD,,
+pymca-5.8.7.data/scripts/pymca_launcher,sha256=Fb--wx4LLVczNN-YP2lGd1GwsrsDI8UKC6RLQaPNfN4,5930
+pymca-5.8.7.data/scripts/pymca_launcher.bat,sha256=Lm_Zznk2TPd-cGs5zg26n3C0tapiGFMiX3N8_y8t1uY,31
+pymca-5.8.7.dist-info/LICENSE,sha256=0xSm7j4zKlKb7GhoOA15734tylOyDqlhp7blkZSg8fo,1817
+pymca-5.8.7.dist-info/METADATA,sha256=PDbz8kghPpEpbTwVqWmMqqqOaQ1fDIjfaz2yjEMsD7Y,1775
+pymca-5.8.7.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+pymca-5.8.7.dist-info/top_level.txt,sha256=LsnUUUmmL7eZNziV16X2GG0U6S4iV2i58f5XXOiq8DU,6
+pymca-5.8.7.dist-info/RECORD,,
```

