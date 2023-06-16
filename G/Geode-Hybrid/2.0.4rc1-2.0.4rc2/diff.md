# Comparing `tmp/Geode_Hybrid-2.0.4rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Hybrid-2.0.4rc2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 2409 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      170 b- defN 23-Jun-14 22:12 geode_hybrid/__init__.py
--rw-rw-rw-  2.0 fat      234 b- defN 23-Jun-14 22:12 geode_hybrid/brep.py
--rw-rw-rw-  2.0 fat     2245 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      487 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/RECORD
-6 files, 3249 bytes uncompressed, 1523 bytes compressed:  53.1%
+Zip file size: 1110999 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      170 b- defN 23-Jun-14 22:49 geode_hybrid/__init__.py
+-rw-rw-rw-  2.0 fat      234 b- defN 23-Jun-14 22:49 geode_hybrid/brep.py
+-rw-rw-rw-  2.0 fat  2164224 b- defN 23-Jun-14 22:49 geode_hybrid/bin/Geode-Hybrid_brep.dll
+-rw-rw-rw-  2.0 fat   136704 b- defN 23-Jun-14 22:49 geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2245 b- defN 23-Jun-14 22:49 Geode_Hybrid-2.0.4rc2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 22:49 Geode_Hybrid-2.0.4rc2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-14 22:49 Geode_Hybrid-2.0.4rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      700 b- defN 23-Jun-14 22:49 Geode_Hybrid-2.0.4rc2.dist-info/RECORD
+8 files, 2304390 bytes uncompressed, 1109773 bytes compressed:  51.8%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: geode_hybrid/__init__.py
 Comment: 
 
 Filename: geode_hybrid/brep.py
 Comment: 
 
-Filename: Geode_Hybrid-2.0.4rc1.dist-info/METADATA
+Filename: geode_hybrid/bin/Geode-Hybrid_brep.dll
 Comment: 
 
-Filename: Geode_Hybrid-2.0.4rc1.dist-info/WHEEL
+Filename: geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Hybrid-2.0.4rc1.dist-info/top_level.txt
+Filename: Geode_Hybrid-2.0.4rc2.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Hybrid-2.0.4rc1.dist-info/RECORD
+Filename: Geode_Hybrid-2.0.4rc2.dist-info/WHEEL
+Comment: 
+
+Filename: Geode_Hybrid-2.0.4rc2.dist-info/top_level.txt
+Comment: 
+
+Filename: Geode_Hybrid-2.0.4rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Geode_Hybrid-2.0.4rc1.dist-info/METADATA` & `Geode_Hybrid-2.0.4rc2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-Hybrid
-Version: 2.0.4rc1
+Version: 2.0.4rc2
 Summary: Hybrid remeshing Geode-solutions OpenGeode module
 Home-page: https://github.com/Geode-solutions/Geode-Hybrid
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.4rc1 Summary: Hybrid
+Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.4rc2 Summary: Hybrid
 remeshing Geode-solutions OpenGeode module Home-page: https://github.com/Geode-
 solutions/Geode-Hybrid Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
 text/markdown Requires-Dist: geode-background (==7.*,>=7.2.1) Requires-Dist:
 geode-common (==26.*,>=26.1.0rc2) Requires-Dist: geode-numerics (==3.*,>=3.0.5)
 Requires-Dist: geode-simplex (==6.*,>=6.0.12rc2) Requires-Dist: opengeode-core
 (==14.*,>=14.3.2rc3)
```

