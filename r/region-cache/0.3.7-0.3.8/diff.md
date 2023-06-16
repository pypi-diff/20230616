# Comparing `tmp/region_cache-0.3.7-py2.py3-none-any.whl.zip` & `tmp/region_cache-0.3.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10377 bytes, number of entries: 9
--rw-r--r--  2.0 unx     2182 b- defN 21-Dec-13 16:50 region_cache/__init__.py
--rw-r--r--  2.0 unx     8682 b- defN 21-Dec-13 17:04 region_cache/region.py
--rw-r--r--  2.0 unx    10506 b- defN 21-Dec-13 16:50 region_cache/region_cache.py
--rw-r--r--  2.0 unx      161 b- defN 21-Dec-13 18:18 region_cache-0.3.7.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx     1086 b- defN 21-Dec-13 18:18 region_cache-0.3.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4098 b- defN 21-Dec-13 18:18 region_cache-0.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Dec-13 18:18 region_cache-0.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 21-Dec-13 18:18 region_cache-0.3.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      754 b- defN 21-Dec-13 18:18 region_cache-0.3.7.dist-info/RECORD
-9 files, 27592 bytes uncompressed, 9075 bytes compressed:  67.1%
+Zip file size: 10350 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     2182 b- defN 23-Jun-16 13:45 region_cache/__init__.py
+-rw-r--r--  2.0 unx     8682 b- defN 23-Jun-16 13:45 region_cache/region.py
+-rw-r--r--  2.0 unx    10507 b- defN 23-Jun-16 13:45 region_cache/region_cache.py
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-16 13:48 region_cache-0.3.8.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx     1086 b- defN 23-Jun-16 13:48 region_cache-0.3.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4050 b- defN 23-Jun-16 13:48 region_cache-0.3.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-16 13:48 region_cache-0.3.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-16 13:48 region_cache-0.3.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      754 b- defN 23-Jun-16 13:48 region_cache-0.3.8.dist-info/RECORD
+9 files, 27545 bytes uncompressed, 9048 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: region_cache/region.py
 Comment: 
 
 Filename: region_cache/region_cache.py
 Comment: 
 
-Filename: region_cache-0.3.7.dist-info/AUTHORS.rst
+Filename: region_cache-0.3.8.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: region_cache-0.3.7.dist-info/LICENSE
+Filename: region_cache-0.3.8.dist-info/LICENSE
 Comment: 
 
-Filename: region_cache-0.3.7.dist-info/METADATA
+Filename: region_cache-0.3.8.dist-info/METADATA
 Comment: 
 
-Filename: region_cache-0.3.7.dist-info/WHEEL
+Filename: region_cache-0.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: region_cache-0.3.7.dist-info/top_level.txt
+Filename: region_cache-0.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: region_cache-0.3.7.dist-info/RECORD
+Filename: region_cache-0.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## region_cache/region_cache.py

```diff
@@ -240,15 +240,15 @@
             names.append(self._root_name)
         parts = []
         fqname = ''
         while names:
             parts.append(names.pop())
             fqname = '.'.join(parts)
             if fqname not in self._regions:
-                _logger.info("Initializing region %s", fqname)
+                _logger.debug("Initializing region %s", fqname)
                 self._regions[fqname] = Region(
                     self, fqname,
                     timeout=timeout,
                     update_resets_timeout=update_resets_timeout,
                     serializer=serializer or self._serializer
                 )
```

## Comparing `region_cache-0.3.7.dist-info/LICENSE` & `region_cache-0.3.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `region_cache-0.3.7.dist-info/METADATA` & `region_cache-0.3.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: region-cache
-Version: 0.3.7
+Version: 0.3.8
 Summary: Region-based caching for Python/Flask with Redis
 Home-page: https://github.com/jheard-tw/region_cache
 Author: Jefferson Heard
 Author-email: jheard@teamworks.com
 License: MIT license
 Keywords: region_cache
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-License-File: LICENSE
-License-File: AUTHORS.rst
 Requires-Dist: blinker
 Requires-Dist: redis
 Requires-Dist: hiredis
 
 ============
 region_cache
 ============
```

## Comparing `region_cache-0.3.7.dist-info/RECORD` & `region_cache-0.3.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 region_cache/__init__.py,sha256=gKy8BaPyQOOSm3fTPmA3yvIHilQfn_1gK1zCiVjlRG8,2182
 region_cache/region.py,sha256=lj9H_sB1IC0XgA62IJdSayK_KNZ_C3w_NmeruQWtk6Q,8682
-region_cache/region_cache.py,sha256=R9vj7a-ag-zSgeDyQwHGebbXVCty7DeXdScRmKw2Dh0,10506
-region_cache-0.3.7.dist-info/AUTHORS.rst,sha256=1qLyDUoIsb26FLlZHceekMbQhBgyEBwMwoFFbUxnxAg,161
-region_cache-0.3.7.dist-info/LICENSE,sha256=gIdd3k39VuAb7sew6jiToWOEQxB-J1cr2s-5upe-bLc,1086
-region_cache-0.3.7.dist-info/METADATA,sha256=RJNbmtK9VLhyzouPSMs853UCdb3Iaf82WAJCtfraJNA,4098
-region_cache-0.3.7.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-region_cache-0.3.7.dist-info/top_level.txt,sha256=2CyJ98gwgGn8dLqXngtfDK4KfOneLJIkALa6sQcL7jw,13
-region_cache-0.3.7.dist-info/RECORD,,
+region_cache/region_cache.py,sha256=nsmM9MpaxjLRV3geNrzHxGrUH5TGShAU0q1cFuNp-e8,10507
+region_cache-0.3.8.dist-info/AUTHORS.rst,sha256=1qLyDUoIsb26FLlZHceekMbQhBgyEBwMwoFFbUxnxAg,161
+region_cache-0.3.8.dist-info/LICENSE,sha256=gIdd3k39VuAb7sew6jiToWOEQxB-J1cr2s-5upe-bLc,1086
+region_cache-0.3.8.dist-info/METADATA,sha256=CvNecWNq1Q049ScMGMXWeuNERj4joeM48dSl2l8LVi0,4050
+region_cache-0.3.8.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
+region_cache-0.3.8.dist-info/top_level.txt,sha256=2CyJ98gwgGn8dLqXngtfDK4KfOneLJIkALa6sQcL7jw,13
+region_cache-0.3.8.dist-info/RECORD,,
```

