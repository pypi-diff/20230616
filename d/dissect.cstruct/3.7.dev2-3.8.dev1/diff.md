# Comparing `tmp/dissect.cstruct-3.7.dev2.tar.gz` & `tmp/dissect.cstruct-3.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.cstruct-3.7.dev2.tar", last modified: Tue May 16 13:25:13 2023, max compression
+gzip compressed data, was "dissect.cstruct-3.8.dev1.tar", last modified: Fri Jun 16 12:49:00 2023, max compression
```

## Comparing `dissect.cstruct-3.7.dev2.tar` & `dissect.cstruct-3.8.dev1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.783991 dissect.cstruct-3.7.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-16 13:25:13.783991 dissect.cstruct-3.7.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.771991 dissect.cstruct-3.7.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.775991 dissect.cstruct-3.7.dev2/dissect/cstruct/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    19285 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.775991 dissect.cstruct-3.7.dev2/dissect/cstruct/types/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/bytesinteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/chartype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/packedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/voidtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/types/wchartype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/dissect/cstruct/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.771991 dissect.cstruct-3.7.dev2/dissect.cstruct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-16 13:25:13.000000 dissect.cstruct-3.7.dev2/dissect.cstruct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-16 13:25:13.000000 dissect.cstruct-3.7.dev2/dissect.cstruct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:13.000000 dissect.cstruct-3.7.dev2/dissect.cstruct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:13.000000 dissect.cstruct-3.7.dev2/dissect.cstruct.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.779991 dissect.cstruct-3.7.dev2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/examples/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/examples/mirai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/examples/pe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/examples/secdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-16 13:25:03.000000 dissect.cstruct-3.7.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:13.783991 dissect.cstruct-3.7.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.783991 dissect.cstruct-3.7.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.783991 dissect.cstruct-3.7.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/data/testdef.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:13.783991 dissect.cstruct-3.7.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_bitfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_bytesinteger.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_ctypes_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_packedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:00.000000 dissect.cstruct-3.7.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.245746 dissect.cstruct-3.8.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-16 12:49:00.245746 dissect.cstruct-3.8.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.225746 dissect.cstruct-3.8.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.233746 dissect.cstruct-3.8.dev1/dissect/cstruct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19285 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.237746 dissect.cstruct-3.8.dev1/dissect/cstruct/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/bytesinteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/chartype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/packedtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/voidtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/types/wchartype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/dissect/cstruct/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.229746 dissect.cstruct-3.8.dev1/dissect.cstruct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-16 12:49:00.000000 dissect.cstruct-3.8.dev1/dissect.cstruct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-16 12:49:00.000000 dissect.cstruct-3.8.dev1/dissect.cstruct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:49:00.000000 dissect.cstruct-3.8.dev1/dissect.cstruct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:49:00.000000 dissect.cstruct-3.8.dev1/dissect.cstruct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.237746 dissect.cstruct-3.8.dev1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/examples/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/examples/mirai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/examples/pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/examples/secdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-16 12:48:50.000000 dissect.cstruct-3.8.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:49:00.245746 dissect.cstruct-3.8.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.241746 dissect.cstruct-3.8.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.241746 dissect.cstruct-3.8.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/data/testdef.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:00.245746 dissect.cstruct-3.8.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_bitfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_bytesinteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_ctypes_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_packedtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:48:46.000000 dissect.cstruct-3.8.dev1/tox.ini
```

### Comparing `dissect.cstruct-3.7.dev2/LICENSE` & `dissect.cstruct-3.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/PKG-INFO` & `dissect.cstruct-3.8.dev1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dissect.cstruct
-Version: 3.7.dev2
-Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Apache License 2.0
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
-Project-URL: repository, https://github.com/fox-it/dissect.cstruct
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.cstruct
 
 A Dissect module implementing a parser for C-like structures. Structure parsing in Python made easy. With cstruct, you
 can write C-like structures and use them to parse binary data, either as file-like objects or bytestrings.
 
 Parsing binary data with cstruct feels familiar and easy. No need to learn a new syntax or the quirks of a new parsing
 library before you can start parsing data. The syntax isn't strict C but it's compatible with most common structure
