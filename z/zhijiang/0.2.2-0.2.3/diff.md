# Comparing `tmp/zhijiang-0.2.2-py3-none-any.whl.zip` & `tmp/zhijiang-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 9828 bytes, number of entries: 17
+Zip file size: 9841 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx     2651 b- defN 23-Jun-09 06:16 zhijiang/__init__.py
 -rw-rw-r--  2.0 unx      231 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/alias
 -rw-rw-r--  2.0 unx       75 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/dockerignore
 -rw-rw-r--  2.0 unx      393 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/gdbinit
 -rw-rw-r--  2.0 unx      118 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/gitconfig
 -rw-rw-r--  2.0 unx      561 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/inputrc
 -rw-rw-r--  2.0 unx      153 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/tmux.config
 -rw-rw-r--  2.0 unx      415 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/vimrc
 -rw-rw-r--  2.0 unx      480 b- defN 23-Jun-09 06:13 zhijiang/scripts/enhance_python.sh
 -rw-rw-r--  2.0 unx     1150 b- defN 23-Jun-09 06:13 zhijiang/scripts/install_useful_tools.sh
--rw-rw-r--  2.0 unx     6619 b- defN 23-Jun-12 02:31 zhijiang/scripts/useful_func.py
--rw-rw-r--  2.0 unx     1081 b- defN 23-Jun-12 02:36 zhijiang-0.2.2.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-12 02:36 zhijiang-0.2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 02:36 zhijiang-0.2.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       43 b- defN 23-Jun-12 02:36 zhijiang-0.2.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-12 02:36 zhijiang-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1449 b- defN 23-Jun-12 02:36 zhijiang-0.2.2.dist-info/RECORD
-17 files, 16441 bytes uncompressed, 7412 bytes compressed:  54.9%
+-rw-rw-r--  2.0 unx     6665 b- defN 23-Jun-16 02:50 zhijiang/scripts/useful_func.py
+-rw-rw-r--  2.0 unx     1081 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       43 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1449 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/RECORD
+17 files, 16487 bytes uncompressed, 7425 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: zhijiang/scripts/install_useful_tools.sh
 Comment: 
 
 Filename: zhijiang/scripts/useful_func.py
 Comment: 
 
-Filename: zhijiang-0.2.2.dist-info/LICENSE.txt
+Filename: zhijiang-0.2.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: zhijiang-0.2.2.dist-info/METADATA
+Filename: zhijiang-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: zhijiang-0.2.2.dist-info/WHEEL
+Filename: zhijiang-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: zhijiang-0.2.2.dist-info/entry_points.txt
+Filename: zhijiang-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: zhijiang-0.2.2.dist-info/top_level.txt
+Filename: zhijiang-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: zhijiang-0.2.2.dist-info/RECORD
+Filename: zhijiang-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhijiang/scripts/useful_func.py

```diff
@@ -133,16 +133,17 @@
     import torch
     from viztracer import VizTracer
 
     if os.environ.get("VIZTRACER", "0") == "1":
         assert (
             os.environ["CUDA_LAUNCH_BLOCKING"] == "1"
         ), "CUDA_LAUNCH_BLOCKING must be set to 1 when using VizTracer to profile CUDA code"
-        if step == 0:
-            tracer = VizTracer(output_file=f"trace_{os.getpid()}.json")
+        if step == 1:
+            global tracer
+            tracer = VizTracer(output_file=f"trace_{os.environ.get('LOCAL_RANK', 0)}.json")
         if step == int(os.environ.get("START_STEP", 10)):
             cprint("Start tracing", "red")
             tracer.start()
         if step == int(os.environ.get("END_STEP", 20)):
             cprint("Stop tracing", "red")
             tracer.stop()
             tracer.save()
@@ -172,15 +173,15 @@
 
 
 @zhijxu_run_once
 def zhijxu_enter_pdb_at_exception():
     """
         register a hook which will enter pdb when process wants to exit, this will help debugging when process has un-caught exception
     """
-    import axexit
+    import atexit
 
     atexit.register(pdb.pm)
 
 
 def zhijxu_open_onnx_in_tensorboard(model, port):
     """
     give the onnx model path and tensorboard port, then will convert to tensorboard and launch tensorboard automatically for you
```

