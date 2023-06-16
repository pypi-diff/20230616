# Comparing `tmp/webhdfs_py_client-0.10-py2.py3-none-any.whl.zip` & `tmp/webhdfs_py_client-0.11-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,14 @@
-Zip file size: 13053 bytes, number of entries: 14
+Zip file size: 11274 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Jun-15 20:24 webhdfs_py/__init__.py
 -rw-rw-rw-  2.0 fat      493 b- defN 23-Jun-01 19:50 webhdfs_py/errors.py
 -rw-rw-rw-  2.0 fat      445 b- defN 23-Jun-16 15:34 webhdfs_py/operations.py
 -rw-rw-rw-  2.0 fat    28050 b- defN 23-Jun-16 15:36 webhdfs_py/webhdfs.py
 -rw-rw-rw-  2.0 fat       38 b- defN 23-Jun-15 20:46 webhdfs_py/example/__init__.py
--rw-rw-rw-  2.0 fat     1160 b- defN 23-Jun-01 02:02 webhdfs_py/example/hello.py
 -rw-rw-rw-  2.0 fat      372 b- defN 23-Jun-16 17:49 webhdfs_py/example/run.py
 -rw-rw-rw-  2.0 fat      390 b- defN 23-Jun-01 02:08 webhdfs_py/example/utils.py
--rw-rw-rw-  2.0 fat     1651 b- defN 23-Jun-15 21:25 webhdfs_py/example/pages/dataframe.py
 -rw-rw-rw-  2.0 fat     5491 b- defN 23-Jun-16 17:38 webhdfs_py/example/pages/main.py
--rw-rw-rw-  2.0 fat     3772 b- defN 23-Jun-16 17:50 webhdfs_py_client-0.10.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-16 17:50 webhdfs_py_client-0.10.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-16 17:50 webhdfs_py_client-0.10.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1163 b- defN 23-Jun-16 17:50 webhdfs_py_client-0.10.dist-info/RECORD
-14 files, 43192 bytes uncompressed, 11109 bytes compressed:  74.3%
+-rw-rw-rw-  2.0 fat     3772 b- defN 23-Jun-16 17:55 webhdfs_py_client-0.11.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-16 17:55 webhdfs_py_client-0.11.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-16 17:55 webhdfs_py_client-0.11.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      985 b- defN 23-Jun-16 17:55 webhdfs_py_client-0.11.dist-info/RECORD
+12 files, 40203 bytes uncompressed, 9610 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -9,35 +9,29 @@
 
 Filename: webhdfs_py/webhdfs.py
 Comment: 
 
 Filename: webhdfs_py/example/__init__.py
 Comment: 
 
-Filename: webhdfs_py/example/hello.py
-Comment: 
-
 Filename: webhdfs_py/example/run.py
 Comment: 
 
 Filename: webhdfs_py/example/utils.py
 Comment: 
 
-Filename: webhdfs_py/example/pages/dataframe.py
-Comment: 
-
 Filename: webhdfs_py/example/pages/main.py
 Comment: 
 
-Filename: webhdfs_py_client-0.10.dist-info/METADATA
+Filename: webhdfs_py_client-0.11.dist-info/METADATA
 Comment: 
 
-Filename: webhdfs_py_client-0.10.dist-info/WHEEL
+Filename: webhdfs_py_client-0.11.dist-info/WHEEL
 Comment: 
 
-Filename: webhdfs_py_client-0.10.dist-info/top_level.txt
+Filename: webhdfs_py_client-0.11.dist-info/top_level.txt
 Comment: 
 
-Filename: webhdfs_py_client-0.10.dist-info/RECORD
+Filename: webhdfs_py_client-0.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `webhdfs_py_client-0.10.dist-info/METADATA` & `webhdfs_py_client-0.11.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhdfs-py-client
-Version: 0.10
+Version: 0.11
 Summary: Python wrapper for the Hadoop WebHDFS REST API
 Home-page: 
 Author: Erik Alejandro Abdala
 Author-email: e.ale.abdala@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `webhdfs_py_client-0.10.dist-info/RECORD` & `webhdfs_py_client-0.11.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 webhdfs_py/__init__.py,sha256=b9mi_EOUiHBBqKdbLbluJuiCdCLaBLnOK5pHEYvBNPM,46
 webhdfs_py/errors.py,sha256=3YiIz_-1WP8YIwxENcZEmgzQBHiJsCMxxxpafLlOo88,493
 webhdfs_py/operations.py,sha256=nv1hfD1wK__2EtfCiNP-CHSltAPsx4HNpvBnoABpPeo,445
 webhdfs_py/webhdfs.py,sha256=sEh0k2dCt-mu-MrQ3MfcXY26UcMOzvU52dqwaWK977o,28050
 webhdfs_py/example/__init__.py,sha256=V0cl8MZIMc93oz3NIgy3qBw_oNUtGxOcdZ0uCTE7QIQ,38
-webhdfs_py/example/hello.py,sha256=Z77VQ8JSZq0-bT129HVCkH8vqMMBPFWBFX9b5IlKA58,1160
 webhdfs_py/example/run.py,sha256=rskbfNZWigTD_SN2yjCPRJfTOtymRP9rNGowOa0TiNA,372
 webhdfs_py/example/utils.py,sha256=TpXLcEeK1zmPAwyWCYh3TZL2BWl0Pp1_H19f1Fpcihc,390
-webhdfs_py/example/pages/dataframe.py,sha256=YAWElNV6wCXzsSyifx4gc3WbtUTJZzyxKGrwdQ79eQ8,1651
 webhdfs_py/example/pages/main.py,sha256=iJMbAqwmr2FxKCj-MTHrIR--ey444Sk72PorzLo8BPU,5491
-webhdfs_py_client-0.10.dist-info/METADATA,sha256=hM88Ya_rxZj7EIDUX3D81VqcwpXRV7kvi0nsxScXH_I,3772
-webhdfs_py_client-0.10.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-webhdfs_py_client-0.10.dist-info/top_level.txt,sha256=U-g45ZCFQMp3TX9DsicMZluP7m5tVb_V88Xs3Wj5A1Q,11
-webhdfs_py_client-0.10.dist-info/RECORD,,
+webhdfs_py_client-0.11.dist-info/METADATA,sha256=_0lcCoRYE5TxOhz4RHfepHlgewWtU1xDuw899TDC4gw,3772
+webhdfs_py_client-0.11.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+webhdfs_py_client-0.11.dist-info/top_level.txt,sha256=U-g45ZCFQMp3TX9DsicMZluP7m5tVb_V88Xs3Wj5A1Q,11
+webhdfs_py_client-0.11.dist-info/RECORD,,
```

