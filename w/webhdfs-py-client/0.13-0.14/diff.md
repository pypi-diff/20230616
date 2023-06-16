# Comparing `tmp/webhdfs_py_client-0.13-py2.py3-none-any.whl.zip` & `tmp/webhdfs_py_client-0.14-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 11274 bytes, number of entries: 12
+Zip file size: 12765 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Jun-15 20:24 webhdfs_py/__init__.py
 -rw-rw-rw-  2.0 fat      493 b- defN 23-Jun-01 19:50 webhdfs_py/errors.py
 -rw-rw-rw-  2.0 fat      445 b- defN 23-Jun-16 15:34 webhdfs_py/operations.py
 -rw-rw-rw-  2.0 fat    28050 b- defN 23-Jun-16 15:36 webhdfs_py/webhdfs.py
+-rw-rw-rw-  2.0 fat     2941 b- defN 23-Jun-16 18:07 webhdfs_py/example/README.py
 -rw-rw-rw-  2.0 fat       38 b- defN 23-Jun-15 20:46 webhdfs_py/example/__init__.py
 -rw-rw-rw-  2.0 fat      372 b- defN 23-Jun-16 18:01 webhdfs_py/example/run.py
 -rw-rw-rw-  2.0 fat      390 b- defN 23-Jun-01 02:08 webhdfs_py/example/utils.py
--rw-rw-rw-  2.0 fat     5484 b- defN 23-Jun-16 18:00 webhdfs_py/example/pages/main.py
--rw-rw-rw-  2.0 fat     3772 b- defN 23-Jun-16 18:03 webhdfs_py_client-0.13.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-16 18:03 webhdfs_py_client-0.13.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-16 18:03 webhdfs_py_client-0.13.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      985 b- defN 23-Jun-16 18:03 webhdfs_py_client-0.13.dist-info/RECORD
-12 files, 40196 bytes uncompressed, 9610 bytes compressed:  76.1%
+-rw-rw-rw-  2.0 fat     5484 b- defN 23-Jun-16 18:07 webhdfs_py/example/pages/main.py
+-rw-rw-rw-  2.0 fat     3772 b- defN 23-Jun-16 18:07 webhdfs_py_client-0.14.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-16 18:07 webhdfs_py_client-0.14.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-16 18:07 webhdfs_py_client-0.14.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1070 b- defN 23-Jun-16 18:07 webhdfs_py_client-0.14.dist-info/RECORD
+13 files, 43222 bytes uncompressed, 10969 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -6,32 +6,35 @@
 
 Filename: webhdfs_py/operations.py
 Comment: 
 
 Filename: webhdfs_py/webhdfs.py
 Comment: 
 
+Filename: webhdfs_py/example/README.py
+Comment: 
+
 Filename: webhdfs_py/example/__init__.py
 Comment: 
 
 Filename: webhdfs_py/example/run.py
 Comment: 
 
 Filename: webhdfs_py/example/utils.py
 Comment: 
 
 Filename: webhdfs_py/example/pages/main.py
 Comment: 
 
-Filename: webhdfs_py_client-0.13.dist-info/METADATA
+Filename: webhdfs_py_client-0.14.dist-info/METADATA
 Comment: 
 
-Filename: webhdfs_py_client-0.13.dist-info/WHEEL
+Filename: webhdfs_py_client-0.14.dist-info/WHEEL
 Comment: 
 
-Filename: webhdfs_py_client-0.13.dist-info/top_level.txt
+Filename: webhdfs_py_client-0.14.dist-info/top_level.txt
 Comment: 
 
-Filename: webhdfs_py_client-0.13.dist-info/RECORD
+Filename: webhdfs_py_client-0.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webhdfs_py/example/pages/main.py

```diff
@@ -118,8 +118,8 @@
                 st.code(
                     """hdfs = PyWebHdfsClient(host='host',port='50070', user_name='hdfs') 
                     my_file = 'user/hdfs/data/myfile.txt' 
                     hdfs.delete_file_dir(my_file)""")
 
 
     else:
-         st.write(open(BASE_DIR /'README.MD', 'r', encoding='utf-8').read())
+         st.write(open(BASE_DIR /'README.py', 'r', encoding='utf-8').read())
```

## Comparing `webhdfs_py_client-0.13.dist-info/METADATA` & `webhdfs_py_client-0.14.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhdfs-py-client
-Version: 0.13
+Version: 0.14
 Summary: Python wrapper for the Hadoop WebHDFS REST API
 Home-page: 
 Author: Erik Alejandro Abdala
 Author-email: e.ale.abdala@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `webhdfs_py_client-0.13.dist-info/RECORD` & `webhdfs_py_client-0.14.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 webhdfs_py/__init__.py,sha256=b9mi_EOUiHBBqKdbLbluJuiCdCLaBLnOK5pHEYvBNPM,46
 webhdfs_py/errors.py,sha256=3YiIz_-1WP8YIwxENcZEmgzQBHiJsCMxxxpafLlOo88,493
 webhdfs_py/operations.py,sha256=nv1hfD1wK__2EtfCiNP-CHSltAPsx4HNpvBnoABpPeo,445
 webhdfs_py/webhdfs.py,sha256=sEh0k2dCt-mu-MrQ3MfcXY26UcMOzvU52dqwaWK977o,28050
+webhdfs_py/example/README.py,sha256=NQZuoeABZMz4z2jHFtfvaZFLG0eqRv8tca822IruAdw,2941
 webhdfs_py/example/__init__.py,sha256=V0cl8MZIMc93oz3NIgy3qBw_oNUtGxOcdZ0uCTE7QIQ,38
 webhdfs_py/example/run.py,sha256=rskbfNZWigTD_SN2yjCPRJfTOtymRP9rNGowOa0TiNA,372
 webhdfs_py/example/utils.py,sha256=TpXLcEeK1zmPAwyWCYh3TZL2BWl0Pp1_H19f1Fpcihc,390
-webhdfs_py/example/pages/main.py,sha256=3ajWDPe1US75DAEdm8UCofe_vFUPgRr_GtmqDnFuUlo,5484
-webhdfs_py_client-0.13.dist-info/METADATA,sha256=WlZLYg6JGrJRY8Ogbk5Y00JhZAniV8oC2nCwaQmIEjc,3772
-webhdfs_py_client-0.13.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-webhdfs_py_client-0.13.dist-info/top_level.txt,sha256=U-g45ZCFQMp3TX9DsicMZluP7m5tVb_V88Xs3Wj5A1Q,11
-webhdfs_py_client-0.13.dist-info/RECORD,,
+webhdfs_py/example/pages/main.py,sha256=cnc22lFv-5ES2kp0uW2_x_LdUP-xO7QbjIUwejtY8z8,5484
+webhdfs_py_client-0.14.dist-info/METADATA,sha256=olG-wAwKlUjV3ZARkb-NUKIkD_RuWxlWLouzOmwDze4,3772
+webhdfs_py_client-0.14.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+webhdfs_py_client-0.14.dist-info/top_level.txt,sha256=U-g45ZCFQMp3TX9DsicMZluP7m5tVb_V88Xs3Wj5A1Q,11
+webhdfs_py_client-0.14.dist-info/RECORD,,
```