## Comparing `zhijiang-0.2.2.dist-info/LICENSE.txt` & `zhijiang-0.2.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `zhijiang-0.2.2.dist-info/METADATA` & `zhijiang-0.2.3.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhijiang
-Version: 0.2.2
+Version: 0.2.3
 Summary: setup linux env, such as bashrc etc.
 Home-page: https://github.com/xu-zhijiang/env-setup.git
 Author: Xu Zhijiang
 Author-email: 15852939122@163.com
 Project-URL: Funding, https://github.com/xu-zhijiang
 Project-URL: Source, https://github.com/xu-zhijiang/env-setup.git
 Keywords: env setup,development,zhijiang
```

## Comparing `zhijiang-0.2.2.dist-info/RECORD` & `zhijiang-0.2.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 zhijiang/data/rc_files/gdbinit,sha256=Om1pIhhf-_lIfLgx8Gt730W2R4vvZLr05hbgnhNy0Hs,393
 zhijiang/data/rc_files/gitconfig,sha256=kJZIubN64CoqXqHlHlkof8HzGh0E0KlAWWRHCkpQc6Y,118
 zhijiang/data/rc_files/inputrc,sha256=yl22z2lj2jWLaE85I9QpV9NjoYoOhpmPemNxEsxMC5Y,561
 zhijiang/data/rc_files/tmux.config,sha256=m0TZ9DBK72V3IXXWir2YqHjLWbuTLwxqkYrhdTvEgRc,153
 zhijiang/data/rc_files/vimrc,sha256=T-rxTkB8WJdxuQRLIbNYe-ybahRXmssVi7nE2ER7RsM,415
 zhijiang/scripts/enhance_python.sh,sha256=l9YzkTTMLRzUV_nkCi8PS029QqIx8__bKmD3HCkEycE,480
 zhijiang/scripts/install_useful_tools.sh,sha256=7C287YLb57j0hxKWLWeM2KIZcI6cM1L4DDHGIlju9UE,1150
-zhijiang/scripts/useful_func.py,sha256=SiZq5xcFSVl5c2Y-N4-U7eJjtMJ3WHrHV3IsJz4CNDg,6619
-zhijiang-0.2.2.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
-zhijiang-0.2.2.dist-info/METADATA,sha256=PX_h7H2JQ_uAQS8RKSveiwXNFpQ7cE844OZJKSYHlSg,921
-zhijiang-0.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-zhijiang-0.2.2.dist-info/entry_points.txt,sha256=Q_-WKs0WMLyxX1t8rWQzIE94DfhcGxeqYzdM-09IxCs,43
-zhijiang-0.2.2.dist-info/top_level.txt,sha256=CLVD_HFtdNB3uaa7tp2r1-vOsvccTYHrlIxNxW06rAU,9
-zhijiang-0.2.2.dist-info/RECORD,,
+zhijiang/scripts/useful_func.py,sha256=2P-7bYHxFzPcf7-AlIuXIny4AEHWR-y7BvP_pBpAfgE,6665
+zhijiang-0.2.3.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
+zhijiang-0.2.3.dist-info/METADATA,sha256=U-RtTQ8OOEhJ5ejk_Unbh6j0a1zhUGYR6rZiS78wFJc,921
+zhijiang-0.2.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+zhijiang-0.2.3.dist-info/entry_points.txt,sha256=Q_-WKs0WMLyxX1t8rWQzIE94DfhcGxeqYzdM-09IxCs,43
+zhijiang-0.2.3.dist-info/top_level.txt,sha256=CLVD_HFtdNB3uaa7tp2r1-vOsvccTYHrlIxNxW06rAU,9
+zhijiang-0.2.3.dist-info/RECORD,,
```

