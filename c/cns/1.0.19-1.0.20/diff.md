# Comparing `tmp/cns-1.0.19-py3-none-any.whl.zip` & `tmp/cns-1.0.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 399371 bytes, number of entries: 15
+Zip file size: 403283 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat   173056 b- defN 23-Jun-15 05:40 cns/DataX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   156672 b- defN 23-Jun-15 05:40 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    75264 b- defN 23-Jun-16 07:35 cns/TextX.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    64000 b- defN 23-Jun-16 07:35 cns/TextX.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    78848 b- defN 23-Jun-16 12:54 cns/TextX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    68096 b- defN 23-Jun-16 12:55 cns/TextX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      342 b- defN 23-Jun-15 01:47 cns/__init__.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-16 08:43 cns-1.0.19.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1905 b- defN 23-Jun-16 08:43 cns-1.0.19.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-16 08:43 cns-1.0.19.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-16 08:43 cns-1.0.19.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1228 b- defN 23-Jun-16 08:43 cns-1.0.19.dist-info/RECORD
-15 files, 903633 bytes uncompressed, 397363 bytes compressed:  56.0%
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-16 13:09 cns-1.0.20.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1905 b- defN 23-Jun-16 13:09 cns-1.0.20.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-16 13:09 cns-1.0.20.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-16 13:09 cns-1.0.20.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1228 b- defN 23-Jun-16 13:09 cns-1.0.20.dist-info/RECORD
+15 files, 911313 bytes uncompressed, 401275 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: cns/TextX.cp39-win_amd64.pyd
 Comment: 
 
 Filename: cns/__init__.py
 Comment: 
 
-Filename: cns-1.0.19.dist-info/LICENSE
+Filename: cns-1.0.20.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.19.dist-info/METADATA
+Filename: cns-1.0.20.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.19.dist-info/WHEEL
+Filename: cns-1.0.20.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.19.dist-info/top_level.txt
+Filename: cns-1.0.20.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.19.dist-info/RECORD
+Filename: cns-1.0.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cns-1.0.19.dist-info/METADATA` & `cns-1.0.20.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.19
+Version: 1.0.20
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: rambo
 Author-email: 6566666@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cns-1.0.19.dist-info/RECORD` & `cns-1.0.20.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 cns/DataX.cp36-win_amd64.pyd,sha256=vzrdaWShZrcUu-_pnaAJQxQ9kTXF599gecdQz-_6dTw,173056
 cns/DataX.cp39-win_amd64.pyd,sha256=eJ-mQhJro8bK9O0sO454tNLb-uvVDvmsSQSKtnodkmc,156672
 cns/DateTimeX.cp36-win32.pyd,sha256=X6jjFZbOMmTTqnw0r3SfmiTRG9RFEpRdfVyU6AiFvCk,82944
 cns/DateTimeX.cp36-win_amd64.pyd,sha256=w-g6QPTK_U3il2bFu7PcucBGixhSX2Gm4M54ItAYMTk,99840
 cns/DateTimeX.cp39-win_amd64.pyd,sha256=bp9N6_ettlJ1odtrHJ3qU_yTBAsvULggzIyfz-eJuEk,88576
 cns/SQLstrX.cp36-win_amd64.pyd,sha256=3NLRKJa7q2Dl1sKlzVBbScgYjcgoSgMOClS2BuxDIzI,84992
 cns/SQLstrX.cp39-win_amd64.pyd,sha256=B0wq2UBpInSyGEq6aGOvKiqwAov8_ynHtlkPnaYav8k,74240
-cns/TextX.cp36-win_amd64.pyd,sha256=MsRYZcpDL9xsj8DA8xtwaMC-qN9foWXREjZgivYq5NY,75264
-cns/TextX.cp39-win_amd64.pyd,sha256=YD3ORE6GAfAI9wQAg4GvDX4907YXoBBvc9OpWheZwmU,64000
+cns/TextX.cp36-win_amd64.pyd,sha256=wx5TIuhcbvWGLDnL_slEzGvKl7SftO4rd6M4dNxyCnc,78848
+cns/TextX.cp39-win_amd64.pyd,sha256=m3JQI8gBobDLLqdgA7wx-BT0xQ6kBX0kraP-51VC59w,68096
 cns/__init__.py,sha256=E3XCxd-Z01Q13FBOOMwYpfPHdhGSSaB12uEwy33EqBg,342
-cns-1.0.19.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.0.19.dist-info/METADATA,sha256=PSa3bA4elNdCMLUXEaVFxYVztTUpyUXikUKuHnf6u1Y,1905
-cns-1.0.19.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.0.19.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.0.19.dist-info/RECORD,,
+cns-1.0.20.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.0.20.dist-info/METADATA,sha256=Bdwi-mpuRSay0TgaQIZ9EoxuloAj8DrT-ZK9sVCRI1s,1905
+cns-1.0.20.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.0.20.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.0.20.dist-info/RECORD,,
```

