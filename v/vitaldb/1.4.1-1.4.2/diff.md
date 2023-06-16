# Comparing `tmp/vitaldb-1.4.1-py3-none-any.whl.zip` & `tmp/vitaldb-1.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 54942 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   103087 b- defN 22-Jun-27 00:52 vitaldb/__init__.py
--rw-rw-rw-  2.0 fat     4497 b- defN 23-Apr-03 06:42 vitaldb/api.py
--rw-rw-rw-  2.0 fat     3305 b- defN 22-Sep-19 15:02 vitaldb/dataset.py
--rw-rw-rw-  2.0 fat    80162 b- defN 23-Jun-11 21:54 vitaldb/utils.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      520 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      682 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/RECORD
-9 files, 193438 bytes uncompressed, 53784 bytes compressed:  72.2%
+Zip file size: 54953 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   103087 b- defN 23-Jun-16 07:55 vitaldb/__init__.py
+-rw-rw-rw-  2.0 fat     4653 b- defN 23-Jun-16 07:55 vitaldb/api.py
+-rw-rw-rw-  2.0 fat     3305 b- defN 23-Jun-16 07:55 vitaldb/dataset.py
+-rw-rw-rw-  2.0 fat    80200 b- defN 23-Jun-16 07:55 vitaldb/utils.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-16 07:57 vitaldb-1.4.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      520 b- defN 23-Jun-16 07:57 vitaldb-1.4.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-16 07:57 vitaldb-1.4.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-16 07:57 vitaldb-1.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      682 b- defN 23-Jun-16 07:57 vitaldb-1.4.2.dist-info/RECORD
+9 files, 193632 bytes uncompressed, 53795 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: vitaldb/dataset.py
 Comment: 
 
 Filename: vitaldb/utils.py
 Comment: 
 
-Filename: vitaldb-1.4.1.dist-info/LICENSE
+Filename: vitaldb-1.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: vitaldb-1.4.1.dist-info/METADATA
+Filename: vitaldb-1.4.2.dist-info/METADATA
 Comment: 
 
-Filename: vitaldb-1.4.1.dist-info/WHEEL
+Filename: vitaldb-1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: vitaldb-1.4.1.dist-info/top_level.txt
+Filename: vitaldb-1.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: vitaldb-1.4.1.dist-info/RECORD
+Filename: vitaldb-1.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vitaldb/api.py

```diff
@@ -118,31 +118,35 @@
     if os.path.isdir(localpath):
         localpath = os.path.join(localpath, filename)
     with open(localpath, "wb") as f:
         f.write(res.content)
     return True
 
 
-def receive(vrcode, bedname=None, dtstart=None, dtend=None):
+def receive(vrcode=None, bedname=None, dtstart=None, dtend=None):
+    global access_token
+    if access_token is None:
+        raise Exception('Please login first')
+
     if isinstance(dtstart, datetime.datetime):
         dtstart = dtstart.timestamp()
     if isinstance(dtend, datetime.datetime):
         dtend = dtend.timestamp()
-    pars = {'vrcode':vrcode}
+    pars = {"access_token": access_token, 'vrcode':vrcode}
     if bedname:
         pars['bedname'] = bedname
     if dtstart:
         pars['dtstart'] = dtstart
     if dtend:
         pars['dtend'] = dtend
 
     res = requests.get(API_URL + "receive", params=pars)
     if 200 != res.status_code:
         raise Exception('API Server Error: ' + res.content.decode('utf-8'))
-    return json.loads(res.content)
+    return json.loads(gzip.decompress(res.content))
 
 
 if __name__ == '__main__':
     # path to save downloaded files
     DOWNLOAD_DIR = "Download"
     if not os.path.exists(DOWNLOAD_DIR):
         os.mkdir(DOWNLOAD_DIR)
```

## vitaldb/utils.py

```diff
@@ -1726,14 +1726,16 @@
             ret.extend(list_wfdb(f'{dbname}/{hea_name}'))
         else:
             ret.append(f'{dbname}/{hea_name}.hea')
     return ret
 
 
 if __name__ == '__main__':
+    VitalFile('1.vital')
+    quit()
     srate = 500  # sampling rate for ecg
 
     # sample data from the VitalDB open dataset
     vf = VitalFile(1, ['ECG_II', 'HR'])
     ecg = vf.to_numpy('ECG_II', 1/srate).flatten()  # ecg waveform (500Hz) = [     nan      nan      nan ... 0.33651  0.435255 0.237764]
     hrs = vf.to_numpy('HR', 1).flatten()  # heart rates (1 sec) = [nan 88. nan ... nan nan nan]
```

## Comparing `vitaldb-1.4.1.dist-info/LICENSE` & `vitaldb-1.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vitaldb-1.4.1.dist-info/METADATA` & `vitaldb-1.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitaldb
-Version: 1.4.1
+Version: 1.4.2
 Summary: VitalDB Python Libray
 Home-page: https://github.com/vitaldb/vitalutils
 Author: Hyung-Chul Lee
 Author-email: vital@snu.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `vitaldb-1.4.1.dist-info/RECORD` & `vitaldb-1.4.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 vitaldb/__init__.py,sha256=ZAUDnWqcM5E6UVFwF4GrevwVeYjH3SvonnTeXpse7X4,103087
-vitaldb/api.py,sha256=doQkWvCV2Lxt4srHKIDiGFWCafTmuyhl-DAzLzNO-TE,4497
+vitaldb/api.py,sha256=Kdmz9GGHSqLrgIPyZX_EnoR0ritjdCiRAWKtsIbpguc,4653
 vitaldb/dataset.py,sha256=qlwphbk8ayfdMdPsQtHZNHfXQPYQtx0yC5QVCn66tVw,3305
-vitaldb/utils.py,sha256=_6ABHDz5bJ863QiT_TTKcta2n1Ho9d33n12FRz3deSY,80162
-vitaldb-1.4.1.dist-info/LICENSE,sha256=h_p8qyePNkMbAgB4B_dsGwtNhTR3fSM38fGQIpTuodI,1085
-vitaldb-1.4.1.dist-info/METADATA,sha256=bDmTBTzjytUrtaNeMjvZ_OVqjiZVil5nwgWlqm6o5Ww,520
-vitaldb-1.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vitaldb-1.4.1.dist-info/top_level.txt,sha256=xJoTTkaIm_WeMoAfX0de2vl5Ns40HOLc0FX-dI2IoDw,8
-vitaldb-1.4.1.dist-info/RECORD,,
+vitaldb/utils.py,sha256=SDSsvaTsPc4MQjIk-Z_EsX7Fu6vyq0mxGRWhEJQgTfE,80200
+vitaldb-1.4.2.dist-info/LICENSE,sha256=h_p8qyePNkMbAgB4B_dsGwtNhTR3fSM38fGQIpTuodI,1085
+vitaldb-1.4.2.dist-info/METADATA,sha256=rKgWr5qM9ZVLPat0hGeJd7vlZkZOiEXsEzHl588rtDM,520
+vitaldb-1.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vitaldb-1.4.2.dist-info/top_level.txt,sha256=xJoTTkaIm_WeMoAfX0de2vl5Ns40HOLc0FX-dI2IoDw,8
+vitaldb-1.4.2.dist-info/RECORD,,
```