```

### Comparing `dissect.cstruct-3.7.dev2/README.md` & `dissect.cstruct-3.8.dev1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: dissect.cstruct
+Version: 3.8.dev1
+Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Apache License 2.0
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
+Project-URL: repository, https://github.com/fox-it/dissect.cstruct
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
 # dissect.cstruct
 
 A Dissect module implementing a parser for C-like structures. Structure parsing in Python made easy. With cstruct, you
 can write C-like structures and use them to parse binary data, either as file-like objects or bytestrings.
 
 Parsing binary data with cstruct feels familiar and easy. No need to learn a new syntax or the quirks of a new parsing
 library before you can start parsing data. The syntax isn't strict C but it's compatible with most common structure
```

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/__init__.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/bitbuffer.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/bitbuffer.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/compiler.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/compiler.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/cstruct.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/cstruct.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/expression.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/expression.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/parser.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/parser.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/__init__.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/base.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/base.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/bytesinteger.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/bytesinteger.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/chartype.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/chartype.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/enum.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/enum.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/flag.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/flag.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/instance.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/instance.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/packedtype.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/packedtype.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/pointer.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/pointer.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/structure.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/structure.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/types/wchartype.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/types/wchartype.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect/cstruct/utils.py` & `dissect.cstruct-3.8.dev1/dissect/cstruct/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/dissect.cstruct.egg-info/PKG-INFO` & `dissect.cstruct-3.8.dev1/dissect.cstruct.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 3.7.dev2
+Version: 3.8.dev1
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
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
 
 # dissect.cstruct
```

### Comparing `dissect.cstruct-3.7.dev2/dissect.cstruct.egg-info/SOURCES.txt` & `dissect.cstruct-3.8.dev1/dissect.cstruct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/examples/disk.py` & `dissect.cstruct-3.8.dev1/examples/disk.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/examples/mirai.py` & `dissect.cstruct-3.8.dev1/examples/mirai.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/examples/pe.py` & `dissect.cstruct-3.8.dev1/examples/pe.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/examples/secdesc.py` & `dissect.cstruct-3.8.dev1/examples/secdesc.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/pyproject.toml` & `dissect.cstruct-3.8.dev1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,25 @@
 readme = "README.md"
 requires-python = "~=3.9"
 license.text = "Apache License 2.0"
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
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://dissect.tools"
 documentation = "https://docs.dissect.tools/en/latest/projects/dissect.cstruct"
 repository = "https://github.com/fox-it/dissect.cstruct"
```

### Comparing `dissect.cstruct-3.7.dev2/tests/docs/Makefile` & `dissect.cstruct-3.8.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/docs/conf.py` & `dissect.cstruct-3.8.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_align.py` & `dissect.cstruct-3.8.dev1/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_basic.py` & `dissect.cstruct-3.8.dev1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_bitbuffer.py` & `dissect.cstruct-3.8.dev1/tests/test_bitbuffer.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_bitfield.py` & `dissect.cstruct-3.8.dev1/tests/test_bitfield.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_bytesinteger.py` & `dissect.cstruct-3.8.dev1/tests/test_bytesinteger.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_ctypes_type.py` & `dissect.cstruct-3.8.dev1/tests/test_ctypes_type.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_enum.py` & `dissect.cstruct-3.8.dev1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_expression.py` & `dissect.cstruct-3.8.dev1/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_flag.py` & `dissect.cstruct-3.8.dev1/tests/test_flag.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_packedtype.py` & `dissect.cstruct-3.8.dev1/tests/test_packedtype.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_pointer.py` & `dissect.cstruct-3.8.dev1/tests/test_pointer.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_struct.py` & `dissect.cstruct-3.8.dev1/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_union.py` & `dissect.cstruct-3.8.dev1/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_util.py` & `dissect.cstruct-3.8.dev1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tests/test_utils.py` & `dissect.cstruct-3.8.dev1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.7.dev2/tox.ini` & `dissect.cstruct-3.8.dev1/tox.ini`

 * *Files identical despite different names*

