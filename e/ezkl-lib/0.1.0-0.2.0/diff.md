# Comparing `tmp/ezkl_lib-0.1.0-cp37-abi3-win_amd64.whl.zip` & `tmp/ezkl_lib-0.2.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10009263 bytes, number of entries: 6
--rw-r--r--  4.6 unx     4490 b- defN 23-Jun-06 14:24 ezkl_lib-0.1.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jun-06 14:24 ezkl_lib-0.1.0.dist-info/WHEEL
--rw-r--r--  4.6 unx    11558 b- defN 23-Jun-06 14:24 ezkl_lib-0.1.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      115 b- defN 23-Jun-06 14:24 ezkl_lib/__init__.py
--rwxr-xr-x  4.6 unx 28250112 b- defN 23-Jun-06 14:24 ezkl_lib/ezkl_lib.pyd
--rw-r--r--  4.6 unx      471 b- defN 23-Jun-06 14:24 ezkl_lib-0.1.0.dist-info/RECORD
-6 files, 28266842 bytes uncompressed, 10008423 bytes compressed:  64.6%
+Zip file size: 9696455 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     4496 b- defN 23-Jun-15 23:50 ezkl_lib-0.2.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-15 23:50 ezkl_lib-0.2.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11558 b- defN 23-Jun-15 23:50 ezkl_lib-0.2.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      115 b- defN 23-Jun-15 23:50 ezkl_lib/__init__.py
+-rwxr-xr-x  4.6 unx 27647488 b- defN 23-Jun-15 23:50 ezkl_lib/ezkl_lib.pyd
+-rw-r--r--  4.6 unx      471 b- defN 23-Jun-15 23:50 ezkl_lib-0.2.0.dist-info/RECORD
+6 files, 27664224 bytes uncompressed, 9695615 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: ezkl_lib-0.1.0.dist-info/METADATA
+Filename: ezkl_lib-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: ezkl_lib-0.1.0.dist-info/WHEEL
+Filename: ezkl_lib-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: ezkl_lib-0.1.0.dist-info/license_files/LICENSE
+Filename: ezkl_lib-0.2.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: ezkl_lib/__init__.py
 Comment: 
 
 Filename: ezkl_lib/ezkl_lib.pyd
 Comment: 
 
-Filename: ezkl_lib-0.1.0.dist-info/RECORD
+Filename: ezkl_lib-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ezkl_lib-0.1.0.dist-info/METADATA` & `ezkl_lib-0.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezkl_lib
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
@@ -32,14 +32,18 @@
 
 > "I ran my private neural network on some public data and it produced this output"
 
 > "I correctly ran this publicly available neural network on some public data and it produced this output"
 
 In the backend we use [Halo2](https://github.com/privacy-scaling-explorations/halo2) as a proof system.
 
+
+- If you have any questions, we'd love for you to open up a discussion topic in [Discussions](https://github.com/zkonduit/ezkl/discussions). Alternatively, you can join the ✨[EZKL Community Telegram Group](https://t.me/+76OjHb5CwJtkMTBh)💫.
+
+
 ### resources 📖
 
 |  |  |
 | --- | --- |
 | [docs](https://docs.ezkl.xyz ) | the official ezkl docs page |
 | [tutorial](https://github.com/zkonduit/pyezkl/tree/main/examples/tutorial) | end-to-end tutorial using pytorch and ezkl |
 | [notebook](https://github.com/zkonduit/pyezkl/blob/main/examples/ezkl_demo.ipynb) | end-to-end tutorial using pytorch and ezkl in a jupyter notebook |
@@ -99,30 +103,25 @@
 | [@zkonduit/ezkl](https://github.com/zkonduit/ezkl) | the main ezkl repo in rust |
 | [@zkonduit/pyezkl](https://github.com/zkonduit/pyezkl) | helper functions in python for processing onnx files |
 | [@zkonduit/ezkl-docs](https://github.com/zkonduit/ezkl-docs) | official ezkl docs |
 
 
 
 
-
-
-
 ----------------------
 
 ## Contributing 🌎
 
 If you're interested in contributing and are unsure where to start, reach out to one of the maintainers:
 
 * dante (alexander-camuto)
 * jason (jasonmorton)
 
 More broadly:
 
-- Feel free to open up a discussion topic in [Discussions](https://github.com/zkonduit/ezkl/discussions) to ask questions. Alternatively, you may join the [EZKL Community Telegram Group](https://t.me/+76OjHb5CwJtkMTBh) to ask questions.
-
 - See currently open issues for ideas on how to contribute.
 
 - For PRs we use the [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) naming convention.
 
 - To report bugs or request new features [create a new issue within Issues](https://github.com/zkonduit/ezkl/issues) to inform the greater community.
```

## Comparing `ezkl_lib-0.1.0.dist-info/license_files/LICENSE` & `ezkl_lib-0.2.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

