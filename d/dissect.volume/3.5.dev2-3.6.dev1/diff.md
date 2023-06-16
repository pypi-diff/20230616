# Comparing `tmp/dissect.volume-3.5.dev2.tar.gz` & `tmp/dissect.volume-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.volume-3.5.dev2.tar", last modified: Tue May 16 13:27:06 2023, max compression
+gzip compressed data, was "dissect.volume-3.6.dev1.tar", last modified: Fri Jun 16 12:51:26 2023, max compression
```

## Comparing `dissect.volume-3.5.dev2.tar` & `dissect.volume-3.6.dev1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:06.008915 dissect.volume-3.5.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-16 13:27:06.008915 dissect.volume-3.5.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.984915 dissect.volume-3.5.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.992915 dissect.volume-3.5.dev2/dissect/volume/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.996915 dissect.volume-3.5.dev2/dissect/volume/disk/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/disk/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/disk/partition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.996915 dissect.volume-3.5.dev2/dissect/volume/disk/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/disk/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/disk/schemes/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/disk/schemes/bsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/disk/schemes/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/disk/schemes/mbr.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/ldm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:06.000915 dissect.volume-3.5.dev2/dissect/volume/lvm/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/lvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/lvm/lvm2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/lvm/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/lvm/physical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/dissect/volume/vss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.992915 dissect.volume-3.5.dev2/dissect.volume.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-16 13:27:05.000000 dissect.volume-3.5.dev2/dissect.volume.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-16 13:27:05.000000 dissect.volume-3.5.dev2/dissect.volume.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:27:05.000000 dissect.volume-3.5.dev2/dissect.volume.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:27:05.000000 dissect.volume-3.5.dev2/dissect.volume.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:27:05.000000 dissect.volume-3.5.dev2/dissect.volume.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-16 13:26:56.000000 dissect.volume-3.5.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:27:06.008915 dissect.volume-3.5.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:06.004915 dissect.volume-3.5.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:06.004915 dissect.volume-3.5.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/apm.bin
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/bsd.bin
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/bsd64.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/gpt.bin
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/gpt_4k.bin
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/gpt_esxi.bin
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/gpt_hybrid.bin
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/gpt_no_name_xff.bin
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/lvm.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/data/mbr.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:06.008915 dissect.volume-3.5.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/test_apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/test_bsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/test_gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/test_lvm.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tests/test_mbr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:26:50.000000 dissect.volume-3.5.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.510661 dissect.volume-3.6.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.518661 dissect.volume-3.6.dev1/dissect/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.518661 dissect.volume-3.6.dev1/dissect/volume/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.518661 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/bsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/mbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/ldm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.522661 dissect.volume-3.6.dev1/dissect/volume/lvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/lvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/lvm/lvm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/lvm/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/lvm/physical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/vss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.518661 dissect.volume-3.6.dev1/dissect.volume.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-16 12:51:16.000000 dissect.volume-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.522661 dissect.volume-3.6.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/apm.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/bsd.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/bsd64.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt_4k.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt_esxi.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt_hybrid.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt_no_name_xff.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/lvm.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/mbr.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_bsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_lvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_mbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tox.ini
```

### Comparing `dissect.volume-3.5.dev2/LICENSE` & `dissect.volume-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/PKG-INFO` & `dissect.volume-3.6.dev1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dissect.volume
-Version: 3.5.dev2
-Summary: A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.volume
-Project-URL: repository, https://github.com/fox-it/dissect.volume
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.volume
 
 A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR.
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.volume/index.html).
 
 ## Requirements
```

### Comparing `dissect.volume-3.5.dev2/README.md` & `dissect.volume-3.6.dev1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: dissect.volume
+Version: 3.6.dev1
+Summary: A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Affero General Public License v3
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.volume
+Project-URL: repository, https://github.com/fox-it/dissect.volume
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: COPYRIGHT
+
 # dissect.volume
 
 A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR.
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.volume/index.html).
 
 ## Requirements
