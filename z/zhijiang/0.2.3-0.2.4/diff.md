# Comparing `tmp/zhijiang-0.2.3-py3-none-any.whl.zip` & `tmp/zhijiang-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 9841 bytes, number of entries: 17
+Zip file size: 11735 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx     2651 b- defN 23-Jun-09 06:16 zhijiang/__init__.py
 -rw-rw-r--  2.0 unx      231 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/alias
 -rw-rw-r--  2.0 unx       75 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/dockerignore
 -rw-rw-r--  2.0 unx      393 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/gdbinit
 -rw-rw-r--  2.0 unx      118 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/gitconfig
 -rw-rw-r--  2.0 unx      561 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/inputrc
 -rw-rw-r--  2.0 unx      153 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/tmux.config
 -rw-rw-r--  2.0 unx      415 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/vimrc
--rw-rw-r--  2.0 unx      480 b- defN 23-Jun-09 06:13 zhijiang/scripts/enhance_python.sh
+-rw-rw-r--  2.0 unx      545 b- defN 23-Jun-16 08:07 zhijiang/scripts/enhance_python.sh
 -rw-rw-r--  2.0 unx     1150 b- defN 23-Jun-09 06:13 zhijiang/scripts/install_useful_tools.sh
--rw-rw-r--  2.0 unx     6665 b- defN 23-Jun-16 02:50 zhijiang/scripts/useful_func.py
--rw-rw-r--  2.0 unx     1081 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       43 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1449 b- defN 23-Jun-16 02:54 zhijiang-0.2.3.dist-info/RECORD
-17 files, 16487 bytes uncompressed, 7425 bytes compressed:  55.0%
+-rw-rw-r--  2.0 unx     2277 b- defN 23-Jun-16 08:02 zhijiang/scripts/onnx_helper.py
+-rw-rw-r--  2.0 unx     6885 b- defN 23-Jun-16 08:08 zhijiang/scripts/useful_func.py
+-rw-rw-r--  2.0 unx     2277 b- defN 23-Jun-16 08:02 zhijiang/scripts/zhijxu_onnx_helper.py
+-rw-rw-r--  2.0 unx     1081 b- defN 23-Jun-16 08:13 zhijiang-0.2.4.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-16 08:13 zhijiang-0.2.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 08:13 zhijiang-0.2.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       43 b- defN 23-Jun-16 08:13 zhijiang-0.2.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-16 08:13 zhijiang-0.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1632 b- defN 23-Jun-16 08:13 zhijiang-0.2.4.dist-info/RECORD
+19 files, 21509 bytes uncompressed, 9029 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -24,29 +24,35 @@
 
 Filename: zhijiang/scripts/enhance_python.sh
 Comment: 
 
 Filename: zhijiang/scripts/install_useful_tools.sh
 Comment: 
 
+Filename: zhijiang/scripts/onnx_helper.py
+Comment: 
+
 Filename: zhijiang/scripts/useful_func.py
 Comment: 
 
-Filename: zhijiang-0.2.3.dist-info/LICENSE.txt
+Filename: zhijiang/scripts/zhijxu_onnx_helper.py
+Comment: 
+
+Filename: zhijiang-0.2.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: zhijiang-0.2.3.dist-info/METADATA
+Filename: zhijiang-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: zhijiang-0.2.3.dist-info/WHEEL
+Filename: zhijiang-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: zhijiang-0.2.3.dist-info/entry_points.txt
+Filename: zhijiang-0.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: zhijiang-0.2.3.dist-info/top_level.txt
+Filename: zhijiang-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: zhijiang-0.2.3.dist-info/RECORD
+Filename: zhijiang-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhijiang/scripts/enhance_python.sh

```diff
@@ -9,8 +9,9 @@
 else
   ## site.py is unchanged, so backup it
   cp $sitepy_path $backup
 fi
 
 pkg_script_path=`dirname $BASH_SOURCE`
 cat $pkg_script_path/useful_func.py >> $sitepy_path
+cp $pkg_script_path/zhijxu_onnx_helper.py `dirname $sitepy_path`
```

## zhijiang/scripts/useful_func.py

