# Comparing `tmp/fast_model_server-1.1.0.0-py2.py3-none-any.whl.zip` & `tmp/fast_model_server-1.1.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 41546 bytes, number of entries: 44
+Zip file size: 41545 bytes, number of entries: 44
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/__init__.py
 -rw-rw-r--  2.0 unx     3880 b- defN 23-Jun-13 00:53 fast_model_server/application.py
 -rw-rw-r--  2.0 unx     1836 b- defN 23-Jun-13 15:35 fast_model_server/common.py
 -rw-rw-r--  2.0 unx    15304 b- defN 23-Jun-13 15:35 fast_model_server/create.py
 -rw-rw-r--  2.0 unx    11823 b- defN 23-Jun-13 15:35 fast_model_server/main.py
 -rw-rw-r--  2.0 unx      343 b- defN 23-Jun-13 15:35 fast_model_server/router_service.py
 -rw-r--r--  2.0 unx      975 b- defN 23-Jun-13 03:10 fast_model_server/template/router/common.py.template
@@ -35,12 +35,12 @@
 -rw-r--r--  2.0 unx       90 b- defN 23-Jun-13 00:53 fast_model_server/utils/model_manage/model_manage.config.json
 -rw-rw-r--  2.0 unx     4722 b- defN 23-Jun-13 15:57 fast_model_server/utils/model_manage/model_manage.py
 -rw-r--r--  2.0 unx      648 b- defN 23-Jun-13 00:53 fast_model_server/utils/model_manage/pack.sh
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/utils/rule/__init__.py
 -rw-rw-r--  2.0 unx     4059 b- defN 23-Jun-13 16:01 fast_model_server/utils/rule/rule.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 00:53 fast_model_server/utils/rule/test/__init__.py
 -rw-rw-r--  2.0 unx     1464 b- defN 23-Jun-13 15:45 fast_model_server/utils/rule/test/test_rule.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-14 06:47 fast_model_server-1.1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-14 06:47 fast_model_server-1.1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Jun-14 06:47 fast_model_server-1.1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4455 b- defN 23-Jun-14 06:47 fast_model_server-1.1.0.0.dist-info/RECORD
-44 files, 110026 bytes uncompressed, 34106 bytes compressed:  69.0%
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-16 08:04 fast_model_server-1.1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-16 08:04 fast_model_server-1.1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jun-16 08:04 fast_model_server-1.1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4455 b- defN 23-Jun-16 08:04 fast_model_server-1.1.0.1.dist-info/RECORD
+44 files, 110026 bytes uncompressed, 34105 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -114,20 +114,20 @@
 
 Filename: fast_model_server/utils/rule/test/__init__.py
 Comment: 
 
 Filename: fast_model_server/utils/rule/test/test_rule.py
 Comment: 
 
-Filename: fast_model_server-1.1.0.0.dist-info/METADATA
+Filename: fast_model_server-1.1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: fast_model_server-1.1.0.0.dist-info/WHEEL
+Filename: fast_model_server-1.1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: fast_model_server-1.1.0.0.dist-info/top_level.txt
+Filename: fast_model_server-1.1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fast_model_server-1.1.0.0.dist-info/RECORD
+Filename: fast_model_server-1.1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fast_model_server-1.1.0.0.dist-info/METADATA` & `fast_model_server-1.1.0.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: fast-model-server
-Version: 1.1.0.0
+Version: 1.1.0.1
 Summary: python基础服务框架
 Home-page: https://codeup.aliyun.com/64650c96168f0a5963451dec/lib/fast-model-server/blob/master/README.md
 Author: yes_bobo
 Author-email: fb_linux@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi (==0.63.0)
-Requires-Dist: uvicorn (==0.15.0)
-Requires-Dist: pydantic (==1.8.2)
-Requires-Dist: typing (==3.7.4.3)
-Requires-Dist: aiofiles (==0.8.0)
-Requires-Dist: rule-engine (==3.5.0)
-Requires-Dist: langchain (==0.0.194)
+Requires-Dist: fastapi (>=0.63.0)
+Requires-Dist: uvicorn (>=0.15.0)
+Requires-Dist: pydantic (>=1.8.2)
+Requires-Dist: typing (>=3.7.4.3)
+Requires-Dist: aiofiles (>=0.8.0)
+Requires-Dist: rule-engine (>=3.5.0)
+Requires-Dist: langchain (>=0.0.194)
 Requires-Dist: dash (==2.7.1)
 Requires-Dist: bce-python-sdk
 Requires-Dist: httpx
 Requires-Dist: tqdm
 Requires-Dist: redis
 Requires-Dist: networkx
```

## Comparing `fast_model_server-1.1.0.0.dist-info/RECORD` & `fast_model_server-1.1.0.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -34,11 +34,11 @@
 fast_model_server/utils/model_manage/model_manage.config.json,sha256=7IUID818YotaZquUQSvSozv1fn3qf-t7-0Sa5ulwVMo,90
 fast_model_server/utils/model_manage/model_manage.py,sha256=k593aX4Z7EgA9O0Il2TFxLUKeQI2i35nc6dVh1CdHmo,4722
 fast_model_server/utils/model_manage/pack.sh,sha256=NJ76Y6snY5ngmIOmm8g2ZeALETRbpDmRZ9Zyy2D-c28,648
 fast_model_server/utils/rule/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fast_model_server/utils/rule/rule.py,sha256=sq8K2HorzeGAaxb3FSatgUIl0DF6xy7Xgbp4Sfj7ZXk,4059
 fast_model_server/utils/rule/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fast_model_server/utils/rule/test/test_rule.py,sha256=CzysHmPMJ3hLDouzWm-er0QLDb4ojBEKVaVllFhTo_8,1464
-fast_model_server-1.1.0.0.dist-info/METADATA,sha256=LFXPqRXz3GHrR6JDBp1q9dF1OVWbgG0yzSSYNl4iM2k,2727
-fast_model_server-1.1.0.0.dist-info/WHEEL,sha256=oh0NKYrTcu1i1-wgrI1cnhkjYIi8WJ-8qd9Jrr5_y4E,110
-fast_model_server-1.1.0.0.dist-info/top_level.txt,sha256=v0z-TTFnnZC-On43gY1hMZaNWjxGkerzZ4eaqcrqbBo,18
-fast_model_server-1.1.0.0.dist-info/RECORD,,
+fast_model_server-1.1.0.1.dist-info/METADATA,sha256=qkKHGL0SdDrBRqstKvdAzWoR69YfpJ2yQNVOYxTK4Mw,2727
+fast_model_server-1.1.0.1.dist-info/WHEEL,sha256=oh0NKYrTcu1i1-wgrI1cnhkjYIi8WJ-8qd9Jrr5_y4E,110
+fast_model_server-1.1.0.1.dist-info/top_level.txt,sha256=v0z-TTFnnZC-On43gY1hMZaNWjxGkerzZ4eaqcrqbBo,18
+fast_model_server-1.1.0.1.dist-info/RECORD,,
```