```

### Comparing `dissect.volume-3.5.dev2/dissect/volume/disk/disk.py` & `dissect.volume-3.6.dev1/dissect/volume/disk/disk.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/disk/partition.py` & `dissect.volume-3.6.dev1/dissect/volume/disk/partition.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/disk/schemes/apm.py` & `dissect.volume-3.6.dev1/dissect/volume/disk/schemes/apm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/disk/schemes/bsd.py` & `dissect.volume-3.6.dev1/dissect/volume/disk/schemes/bsd.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/disk/schemes/gpt.py` & `dissect.volume-3.6.dev1/dissect/volume/disk/schemes/gpt.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/disk/schemes/mbr.py` & `dissect.volume-3.6.dev1/dissect/volume/disk/schemes/mbr.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/ldm.py` & `dissect.volume-3.6.dev1/dissect/volume/ldm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/lvm/lvm2.py` & `dissect.volume-3.6.dev1/dissect/volume/lvm/lvm2.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/lvm/metadata.py` & `dissect.volume-3.6.dev1/dissect/volume/lvm/metadata.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/lvm/physical.py` & `dissect.volume-3.6.dev1/dissect/volume/lvm/physical.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect/volume/vss.py` & `dissect.volume-3.6.dev1/dissect/volume/vss.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/dissect.volume.egg-info/PKG-INFO` & `dissect.volume-3.6.dev1/dissect.volume.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.volume
-Version: 3.5.dev2
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.volume
 Project-URL: repository, https://github.com/fox-it/dissect.volume
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYRIGHT
 
 # dissect.volume
```

### Comparing `dissect.volume-3.5.dev2/dissect.volume.egg-info/SOURCES.txt` & `dissect.volume-3.6.dev1/dissect.volume.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/pyproject.toml` & `dissect.volume-3.6.dev1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -8,15 +8,25 @@
 readme = "README.md"
 requires-python = "~=3.9"
 license.text = "Affero General Public License v3"
 authors = [
   {name = "Dissect Team", email = "dissect@fox-it.com"}
 ]
 classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "Environment :: Console",
+  "Intended Audience :: Developers",
+  "Intended Audience :: Information Technology",
+  "License :: OSI Approved",
+  "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
+  "Topic :: Internet :: Log Analysis",
+  "Topic :: Scientific/Engineering :: Information Analysis",
+  "Topic :: Security",
+  "Topic :: Utilities",
 ]
 dependencies = [
     "dissect.cstruct>=3.0.dev,<4.0.dev",
     "dissect.util>=3.0.dev,<4.0.dev",
 ]
 dynamic = ["version"]
```

### Comparing `dissect.volume-3.5.dev2/tests/conftest.py` & `dissect.volume-3.6.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/apm.bin` & `dissect.volume-3.6.dev1/tests/data/apm.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/bsd.bin` & `dissect.volume-3.6.dev1/tests/data/bsd.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/bsd64.bin.gz` & `dissect.volume-3.6.dev1/tests/data/bsd64.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/gpt.bin` & `dissect.volume-3.6.dev1/tests/data/gpt.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/gpt_4k.bin` & `dissect.volume-3.6.dev1/tests/data/gpt_4k.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/gpt_esxi.bin` & `dissect.volume-3.6.dev1/tests/data/gpt_esxi.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/gpt_hybrid.bin` & `dissect.volume-3.6.dev1/tests/data/gpt_hybrid.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/gpt_no_name_xff.bin` & `dissect.volume-3.6.dev1/tests/data/gpt_no_name_xff.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/lvm.bin.gz` & `dissect.volume-3.6.dev1/tests/data/lvm.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/data/mbr.bin` & `dissect.volume-3.6.dev1/tests/data/mbr.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/docs/Makefile` & `dissect.volume-3.6.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/docs/conf.py` & `dissect.volume-3.6.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/test_apm.py` & `dissect.volume-3.6.dev1/tests/test_apm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/test_bsd.py` & `dissect.volume-3.6.dev1/tests/test_bsd.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/test_gpt.py` & `dissect.volume-3.6.dev1/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/test_lvm.py` & `dissect.volume-3.6.dev1/tests/test_lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tests/test_mbr.py` & `dissect.volume-3.6.dev1/tests/test_mbr.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.5.dev2/tox.ini` & `dissect.volume-3.6.dev1/tox.ini`

 * *Files identical despite different names*

