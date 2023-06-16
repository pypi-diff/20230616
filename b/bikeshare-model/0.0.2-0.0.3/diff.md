# Comparing `tmp/bikeshare_model-0.0.2-py3-none-any.whl.zip` & `tmp/bikeshare_model-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 576814 bytes, number of entries: 21
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-15 15:36 bikeshare_model/VERSION
+Zip file size: 577337 bytes, number of entries: 22
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jun-16 16:18 .DS_Store
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-16 16:47 bikeshare_model/VERSION
 -rw-r--r--  2.0 unx      253 b- defN 23-Jun-08 23:54 bikeshare_model/__init__.py
 -rw-rw-r--  2.0 unx     2061 b- defN 23-Jun-09 22:47 bikeshare_model/config.yml
 -rw-r--r--  2.0 unx     2134 b- defN 23-Jun-09 21:41 bikeshare_model/pipeline.py
 -rw-r--r--  2.0 unx     1878 b- defN 23-Jun-10 01:55 bikeshare_model/predict.py
 -rw-r--r--  2.0 unx     1679 b- defN 23-Jun-09 22:58 bikeshare_model/train_pipeline.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:16 bikeshare_model/config/__init__.py
 -rw-r--r--  2.0 unx     2928 b- defN 23-Jun-10 04:30 bikeshare_model/config/core.py
@@ -12,12 +13,12 @@
 -rw-rw-r--  2.0 unx   318833 b- defN 23-Jun-10 04:13 bikeshare_model/datasets/test.csv
 -rw-r--r--  2.0 unx        2 b- defN 23-Jun-02 13:16 bikeshare_model/processing/__init__.py
 -rw-r--r--  2.0 unx     2967 b- defN 23-Jun-09 23:12 bikeshare_model/processing/data_manager.py
 -rw-r--r--  2.0 unx     3241 b- defN 23-Jun-09 23:14 bikeshare_model/processing/features.py
 -rw-r--r--  2.0 unx      219 b- defN 23-Jun-09 23:42 bikeshare_model/processing/validation.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:16 bikeshare_model/trained_models/__init__.py
 -rw-rw-r--  2.0 unx   659402 b- defN 23-Jun-10 04:30 bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl
--rw-r--r--  2.0 unx     1127 b- defN 23-Jun-15 15:38 bikeshare_model-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 15:38 bikeshare_model-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-15 15:38 bikeshare_model-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1898 b- defN 23-Jun-15 15:38 bikeshare_model-0.0.2.dist-info/RECORD
-21 files, 2597189 bytes uncompressed, 573658 bytes compressed:  77.9%
+-rw-r--r--  2.0 unx     1127 b- defN 23-Jun-16 16:47 bikeshare_model-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 16:47 bikeshare_model-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-16 16:47 bikeshare_model-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1964 b- defN 23-Jun-16 16:47 bikeshare_model-0.0.3.dist-info/RECORD
+22 files, 2603403 bytes uncompressed, 574087 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: .DS_Store
+Comment: 
+
 Filename: bikeshare_model/VERSION
 Comment: 
 
 Filename: bikeshare_model/__init__.py
 Comment: 
 
 Filename: bikeshare_model/config.yml
@@ -45,20 +48,20 @@
 
 Filename: bikeshare_model/trained_models/__init__.py
 Comment: 
 
 Filename: bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl
 Comment: 
 
-Filename: bikeshare_model-0.0.2.dist-info/METADATA
+Filename: bikeshare_model-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: bikeshare_model-0.0.2.dist-info/WHEEL
+Filename: bikeshare_model-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: bikeshare_model-0.0.2.dist-info/top_level.txt
+Filename: bikeshare_model-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bikeshare_model-0.0.2.dist-info/RECORD
+Filename: bikeshare_model-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bikeshare_model/VERSION

```diff
@@ -1 +1 @@
-0.0.2
+0.0.3
```

## Comparing `bikeshare_model-0.0.2.dist-info/METADATA` & `bikeshare_model-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bikeshare-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bikeshare dataset classification model package 
 Author: Ajay Singh
 Author-email: ajaytevatia@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `bikeshare_model-0.0.2.dist-info/RECORD` & `bikeshare_model-0.0.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-bikeshare_model/VERSION,sha256=y-NTX1iTRVRydKI09GknkRSUGWd6Z3N7bhfzcbY_3e0,5
+.DS_Store,sha256=JYjWrVq6wfd_yH8dN34ccrBeu88OKEKk75boDZo3c9M,6148
+bikeshare_model/VERSION,sha256=dEj8KrFke0LnS0oaAsirXMHgTLLcLZS-xELsN8s-KUg,5
 bikeshare_model/__init__.py,sha256=FBsKr5BGRd1vc2e9OTnoCb4J8Nhb_RWLwuwdDinJYlc,253
 bikeshare_model/config.yml,sha256=ObXJC4ZYuTQXeBwmzNI0eTqhyqajQOo1fxV-ccKWkZg,2061
 bikeshare_model/pipeline.py,sha256=Iv5zp0Eo6aZB5rYo6GG_G5ikheeTdUYkDyb_6VFtWIs,2134
 bikeshare_model/predict.py,sha256=Emdw-4st-Me2WDJ54C4m7MGUv3Gm6xRuDSheFV_UJDs,1878
 bikeshare_model/train_pipeline.py,sha256=FT8b5Zn1i6c6DH_odV2xqeyBazLmZ_PvSEIIswjPlh8,1679
 bikeshare_model/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bikeshare_model/config/core.py,sha256=SIN1ruGN2QvueaySxmc--5-4OS5TeH4RTzTaQxywkPQ,2928
@@ -11,11 +12,11 @@
 bikeshare_model/datasets/test.csv,sha256=qUBW4-MjYr_g-YqdY4wwl8_hNSYfPiAMjAo-TdG1Jhw,318833
 bikeshare_model/processing/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 bikeshare_model/processing/data_manager.py,sha256=ua314xx_3L6NWmPaEIJ2ybxGzVAfGgOmptYZKMlTUfM,2967
 bikeshare_model/processing/features.py,sha256=RUwJx34n45bcuwHIJuDoiIg-aX71Gf-fr30XGqYgcGc,3241
 bikeshare_model/processing/validation.py,sha256=LaIVpKihGSMDt4G9dPKPip1XbdP9lXV9f1rm87K55A4,219
 bikeshare_model/trained_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl,sha256=WCN9pbYeC4IKpjYdl-dX2m1BfQBP7SAagIjXngLg7sQ,659402
-bikeshare_model-0.0.2.dist-info/METADATA,sha256=WGzQ_pNk1L0C47mEBn66NmZnegu4d4vmjpEp-B4I_Dc,1127
-bikeshare_model-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bikeshare_model-0.0.2.dist-info/top_level.txt,sha256=ZKIHSbGTS6ZE2aLhfpCV8HFAqGuZmXzRWQVz-N03wPI,16
-bikeshare_model-0.0.2.dist-info/RECORD,,
+bikeshare_model-0.0.3.dist-info/METADATA,sha256=a695pv8ECX-pjRqg-sDva4PKZE-p63ZiFVbElCyWUnI,1127
+bikeshare_model-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bikeshare_model-0.0.3.dist-info/top_level.txt,sha256=ZKIHSbGTS6ZE2aLhfpCV8HFAqGuZmXzRWQVz-N03wPI,16
+bikeshare_model-0.0.3.dist-info/RECORD,,
```