```diff
@@ -1,13 +1,25 @@
 import os
 import sys
 import pdb
 import inspect
 import builtins
 from functools import wraps
+import atexit
+import time
+from tempfile import mkdtemp
+
+try:
+    import torch
+    import debugpy
+    from termcolor import cprint
+    from viztracer import VizTracer
+    from zhijxu_onnx_helper import Analyze_onnx_model
+except ImportError:
+    pass
 
 
 def __zhijxu_is_rank_0():
     if os.environ.get("LOCAL_RANK", "0") == "0":
         return True
     return False
 
@@ -24,21 +36,17 @@
 
 
 @zhijxu_run_once
 def zhijxu_vscode_attach(sleep_time_sec=3):
     """
     only rank 0 will wait for vscode debug attach, other rank continue to run
     """
-    import debugpy
-    from termcolor import cprint
-    import time as tmp_time
-
     if __zhijxu_is_rank_0():
         debugpy.listen(("localhost", 56789))
-        tmp_time.sleep(
+        time.sleep(
             sleep_time_sec
         )  # so the next print can be shown at last line of terminal in multiprocess case
         cprint("\n\nzhijxu, waiting for debug connect\n\n", color="red", flush=True)
         debugpy.wait_for_client()
         cprint("\n\nzhijxu,debug connection done!!!\n\n", color="red", flush=True)
 
 
@@ -65,16 +73,14 @@
     :param grad_to_none: Reset the gradient of the provided tensor to None
     :type grad_to_none: torch.tensor, optional
     :param percentiles: Performance percentile to return in addition to the median.
     :type percentiles: list[float]
     :param fast_flush: Use faster kernel to flush L2 between measurements
     :type fast_flush: bool
     """
-    import torch
-
     # Estimate the runtime of the function
     fn()
     torch.cuda.synchronize()
     start_event = torch.cuda.Event(enable_timing=True)
     end_event = torch.cuda.Event(enable_timing=True)
     start_event.record()
     for _ in range(5):
@@ -125,18 +131,14 @@
     """
     the control env and its possible values are:
         - VIZTRACER, 0/1
         - NSYS, 0/1
         - START_STEP, any integer larger than 0
         - END_STEP, any integer larger than START_STEP
     """
-    from termcolor import cprint
-    import torch
-    from viztracer import VizTracer
-
     if os.environ.get("VIZTRACER", "0") == "1":
         assert (
             os.environ["CUDA_LAUNCH_BLOCKING"] == "1"
         ), "CUDA_LAUNCH_BLOCKING must be set to 1 when using VizTracer to profile CUDA code"
         if step == 1:
             global tracer
             tracer = VizTracer(output_file=f"trace_{os.environ.get('LOCAL_RANK', 0)}.json")
@@ -162,42 +164,44 @@
 
 @zhijxu_run_once
 def zhijxu_pdb():
     """
         only rank 0 will enter pdb, other ranks continue execution
     """
     if __zhijxu_is_rank_0():
-        from termcolor import cprint
-
         cprint("zhijxu, i am rank 0, enter pdb now", "red")
         pdb.set_trace()
 
 
 @zhijxu_run_once
 def zhijxu_enter_pdb_at_exception():
     """
         register a hook which will enter pdb when process wants to exit, this will help debugging when process has un-caught exception
     """
-    import atexit
-
     atexit.register(pdb.pm)
 
 
 def zhijxu_open_onnx_in_tensorboard(model, port):
     """
     give the onnx model path and tensorboard port, then will convert to tensorboard and launch tensorboard automatically for you
     """
-    from tempfile import mkdtemp
     tmp_dir = mkdtemp(prefix="onnx-tensorboard-")
-    from termcolor import cprint
     cprint(f"converted tensorboard is put at {tmp_dir}", "red")
     os.system(f"python /home/zhijxu/onnxruntime/tools/python/onnx2tfevents.py --logdir={tmp_dir} --model {model}")
     os.system(f"tensorboard --logdir={tmp_dir} --port {port} &")
 
 
+def zhijxu_analyze_onnx_model(onnx_file):
+    os.system("reset")
+    model = Analyze_onnx_model(onnx_file)
+    model.print_info()
+    cprint("1. search items by \"zhijxu,\"\n2. return class object has attribute \"constant_registery\" to get constant value", "red")
+    return model
+
+
 fset = {
     name: obj
     for name, obj in inspect.getmembers(sys.modules[__name__])
     if inspect.isfunction(obj) and name.startswith("zhijxu_")
 }
 for name, obj in fset.items():
     if inspect.isfunction(obj):
```

## Comparing `zhijiang-0.2.3.dist-info/LICENSE.txt` & `zhijiang-0.2.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `zhijiang-0.2.3.dist-info/METADATA` & `zhijiang-0.2.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhijiang
-Version: 0.2.3
+Version: 0.2.4
 Summary: setup linux env, such as bashrc etc.
 Home-page: https://github.com/xu-zhijiang/env-setup.git
 Author: Xu Zhijiang
 Author-email: 15852939122@163.com
 Project-URL: Funding, https://github.com/xu-zhijiang
 Project-URL: Source, https://github.com/xu-zhijiang/env-setup.git
 Keywords: env setup,development,zhijiang
```

