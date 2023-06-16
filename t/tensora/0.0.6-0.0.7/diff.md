# Comparing `tmp/tensora-0.0.6.tar.gz` & `tmp/tensora-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensora-0.0.6.tar", last modified: Sun May 23 10:41:02 2021, max compression
+gzip compressed data, was "tensora-0.0.7.tar", last modified: Fri Jun 16 11:43:57 2023, max compression
```

## Comparing `tensora-0.0.6.tar` & `tensora-0.0.7.tar`

### file list

```diff
@@ -1,274 +1,784 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/
--rw-rw-r--   0 david     (1000) david     (1000)       12 2020-07-08 11:47:39.000000 tensora-0.0.6/.gitattributes
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/.github/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/.github/workflows/
--rw-r--r--   0 david     (1000) david     (1000)      610 2021-05-23 10:25:20.000000 tensora-0.0.6/.github/workflows/python.yml
--rw-rw-r--   0 david     (1000) david     (1000)      103 2020-07-08 11:47:39.000000 tensora-0.0.6/.gitignore
--rw-rw-r--   0 david     (1000) david     (1000)       87 2020-07-08 11:47:39.000000 tensora-0.0.6/.gitmodules
--rw-rw-r--   0 david     (1000) david     (1000)     1057 2020-07-08 11:47:39.000000 tensora-0.0.6/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      226 2020-07-08 11:47:39.000000 tensora-0.0.6/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)    10375 2021-05-23 10:41:02.000000 tensora-0.0.6/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     8222 2020-07-08 11:47:39.000000 tensora-0.0.6/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       52 2021-01-25 01:33:50.000000 tensora-0.0.6/dev-requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       32 2020-09-13 14:58:56.000000 tensora-0.0.6/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2021-05-23 10:41:02.000000 tensora-0.0.6/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     2933 2021-05-23 10:28:58.000000 tensora-0.0.6/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/
--rw-r--r--   0 david     (1000) david     (1000)     2994 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/CMakeLists.txt
--rw-r--r--   0 david     (1000) david     (1000)     1693 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/Doxyfile
--rw-r--r--   0 david     (1000) david     (1000)     1172 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     3965 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/apps/
--rw-r--r--   0 david     (1000) david     (1000)       38 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/apps/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/apps/tensor_times_vector/
--rw-r--r--   0 david     (1000) david     (1000)      899 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/apps/tensor_times_vector/CMakeLists.txt
--rw-r--r--   0 david     (1000) david     (1000)      376 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/apps/tensor_times_vector/README.md
--rw-r--r--   0 david     (1000) david     (1000)      824 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/apps/tensor_times_vector/tensor_times_vector.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/
--rw-r--r--   0 david     (1000) david     (1000)      437 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/codegen/
--rw-r--r--   0 david     (1000) david     (1000)     2569 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/codegen/module.h
--rw-r--r--   0 david     (1000) david     (1000)      878 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/cuda.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/error/
--rw-r--r--   0 david     (1000) david     (1000)     1010 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/error/error_messages.h
--rw-r--r--   0 david     (1000) david     (1000)     3115 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/error.h
--rw-r--r--   0 david     (1000) david     (1000)     6702 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/format.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/index_notation/
--rw-r--r--   0 david     (1000) david     (1000)     4642 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/index_notation/README.md
--rw-r--r--   0 david     (1000) david     (1000)    23245 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/index_notation/index_notation.h
--rw-r--r--   0 david     (1000) david     (1000)     6878 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_nodes.h
--rw-r--r--   0 david     (1000) david     (1000)     1879 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_nodes_abstract.h
--rw-r--r--   0 david     (1000) david     (1000)     1384 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_printer.h
--rw-r--r--   0 david     (1000) david     (1000)     4068 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_rewriter.h
--rw-r--r--   0 david     (1000) david     (1000)     6581 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_visitor.h
--rw-r--r--   0 david     (1000) david     (1000)     2180 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/index_notation/intrinsic.h
--rw-r--r--   0 david     (1000) david     (1000)     2252 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/index_notation/kernel.h
--rw-r--r--   0 david     (1000) david     (1000)      929 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/index_notation/schedule.h
--rw-r--r--   0 david     (1000) david     (1000)     4128 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/index_notation/transformations.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/ir/
--rw-r--r--   0 david     (1000) david     (1000)    17200 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/ir/ir.h
--rw-r--r--   0 david     (1000) david     (1000)     2779 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/ir/ir_printer.h
--rw-r--r--   0 david     (1000) david     (1000)     2246 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/ir/ir_rewriter.h
--rw-r--r--   0 david     (1000) david     (1000)      410 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/ir/ir_verifier.h
--rw-r--r--   0 david     (1000) david     (1000)     4430 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/ir/ir_visitor.h
--rw-r--r--   0 david     (1000) david     (1000)      349 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/ir/simplify.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/lower/
--rw-r--r--   0 david     (1000) david     (1000)     7441 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/lower/iterator.h
--rw-r--r--   0 david     (1000) david     (1000)     1835 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/lower/lower.h
--rw-r--r--   0 david     (1000) david     (1000)    12806 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/lower/lowerer_impl.h
--rw-r--r--   0 david     (1000) david     (1000)     5181 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/lower/merge_lattice.h
--rw-r--r--   0 david     (1000) david     (1000)     2212 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/lower/mode.h
--rw-r--r--   0 david     (1000) david     (1000)     1802 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/lower/mode_format_compressed.h
--rw-r--r--   0 david     (1000) david     (1000)     1280 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/lower/mode_format_dense.h
--rw-r--r--   0 david     (1000) david     (1000)     5905 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/lower/mode_format_impl.h
--rw-r--r--   0 david     (1000) david     (1000)     1418 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/lower/mode_format_singleton.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/parser/
--rw-r--r--   0 david     (1000) david     (1000)      789 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/parser/lexer.h
--rw-r--r--   0 david     (1000) david     (1000)     2853 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/parser/parser.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/storage/
--rw-r--r--   0 david     (1000) david     (1000)     2388 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/storage/array.h
--rw-r--r--   0 david     (1000) david     (1000)     1650 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/storage/coordinate.h
--rw-r--r--   0 david     (1000) david     (1000)     1499 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/storage/file_io_mtx.h
--rw-r--r--   0 david     (1000) david     (1000)     2463 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/storage/file_io_rb.h
--rw-r--r--   0 david     (1000) david     (1000)      916 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/storage/file_io_tns.h
--rw-r--r--   0 david     (1000) david     (1000)     2451 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/storage/index.h
--rw-r--r--   0 david     (1000) david     (1000)     1623 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/storage/pack.h
--rw-r--r--   0 david     (1000) david     (1000)     2000 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/storage/storage.h
--rw-r--r--   0 david     (1000) david     (1000)     9975 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/storage/typed_index.h
--rw-r--r--   0 david     (1000) david     (1000)    10600 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/storage/typed_value.h
--rw-r--r--   0 david     (1000) david     (1000)     8556 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/storage/typed_vector.h
--rw-r--r--   0 david     (1000) david     (1000)     1144 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/taco_tensor_t.h
--rw-r--r--   0 david     (1000) david     (1000)     1386 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/target.h
--rw-r--r--   0 david     (1000) david     (1000)    27158 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/tensor.h
--rw-r--r--   0 david     (1000) david     (1000)     6755 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/type.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/include/taco/util/
--rw-r--r--   0 david     (1000) david     (1000)     9963 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/collections.h
--rw-r--r--   0 david     (1000) david     (1000)     1056 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/comparable.h
--rw-r--r--   0 david     (1000) david     (1000)     2072 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/env.h
--rw-r--r--   0 david     (1000) david     (1000)      268 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/files.h
--rw-r--r--   0 david     (1000) david     (1000)     9333 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/fill.h
--rw-r--r--   0 david     (1000) david     (1000)     3076 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/util/intrusive_ptr.h
--rw-r--r--   0 david     (1000) david     (1000)      463 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/util/name_generator.h
--rw-r--r--   0 david     (1000) david     (1000)      352 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/printable.h
--rw-r--r--   0 david     (1000) david     (1000)     1854 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/util/scopedmap.h
--rw-r--r--   0 david     (1000) david     (1000)     1124 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/scopedset.h
--rw-r--r--   0 david     (1000) david     (1000)      339 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/singleton.h
--rw-r--r--   0 david     (1000) david     (1000)     1963 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/util/strings.h
--rw-r--r--   0 david     (1000) david     (1000)     4535 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/util/timers.h
--rw-r--r--   0 david     (1000) david     (1000)      300 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco/util/uncopyable.h
--rw-r--r--   0 david     (1000) david     (1000)     2868 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/include/taco/util/variadic.h
--rw-r--r--   0 david     (1000) david     (1000)      147 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/include/taco.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/misc/
--rw-r--r--   0 david     (1000) david     (1000)      523 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/misc/mainpage.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/
--rw-r--r--   0 david     (1000) david     (1000)     1016 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/codegen/
--rw-r--r--   0 david     (1000) david     (1000)    15662 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/codegen/codegen.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2842 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/codegen/codegen.h
--rw-r--r--   0 david     (1000) david     (1000)    12455 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/codegen/codegen_c.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1378 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/codegen/codegen_c.h
--rw-r--r--   0 david     (1000) david     (1000)    26873 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/codegen/codegen_cuda.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2376 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/codegen/codegen_cuda.h
--rw-r--r--   0 david     (1000) david     (1000)     5363 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/codegen/module.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1923 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/cuda.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/error/
--rw-r--r--   0 david     (1000) david     (1000)     5403 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/error/error_checks.cpp
--rw-r--r--   0 david     (1000) david     (1000)      929 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/error/error_checks.h
--rw-r--r--   0 david     (1000) david     (1000)     1230 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/error/error_messages.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1582 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/error.cpp
--rw-r--r--   0 david     (1000) david     (1000)    10527 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/format.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/index_notation/
--rw-r--r--   0 david     (1000) david     (1000)      356 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/index_notation/README.md
--rw-r--r--   0 david     (1000) david     (1000)    53303 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/index_notation/index_notation.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1016 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/index_notation/index_notation_nodes.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1049 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/index_notation/index_notation_nodes_abstract.cpp
--rw-r--r--   0 david     (1000) david     (1000)     6206 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/index_notation/index_notation_printer.cpp
--rw-r--r--   0 david     (1000) david     (1000)     9015 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/index_notation/index_notation_rewriter.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2523 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/index_notation/index_notation_visitor.cpp
--rw-r--r--   0 david     (1000) david     (1000)    40775 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/index_notation/intrinsic.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4292 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/index_notation/kernel.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1424 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/index_notation/schedule.cpp
--rw-r--r--   0 david     (1000) david     (1000)    21577 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/index_notation/transformations.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/ir/
--rw-r--r--   0 david     (1000) david     (1000)      239 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/ir/README.md
--rw-r--r--   0 david     (1000) david     (1000)    24838 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/ir/ir.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1621 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/ir/ir_generators.cpp
--rw-r--r--   0 david     (1000) david     (1000)      726 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/ir/ir_generators.h
--rw-r--r--   0 david     (1000) david     (1000)    14895 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/ir/ir_printer.cpp
--rw-r--r--   0 david     (1000) david     (1000)     9750 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/ir/ir_rewriter.cpp
--rw-r--r--   0 david     (1000) david     (1000)     8809 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/ir/ir_verifier.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4139 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/ir/ir_visitor.cpp
--rw-r--r--   0 david     (1000) david     (1000)    13498 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/ir/simplify.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/lower/
--rw-r--r--   0 david     (1000) david     (1000)      260 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/README.md
--rw-r--r--   0 david     (1000) david     (1000)     6987 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/expr_tools.cpp
--rw-r--r--   0 david     (1000) david     (1000)      870 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/expr_tools.h
--rw-r--r--   0 david     (1000) david     (1000)     6683 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/iteration_forest.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1020 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/iteration_forest.h
--rw-r--r--   0 david     (1000) david     (1000)     8081 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/iteration_graph.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2945 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/iteration_graph.h
--rw-r--r--   0 david     (1000) david     (1000)    15029 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/lower/iterator.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1830 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/lower/lower.cpp
--rw-r--r--   0 david     (1000) david     (1000)    54476 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/lower/lowerer_impl.cpp
--rw-r--r--   0 david     (1000) david     (1000)    24534 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/lower/merge_lattice.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2880 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/mode.cpp
--rw-r--r--   0 david     (1000) david     (1000)      776 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/mode_access.cpp
--rw-r--r--   0 david     (1000) david     (1000)      819 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/mode_access.h
--rw-r--r--   0 david     (1000) david     (1000)     7772 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/lower/mode_format_compressed.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2271 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/lower/mode_format_dense.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4337 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/lower/mode_format_impl.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4468 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/lower/mode_format_singleton.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2930 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/tensor_path.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2200 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/lower/tensor_path.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/parser/
--rw-r--r--   0 david     (1000) david     (1000)      293 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/parser/README.md
--rw-r--r--   0 david     (1000) david     (1000)     3565 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/parser/lexer.cpp
--rw-r--r--   0 david     (1000) david     (1000)    11925 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/parser/parser.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/storage/
--rw-r--r--   0 david     (1000) david     (1000)      152 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/storage/README.md
--rw-r--r--   0 david     (1000) david     (1000)     5348 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/storage/array.cpp
--rw-r--r--   0 david     (1000) david     (1000)     8189 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/storage/file_io_mtx.cpp
--rw-r--r--   0 david     (1000) david     (1000)    11732 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/storage/file_io_rb.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2985 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/storage/file_io_tns.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3551 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/storage/index.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7422 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/storage/pack.cpp
--rw-r--r--   0 david     (1000) david     (1000)     5380 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/storage/storage.cpp
--rw-r--r--   0 david     (1000) david     (1000)    18028 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/storage/typed_index.cpp
--rw-r--r--   0 david     (1000) david     (1000)    23634 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/storage/typed_value.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1918 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/taco_tensor_t.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1904 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/target.cpp
--rw-r--r--   0 david     (1000) david     (1000)    31311 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/tensor.cpp
--rw-r--r--   0 david     (1000) david     (1000)     8567 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/type.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/src/util/
--rw-r--r--   0 david     (1000) david     (1000)      635 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/util/env.cpp
--rw-r--r--   0 david     (1000) david     (1000)      512 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/util/files.cpp
--rw-r--r--   0 david     (1000) david     (1000)      833 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/src/util/name_generator.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1062 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/src/util/strings.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/test/
--rw-r--r--   0 david     (1000) david     (1000)      527 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/test/data/
--rw-r--r--   0 david     (1000) david     (1000)      119 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/2tensor.mtx
--rw-r--r--   0 david     (1000) david     (1000)       36 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/3tensor.tns
--rw-r--r--   0 david     (1000) david     (1000)      267 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/d33.mtx
--rw-r--r--   0 david     (1000) david     (1000)       66 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/d33.ttx
--rw-r--r--   0 david     (1000) david     (1000)      136 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/d432.ttx
--rw-r--r--   0 david     (1000) david     (1000)       88 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/d567.ttx
--rw-r--r--   0 david     (1000) david     (1000)      268 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/ds33.mtx
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/test/data/qcd/
--rw-r--r--   0 david     (1000) david     (1000)    11615 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/qcd/theta.ttx
--rw-r--r--   0 david     (1000) david     (1000)       64 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/qcd/theta_simple.ttx
--rw-r--r--   0 david     (1000) david     (1000)      555 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/qcd/z.ttx
--rw-r--r--   0 david     (1000) david     (1000)       52 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/qcd/z_simple.ttx
--rw-r--r--   0 david     (1000) david     (1000)     1487 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/rua_32.mtx
--rw-r--r--   0 david     (1000) david     (1000)     1986 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/data/rua_32.rb
--rw-r--r--   0 david     (1000) david     (1000)     4650 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/expr_factory.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2589 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/expr_factory.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/test/gtest/
--rw-r--r--   0 david     (1000) david     (1000)     1475 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/gtest/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      155 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/gtest/README.TAC
--rw-r--r--   0 david     (1000) david     (1000)   365644 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/gtest/gtest-all.cc
--rw-r--r--   0 david     (1000) david     (1000)   848773 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/gtest/gtest.h
--rw-r--r--   0 david     (1000) david     (1000)     1461 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/test.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3363 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/test.h
--rw-r--r--   0 david     (1000) david     (1000)    10837 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/test_tensors.cpp
--rw-r--r--   0 david     (1000) david     (1000)     5513 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/test_tensors.h
--rw-r--r--   0 david     (1000) david     (1000)    12162 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-api.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2561 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-copyprop.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1152 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-error.cpp
--rw-r--r--   0 david     (1000) david     (1000)      493 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-expr-reduction.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4119 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-expr.cpp
--rw-r--r--   0 david     (1000) david     (1000)    43178 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-expr_storage.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2112 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-format.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1044 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-index.cpp
--rw-r--r--   0 david     (1000) david     (1000)     8779 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-index_notation.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2058 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-indexexpr.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2918 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-indexstmt.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3609 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-io.cpp
--rw-r--r--   0 david     (1000) david     (1000)    45067 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-lower.cpp
--rw-r--r--   0 david     (1000) david     (1000)    23161 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-merge_lattice.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7101 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-parafac.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1632 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-qcd.cpp
--rw-r--r--   0 david     (1000) david     (1000)       68 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-regression.cpp
--rw-r--r--   0 david     (1000) david     (1000)    14078 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-storage.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3531 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-storage_alloc.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3105 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-tensor.cpp
--rw-r--r--   0 david     (1000) david     (1000)    13605 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-tensor_types.cpp
--rw-r--r--   0 david     (1000) david     (1000)    12778 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-transformation.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2758 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/test/tests-transpose.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3576 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/test/tests-type.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/taco/tools/
--rw-r--r--   0 david     (1000) david     (1000)      407 2020-07-08 22:41:29.000000 tensora-0.0.6/src/taco/tools/CMakeLists.txt
--rw-r--r--   0 david     (1000) david     (1000)    30020 2021-02-21 01:06:14.000000 tensora-0.0.6/src/taco/tools/taco.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora/
--rw-rw-r--   0 david     (1000) david     (1000)      148 2020-07-08 11:47:39.000000 tensora-0.0.6/src/tensora/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    16835 2021-05-23 10:25:20.000000 tensora-0.0.6/src/tensora/compile.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora/expression/
--rw-rw-r--   0 david     (1000) david     (1000)       93 2021-05-23 10:25:20.000000 tensora-0.0.6/src/tensora/expression/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5267 2020-07-08 11:47:39.000000 tensora-0.0.6/src/tensora/expression/ast.py
--rw-rw-r--   0 david     (1000) david     (1000)     1652 2020-07-08 11:47:39.000000 tensora-0.0.6/src/tensora/expression/parser.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora/format/
--rw-rw-r--   0 david     (1000) david     (1000)       94 2020-07-08 11:47:39.000000 tensora-0.0.6/src/tensora/format/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1305 2020-07-08 11:47:39.000000 tensora-0.0.6/src/tensora/format/format.py
--rw-rw-r--   0 david     (1000) david     (1000)     1469 2020-07-08 11:47:39.000000 tensora-0.0.6/src/tensora/format/parser.py
--rw-rw-r--   0 david     (1000) david     (1000)     7052 2020-07-08 11:47:39.000000 tensora-0.0.6/src/tensora/function.py
--rw-rw-r--   0 david     (1000) david     (1000)    23902 2021-05-23 10:25:20.000000 tensora-0.0.6/src/tensora/tensor.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    10375 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     8011 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2020-07-13 14:35:52.000000 tensora-0.0.6/src/tensora.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)       58 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2021-05-23 10:41:02.000000 tensora-0.0.6/src/tensora.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-05-23 10:41:02.000000 tensora-0.0.6/tests/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2020-07-08 11:47:39.000000 tensora-0.0.6/tests/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4828 2021-05-23 10:25:20.000000 tensora-0.0.6/tests/test_combinatorically.py
--rw-rw-r--   0 david     (1000) david     (1000)     2685 2020-07-08 11:47:39.000000 tensora-0.0.6/tests/test_expression.py
--rw-rw-r--   0 david     (1000) david     (1000)     1686 2020-07-08 11:47:39.000000 tensora-0.0.6/tests/test_format.py
--rw-rw-r--   0 david     (1000) david     (1000)     9370 2020-07-08 11:47:39.000000 tensora-0.0.6/tests/test_from_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     2965 2021-05-23 10:25:20.000000 tensora-0.0.6/tests/test_function.py
--rw-r--r--   0 david     (1000) david     (1000)      583 2021-05-23 10:25:20.000000 tensora-0.0.6/tests/test_numpy.py
--rw-rw-r--   0 david     (1000) david     (1000)      668 2020-07-08 11:47:39.000000 tensora-0.0.6/tests/test_operators.py
--rw-rw-r--   0 david     (1000) david     (1000)    10193 2021-05-23 10:25:20.000000 tensora-0.0.6/tests/test_tensor.py
--rw-rw-r--   0 david     (1000) david     (1000)     1879 2021-05-23 10:25:20.000000 tensora-0.0.6/tox.ini
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.257709 tensora-0.0.7/
+-rw-rw-r--   0 david     (1000) david     (1000)     1057 2020-07-08 11:47:39.000000 tensora-0.0.7/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      226 2020-07-08 11:47:39.000000 tensora-0.0.7/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     9253 2023-06-16 11:43:57.257709 tensora-0.0.7/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     8222 2020-07-08 11:47:39.000000 tensora-0.0.7/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-16 09:49:57.000000 tensora-0.0.7/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-06-16 11:43:57.257709 tensora-0.0.7/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     3033 2023-06-16 11:18:58.000000 tensora-0.0.7/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.193709 tensora-0.0.7/src/taco/.github/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/.github/workflows/
+-rw-r--r--   0 david     (1000) david     (1000)     2651 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/.github/workflows/buildandtest.yml
+-rw-r--r--   0 david     (1000) david     (1000)     1214 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/.github/workflows/cuda-test-manual.yml
+-rw-r--r--   0 david     (1000) david     (1000)      202 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/.gitmodules
+-rw-r--r--   0 david     (1000) david     (1000)     6274 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)     1693 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/Doxyfile
+-rw-r--r--   0 david     (1000) david     (1000)     1172 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)     6553 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/apps/
+-rw-r--r--   0 david     (1000) david     (1000)       38 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/apps/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/apps/tensor_times_vector/
+-rw-r--r--   0 david     (1000) david     (1000)      961 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/apps/tensor_times_vector/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)      376 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/apps/tensor_times_vector/README.md
+-rw-r--r--   0 david     (1000) david     (1000)      502 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/apps/tensor_times_vector/tensor_times_vector.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/ci/
+-rw-r--r--   0 david     (1000) david     (1000)     4380 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/ci/test-pr.md
+-rw-r--r--   0 david     (1000) david     (1000)     4838 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/ci/test-pr.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/taco/
+-rw-r--r--   0 david     (1000) david     (1000)      437 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/taco/codegen/
+-rw-r--r--   0 david     (1000) david     (1000)     2693 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/codegen/module.h
+-rw-r--r--   0 david     (1000) david     (1000)     1080 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/component.h
+-rw-r--r--   0 david     (1000) david     (1000)     1938 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/coordinate.h
+-rw-r--r--   0 david     (1000) david     (1000)      878 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/cuda.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/taco/error/
+-rw-r--r--   0 david     (1000) david     (1000)     1066 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/error/error_messages.h
+-rw-r--r--   0 david     (1000) david     (1000)     3318 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/error.h
+-rw-r--r--   0 david     (1000) david     (1000)     7184 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/format.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/taco/index_notation/
+-rw-r--r--   0 david     (1000) david     (1000)     4642 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/README.md
+-rw-r--r--   0 david     (1000) david     (1000)    49557 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation.h
+-rw-r--r--   0 david     (1000) david     (1000)    14329 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_nodes.h
+-rw-r--r--   0 david     (1000) david     (1000)     1879 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_nodes_abstract.h
+-rw-r--r--   0 david     (1000) david     (1000)     1520 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_printer.h
+-rw-r--r--   0 david     (1000) david     (1000)     4625 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_rewriter.h
+-rw-r--r--   0 david     (1000) david     (1000)     7113 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_visitor.h
+-rw-r--r--   0 david     (1000) david     (1000)     2180 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/intrinsic.h
+-rw-r--r--   0 david     (1000) david     (1000)     8874 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/iteration_algebra.h
+-rw-r--r--   0 david     (1000) david     (1000)      793 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/iteration_algebra_printer.h
+-rw-r--r--   0 david     (1000) david     (1000)     2252 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/kernel.h
+-rw-r--r--   0 david     (1000) david     (1000)     2423 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/properties.h
+-rw-r--r--   0 david     (1000) david     (1000)     2685 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/property_pointers.h
+-rw-r--r--   0 david     (1000) david     (1000)    23213 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/provenance_graph.h
+-rw-r--r--   0 david     (1000) david     (1000)      929 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/schedule.h
+-rw-r--r--   0 david     (1000) david     (1000)     3389 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/tensor_operator.h
+-rw-r--r--   0 david     (1000) david     (1000)     7475 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/transformations.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/ir/
+-rw-r--r--   0 david     (1000) david     (1000)    19034 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir.h
+-rw-r--r--   0 david     (1000) david     (1000)      922 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_generators.h
+-rw-r--r--   0 david     (1000) david     (1000)     2997 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_printer.h
+-rw-r--r--   0 david     (1000) david     (1000)     2404 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_rewriter.h
+-rw-r--r--   0 david     (1000) david     (1000)      410 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_verifier.h
+-rw-r--r--   0 david     (1000) david     (1000)     4808 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_visitor.h
+-rw-r--r--   0 david     (1000) david     (1000)      349 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/ir/simplify.h
+-rw-r--r--   0 david     (1000) david     (1000)      611 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/workspace_rewriter.h
+-rw-r--r--   0 david     (1000) david     (1000)     1772 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir_tags.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/lower/
+-rw-r--r--   0 david     (1000) david     (1000)    10339 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/iterator.h
+-rw-r--r--   0 david     (1000) david     (1000)     1871 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/lower.h
+-rw-r--r--   0 david     (1000) david     (1000)     3053 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/lowerer_impl.h
+-rw-r--r--   0 david     (1000) david     (1000)    25459 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/lowerer_impl_imperative.h
+-rw-r--r--   0 david     (1000) david     (1000)     8039 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/merge_lattice.h
+-rw-r--r--   0 david     (1000) david     (1000)     2212 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/lower/mode.h
+-rw-r--r--   0 david     (1000) david     (1000)     3232 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/mode_format_compressed.h
+-rw-r--r--   0 david     (1000) david     (1000)     1512 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/mode_format_dense.h
+-rw-r--r--   0 david     (1000) david     (1000)     8570 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/mode_format_impl.h
+-rw-r--r--   0 david     (1000) david     (1000)     2069 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/mode_format_singleton.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/parser/
+-rw-r--r--   0 david     (1000) david     (1000)     1903 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/parser/einsum_parser.h
+-rw-r--r--   0 david     (1000) david     (1000)      789 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/parser/lexer.h
+-rw-r--r--   0 david     (1000) david     (1000)     3015 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/parser/parser.h
+-rw-r--r--   0 david     (1000) david     (1000)      629 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/parser/schedule_parser.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/storage/
+-rw-r--r--   0 david     (1000) david     (1000)     2388 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/array.h
+-rw-r--r--   0 david     (1000) david     (1000)     1650 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/coordinate.h
+-rw-r--r--   0 david     (1000) david     (1000)     1499 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/file_io_mtx.h
+-rw-r--r--   0 david     (1000) david     (1000)     2509 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/file_io_rb.h
+-rw-r--r--   0 david     (1000) david     (1000)      916 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/file_io_tns.h
+-rw-r--r--   0 david     (1000) david     (1000)     2451 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/index.h
+-rw-r--r--   0 david     (1000) david     (1000)     1746 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/pack.h
+-rw-r--r--   0 david     (1000) david     (1000)     2289 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/storage.h
+-rw-r--r--   0 david     (1000) david     (1000)    10031 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/typed_index.h
+-rw-r--r--   0 david     (1000) david     (1000)    10673 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/typed_value.h
+-rw-r--r--   0 david     (1000) david     (1000)     8556 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/typed_vector.h
+-rw-r--r--   0 david     (1000) david     (1000)     1232 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/taco_tensor_t.h
+-rw-r--r--   0 david     (1000) david     (1000)     1386 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/target.h
+-rw-r--r--   0 david     (1000) david     (1000)    47778 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/tensor.h
+-rw-r--r--   0 david     (1000) david     (1000)     7001 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/type.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/util/
+-rw-r--r--   0 david     (1000) david     (1000)    10527 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/collections.h
+-rw-r--r--   0 david     (1000) david     (1000)     1056 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/comparable.h
+-rw-r--r--   0 david     (1000) david     (1000)     2072 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/env.h
+-rw-r--r--   0 david     (1000) david     (1000)      268 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/files.h
+-rw-r--r--   0 david     (1000) david     (1000)     9333 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/fill.h
+-rw-r--r--   0 david     (1000) david     (1000)      523 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/functions.h
+-rw-r--r--   0 david     (1000) david     (1000)     3183 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/intrusive_ptr.h
+-rw-r--r--   0 david     (1000) david     (1000)      483 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/name_generator.h
+-rw-r--r--   0 david     (1000) david     (1000)      352 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/printable.h
+-rw-r--r--   0 david     (1000) david     (1000)     1874 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/scopedmap.h
+-rw-r--r--   0 david     (1000) david     (1000)     1124 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/scopedset.h
+-rw-r--r--   0 david     (1000) david     (1000)      339 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/singleton.h
+-rw-r--r--   0 david     (1000) david     (1000)     2598 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/strings.h
+-rw-r--r--   0 david     (1000) david     (1000)     4597 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/timers.h
+-rw-r--r--   0 david     (1000) david     (1000)      300 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/uncopyable.h
+-rw-r--r--   0 david     (1000) david     (1000)     2886 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/variadic.h
+-rw-r--r--   0 david     (1000) david     (1000)      884 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/version.h.in
+-rw-r--r--   0 david     (1000) david     (1000)      196 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/misc/
+-rw-r--r--   0 david     (1000) david     (1000)      523 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/misc/mainpage.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/python_bindings/
+-rw-r--r--   0 david     (1000) david     (1000)     1333 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)      584 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/Makefile
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/include/
+-rw-r--r--   0 david     (1000) david     (1000)      342 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyDatatypes.h
+-rw-r--r--   0 david     (1000) david     (1000)      372 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyFormat.h
+-rw-r--r--   0 david     (1000) david     (1000)      269 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyIndexNotation.h
+-rw-r--r--   0 david     (1000) david     (1000)      288 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyParsers.h
+-rw-r--r--   0 david     (1000) david     (1000)      242 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyTensor.h
+-rw-r--r--   0 david     (1000) david     (1000)      247 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyTensorIO.h
+-rw-r--r--   0 david     (1000) david     (1000)      168 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyeinsum.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/pybind11/
+-rw-rw-r--   0 david     (1000) david     (1000)     1304 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.appveyor.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      523 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.clang-format
+-rw-rw-r--   0 david     (1000) david     (1000)      242 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.clang-tidy
+-rw-rw-r--   0 david     (1000) david     (1000)     2196 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.cmake-format.yaml
+-rw-rw-r--   0 david     (1000) david     (1000)       75 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.git
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/
+-rw-rw-r--   0 david     (1000) david     (1000)    14415 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/CONTRIBUTING.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 david     (1000) david     (1000)     1270 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      669 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-rw-r--   0 david     (1000) david     (1000)     1180 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/question.md
+-rw-rw-r--   0 david     (1000) david     (1000)      559 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/dependabot.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      116 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/labeler.yml
+-rw-rw-r--   0 david     (1000) david     (1000)       50 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/labeler_merged.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      404 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/pull_request_template.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/
+-rw-rw-r--   0 david     (1000) david     (1000)    24549 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/ci.yml
+-rw-rw-r--   0 david     (1000) david     (1000)     2117 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/configure.yml
+-rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/format.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      333 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/labeler.yml
+-rw-rw-r--   0 david     (1000) david     (1000)     2497 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/pip.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      452 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.gitignore
+-rw-rw-r--   0 david     (1000) david     (1000)     2460 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.pre-commit-config.yaml
+-rw-rw-r--   0 david     (1000) david     (1000)       62 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.readthedocs.yml
+-rw-rw-r--   0 david     (1000) david     (1000)    10364 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     1684 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      256 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     8064 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/README.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)      705 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/Doxyfile
+-rw-rw-r--   0 david     (1000) david     (1000)     7417 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/Makefile
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/_static/
+-rw-rw-r--   0 david     (1000) david     (1000)      254 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/_static/theme_overrides.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/
+-rw-rw-r--   0 david     (1000) david     (1000)     3937 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/chrono.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     3398 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/custom.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    14288 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/eigen.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     3889 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/functional.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     1556 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    11680 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/overview.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     9703 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/stl.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     9372 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/strings.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    45877 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/classes.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     8420 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/embedding.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    14171 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/exceptions.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    25078 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/functions.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    12444 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/misc.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    16538 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     7878 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/object.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     5125 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     6366 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/smart_ptrs.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     9369 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/basics.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     2974 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/benchmark.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3168 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/benchmark.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    73677 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/changelog.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    16122 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/classes.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/cmake/
+-rw-rw-r--   0 david     (1000) david     (1000)      273 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/cmake/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    25511 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/compiling.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    12095 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/conf.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14592 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/faq.rst
+-rw-rw-r--   0 david     (1000) david     (1000)      613 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     3277 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/installing.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     3062 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/limitations.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    58510 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11-logo.png
+-rw-rw-r--   0 david     (1000) david     (1000)    44653 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-rw-r--   0 david     (1000) david     (1000)    87708 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-rw-r--   0 david     (1000) david     (1000)    41121 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-rw-r--   0 david     (1000) david     (1000)    85853 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-rw-r--   0 david     (1000) david     (1000)     2113 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/reference.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     4028 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/release.rst
+-rw-rw-r--   0 david     (1000) david     (1000)      168 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)    21940 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/upgrade.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/python_bindings/pybind11/include/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.217709 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/
+-rw-rw-r--   0 david     (1000) david     (1000)    21412 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 david     (1000) david     (1000)     6118 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 david     (1000) david     (1000)    95557 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 david     (1000) david     (1000)     8185 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 david     (1000) david     (1000)      120 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 david     (1000) david     (1000)     2037 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.217709 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 david     (1000) david     (1000)    27823 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 david     (1000) david     (1000)    40452 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 david     (1000) david     (1000)     3602 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 david     (1000) david     (1000)    16397 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 david     (1000) david     (1000)    16375 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 david     (1000) david     (1000)     1486 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-r--   0 david     (1000) david     (1000)    29086 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 david     (1000) david     (1000)     7843 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 david     (1000) david     (1000)     5079 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 david     (1000) david     (1000)     3709 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 david     (1000) david     (1000)     6084 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 david     (1000) david     (1000)    69310 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 david     (1000) david     (1000)     9085 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 david     (1000) david     (1000)     2049 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 david     (1000) david     (1000)   111558 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 david     (1000) david     (1000)    66118 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/pytypes.h
+-rw-rw-r--   0 david     (1000) david     (1000)    14136 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 david     (1000) david     (1000)    23912 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.217709 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/
+-rw-rw-r--   0 david     (1000) david     (1000)      217 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/__main__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      202 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/_version.py
+-rw-rw-r--   0 david     (1000) david     (1000)      137 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/_version.pyi
+-rw-rw-r--   0 david     (1000) david     (1000)      663 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/commands.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/py.typed
+-rw-rw-r--   0 david     (1000) david     (1000)    15110 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/setup_helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1899 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/setup_helpers.pyi
+-rw-rw-r--   0 david     (1000) david     (1000)      118 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     2185 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     3499 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)    15362 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     4841 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/conftest.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11157 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/constructor_stats.h
+-rw-rw-r--   0 david     (1000) david     (1000)     1819 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/cross_module_gil_utils.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      376 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/env.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_python_package/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_python_package/pytest.ini
+-rw-rw-r--   0 david     (1000) david     (1000)     7074 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_python_package/test_files.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_setuptools/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_setuptools/pytest.ini
+-rw-rw-r--   0 david     (1000) david     (1000)     2581 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2144 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/local_bindings.h
+-rw-rw-r--   0 david     (1000) david     (1000)     5389 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/object.h
+-rw-rw-r--   0 david     (1000) david     (1000)     5285 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     3647 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_tests.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     2733 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_tests.h
+-rw-rw-r--   0 david     (1000) david     (1000)      626 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pytest.ini
+-rw-rw-r--   0 david     (1000) david     (1000)      736 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      864 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_async.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      558 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_async.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8048 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_buffers.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4946 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_buffers.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13475 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_builtin_casters.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    17214 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_builtin_casters.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3702 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_call_policies.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     5728 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_call_policies.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6600 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_callbacks.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4405 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_callbacks.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3406 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_chrono.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     6276 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_chrono.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21623 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_class.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    14273 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_class.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/
+-rw-rw-r--   0 david     (1000) david     (1000)     2639 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      656 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/embed.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-r--   0 david     (1000) david     (1000)     1175 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-r--   0 david     (1000) david     (1000)     1259 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-r--   0 david     (1000) david     (1000)     1653 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      152 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/main.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-r--   0 david     (1000) david     (1000)     1357 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-r--   0 david     (1000) david     (1000)     1333 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      166 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/test.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5346 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     1522 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9629 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_copy_move.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4645 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_copy_move.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5513 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4015 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2514 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_docstring_options.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     1630 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_docstring_options.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16867 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eigen.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    28282 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eigen.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/
+-rw-rw-r--   0 david     (1000) david     (1000)     1758 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      637 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/catch.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      554 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/external_module.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    10209 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      219 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/test_interpreter.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2610 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_enum.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     7694 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_enum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2628 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eval.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      768 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eval.py
+-rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eval_call.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7862 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_exceptions.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     6753 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16562 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_factory_constructors.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    16637 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_factory_constructors.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1760 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_gil_scoped.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     3128 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_gil_scoped.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3381 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_iostream.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     5799 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_iostream.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6489 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    10048 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4333 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_local_bindings.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     8102 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_local_bindings.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19446 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    17310 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3742 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_modules.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     2841 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_modules.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8863 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     9495 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17781 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_array.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    18647 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_array.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17721 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    13484 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3832 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     9709 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2731 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_opaque_types.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     1906 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_opaque_types.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8431 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_operator_overloading.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4136 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_operator_overloading.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4945 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pickling.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     1191 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pickling.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13347 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pytypes.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    13720 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pytypes.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13120 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     5966 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17913 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_smart_ptr.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     9620 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_smart_ptr.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12793 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     8557 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4403 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl_binders.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     7182 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl_binders.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4458 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      765 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.py
+-rw-rw-r--   0 david     (1000) david     (1000)      603 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_union.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_union.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18454 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_virtual_functions.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    11646 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_virtual_functions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2558 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-rw-r--   0 david     (1000) david     (1000)     3103 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/valgrind-python.supp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/
+-rw-rw-r--   0 david     (1000) david     (1000)     2295 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)     3105 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)     9977 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindPythonLibsNew.cmake
+-rwxrwxr-x   0 david     (1000) david     (1000)     1427 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/check-style.sh
+-rw-rw-r--   0 david     (1000) david     (1000)      952 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1121 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/libsize.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     1202 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14003 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)     7010 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 david     (1000) david     (1000)     9172 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)     7276 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     1822 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/setup_main.py.in
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/pytaco/
+-rw-r--r--   0 david     (1000) david     (1000)       57 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     1542 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/numpy_license.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/
+-rw-r--r--   0 david     (1000) david     (1000)       51 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)   111090 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/taco_tensor.py
+-rw-r--r--   0 david     (1000) david     (1000)     2248 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/tensorIO.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/source/
+-rw-r--r--   0 david     (1000) david     (1000)     2526 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/conf.py
+-rw-r--r--   0 david     (1000) david     (1000)      480 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/index.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/source/rst_files/
+-rw-r--r--   0 david     (1000) david     (1000)      114 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/as_np_dt.rst
+-rw-r--r--   0 david     (1000) david     (1000)      102 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/datatype.rst
+-rw-r--r--   0 david     (1000) david     (1000)       87 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/dtype_object.rst
+-rw-r--r--   0 david     (1000) david     (1000)      458 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/expr_funcs.rst
+-rw-r--r--   0 david     (1000) david     (1000)      780 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/file_io.rst
+-rw-r--r--   0 david     (1000) david     (1000)      111 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/format.rst
+-rw-r--r--   0 david     (1000) david     (1000)       73 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/format_class.rst
+-rw-r--r--   0 david     (1000) david     (1000)       71 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/format_funcs.rst
+-rw-r--r--   0 david     (1000) david     (1000)       91 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/idx_exp_obj.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1028 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/index_expressions.rst
+-rw-r--r--   0 david     (1000) david     (1000)       79 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/index_vars.rst
+-rw-r--r--   0 david     (1000) david     (1000)      131 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/iv_funcs.rst
+-rw-r--r--   0 david     (1000) david     (1000)       71 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/mode_format.rst
+-rw-r--r--   0 david     (1000) david     (1000)      152 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/parsers.rst
+-rw-r--r--   0 david     (1000) david     (1000)      199 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/sched.rst
+-rw-r--r--   0 david     (1000) david     (1000)       62 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/tensor_class.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1233 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/tensor_info.rst
+-rw-r--r--   0 david     (1000) david     (1000)       63 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/tensors.rst
+-rw-r--r--   0 david     (1000) david     (1000)      312 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/udfs.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/src/
+-rw-r--r--   0 david     (1000) david     (1000)     4505 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyDatatypes.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11285 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyFormat.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    34934 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyIndexNotation.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3194 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyParsers.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    18175 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyTensor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      805 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyTensorIO.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4379 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pytaco.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    10971 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/unit_tests.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/src/
+-rw-r--r--   0 david     (1000) david     (1000)     1031 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/src/codegen/
+-rw-r--r--   0 david     (1000) david     (1000)    19006 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3120 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen.h
+-rw-r--r--   0 david     (1000) david     (1000)    17904 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen_c.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1454 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen_c.h
+-rw-r--r--   0 david     (1000) david     (1000)    49177 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen_cuda.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3090 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen_cuda.h
+-rw-r--r--   0 david     (1000) david     (1000)     5739 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/module.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1925 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/cuda.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/src/error/
+-rw-r--r--   0 david     (1000) david     (1000)     5070 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/error/error_checks.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      902 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/error/error_checks.h
+-rw-r--r--   0 david     (1000) david     (1000)     1309 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/error/error_messages.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1730 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/error.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11646 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/format.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.233709 tensora-0.0.7/src/taco/src/index_notation/
+-rw-r--r--   0 david     (1000) david     (1000)      356 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/README.md
+-rw-r--r--   0 david     (1000) david     (1000)   116223 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2791 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_nodes.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1049 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_nodes_abstract.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7250 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_printer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11661 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_rewriter.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2942 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_visitor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    40775 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/intrinsic.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     8065 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/iteration_algebra.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1309 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/iteration_algebra_printer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4292 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/kernel.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4914 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/properties.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3423 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/property_pointers.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    58668 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/provenance_graph.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1424 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/schedule.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4853 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/tensor_operator.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    74399 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/transformations.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.233709 tensora-0.0.7/src/taco/src/ir/
+-rw-r--r--   0 david     (1000) david     (1000)      239 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/ir/README.md
+-rw-r--r--   0 david     (1000) david     (1000)    26833 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1805 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_generators.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    15742 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_printer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    10832 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_rewriter.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     8912 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_verifier.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4411 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_visitor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    19916 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/simplify.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2669 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/workspace_rewriter.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      573 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir_tags.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.233709 tensora-0.0.7/src/taco/src/lower/
+-rw-r--r--   0 david     (1000) david     (1000)      260 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/README.md
+-rw-r--r--   0 david     (1000) david     (1000)     7225 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/expr_tools.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      870 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/expr_tools.h
+-rw-r--r--   0 david     (1000) david     (1000)     6683 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/iteration_forest.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1020 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/iteration_forest.h
+-rw-r--r--   0 david     (1000) david     (1000)     8081 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/iteration_graph.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2945 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/iteration_graph.h
+-rw-r--r--   0 david     (1000) david     (1000)    23959 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/iterator.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2021 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/lower.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3152 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/lowerer_impl.cpp
+-rw-r--r--   0 david     (1000) david     (1000)   170132 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/lowerer_impl_imperative.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    49768 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/merge_lattice.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2880 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/mode.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      879 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_access.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      819 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/mode_access.h
+-rw-r--r--   0 david     (1000) david     (1000)    11956 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_format_compressed.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2878 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_format_dense.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     8358 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_format_impl.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     6169 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_format_singleton.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2930 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/tensor_path.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2200 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/tensor_path.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.237709 tensora-0.0.7/src/taco/src/parser/
+-rw-r--r--   0 david     (1000) david     (1000)      293 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/parser/README.md
+-rw-r--r--   0 david     (1000) david     (1000)     9758 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/parser/einsum_parser.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3565 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/parser/lexer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11905 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/parser/parser.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7141 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/parser/schedule_parser.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.237709 tensora-0.0.7/src/taco/src/storage/
+-rw-r--r--   0 david     (1000) david     (1000)      152 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/storage/README.md
+-rw-r--r--   0 david     (1000) david     (1000)     5348 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/storage/array.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    12244 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/file_io_mtx.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13141 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/file_io_rb.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4661 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/file_io_tns.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3551 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/storage/index.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7948 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/pack.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     6004 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/storage.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    18028 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/storage/typed_index.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    23635 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/typed_value.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2366 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/taco_tensor_t.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1904 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/target.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    47292 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/tensor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     9240 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/type.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.237709 tensora-0.0.7/src/taco/src/util/
+-rw-r--r--   0 david     (1000) david     (1000)      635 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/util/env.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      512 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/util/files.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      880 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/util/name_generator.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1062 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/util/strings.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/
+-rw-r--r--   0 david     (1000) david     (1000)      931 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)     3773 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/README_testing.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/
+-rw-rw-r--   0 david     (1000) david     (1000)      546 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.appveyor.yml
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/.devcontainer/
+-rw-rw-r--   0 david     (1000) david     (1000)      519 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.devcontainer/Dockerfile
+-rw-rw-r--   0 david     (1000) david     (1000)       83 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.devcontainer/devcontainer.json
+-rw-rw-r--   0 david     (1000) david     (1000)      687 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.editorconfig
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/test/bats/.git
+-rwxrwxr-x   0 david     (1000) david     (1000)       41 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.gitattributes
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.gitignore
+-rw-rw-r--   0 david     (1000) david     (1000)      800 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.travis.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      219 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/AUTHORS
+-rw-rw-r--   0 david     (1000) david     (1000)      386 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/Dockerfile
+-rw-rw-r--   0 david     (1000) david     (1000)     2535 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/LICENSE.md
+-rw-rw-r--   0 david     (1000) david     (1000)    23464 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/bin/
+-rwxrwxr-x   0 david     (1000) david     (1000)     1675 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/bin/bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/contrib/
+-rwxrwxr-x   0 david     (1000) david     (1000)     3795 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/contrib/release.sh
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/contrib/rpm/
+-rw-rw-r--   0 david     (1000) david     (1000)     1575 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/contrib/rpm/bats.spec
+-rwxrwxr-x   0 david     (1000) david     (1000)     7973 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/contrib/semver
+-rw-rw-r--   0 david     (1000) david     (1000)      147 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docker-compose.override.dist
+-rw-rw-r--   0 david     (1000) david     (1000)      244 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docker-compose.yml
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)     7042 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)      211 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/CODEOWNERS
+-rw-rw-r--   0 david     (1000) david     (1000)     3643 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 david     (1000) david     (1000)    17557 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/CONTRIBUTING.md
+-rw-rw-r--   0 david     (1000) david     (1000)      317 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/docs/examples/
+-rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/examples/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      604 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/examples/package-tarball
+-rwxrwxr-x   0 david     (1000) david     (1000)      869 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/examples/package-tarball.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     3979 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/releasing.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2338 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/usage.md
+-rw-rw-r--   0 david     (1000) david     (1000)      287 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/versions.md
+-rwxrwxr-x   0 david     (1000) david     (1000)      627 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/install.sh
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/test/bats/lib/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.245709 tensora-0.0.7/src/taco/test/bats/lib/bats-core/
+-rw-rw-r--   0 david     (1000) david     (1000)      827 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/lib/bats-core/preprocessing.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     2646 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/lib/bats-core/test_functions.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     4197 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/lib/bats-core/tracing.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     1002 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/lib/bats-core/validator.bash
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/test/bats/libexec/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.245709 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/
+-rwxrwxr-x   0 david     (1000) david     (1000)     5567 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats
+-rwxrwxr-x   0 david     (1000) david     (1000)     5654 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-file
+-rwxrwxr-x   0 david     (1000) david     (1000)     2386 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-suite
+-rwxrwxr-x   0 david     (1000) david     (1000)     4762 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-test
+-rwxrwxr-x   0 david     (1000) david     (1000)     3436 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-format-junit
+-rwxrwxr-x   0 david     (1000) david     (1000)     4421 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-format-pretty
+-rwxrwxr-x   0 david     (1000) david     (1000)       32 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-format-tap
+-rwxrwxr-x   0 david     (1000) david     (1000)     1308 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-preprocess
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.245709 tensora-0.0.7/src/taco/test/bats/man/
+-rw-rw-r--   0 david     (1000) david     (1000)      427 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/Makefile
+-rw-rw-r--   0 david     (1000) david     (1000)      253 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)     3836 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/bats.1
+-rw-rw-r--   0 david     (1000) david     (1000)     3544 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/bats.1.ronn
+-rw-rw-r--   0 david     (1000) david     (1000)     4928 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/bats.7
+-rw-rw-r--   0 david     (1000) david     (1000)     4510 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/bats.7.ronn
+-rw-rw-r--   0 david     (1000) david     (1000)      641 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/package.json
+-rwxrwxr-x   0 david     (1000) david     (1000)      277 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/shellcheck.sh
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.245709 tensora-0.0.7/src/taco/test/bats/test/
+-rwxrwxr-x   0 david     (1000) david     (1000)    20307 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/bats.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     7356 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/file_setup_teardown.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/test/bats/test/fixtures/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/
+-rw-rw-r--   0 david     (1000) david     (1000)      171 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/ambiguous
+-rw-rw-r--   0 david     (1000) david     (1000)      179 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/ambiguous.bash
+-rwxrwxr-x   0 david     (1000) david     (1000)      295 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/cmd_using_stdin.bash
+-rw-rw-r--   0 david     (1000) david     (1000)       35 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/dos_line.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      233 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/duplicate-tests.bats
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/empty.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      138 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/environment.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/expand_var_in_test_name.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      104 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/exported_function.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     1186 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/external_function_calls.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       72 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing_and_passing.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       80 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing_helper.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing_setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       83 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing_teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/intact.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      118 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/load.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      239 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/loop_keep_IFS.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/no-final-newline.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      331 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/output.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/parallel.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/passing.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/passing_and_failing.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/passing_and_skipping.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      106 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/passing_failing_and_skipping.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      109 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/quoted_and_unquoted_test_names.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      501 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/read_from_stdin.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       81 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      179 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter_in_setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      113 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter_in_teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      266 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      144 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/single_line.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/skipped.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/skipped_with_parens.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       72 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      170 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file_in_setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      104 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file_in_teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      169 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      267 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/test_helper.bash
+-rw-rw-r--   0 david     (1000) david     (1000)      331 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/unbound_variable.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       50 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/unofficial_bash_strict_mode.bash
+-rw-rw-r--   0 david     (1000) david     (1000)       92 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/unofficial_bash_strict_mode.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      593 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/whitespace.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       24 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/without_trailing_newline.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/
+-rw-rw-r--   0 david     (1000) david     (1000)       25 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/no_setup_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       26 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/no_teardown_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      317 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       91 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_does_not_leak_env.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       69 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_does_not_leak_env2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      125 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_even_if_all_tests_are_skipped.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       84 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_failed.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       71 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_halfway_error.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      117 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      117 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       96 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_after_failing_test.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      152 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_after_long_test.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      108 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_does_not_leak.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_does_not_leak2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_even_if_all_tests_are_skipped.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       57 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_failed.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       75 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_halfway_error.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/
+-rw-rw-r--   0 david     (1000) david     (1000)      191 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/parallel-preserve-environment.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/parallel.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file1.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file3.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/parallel1.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/parallel2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/parallel3.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/parallel4.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/empty/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/empty/.gitkeep
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/filter/
+-rw-rw-r--   0 david     (1000) david     (1000)       65 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/filter/a.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       66 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/filter/b.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       68 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/filter/c.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/multiple/
+-rw-rw-r--   0 david     (1000) david     (1000)       25 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/multiple/a.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       73 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/multiple/b.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/recursive/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/recursive/subsuite/
+-rw-rw-r--   0 david     (1000) david     (1000)       40 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/recursive/subsuite/test2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/recursive/test.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/single/
+-rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/single/test.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/
+-rw-rw-r--   0 david     (1000) david     (1000)      319 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-setup-and-teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      194 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      158 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      245 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-test-and-teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      131 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-test.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     2116 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/install.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      583 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/junit-formatter.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     2323 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/parallell.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     2883 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/root.bats
+-rwxrwxr-x   0 david     (1000) david     (1000)     4913 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/suite.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     1034 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/test_helper.bash
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/data/
+-rw-r--r--   0 david     (1000) david     (1000)      119 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/2tensor.mtx
+-rw-r--r--   0 david     (1000) david     (1000)       36 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/3tensor.tns
+-rw-r--r--   0 david     (1000) david     (1000)      267 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/d33.mtx
+-rw-r--r--   0 david     (1000) david     (1000)       66 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/d33.ttx
+-rw-r--r--   0 david     (1000) david     (1000)      136 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/d432.ttx
+-rw-r--r--   0 david     (1000) david     (1000)       88 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/d567.ttx
+-rw-r--r--   0 david     (1000) david     (1000)      268 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/ds33.mtx
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/data/qcd/
+-rw-r--r--   0 david     (1000) david     (1000)    11615 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/qcd/theta.ttx
+-rw-r--r--   0 david     (1000) david     (1000)       64 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/qcd/theta_simple.ttx
+-rw-r--r--   0 david     (1000) david     (1000)      555 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/qcd/z.ttx
+-rw-r--r--   0 david     (1000) david     (1000)       52 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/qcd/z_simple.ttx
+-rw-r--r--   0 david     (1000) david     (1000)     1487 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/rua_32.mtx
+-rw-r--r--   0 david     (1000) david     (1000)     1986 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/rua_32.rb
+-rw-r--r--   0 david     (1000) david     (1000)     4650 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/expr_factory.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2589 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/expr_factory.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/gtest/
+-rw-r--r--   0 david     (1000) david     (1000)     1475 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/gtest/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      155 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/gtest/README.TAC
+-rw-r--r--   0 david     (1000) david     (1000)   365644 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/gtest/gtest-all.cc
+-rw-r--r--   0 david     (1000) david     (1000)   849134 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/gtest/gtest.h
+-rw-r--r--   0 david     (1000) david     (1000)     4788 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/op_factory.h
+-rwxr-xr-x   0 david     (1000) david     (1000)    12555 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/taco-cli-test.bats
+-rw-r--r--   0 david     (1000) david     (1000)     7165 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test-iteration_algebra.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1110 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test-typedcomponent-memory.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1897 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3618 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test.h
+-rw-r--r--   0 david     (1000) david     (1000)     3125 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test_properties.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11493 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test_tensors.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     5687 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test_tensors.h
+-rw-r--r--   0 david     (1000) david     (1000)    12251 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-api.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2561 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-copyprop.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1310 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-error.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      493 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-expr-reduction.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     5044 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-expr.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    43783 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-expr_storage.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3200 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-format-mm-permute.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2112 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-format.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1044 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-index.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13133 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-index_notation.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2306 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-indexexpr.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2918 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-indexstmt.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3609 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-io.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    55894 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-lower.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    59718 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-merge_lattice.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7101 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-parafac.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1837 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-qcd.cpp
+-rw-r--r--   0 david     (1000) david     (1000)       68 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-regression.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3602 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-schedule-parser.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    76554 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-scheduling-eval.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    32561 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-scheduling.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    14078 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-storage.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3573 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-storage_alloc.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13383 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-tensor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13605 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-tensor_types.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    14092 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-transformation.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3574 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-transpose.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3576 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-type.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    19463 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-windowing.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    17609 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-workspaces.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/tools/
+-rw-r--r--   0 david     (1000) david     (1000)      490 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/tools/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)    52311 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/tools/taco.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/tensora/
+-rw-rw-r--   0 david     (1000) david     (1000)      148 2020-07-08 11:47:39.000000 tensora-0.0.7/src/tensora/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19747 2023-01-16 18:11:03.000000 tensora-0.0.7/src/tensora/compile.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/tensora/expression/
+-rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:57:19.000000 tensora-0.0.7/src/tensora/expression/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5267 2020-07-08 11:47:39.000000 tensora-0.0.7/src/tensora/expression/ast.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1676 2023-06-15 20:57:23.000000 tensora-0.0.7/src/tensora/expression/parser.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/tensora/format/
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2020-07-08 11:47:39.000000 tensora-0.0.7/src/tensora/format/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1305 2020-07-08 11:47:39.000000 tensora-0.0.7/src/tensora/format/format.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1502 2023-06-16 10:05:44.000000 tensora-0.0.7/src/tensora/format/parser.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7052 2023-06-15 20:57:23.000000 tensora-0.0.7/src/tensora/function.py
+-rw-rw-r--   0 david     (1000) david     (1000)    23902 2023-06-15 20:57:23.000000 tensora-0.0.7/src/tensora/tensor.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/tensora.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     9253 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)    33517 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.257709 tensora-0.0.7/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     4741 2023-06-15 20:57:19.000000 tensora-0.0.7/tests/test_combinatorically.py
+-rw-r--r--   0 david     (1000) david     (1000)     2852 2023-01-16 18:11:03.000000 tensora-0.0.7/tests/test_compile.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2685 2023-06-15 20:57:23.000000 tensora-0.0.7/tests/test_expression.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1686 2023-06-15 20:57:23.000000 tensora-0.0.7/tests/test_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9370 2020-07-08 11:47:39.000000 tensora-0.0.7/tests/test_from_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2901 2023-01-16 18:11:03.000000 tensora-0.0.7/tests/test_function.py
+-rw-r--r--   0 david     (1000) david     (1000)      583 2023-01-16 18:11:03.000000 tensora-0.0.7/tests/test_numpy.py
+-rw-rw-r--   0 david     (1000) david     (1000)      668 2020-07-08 11:47:39.000000 tensora-0.0.7/tests/test_operators.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10193 2023-01-16 18:11:03.000000 tensora-0.0.7/tests/test_tensor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tensora-0.0.6/LICENSE` & `tensora-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/PKG-INFO` & `tensora-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,180 @@
 Metadata-Version: 2.1
 Name: tensora
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library for dense and sparse tensors built on the tensor algebra compiler.
 Home-page: https://github.com/drhagen/tensora
 Author: David Hagen
 Author-email: david@drhagen.com
 License: MIT
-Description: # Tensora
-        
-        A fast and easy-to-use dense/sparse tensor library for Python. Evaluate arbitrary tensor expressions with tensors in a variety of sparsity formats.
-        
-        Tensors are n-dimensional generalizations of matrices. Instead of being confined to 1 or 2 dimensions, tensors may have 3, 4, or more dimensions. They are useful in a variety of applications. NumPy is the best known tensor library in Python; its central `ndarray` object is an example of a dense tensor. 
-        
-        In a dense tensor, each element is explicitly stored in memory. If the vast majority of elements are zero, then this is an inefficient layout, taking far more memory to store and far more time to operate on. There are many different sparse tensor formats, each one better or worse depending on which elements of the tensor are nonzero.
-        
-        Many tensor kernels (functions that perform a specific algebraic calculation between tensors with specific sparse formats) have been written to solve specific problems. Recently, the [Tensor Algebra Compiler](http://tensor-compiler.org/) (taco) was invented to automate the construction and optimization of tensor kernels for arbitrary algebraic expressions for arbitrary sparse formats. taco takes an algebraic expression and description of the format of each tensor in the expression and returns a C function that efficiently evaluates the given expression for those tensor arguments.
-        
-        Tensora is a Python wrapper around taco. Tensora has a central class `Tensor` that simply has a pointer to a taco tensor held in C memory, managed by the `cffi` package. Tensora exposes functions that take a string of an algebraic expression and return a Python function the performs that operation in fast C code. In order to do that, the string is parsed and passed to taco; the C code generated by taco is compiled "on the fly" by `cffi` and then wrapped by code that provides good error handling.
-        
-        **This package is highly experimental. Do not trust the results without independently verifying the output for any particular problem.** This is mostly because the underlying taco compiler is itself highly experimental. Much of Tensora's test suite is skipped because of known underlying bugs in the generated kernels. As the research on taco improves, the test suite of Tensora will be expanded and the documentation improved.
-        
-        
-        ## Getting started
-        
-        Tensora can be installed with `pip` from PyPI:
-         
-        ```bash
-        pip install tensora
-        ```
-        
-        The class `Tensor` and the function `evaluate` together provide the porcelain interface for Tensora.
-        
-        Here is an example of multiplying a sparse matrix in CSR format with a dense vector:
-        
-        ```python
-        from tensora import Tensor, evaluate
-        
-        elements = {
-            (1,0): 2.0,
-            (0,1): -2.0,
-            (1,2): 4.0, 
-        }
-        
-        A = Tensor.from_dok(elements, dimensions=(2,3), format='ds')
-        x = Tensor.from_lol([0, -1, 2])
-        
-        y = evaluate('y(i) = A(i,j) * x(j)', 'd', A=A, x=x)
-        
-        assert y == Tensor.from_lol([2,8])
-        ``` 
-        
-        
-        ## Creating `Tensor`s
-        
-        Creating a `Tensor` is best done via the `Tensor.from_*` methods. These methods convert a variety of data types into a `Tensor`. Most of the conversion methods optionally take both `dimensions` and `format` to determine the dimensions and format of the resulting tensor. 
-        
-        ### `from_lol`: list of lists
-        
-        ```python
-        Tensor.from_lol(lol, *, 
-                        dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
-        ```
-        
-        Convert a dense list of lists to a `Tensor`.
-        
-        * `lol` is a list of lists, possibly deeply nested. That is, `lol` is a `float`, a `List[float]`, a `List[List[float]]`, etc. to an arbitrary depth of `List`s. The values are read in row-major format, meaning the top-level list is the first dimension and the deepest list (the one containing actual scalars) is the last dimension. All lists at the same level must have the same length. For those familiar, this is identical to the NumPy behavior when constructing an array from lists of lists via `numpy.array`.
-        
-        * `dimensions` has a default value that is inferred from the structure of `lol`. If provided, it must be consistent with the structure of `lol`. Providing the dimensions is typically only useful when one or more non-final dimensions may have size zero. For example, `Tensor.from_lol([[], []])` has dimensions of `(2,0)`, while `Tensor.from_lol([[], []], dimensions=(2,0,3))` has dimensions of `(2,0,3)`.
-        
-        * `format` has a default value of all dense dimensions.
-        
-        ### `from_dok`: dictionary of keys
-        
-        ```python
-        Tensor.from_dok(dok: Dict[Tuple[int, ...], float], *, 
-                        dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
-        ```
-        
-        Convert a dictionary of keys to a `Tensor`.
-        
-        * `dok` is a Python dictionary where each key is the coordinate of one non-zero value and the value of the entry is the value of the tensor at that coordinate. All coordinates not mentioned are implicitly zero.
-        
-        * `dimensions` has a default value that is the largest size in each dimension found among the coordinates.
-        
-        * `format` has a default value of dense dimensions as long as the number of nonzeros is larger than the product of those dimensions and then sparse dimensions after that. The default value is subject to change with experience.
-        
-        ### `from_aos`: array of structs
-        
-        ```python
-        Tensor.from_aos(aos: Iterable[Tuple[int, ...]], values: Iterable[float], *, 
-                        dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
-        ```
-        
-        Convert a list of coordinates and a corresponding list of values to a `Tensor`.
-        
-        * `aos` is an iterable of the coordinates of the non-zero values.
-        
-        * `values` must be the same length as `aos` and each value is the non-zero value at the corresponding coordinate.
-        
-        * `dimensions` has the same default as `Tensor.from_dok`, the largest size in each dimension.
-        
-        * `format`has the same default as `Tensor.from_dok`, dense for an many dimensions as needed to fit the non-zeros.
-        
-        ### `from_soa`: struct of arrays
-        
-        ```python
-        Tensor.from_soa(soa: Tuple[Iterable[int], ...], values: Iterable[float], *, 
-                        dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
-        ```
-        
-        Convert lists of indexes for each dimension and a corresponding list of values to a `Tensor`.
-        
-        * `soa` is a tuple of iterables, where each iterable is all the indexes of the corresponding dimension. All iterables must be the same length.
-        
-        * `values` must be the same length as the iterables in coordinates and each value is the non-zero value at the corresponding coordinate.
-        
-        * `dimensions` has the same default as `Tensor.from_dok`, the largest size in each dimension.
-        
-        * `format`has the same default as `Tensor.from_dok`, dense for an many dimensions as needed to fit the non-zeros.
-        
-        ### `from_numpy`: convert a NumPy array
-        
-        ```python
-        Tensor.from_numpy(array: numpy.ndarray, *, 
-                          format: Union[Format, str] = None)
-        ```
-        
-        Convert a NumPy array to a `Tensor`.
-        
-        * `array` is any `NumPy.ndarray`. The resulting `Tensor` will have the same order, dimensions, and values of this array. 
-        
-        * `format` has a default value of all dense dimensions.
-        
-        ### `from_scipy_sparse`: convert a SciPy sparse matrix
-        
-        ```python
-        Tensor.from_scipy_sparse(data: scipy.sparse.spmatrix, *, 
-                                 format: Union[Format, str] = None)
-        ```
-        
-        Convert a SciPy sparse matrix to a `Tensor`.
-        
-        * `matrix` is any `SciPy.sparse.spmatrix`. The resulting `Tensor` will have the same order, dimensions, and values of this matrix. The tensor will always have order 2.
-        
-        * `format` has a default value of `ds` for `csr_matrix` and `d1s0` for `csc_matrix` and also `ds` for the other sparse matrix types, though that is subject to changes as taco adds new format mode types.
-        
-        
-        ## Evaluating expressions
-        
-        Taco generates kernels for algebraic expressions of tensor kernels. Tensora wraps this process with the `evaluate` function.
-        
-        ```python
-        evaluate(assignment: str, output_format: str, **inputs: Tensor)
-        ``` 
-        
-        * `assignment` is parsable as an algebraic tensor assignment.
-        
-        * `output_format` is the desired format of the output tensor.
-        
-        * `inputs` is all the inputs to the expression. There must be one named argument for each variable name in `assignment`. The dimensions of the tensors in `inputs` must be consistent with `assignment` and with each other.
 Keywords: tensor sparse matrix array
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: numpy
 Provides-Extra: scipy
+License-File: LICENSE
+
+# Tensora
+
+A fast and easy-to-use dense/sparse tensor library for Python. Evaluate arbitrary tensor expressions with tensors in a variety of sparsity formats.
+
+Tensors are n-dimensional generalizations of matrices. Instead of being confined to 1 or 2 dimensions, tensors may have 3, 4, or more dimensions. They are useful in a variety of applications. NumPy is the best known tensor library in Python; its central `ndarray` object is an example of a dense tensor. 
+
+In a dense tensor, each element is explicitly stored in memory. If the vast majority of elements are zero, then this is an inefficient layout, taking far more memory to store and far more time to operate on. There are many different sparse tensor formats, each one better or worse depending on which elements of the tensor are nonzero.
+
+Many tensor kernels (functions that perform a specific algebraic calculation between tensors with specific sparse formats) have been written to solve specific problems. Recently, the [Tensor Algebra Compiler](http://tensor-compiler.org/) (taco) was invented to automate the construction and optimization of tensor kernels for arbitrary algebraic expressions for arbitrary sparse formats. taco takes an algebraic expression and description of the format of each tensor in the expression and returns a C function that efficiently evaluates the given expression for those tensor arguments.
+
+Tensora is a Python wrapper around taco. Tensora has a central class `Tensor` that simply has a pointer to a taco tensor held in C memory, managed by the `cffi` package. Tensora exposes functions that take a string of an algebraic expression and return a Python function the performs that operation in fast C code. In order to do that, the string is parsed and passed to taco; the C code generated by taco is compiled "on the fly" by `cffi` and then wrapped by code that provides good error handling.
+
+**This package is highly experimental. Do not trust the results without independently verifying the output for any particular problem.** This is mostly because the underlying taco compiler is itself highly experimental. Much of Tensora's test suite is skipped because of known underlying bugs in the generated kernels. As the research on taco improves, the test suite of Tensora will be expanded and the documentation improved.
+
+
+## Getting started
+
+Tensora can be installed with `pip` from PyPI:
+ 
+```bash
+pip install tensora
+```
+
+The class `Tensor` and the function `evaluate` together provide the porcelain interface for Tensora.
+
+Here is an example of multiplying a sparse matrix in CSR format with a dense vector:
+
+```python
+from tensora import Tensor, evaluate
+
+elements = {
+    (1,0): 2.0,
+    (0,1): -2.0,
+    (1,2): 4.0, 
+}
+
+A = Tensor.from_dok(elements, dimensions=(2,3), format='ds')
+x = Tensor.from_lol([0, -1, 2])
+
+y = evaluate('y(i) = A(i,j) * x(j)', 'd', A=A, x=x)
+
+assert y == Tensor.from_lol([2,8])
+``` 
+
+
+## Creating `Tensor`s
+
+Creating a `Tensor` is best done via the `Tensor.from_*` methods. These methods convert a variety of data types into a `Tensor`. Most of the conversion methods optionally take both `dimensions` and `format` to determine the dimensions and format of the resulting tensor. 
+
+### `from_lol`: list of lists
+
+```python
+Tensor.from_lol(lol, *, 
+                dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
+```
+
+Convert a dense list of lists to a `Tensor`.
+
+* `lol` is a list of lists, possibly deeply nested. That is, `lol` is a `float`, a `List[float]`, a `List[List[float]]`, etc. to an arbitrary depth of `List`s. The values are read in row-major format, meaning the top-level list is the first dimension and the deepest list (the one containing actual scalars) is the last dimension. All lists at the same level must have the same length. For those familiar, this is identical to the NumPy behavior when constructing an array from lists of lists via `numpy.array`.
+
+* `dimensions` has a default value that is inferred from the structure of `lol`. If provided, it must be consistent with the structure of `lol`. Providing the dimensions is typically only useful when one or more non-final dimensions may have size zero. For example, `Tensor.from_lol([[], []])` has dimensions of `(2,0)`, while `Tensor.from_lol([[], []], dimensions=(2,0,3))` has dimensions of `(2,0,3)`.
+
+* `format` has a default value of all dense dimensions.
+
+### `from_dok`: dictionary of keys
+
+```python
+Tensor.from_dok(dok: Dict[Tuple[int, ...], float], *, 
+                dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
+```
+
+Convert a dictionary of keys to a `Tensor`.
+
+* `dok` is a Python dictionary where each key is the coordinate of one non-zero value and the value of the entry is the value of the tensor at that coordinate. All coordinates not mentioned are implicitly zero.
+
+* `dimensions` has a default value that is the largest size in each dimension found among the coordinates.
+
+* `format` has a default value of dense dimensions as long as the number of nonzeros is larger than the product of those dimensions and then sparse dimensions after that. The default value is subject to change with experience.
+
+### `from_aos`: array of structs
+
+```python
+Tensor.from_aos(aos: Iterable[Tuple[int, ...]], values: Iterable[float], *, 
+                dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
+```
+
+Convert a list of coordinates and a corresponding list of values to a `Tensor`.
+
+* `aos` is an iterable of the coordinates of the non-zero values.
+
+* `values` must be the same length as `aos` and each value is the non-zero value at the corresponding coordinate.
+
+* `dimensions` has the same default as `Tensor.from_dok`, the largest size in each dimension.
+
+* `format`has the same default as `Tensor.from_dok`, dense for an many dimensions as needed to fit the non-zeros.
+
+### `from_soa`: struct of arrays
+
+```python
+Tensor.from_soa(soa: Tuple[Iterable[int], ...], values: Iterable[float], *, 
+                dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
+```
+
+Convert lists of indexes for each dimension and a corresponding list of values to a `Tensor`.
+
+* `soa` is a tuple of iterables, where each iterable is all the indexes of the corresponding dimension. All iterables must be the same length.
+
+* `values` must be the same length as the iterables in coordinates and each value is the non-zero value at the corresponding coordinate.
+
+* `dimensions` has the same default as `Tensor.from_dok`, the largest size in each dimension.
+
+* `format`has the same default as `Tensor.from_dok`, dense for an many dimensions as needed to fit the non-zeros.
+
+### `from_numpy`: convert a NumPy array
+
+```python
+Tensor.from_numpy(array: numpy.ndarray, *, 
+                  format: Union[Format, str] = None)
+```
+
+Convert a NumPy array to a `Tensor`.
+
+* `array` is any `NumPy.ndarray`. The resulting `Tensor` will have the same order, dimensions, and values of this array. 
+
+* `format` has a default value of all dense dimensions.
+
+### `from_scipy_sparse`: convert a SciPy sparse matrix
+
+```python
+Tensor.from_scipy_sparse(data: scipy.sparse.spmatrix, *, 
+                         format: Union[Format, str] = None)
+```
+
+Convert a SciPy sparse matrix to a `Tensor`.
+
+* `matrix` is any `SciPy.sparse.spmatrix`. The resulting `Tensor` will have the same order, dimensions, and values of this matrix. The tensor will always have order 2.
+
+* `format` has a default value of `ds` for `csr_matrix` and `d1s0` for `csc_matrix` and also `ds` for the other sparse matrix types, though that is subject to changes as taco adds new format mode types.
+
+
+## Evaluating expressions
+
+Taco generates kernels for algebraic expressions of tensor kernels. Tensora wraps this process with the `evaluate` function.
+
+```python
+evaluate(assignment: str, output_format: str, **inputs: Tensor)
+``` 
+
+* `assignment` is parsable as an algebraic tensor assignment.
+
+* `output_format` is the desired format of the output tensor.
+
+* `inputs` is all the inputs to the expression. There must be one named argument for each variable name in `assignment`. The dimensions of the tensors in `inputs` must be consistent with `assignment` and with each other.
```

### Comparing `tensora-0.0.6/README.md` & `tensora-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/setup.py` & `tensora-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         # Ensure that platform tag is included because binaries are platform-specific
         self.root_is_pure = False
 
 
 setup(
     name='tensora',
-    version='0.0.6',
+    version='0.0.7',
 
     description='Library for dense and sparse tensors built on the tensor algebra compiler.',
     long_description=Path('README.md').read_text(encoding='utf-8'),
     long_description_content_type='text/markdown',
     keywords='tensor sparse matrix array',
 
     author='David Hagen',
@@ -70,16 +70,18 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     cmdclass={
         'build': TensoraBuild,
         'bdist_wheel': TensoraBdistWheel,
     },
     zip_safe=False,
```

### Comparing `tensora-0.0.6/src/taco/Doxyfile` & `tensora-0.0.7/src/taco/Doxyfile`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/LICENSE` & `tensora-0.0.7/src/taco/LICENSE`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/apps/tensor_times_vector/CMakeLists.txt` & `tensora-0.0.7/src/taco/apps/tensor_times_vector/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-cmake_minimum_required(VERSION 2.8)
+cmake_minimum_required(VERSION 2.8.12)
+if(POLICY CMP0048)
+  cmake_policy(SET CMP0048 NEW)
+endif()
 project(tensor_times_vector)
 
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
 file(GLOB SOURCE_CODE ${PROJECT_SOURCE_DIR}/*.cpp)
 add_executable(${PROJECT_NAME} ${SOURCE_CODE})
 
 # To let the app be a standalone project
```

### Comparing `tensora-0.0.6/src/taco/include/taco/codegen/module.h` & `tensora-0.0.7/src/taco/include/taco/codegen/module.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef TACO_MODULE_H
 #define TACO_MODULE_H
 
 #include <map>
 #include <vector>
 #include <string>
 #include <utility>
+#include <random>
 
 #include "taco/target.h"
 #include "taco/ir/ir.h"
 
 namespace taco {
 namespace ir {
 
@@ -17,16 +18,14 @@
   /// Create a module for some target
   Module(Target target=getTargetFromEnvironment())
     : lib_handle(nullptr), moduleFromUserSource(false), target(target) {
     setJITLibname();
     setJITTmpdir();
   }
 
-  void reset();
-
   /// Compile the source into a library, returning its full path
   std::string compile();
   
   /// Compile the module into a source file located at the specified location
   /// path and prefix.  The generated source will be path/prefix.{.c|.bc, .h}
   void compileToSource(std::string path, std::string prefix);
   
@@ -78,12 +77,16 @@
   // true iff the module was created from user-provided source
   bool moduleFromUserSource;
 
   Target target;
   
   void setJITLibname();
   void setJITTmpdir();
+
+  static std::string chars;
+  static std::default_random_engine gen;
+  static std::uniform_int_distribution<int> randint;
 };
 
 } // namespace ir
 } // namespace taco
 #endif
```

### Comparing `tensora-0.0.6/src/taco/include/taco/cuda.h` & `tensora-0.0.7/src/taco/include/taco/cuda.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/error/error_messages.h` & `tensora-0.0.7/src/taco/include/taco/error/error_messages.h`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 extern const std::string expr_dimension_mismatch;
 extern const std::string expr_transposition;
 extern const std::string expr_distribution;
 extern const std::string expr_einsum_missformed;
 
 // compile error messages
 extern const std::string compile_without_expr;
+extern const std::string compile_tensor_name_collision;
 
 // assemble error messages
 extern const std::string assemble_without_compile;
 
 // compute error messages
 extern const std::string compute_without_compile;
```

### Comparing `tensora-0.0.6/src/taco/include/taco/error.h` & `tensora-0.0.7/src/taco/include/taco/error.h`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 
 #include <string>
 #include <sstream>
 #include <ostream>
 
 namespace taco {
 
+class TacoException : public std::exception{
+
+public:
+  explicit TacoException(std::string message);
+  const char * what() const noexcept;
+
+private:
+  std::string message;
+
+};
+
 /// Error report (based on Halide's Error.h)
 struct ErrorReport {
   enum Kind { User, Internal, Temporary };
 
   std::ostringstream *msg;
   const char *file;
   const char *func;
@@ -42,18 +53,18 @@
     return *this;
   }
 
   ~ErrorReport() noexcept(false) {
     if (condition) {
       return;
     }
-    explode();
+    explodeWithException();
   }
 
-  void explode();
+  void explodeWithException();
 };
 
 // internal asserts
 #ifdef TACO_ASSERTS
   #define taco_iassert(c)                                                     \
     taco::ErrorReport(__FILE__, __FUNCTION__, __LINE__, (c), #c,              \
                       taco::ErrorReport::Internal, false)
```

### Comparing `tensora-0.0.6/src/taco/include/taco/format.h` & `tensora-0.0.7/src/taco/include/taco/format.h`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #include "taco/type.h"
 
 namespace taco {
 
 class ModeFormat;
 class ModeFormatPack;
 class ModeFormatImpl;
+class AttrQuery;
+class IndexVar;
 
 
 /// A Format describes the data layout of a tensor, and the sparse index data
 /// structures that describe locations of non-zero tensor components.
 class Format {
 public:
   /// Create a format for a 0-order tensor (a scalar).
@@ -91,15 +93,16 @@
   static ModeFormat Compressed;  /// alias for compressed
   static ModeFormat Sparse;      /// alias for compressed
   static ModeFormat Singleton;   /// alias for singleton
 
   /// Properties of a mode format
   enum Property {
     FULL, NOT_FULL, ORDERED, NOT_ORDERED, UNIQUE, NOT_UNIQUE, BRANCHLESS,
-    NOT_BRANCHLESS, COMPACT, NOT_COMPACT
+    NOT_BRANCHLESS, COMPACT, NOT_COMPACT, ZEROLESS, NOT_ZEROLESS, PADDED, 
+    NOT_PADDED
   };
 
   /// Instantiates an undefined mode format
   ModeFormat();
 
   /// Instantiates a new mode format
   ModeFormat(const std::shared_ptr<ModeFormatImpl> impl);
@@ -122,22 +125,34 @@
 
   /// Returns true if a mode format has a specific property, false otherwise
   bool isFull() const;
   bool isOrdered() const;
   bool isUnique() const;
   bool isBranchless() const;
   bool isCompact() const;
+  bool isZeroless() const;
+  bool isPadded() const;
 
   /// Returns true if a mode format has a specific capability, false otherwise
   bool hasCoordValIter() const;
   bool hasCoordPosIter() const;
   bool hasLocate() const;
   bool hasInsert() const;
   bool hasAppend() const;
 
+  /// Returns true if a mode format has ungrouped insertion functions with 
+  /// specific attributes, false otherwise
+  bool hasSeqInsertEdge() const;
+  bool hasInsertCoord() const;
+  bool isYieldPosPure() const;
+
+  std::vector<AttrQuery> getAttrQueries(
+      std::vector<IndexVar> parentCoords, 
+      std::vector<IndexVar> childCoords) const;
+
   /// Returns true if mode format is defined, false otherwise. An undefined mode
   /// type can be used to indicate a mode whose format is not (yet) known.
   bool defined() const;
 
   friend bool operator==(const ModeFormat&, const ModeFormat&);
   friend bool operator!=(const ModeFormat&, const ModeFormat&);
   friend std::ostream& operator<<(std::ostream&, const ModeFormat&);
```

### Comparing `tensora-0.0.6/src/taco/include/taco/index_notation/README.md` & `tensora-0.0.7/src/taco/include/taco/index_notation/README.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_nodes_abstract.h` & `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_nodes_abstract.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_printer.h` & `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_printer.h`

 * *Files 22% similar despite different names*

```diff
@@ -21,24 +21,28 @@
   void visit(const NegNode*);
   void visit(const SqrtNode*);
   void visit(const AddNode*);
   void visit(const SubNode*);
   void visit(const MulNode*);
   void visit(const DivNode*);
   void visit(const CastNode*);
+  void visit(const CallNode*);
   void visit(const CallIntrinsicNode*);
   void visit(const ReductionNode*);
+  void visit(const IndexVarNode*);
 
   // Tensor Expressions
   void visit(const AssignmentNode*);
   void visit(const YieldNode*);
   void visit(const ForallNode*);
   void visit(const WhereNode*);
   void visit(const MultiNode*);
   void visit(const SequenceNode*);
+  void visit(const AssembleNode*);
+  void visit(const SuchThatNode*);
 
 private:
   std::ostream& os;
 
   enum class Precedence {
     ACCESS = 2,
     FUNC = 2,
```

### Comparing `tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_rewriter.h` & `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_rewriter.h`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,18 @@
   virtual void visit(const NegNode* op) = 0;
   virtual void visit(const SqrtNode* op) = 0;
   virtual void visit(const AddNode* op) = 0;
   virtual void visit(const SubNode* op) = 0;
   virtual void visit(const MulNode* op) = 0;
   virtual void visit(const DivNode* op) = 0;
   virtual void visit(const CastNode* op) = 0;
+  virtual void visit(const CallNode* op) = 0;
   virtual void visit(const CallIntrinsicNode* op) = 0;
   virtual void visit(const ReductionNode* op) = 0;
+  virtual void visit(const IndexVarNode* op) = 0;
 };
 
 
 /// Extend this class to rewrite all index statements.
 class IndexStmtRewriterStrict : public IndexStmtVisitorStrict {
 public:
   virtual ~IndexStmtRewriterStrict() {}
@@ -52,15 +54,17 @@
   using IndexStmtVisitorStrict::visit;
 
   virtual void visit(const AssignmentNode* op) = 0;
   virtual void visit(const YieldNode* op) = 0;
   virtual void visit(const ForallNode* op) = 0;
   virtual void visit(const WhereNode* op) = 0;
   virtual void visit(const SequenceNode* op) = 0;
+  virtual void visit(const AssembleNode* op) = 0;
   virtual void visit(const MultiNode* op) = 0;
+  virtual void visit(const SuchThatNode* op) = 0;
 };
 
 
 /// Extend this class to rewrite all index expressions and statements.
 class IndexNotationRewriterStrict : public IndexExprRewriterStrict,
                                     public IndexStmtRewriterStrict {
 public:
@@ -88,23 +92,27 @@
   virtual void visit(const NegNode* op);
   virtual void visit(const SqrtNode* op);
   virtual void visit(const AddNode* op);
   virtual void visit(const SubNode* op);
   virtual void visit(const MulNode* op);
   virtual void visit(const DivNode* op);
   virtual void visit(const CastNode* op);
+  virtual void visit(const CallNode* op);
   virtual void visit(const CallIntrinsicNode* op);
   virtual void visit(const ReductionNode* op);
+  virtual void visit(const IndexVarNode* op);
 
   virtual void visit(const AssignmentNode* op);
   virtual void visit(const YieldNode* op);
   virtual void visit(const ForallNode* op);
   virtual void visit(const WhereNode* op);
   virtual void visit(const SequenceNode* op);
+  virtual void visit(const AssembleNode* op);
   virtual void visit(const MultiNode* op);
+  virtual void visit(const SuchThatNode* op);
 };
 
 
 /// Rewrites the expression to replace sub-expressions with new expressions.
 IndexExpr replace(IndexExpr expr,
                   const std::map<IndexExpr,IndexExpr>& substitutions);
 
@@ -120,9 +128,13 @@
 IndexStmt replace(IndexStmt stmt,
                   const std::map<IndexStmt,IndexStmt>& substitutions);
 
 /// Rewrites the statement to replace tensor variables.
 IndexStmt replace(IndexStmt stmt,
                   const std::map<TensorVar,TensorVar>& substitutions);
 
+/// Rewrites the statement to replace an index variable with a new variable.
+IndexStmt replace(IndexStmt stmt,
+                  const std::map<IndexVar,IndexVar>& substitutions);
+
 }
 #endif
```

### Comparing `tensora-0.0.6/src/taco/include/taco/index_notation/index_notation_visitor.h` & `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_visitor.h`

 * *Files 10% similar despite different names*

```diff
@@ -16,25 +16,29 @@
 struct NegNode;
 struct AddNode;
 struct SubNode;
 struct MulNode;
 struct DivNode;
 struct SqrtNode;
 struct CastNode;
+struct CallNode;
 struct CallIntrinsicNode;
 struct UnaryExprNode;
 struct BinaryExprNode;
 struct ReductionNode;
+struct IndexVarNode;
 
 struct AssignmentNode;
 struct YieldNode;
 struct ForallNode;
 struct WhereNode;
 struct MultiNode;
 struct SequenceNode;
+struct AssembleNode;
+struct SuchThatNode;
 
 /// Visit the nodes in an expression.  This visitor provides some type safety
 /// by requing all visit methods to be overridden.
 class IndexExprVisitorStrict {
 public:
   virtual ~IndexExprVisitorStrict();
 
@@ -45,30 +49,34 @@
   virtual void visit(const NegNode*) = 0;
   virtual void visit(const AddNode*) = 0;
   virtual void visit(const SubNode*) = 0;
   virtual void visit(const MulNode*) = 0;
   virtual void visit(const DivNode*) = 0;
   virtual void visit(const SqrtNode*) = 0;
   virtual void visit(const CastNode*) = 0;
+  virtual void visit(const CallNode*) = 0;
   virtual void visit(const CallIntrinsicNode*) = 0;
   virtual void visit(const ReductionNode*) = 0;
+  virtual void visit(const IndexVarNode*) = 0;
 };
 
 class IndexStmtVisitorStrict {
 public:
   virtual ~IndexStmtVisitorStrict();
 
   void visit(const IndexStmt&);
 
   virtual void visit(const AssignmentNode*) = 0;
   virtual void visit(const YieldNode*) = 0;
   virtual void visit(const ForallNode*) = 0;
   virtual void visit(const WhereNode*) = 0;
   virtual void visit(const SequenceNode*) = 0;
+  virtual void visit(const AssembleNode*) = 0;
   virtual void visit(const MultiNode*) = 0;
+  virtual void visit(const SuchThatNode*) = 0;
 };
 
 /// Visit nodes in index notation
 class IndexNotationVisitorStrict : public IndexExprVisitorStrict,
                                    public IndexStmtVisitorStrict {
 public:
   virtual ~IndexNotationVisitorStrict();
@@ -90,26 +98,30 @@
   virtual void visit(const NegNode* node);
   virtual void visit(const AddNode* node);
   virtual void visit(const SubNode* node);
   virtual void visit(const MulNode* node);
   virtual void visit(const DivNode* node);
   virtual void visit(const SqrtNode* node);
   virtual void visit(const CastNode* node);
+  virtual void visit(const CallNode* node);
   virtual void visit(const CallIntrinsicNode* node);
   virtual void visit(const UnaryExprNode* node);
   virtual void visit(const BinaryExprNode* node);
   virtual void visit(const ReductionNode* node);
+  virtual void visit(const IndexVarNode* node);
 
   // Index Statments
   virtual void visit(const AssignmentNode* node);
   virtual void visit(const YieldNode* node);
   virtual void visit(const ForallNode* node);
   virtual void visit(const WhereNode* node);
   virtual void visit(const SequenceNode* node);
+  virtual void visit(const AssembleNode* node);
   virtual void visit(const MultiNode* node);
+  virtual void visit(const SuchThatNode* node);
 };
 
 
 #define RULE(Rule)                                                             \
 std::function<void(const Rule*)> Rule##Func;                                   \
 std::function<void(const Rule*, Matcher*)> Rule##CtxFunc;                      \
 void unpack(std::function<void(const Rule*)> pattern) {                        \
@@ -157,26 +169,30 @@
   RULE(NegNode)
   RULE(SqrtNode)
   RULE(AddNode)
   RULE(SubNode)
   RULE(MulNode)
   RULE(DivNode)
   RULE(CastNode)
+  RULE(CallNode)
   RULE(CallIntrinsicNode)
   RULE(ReductionNode)
 
   RULE(BinaryExprNode)
   RULE(UnaryExprNode)
+  RULE(IndexVarNode)
 
   RULE(AssignmentNode)
   RULE(YieldNode)
   RULE(ForallNode)
   RULE(WhereNode)
   RULE(MultiNode)
   RULE(SequenceNode)
+  RULE(AssembleNode)
+  RULE(SuchThatNode)
 };
 
 /**
   Match patterns to the IR.  Use lambda closures to capture environment
   variables (e.g. [&]):
 
   For example, to print all AddNode and SubNode objects in func:
```

### Comparing `tensora-0.0.6/src/taco/include/taco/index_notation/intrinsic.h` & `tensora-0.0.7/src/taco/include/taco/index_notation/intrinsic.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/index_notation/kernel.h` & `tensora-0.0.7/src/taco/include/taco/index_notation/kernel.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/index_notation/schedule.h` & `tensora-0.0.7/src/taco/include/taco/index_notation/schedule.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/ir/ir.h` & `tensora-0.0.7/src/taco/include/taco/ir/ir.h`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 #include "taco/type.h"
 #include "taco/error.h"
 #include "taco/util/intrusive_ptr.h"
 #include "taco/util/uncopyable.h"
 #include "taco/storage/typed_value.h"
 #include <cstring>
+#include "taco/ir_tags.h"
 
 namespace taco {
 namespace ir {
 
 class IRVisitorStrict;
 
 /** All IR nodes get unique IDs for RTTI */
@@ -37,14 +38,15 @@
   Neq,
   Gt,
   Lt,
   Gte,
   Lte,
   And,
   Or,
+  BinOp,
   Cast,
   Call,
   IfThenElse,
   Case,
   Switch,
   Load,
   Malloc,
@@ -59,25 +61,29 @@
   VarAssign,
   Yield,
   Allocate,
   Free,
   Comment,
   BlankLine,
   Print,
-  GetProperty
+  GetProperty,
+  Continue,
+  Sort,
+  Break
 };
 
 enum class TensorProperty {
   Order,
   Dimension,
   ComponentSize,
   ModeOrdering,
   ModeTypes,
   Indices,
   Values,
+  FillValue,
   ValuesSize
 };
 
 /** Base class for backend IR */
 struct IRNode : private util::Uncopyable {
   IRNode() {}
   virtual ~IRNode() {}
@@ -227,14 +233,22 @@
 
   template <typename T>
   T getValue() const {
     taco_iassert(taco::type<T>() == type);
     return *static_cast<const T*>(value.get());
   }
 
+  Expr promote(Datatype dt) const {
+    taco_iassert(max_type(dt, type) == dt);
+    if(type == dt) {
+      return Literal::make(getTypedVal(), dt);
+    }
+    return Expr();
+  }
+
   TypedComponentVal getTypedVal() const {
     return *value;
   }
 
   bool getBoolValue() const;
   int64_t getIntValue() const;
   uint64_t getUIntValue() const;
@@ -248,17 +262,18 @@
 
 
 /** A variable.  */
 struct Var : public ExprNode<Var> {
   std::string name;
   bool is_ptr;
   bool is_tensor;
+  bool is_parameter; 
 
   static Expr make(std::string name, Datatype type, bool is_ptr=false, 
-                   bool is_tensor=false);
+                   bool is_tensor=false, bool is_parameter=false);
 
   static const IRNodeType _type_info = IRNodeType::Var;
 };
 
 
 /** Negation */
 struct Neg : public ExprNode<Neg> {
@@ -343,19 +358,20 @@
   static Expr make(std::vector<Expr> operands, Datatype type);
 
   static const IRNodeType _type_info = IRNodeType::Min;
 };
 
 /** Maximum of two values. */
 struct Max : public ExprNode<Max> {
-  Expr a;
-  Expr b;
+  std::vector<Expr> operands;
 
   static Expr make(Expr a, Expr b);
   static Expr make(Expr a, Expr b, Datatype type);
+  static Expr make(std::vector<Expr> operands);
+  static Expr make(std::vector<Expr> operands, Datatype type);
 
   static const IRNodeType _type_info = IRNodeType::Max;
 };
 
 /** Bitwise and: a & b */
 struct BitAnd : public ExprNode<BitAnd> {
   Expr a;
@@ -453,14 +469,28 @@
   Expr b;
 
   static Expr make(Expr a, Expr b);
 
   static const IRNodeType _type_info = IRNodeType::Or;
 };
 
+/** [Sparse Array Programming] Generic Binary Op for Ufuncs**/
+struct BinOp : public ExprNode<BinOp> {
+  Expr a;
+  Expr b;
+  std::string strStart = "";
+  std::string strMid = "";
+  std::string strEnd = "";
+
+  static Expr make(Expr a, Expr b, std::string op);
+  static Expr make(Expr a, Expr b, std::string strStart, std::string strMid, std::string strEnd);
+
+  static const IRNodeType _type_info = IRNodeType::BinOp;
+};
+
 /** Type cast. */
 struct Cast : public ExprNode<Cast> {
   Expr a;
 
   static Expr make(Expr a, Datatype newType);
 
   static const IRNodeType _type_info = IRNodeType::Cast;
@@ -541,16 +571,18 @@
 };
 
 /** A store to an array location: arr[loc] = data */
 struct Store : public StmtNode<Store> {
   Expr arr;
   Expr loc;
   Expr data;
+  bool use_atomics;
+  ParallelUnit atomic_parallel_unit;
 
-  static Stmt make(Expr arr, Expr loc, Expr data);
+  static Stmt make(Expr arr, Expr loc, Expr data, bool use_atomics=false, ParallelUnit atomic_parallel_unit=ParallelUnit::NotParallel);
 
   static const IRNodeType _type_info = IRNodeType::Store;
 };
 
 /** A conditional statement. */
 struct IfThenElse : public StmtNode<IfThenElse> {
   Expr cond;
@@ -579,15 +611,15 @@
   Expr controlExpr;
   
   static Stmt make(std::vector<std::pair<Expr,Stmt>> cases, Expr controlExpr);
   
   static const IRNodeType _type_info = IRNodeType::Switch;
 };
 
-enum class LoopKind {Serial, Static, Dynamic, Runtime, Vectorized};
+enum class LoopKind {Serial, Static, Dynamic, Runtime, Vectorized, Static_Chunked};
 
 /** A for loop from start to end by increment.
  * A vectorized loop will require the increment to be 1 and the
  * end to be (start + Literal) or possibly (start + Var).
  *
  * If the loop is vectorized, the width says which vector width
  * to use.  By default (0), it will not set a specific width and
@@ -597,19 +629,20 @@
   Expr var;
   Expr start;
   Expr end;
   Expr increment;
   Stmt contents;
   LoopKind kind;
   int vec_width;  // vectorization width
-  bool accelerator;
+  ParallelUnit parallel_unit;
+  size_t unrollFactor;
   
   static Stmt make(Expr var, Expr start, Expr end, Expr increment,
                    Stmt contents, LoopKind kind=LoopKind::Serial,
-                   bool accelerator=false, int vec_width=0);
+                   ParallelUnit parallel_unit=ParallelUnit::NotParallel, size_t unrollFactor=0, int vec_width=0);
   
   static const IRNodeType _type_info = IRNodeType::For;
 };
 
 /** A while loop.  We prefer For loops when possible, but
  * these are necessary for merging.
  */
@@ -651,16 +684,18 @@
   static const IRNodeType _type_info = IRNodeType::VarDecl;
 };
 
 /** Assigning a Var to an expression */
 struct Assign : public StmtNode<Assign> {
   Expr lhs;
   Expr rhs;
+  bool use_atomics;
+  ParallelUnit atomic_parallel_unit;
   
-  static Stmt make(Expr lhs, Expr rhs);
+  static Stmt make(Expr lhs, Expr rhs, bool use_atomics=false, ParallelUnit atomic_parallel_unit=ParallelUnit::NotParallel);
   
   static const IRNodeType _type_info = IRNodeType::VarAssign;
 };
 
 /** Yield a result component */
 struct Yield : public StmtNode<Yield> {
   std::vector<Expr> coords;
@@ -673,17 +708,18 @@
 
 /** Allocate memory for a ptr var */
 struct Allocate : public StmtNode<Allocate> {
   Expr var;
   Expr num_elements;
   Expr old_elements; // used for realloc in CUDA
   bool is_realloc;
+  bool clear; // Whether to use calloc to allocate this memory.
   
   static Stmt make(Expr var, Expr num_elements, bool is_realloc=false,
-                   Expr old_elements=Expr());
+                   Expr old_elements=Expr(), bool clear=false);
   
   static const IRNodeType _type_info = IRNodeType::Allocate;
 };
 
 /** Free memory for a ptr var */
 struct Free : public StmtNode<Free> {
   Expr var;
@@ -705,14 +741,35 @@
 /** A blank statement (no-op) */
 struct BlankLine : public StmtNode<BlankLine> {
   static Stmt make();
 
   static const IRNodeType _type_info = IRNodeType::BlankLine;
 };
 
+/** Continues past current iteration of current loop */
+struct Continue : public StmtNode<Continue> {
+  static Stmt make();
+
+  static const IRNodeType _type_info = IRNodeType::Continue;
+};
+
+/** Breaks out of the current loop */
+struct Break : public StmtNode<Break> {
+  static Stmt make();
+
+  static const IRNodeType _type_info = IRNodeType::Break;
+};
+
+struct Sort : public StmtNode<Sort> {
+  std::vector<Expr> args;
+  static Stmt make(std::vector<Expr> args);
+
+  static const IRNodeType _type_info = IRNodeType::Sort;
+};
+
 /** A print statement.
  * Takes in a printf-style format string and Exprs to pass
  * for the values.
  */
 struct Print : public StmtNode<Print> {
   std::string fmt;
   std::vector<Expr> params;
```

### Comparing `tensora-0.0.6/src/taco/include/taco/ir/ir_printer.h` & `tensora-0.0.7/src/taco/include/taco/ir/ir_printer.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #ifndef TACO_IR_PRINTER_H
 #define TACO_IR_PRINTER_H
 
 #include <ostream>
 #include <map>
 #include <string>
+#include "taco/ir/ir.h"
 #include "taco/ir/ir_visitor.h"
 #include "taco/util/scopedmap.h"
 #include "taco/util/name_generator.h"
 
 namespace taco {
 namespace ir {
 
@@ -39,14 +40,15 @@
   virtual void visit(const Neq*);
   virtual void visit(const Gt*);
   virtual void visit(const Lt*);
   virtual void visit(const Gte*);
   virtual void visit(const Lte*);
   virtual void visit(const And*);
   virtual void visit(const Or*);
+  virtual void visit(const BinOp*);
   virtual void visit(const Cast*);
   virtual void visit(const Call*);
   virtual void visit(const IfThenElse*);
   virtual void visit(const Case*);
   virtual void visit(const Switch*);
   virtual void visit(const Load*);
   virtual void visit(const Malloc*);
@@ -60,16 +62,19 @@
   virtual void visit(const VarDecl*);
   virtual void visit(const Assign*);
   virtual void visit(const Yield*);
   virtual void visit(const Allocate*);
   virtual void visit(const Free*);
   virtual void visit(const Comment*);
   virtual void visit(const BlankLine*);
+  virtual void visit(const Continue*);
   virtual void visit(const Print*);
   virtual void visit(const GetProperty*);
+  virtual void visit(const Sort*);
+  virtual void visit(const Break*);
 
   std::ostream &stream;
   int indent;
   bool color;
   bool simplify;
 
   enum Precedence {
@@ -100,14 +105,15 @@
   util::NameGenerator varNameGenerator;
   util::ScopedMap<Expr, std::string> varNames;
 
   void resetNameCounters();
 
   void doIndent();
   void printBinOp(Expr a, Expr b, std::string op, Precedence precedence);
+  bool needsParentheses(Precedence precedence);
 
   std::string keywordString(std::string);
   std::string commentString(std::string);
 };
 
 }
 }
```

### Comparing `tensora-0.0.6/src/taco/include/taco/ir/ir_rewriter.h` & `tensora-0.0.7/src/taco/include/taco/ir/ir_rewriter.h`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
   virtual void visit(const Neq* op);
   virtual void visit(const Gt* op);
   virtual void visit(const Lt* op);
   virtual void visit(const Gte* op);
   virtual void visit(const Lte* op);
   virtual void visit(const And* op);
   virtual void visit(const Or* op);
+  virtual void visit(const BinOp* op);
   virtual void visit(const Cast* op);
   virtual void visit(const Call* op);
   virtual void visit(const IfThenElse* op);
   virtual void visit(const Case* op);
   virtual void visit(const Switch* op);
   virtual void visit(const Load* op);
   virtual void visit(const Malloc* op);
@@ -61,13 +62,16 @@
   virtual void visit(const VarDecl* op);
   virtual void visit(const Assign* op);
   virtual void visit(const Yield* op);
   virtual void visit(const Allocate* op);
   virtual void visit(const Free* op);
   virtual void visit(const Comment* op);
   virtual void visit(const BlankLine* op);
+  virtual void visit(const Continue* op);
   virtual void visit(const Print* op);
   virtual void visit(const GetProperty* op);
+  virtual void visit(const Sort *op);
+  virtual void visit(const Break *op);
 };
 
 }}
 #endif
```

### Comparing `tensora-0.0.6/src/taco/include/taco/ir/ir_visitor.h` & `tensora-0.0.7/src/taco/include/taco/ir/ir_visitor.h`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 struct Neq;
 struct Gt;
 struct Lt;
 struct Gte;
 struct Lte;
 struct And;
 struct Or;
+struct BinOp;
 struct Cast;
 struct Call;
 struct IfThenElse;
 struct Case;
 struct Switch;
 struct Load;
 struct Malloc;
@@ -41,16 +42,19 @@
 struct VarDecl;
 struct Assign;
 struct Yield;
 struct Allocate;
 struct Free;
 struct Comment;
 struct BlankLine;
+struct Continue;
 struct Print;
 struct GetProperty;
+struct Sort;
+struct Break;
 
 /// Extend this class to visit every node in the IR.
 class IRVisitorStrict {
 public:
   virtual ~IRVisitorStrict();
   virtual void visit(const Literal*) = 0;
   virtual void visit(const Var*) = 0;
@@ -69,14 +73,15 @@
   virtual void visit(const Neq*) = 0;
   virtual void visit(const Gt*) = 0;
   virtual void visit(const Lt*) = 0;
   virtual void visit(const Gte*) = 0;
   virtual void visit(const Lte*) = 0;
   virtual void visit(const And*) = 0;
   virtual void visit(const Or*) = 0;
+  virtual void visit(const BinOp*) = 0;
   virtual void visit(const Cast*) = 0;
   virtual void visit(const Call*) = 0;
   virtual void visit(const IfThenElse*) = 0;
   virtual void visit(const Case*) = 0;
   virtual void visit(const Switch*) = 0;
   virtual void visit(const Load*) = 0;
   virtual void visit(const Malloc*) = 0;
@@ -90,16 +95,19 @@
   virtual void visit(const VarDecl*) = 0;
   virtual void visit(const Assign*) = 0;
   virtual void visit(const Yield*) = 0;
   virtual void visit(const Allocate*) = 0;
   virtual void visit(const Free*) = 0;
   virtual void visit(const Comment*) = 0;
   virtual void visit(const BlankLine*) = 0;
+  virtual void visit(const Continue*) = 0;
   virtual void visit(const Print*) = 0;
   virtual void visit(const GetProperty*) = 0;
+  virtual void visit(const Sort*) = 0;
+  virtual void visit(const Break*) = 0;
 };
 
 
 /// Extend this class to visit some nodes in the IR.
 class IRVisitor : public IRVisitorStrict {
 public:
   virtual ~IRVisitor();
@@ -121,14 +129,15 @@
   virtual void visit(const Neq* op);
   virtual void visit(const Gt* op);
   virtual void visit(const Lt* op);
   virtual void visit(const Gte* op);
   virtual void visit(const Lte* op);
   virtual void visit(const And* op);
   virtual void visit(const Or* op);
+  virtual void visit(const BinOp* op);
   virtual void visit(const Cast* op);
   virtual void visit(const Call* op);
   virtual void visit(const IfThenElse* op);
   virtual void visit(const Case* op);
   virtual void visit(const Switch* op);
   virtual void visit(const Load* op);
   virtual void visit(const Malloc* op);
@@ -142,13 +151,16 @@
   virtual void visit(const VarDecl* op);
   virtual void visit(const Assign* op);
   virtual void visit(const Yield* op);
   virtual void visit(const Allocate* op);
   virtual void visit(const Free* op);
   virtual void visit(const Comment* op);
   virtual void visit(const BlankLine* op);
+  virtual void visit(const Continue* op);
   virtual void visit(const Print* op);
   virtual void visit(const GetProperty* op);
+  virtual void visit(const Sort* op);
+  virtual void visit(const Break* op);
 };
 
 }}
 #endif
```

### Comparing `tensora-0.0.6/src/taco/include/taco/lower/iterator.h` & `tensora-0.0.7/src/taco/include/taco/lower/iterator.h`

 * *Files 22% similar despite different names*

```diff
@@ -6,22 +6,27 @@
 #include <string>
 #include <tuple>
 #include <vector>
 #include <map>
 
 #include "taco/ir/ir.h"
 #include "taco/util/comparable.h"
-#include "lower/tensor_path.h"
-#include "taco/lower/mode_format_impl.h"
 
 namespace taco {
 class Type;
 class ModeAccess;
 class IndexStmt;
 class IndexVar;
+class ProvenanceGraph;
+class TensorVar;
+class Access;
+class ModeFunction;
+class Mode;
+class Format;
+class AttrQueryResult;
 
 namespace ir {
 class Stmt;
 class Expr;
 }
 
 
@@ -29,56 +34,62 @@
 /// to generate the IR expressions for accessing different level types.
 class Iterator : public util::Comparable<Iterator> {
 public:
   /// Construct an undefind iterator.
   Iterator();
 
   /// Construct a dimension iterator.
-  Iterator(IndexVar indexVar);
+  Iterator(IndexVar indexVar, bool isFull=true);
 
   /// Construct a root iterator.
   Iterator(ir::Expr tensorVar);
 
   /// Construct a non-root iterator.
   Iterator(IndexVar indexVar, ir::Expr tensor, Mode mode, Iterator parent,
-           std::string name);
+           std::string name, bool useNameForPos=true);
 
   /// Returns true if the iterator is a root iterator.
   bool isRoot() const;
 
   /// Returns true if the iterator iterates over the bottommost level.
   bool isLeaf() const;
 
   /// Get the parent of this iterator in its iterator list.
   const Iterator& getParent() const;
 
   /// Get the child of this iterator in its iterator list.
   const Iterator getChild() const;
 
-
   /// Returns true if the iterator iterates over the dimension.
   bool isDimensionIterator() const;
 
   /// Returns true if the iterator iterates over a mode.
   bool isModeIterator() const;
 
   /// Properties of level being iterated.
   bool isFull() const;
   bool isOrdered() const;
   bool isUnique() const;
   bool isBranchless() const;
   bool isCompact() const;
+  bool isZeroless() const;
 
   /// Capabilities supported by levels being iterated.
   bool hasCoordIter() const;
   bool hasPosIter() const;
   bool hasLocate() const;
   bool hasInsert() const;
   bool hasAppend() const;
 
+  /// Attributes of ungrouped insertion level functions.
+  bool hasSeqInsertEdge() const;
+  bool hasInsertCoord() const;
+  bool isYieldPosPure() const;
+
+
   /// Get the index variable this iterator iteratores over.
   IndexVar getIndexVar() const;
 
   /// Returns the tensor this iterator is iterating over.
   ir::Expr getTensor() const;
 
   /// Returns he tensor mode being iterated over, or undefined if the iterator
@@ -115,15 +126,16 @@
   ir::Expr getValidVar() const;
 
   /// Returns the variable that indicates the starting bound for positions of 
   /// coordinates appended to a level belonging to the same subtensor.
   ir::Expr getBeginVar() const;
 
 
-  /// Return code for level functions that implement coordinate value iteration.
+  ModeFunction coordBounds(const ir::Expr& parentPos) const;
+    /// Return code for level functions that implement coordinate value iteration.
   ModeFunction coordBounds(const std::vector<ir::Expr>& parentCoords) const;
   ModeFunction coordAccess(const std::vector<ir::Expr>& coords) const;
   
   /// Return code for level functions that implement coordinate position  
   /// iteration.
   ModeFunction posBounds(const ir::Expr& parentPos) const;
   ModeFunction posAccess(const ir::Expr& pos, 
@@ -149,27 +161,84 @@
   ir::Expr getSize(const ir::Expr& szPrev) const;
   ir::Stmt getAppendInitEdges(const ir::Expr& pPrevBegin, 
       const ir::Expr& pPrevEnd) const;
   ir::Stmt getAppendInitLevel(const ir::Expr& szPrev, const ir::Expr& sz) const;
   ir::Stmt getAppendFinalizeLevel(const ir::Expr& szPrev, 
       const ir::Expr& sz) const;
 
+  /// Return code for level functions that implement ungrouped insert 
+  /// capabilitiy.
+  ir::Expr getAssembledSize(const ir::Expr& prevSize) const;
+  ir::Stmt getSeqInitEdges(const ir::Expr& prevSize, 
+      const std::vector<AttrQueryResult>& queries) const;
+  ir::Stmt getSeqInsertEdge(const ir::Expr& parentPos, 
+      const std::vector<ir::Expr>& coords, 
+      const std::vector<AttrQueryResult>& queries) const;
+  ir::Stmt getInitCoords(const ir::Expr& prevSize, 
+      const std::vector<AttrQueryResult>& queries) const;
+  ir::Stmt getInitYieldPos(const ir::Expr& prevSize) const;
+  ModeFunction getYieldPos(const ir::Expr& parentPos, 
+      const std::vector<ir::Expr>& coords) const;
+  ir::Stmt getInsertCoord(const ir::Expr& parentPos, const ir::Expr& pos, 
+      const std::vector<ir::Expr>& coords) const;
+  ir::Stmt getFinalizeYieldPos(const ir::Expr& prevSize) const;
+
   /// Returns true if the iterator is defined, false otherwise.
   bool defined() const;
 
+  /// Methods for querying and operating on windowed tensor modes.
+
+  /// isWindowed returns true if this iterator is operating over a window
+  /// of a tensor mode.
+  bool isWindowed() const;
+
+  /// isStrided returns true if this iterator has a stride != 1. Currently
+  /// only windowed iterators can have strides.
+  bool isStrided() const;
+
+  /// getWindow{Lower,Upper}Bound return the {Lower,Upper} bound of the
+  /// window that this iterator operates over.
+  ir::Expr getWindowLowerBound() const;
+  ir::Expr getWindowUpperBound() const;
+
+  /// getStride returns an Expr holding the stride that this iterator is
+  /// configured with.
+  ir::Expr getStride() const;
+
+  /// getWindowVar returns a Var specific to thw window that this iterator
+  /// is operating over. It can be used as temporary storage.
+  ir::Expr getWindowVar() const;
+
+  /// Methods for querying and operating on tensor modes projected by an index set.
+
+  /// hasIndexSet returns true if this iterator is operating over an index set.
+  bool hasIndexSet() const;
+
+  /// getIndexSetIterator returns the iterator that corresponds to the tensor
+  /// backing the index set.
+  Iterator getIndexSetIterator() const;
+
   friend bool operator==(const Iterator&, const Iterator&);
   friend bool operator<(const Iterator&, const Iterator&);
   friend std::ostream& operator<<(std::ostream&, const Iterator&);
 
 private:
   struct Content;
   std::shared_ptr<Content> content;
 
   Iterator(std::shared_ptr<Content> content);
   void setChild(const Iterator& iterator) const;
+
+  friend class Iterators;
+
+  /// setWindowBounds sets the window bounds of this iterator.
+  void setWindowBounds(ir::Expr lo, ir::Expr hi, ir::Expr stride);
+
+  /// setIndexSetIterator sets the index set iterator of this iterator.
+  void setIndexSetIterator(Iterator iter);
 };
 
 /**
  * A set of iterators divided into tensor iterators and dimension iterators.
  * Tensor iterators, one iterator chain per tensor access, iterate over tensor
  * coordinate hierarchies and mode iterators iterate over tensor modes.
  */
@@ -191,27 +260,32 @@
 
   /**
    * Retrieve the coordinate hierarchy level iterator corresponding to the
    * given mode access.
    */
   Iterator levelIterator(ModeAccess) const;
 
+  std::map<ModeAccess,Iterator> levelIterators() const;
+
   /**
    * Retrieve the mode access corresponding to the given coordinate hierarchy
    * level iterator.
    */
   ModeAccess modeAccess(Iterator) const;
 
   /**
    * Retrieve the mode iterator corresponding to the given index variable.
    */
   Iterator modeIterator(IndexVar) const;
 
+  std::map<IndexVar, Iterator> modeIterators() const;
+
 private:
-  void createAccessIterators(Access access, Format format, ir::Expr tensorIR);
+  void createAccessIterators(Access access, Format format, ir::Expr tensorIR, ProvenanceGraph provGraph,
+                             const std::map<TensorVar, ir::Expr> &tensorVars);
 
   struct Content;
   std::shared_ptr<Content> content;
 };
 
 /// Filter out and return the iterators with the append capability.
 std::vector<Iterator> getAppenders(const std::vector<Iterator>& iterators);
```

### Comparing `tensora-0.0.6/src/taco/include/taco/lower/lower.h` & `tensora-0.0.7/src/taco/include/taco/lower/lower.h`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 /// Lower a concrete index notation statement to a function in the low-level
 /// imperative IR.  You may specify whether the lowered function should
 /// assemble result indices, compute result values, or both. You may optionally
 /// also provide a custom `Lowerer` to specify custom ways to lower some or all
 /// parts of a concrete index notation statement.
 ir::Stmt lower(IndexStmt stmt, std::string functionName,
-               bool assemble=true, bool compute=true,
+               bool assemble=true, bool compute=true, bool pack=false, bool unpack=false,
                Lowerer lowerer=Lowerer());
 
 /// Check whether the an index statement can be lowered to C code.  If the
 /// statement cannot be lowered and a `reason` string is provided then it is
 /// filled with the a reason.
 bool isLowerable(IndexStmt stmt, std::string* reason=nullptr);
```

### Comparing `tensora-0.0.6/src/taco/include/taco/lower/merge_lattice.h` & `tensora-0.0.7/src/taco/include/taco/lower/merge_lattice.h`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #define TACO_MERGE_LATTICE_H
 
 #include <vector>
 #include <set>
 #include <map>
 #include <ostream>
 #include <memory>
+#include "taco/index_notation/index_notation.h"
 
 namespace taco {
 
 class Iterator;
 class Iterators;
 class Forall;
 class ModeAccess;
@@ -28,16 +29,45 @@
    *
    * \param forall
    *      A forall concrete index notation statement to construct a lattice for.
    *
    * \param iterators
    *      Iterators that iterate over the tensor coordinate hierarchies of every
    *      access expression and that iterate over tensor modes.
+   *
+   * \param provGraph
+   *      Tracks relationships between index variables in concrete notation
+   *
+   * \param definedIndexVars
+   *      The set of index variables that appear in enclosing loops and therefore have
+   *      a concrete value within the context of this merge lattice
+   *
+   * \param whereTempsToResult
+   *      Maps between temporary tensors and where their result will be stored necessary for when
+   *      we use scalar temporaries inside of a loop (to reduce the number of atomic instructions for example),
+   *      but we still need to know what the result location for this temporary is so that it can be properly coiterated
    */
-  static MergeLattice make(Forall forall, Iterators iterators);
+  static MergeLattice make(Forall forall, Iterators iterators, ProvenanceGraph provGraph,
+          std::set<IndexVar> definedIndexVars, std::map<TensorVar, const AccessNode *> whereTempsToResult = {});
+
+
+  /**
+   * Removes lattice points whose iterators are identical to the iterators of an earlier point, since we have
+   * already iterated over this sub-space.
+   */
+  static std::vector<MergePoint> removePointsWithIdenticalIterators(const std::vector<MergePoint>&);
+
+  /**
+   * remove lattice points that lack any of the full iterators of the first point, since when a full iterator exhausts
+   * we have iterated over the whole space.
+   */
+  static std::vector<MergePoint> removePointsThatLackFullIterators(const std::vector<MergePoint>&);
+
+  /// Returns true if we need to emit checks for explicit zeros in the lattice given.
+  bool needExplicitZeroChecks();
 
   /**
    * Returns the sub-lattice rooted at the given merge point.
    */
   MergeLattice subLattice(MergePoint lp) const;
 
   /**
@@ -47,14 +77,19 @@
 
   /**
    * Retrieve all the iterators merged by this lattice.
    */
   const std::vector<Iterator>& iterators() const;
 
   /**
+ * Retrieve all the locators in this lattice.
+ */
+  const std::vector<Iterator>& locators() const;
+
+  /**
    * Returns iterators that have been exhausted prior to the merge point.
    */
   std::set<Iterator> exhausted(MergePoint point);
 
   /**
    * Retrieve all the results written to in this merge lattice.
    */
@@ -62,24 +97,50 @@
 
   /**
    * True if the merge lattice enumerates the iteration space exactly, meaning
    * no point in the space will be considered and discarded.
    */
   bool exact() const;
 
+  /**
+   * True if any of the mode iterators in the lattice is a leaf iterator.
+   *
+   * This method checks both the iterators and locators since they both contain mode iterators.
+   */
+  bool anyModeIteratorIsLeaf() const;
+
+  /**
+   * Get a list of iterators that should be omitted at this merge point.
+   */
+  std::vector<Iterator> retrieveRegionIteratorsToOmit(const MergePoint& point) const;
+
+  /**
+   * Returns a set of sets of tensor iterators. A merge point with a tensorRegion in this set should not
+   * be removed from the lattice.
+   *
+   * Needed so that special regions are kept when applying optimizations that remove merge points.
+   */
+   std::set<std::set<Iterator>> getTensorRegionsToKeep() const;
+
+  /**
+    * Removes points from the lattice that would duplicate iteration over the input tensors.
+    */
+  MergeLattice getLoopLattice() const;
+
 private:
   std::vector<MergePoint> points_;
+  std::set<std::set<Iterator>> regionsToKeep;
 
 public:
   /**
    * Construct a merge lattice containing the given points.  This constructor
    * is primarily intended for testing purposes and most construction should
    * happen through `MergeLattice::make`.
    */
-  MergeLattice(std::vector<MergePoint> points);
+  MergeLattice(std::vector<MergePoint> points, std::set<std::set<Iterator>> regionsToKeep = {});
 };
 
 std::ostream& operator<<(std::ostream&, const MergeLattice&);
 bool operator==(const MergeLattice&, const MergeLattice&);
 bool operator!=(const MergeLattice&, const MergeLattice&);
 
 
@@ -128,27 +189,38 @@
   const std::vector<Iterator>& locators() const;
 
   /**
    * Retrieve the iterators of the results to be appended to or inserted into.
    */
   const std::vector<Iterator>& results() const;
 
+  /**
+   * Returns the iterators that iterate over or locate into tensors
+   */
+  const std::set<Iterator> tensorRegion() const;
+
+  /**
+   * Returns true if this merge point may leave out the tensors it iterates
+   */
+   bool isOmitter() const;
+
 private:
   struct Content;
   std::shared_ptr<Content> content_;
 
 public:
   /**
    * Construct a merge point.  This constructor is primarily intended for
    * testing purposes and most construction should happen through
    * `MergeLattice::make`.
    */
   MergePoint(const std::vector<Iterator>& iterators,
              const std::vector<Iterator>& locators,
-             const std::vector<Iterator>& results);
+             const std::vector<Iterator>& results,
+             bool omitPoint = false);
 };
 
 std::ostream& operator<<(std::ostream&, const MergePoint&);
 bool operator==(const MergePoint&, const MergePoint&);
 bool operator!=(const MergePoint&, const MergePoint&);
 
 /**
```

### Comparing `tensora-0.0.6/src/taco/include/taco/lower/mode.h` & `tensora-0.0.7/src/taco/include/taco/lower/mode.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/lower/mode_format_compressed.h` & `tensora-0.0.7/src/taco/include/taco/lower/mode_format_singleton.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,58 @@
-#ifndef TACO_MODE_FORMAT_COMPRESSED_H
-#define TACO_MODE_FORMAT_COMPRESSED_H
+#ifndef TACO_MODE_FORMAT_SINGLETON_H
+#define TACO_MODE_FORMAT_SINGLETON_H
 
 #include "taco/lower/mode_format_impl.h"
 
 namespace taco {
 
-class CompressedModeFormat : public ModeFormatImpl {
+class SingletonModeFormat : public ModeFormatImpl {
 public:
-  CompressedModeFormat();
-  CompressedModeFormat(bool isFull, bool isOrdered,
-                       bool isUnique, long long allocSize = DEFAULT_ALLOC_SIZE);
+  using ModeFormatImpl::getInsertCoord;
 
-  virtual ~CompressedModeFormat() {}
+  SingletonModeFormat();
+  SingletonModeFormat(bool isFull, bool isOrdered, bool isUnique, 
+                      bool isZeroless, bool isPadded, 
+		      long long allocSize = DEFAULT_ALLOC_SIZE);
 
-  virtual ModeFormat copy(std::vector<ModeFormat::Property> properties) const;
-  
-  virtual ModeFunction posIterBounds(ir::Expr parentPos, Mode mode) const;
-  virtual ModeFunction posIterAccess(ir::Expr pos, std::vector<ir::Expr> coords,
-                                     Mode mode) const;
+  ~SingletonModeFormat() override {}
+
+  ModeFormat copy(std::vector<ModeFormat::Property> properties) const override;
+
+  ModeFunction posIterBounds(ir::Expr parentPos, Mode mode) const override;
+  ModeFunction posIterAccess(ir::Expr pos, std::vector<ir::Expr> coords,
+                             Mode mode) const override;
   
-  virtual ir::Stmt getAppendCoord(ir::Expr pos, ir::Expr coord, 
-                                  Mode mode) const; 
-  virtual ir::Stmt getAppendEdges(ir::Expr parentPos, ir::Expr posBegin, 
-                                  ir::Expr posEnd, Mode mode) const;
-  virtual ir::Expr getSize(ir::Expr parentSize, Mode mode) const;
-  virtual ir::Stmt getAppendInitEdges(ir::Expr parentPosBegin, 
-                                      ir::Expr parentPosEnd, Mode mode) const;
-  virtual ir::Stmt getAppendInitLevel(ir::Expr parentSize, ir::Expr size, 
-                                      Mode mode) const;
-  virtual ir::Stmt getAppendFinalizeLevel(ir::Expr parentSize, ir::Expr size, 
-                                          Mode mode) const;
+  ir::Stmt getAppendCoord(ir::Expr pos, ir::Expr coord, 
+                          Mode mode) const override; 
+  ir::Expr getSize(ir::Expr parentSize, Mode mode) const override;
+  ir::Stmt getAppendInitLevel(ir::Expr parentSize, ir::Expr size, 
+                              Mode mode) const override;
+  ir::Stmt getAppendFinalizeLevel(ir::Expr parentSize, ir::Expr size, 
+                                  Mode mode) const override;
+
+  ir::Expr getAssembledSize(ir::Expr prevSize, Mode mode) const override;
+  ir::Stmt getInitCoords(ir::Expr prevSize, 
+                         std::vector<AttrQueryResult> queries, 
+                         Mode mode) const override;
+  ModeFunction getYieldPos(ir::Expr parentPos, std::vector<ir::Expr> coords, 
+                           Mode mode) const override;
+  ir::Stmt getInsertCoord(ir::Expr parentPos, ir::Expr pos, 
+                          std::vector<ir::Expr> coords, 
+                          Mode mode) const override;
 
-  virtual std::vector<ir::Expr> getArrays(ir::Expr tensor, int mode, 
-                                          int level) const;
+  std::vector<ir::Expr> getArrays(ir::Expr tensor, int mode, 
+                                  int level) const override;
 
 protected:
-  ir::Expr getPosArray(ModePack pack) const;
   ir::Expr getCoordArray(ModePack pack) const;
 
-  ir::Expr getPosCapacity(Mode mode) const;
   ir::Expr getCoordCapacity(Mode mode) const;
 
+  bool equals(const ModeFormatImpl& other) const override;
+
   const long long allocSize;
 };
 
 }
 
 #endif
```

### Comparing `tensora-0.0.6/src/taco/include/taco/lower/mode_format_dense.h` & `tensora-0.0.7/src/taco/include/taco/lower/mode_format_dense.h`

 * *Files 22% similar despite different names*

```diff
@@ -3,36 +3,42 @@
 
 #include "taco/lower/mode_format_impl.h"
 
 namespace taco {
 
 class DenseModeFormat : public ModeFormatImpl {
 public:
+  using ModeFormatImpl::getInsertCoord;
+
   DenseModeFormat();
-  DenseModeFormat(const bool isOrdered, const bool isUnique);
+  DenseModeFormat(const bool isOrdered, const bool isUnique, const bool isZeroless);
 
-  virtual ~DenseModeFormat() {}
+  ~DenseModeFormat() override {}
 
-  virtual ModeFormat copy(std::vector<ModeFormat::Property> properties) const;
+  ModeFormat copy(std::vector<ModeFormat::Property> properties) const override;
   
-  virtual ModeFunction locate(ir::Expr parentPos, std::vector<ir::Expr> coords,
-                              Mode mode) const;
+  ModeFunction locate(ir::Expr parentPos, std::vector<ir::Expr> coords,
+                      Mode mode) const override;
 
-  virtual ir::Stmt getInsertCoord(ir::Expr p, const std::vector<ir::Expr>& i, 
-                                  Mode mode) const;
-  virtual ir::Expr getWidth(Mode mode) const;
-  virtual ir::Stmt getInsertInitCoords(ir::Expr pBegin, ir::Expr pEnd, 
-                                       Mode mode) const;
-  virtual ir::Stmt getInsertInitLevel(ir::Expr szPrev, ir::Expr sz, 
-                                      Mode mode) const;
-  virtual ir::Stmt getInsertFinalizeLevel(ir::Expr szPrev, ir::Expr sz, 
-                                          Mode mode) const;
+  ir::Stmt getInsertCoord(ir::Expr p, const std::vector<ir::Expr>& i, 
+                          Mode mode) const override;
+  ir::Expr getWidth(Mode mode) const override;
+  ir::Stmt getInsertInitCoords(ir::Expr pBegin, ir::Expr pEnd, 
+                               Mode mode) const override;
+  ir::Stmt getInsertInitLevel(ir::Expr szPrev, ir::Expr sz, 
+                              Mode mode) const override;
+  ir::Stmt getInsertFinalizeLevel(ir::Expr szPrev, ir::Expr sz, 
+                                  Mode mode) const override;
   
-  virtual std::vector<ir::Expr> getArrays(ir::Expr tensor, int mode, 
-                                          int level) const;
+  ir::Expr getAssembledSize(ir::Expr prevSize, Mode mode) const override;
+  ModeFunction getYieldPos(ir::Expr parentPos, std::vector<ir::Expr> coords, 
+                           Mode mode) const override;
+
+  std::vector<ir::Expr> getArrays(ir::Expr tensor, int mode, 
+                                  int level) const override;
 
 protected:
   ir::Expr getSizeArray(ModePack pack) const;
 };
 
 }
```

### Comparing `tensora-0.0.6/src/taco/include/taco/lower/mode_format_impl.h` & `tensora-0.0.7/src/taco/include/taco/lower/mode_format_impl.h`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,71 @@
 #define TACO_MODE_FORMAT_IMPL_H
 
 #include <vector>
 #include <initializer_list>
 #include <memory>
 #include <string>
 #include <map>
+#include <tuple>
 
 #include "taco/format.h"
 #include "taco/ir/ir.h"
 #include "taco/lower/mode.h"
+#include "taco/index_notation/index_notation.h"
 
 namespace taco {
 
 class ModeFormatImpl;
 class ModeFormatPack;
 class ModePack;
 
+class AttrQuery {
+public:
+  enum Aggregation { IDENTITY, COUNT, MIN, MAX };
+  struct Attr {
+    Attr(std::tuple<std::string,Aggregation,std::vector<IndexVar>> attr); 
+
+    std::string label;
+    Aggregation aggr;
+    std::vector<IndexVar> params;
+  };
+
+  AttrQuery();
+  AttrQuery(const std::vector<IndexVar>& groupBy, const Attr& attr);
+  AttrQuery(const std::vector<IndexVar>& groupBy, 
+            const std::vector<Attr>& attrs);
+
+  const std::vector<IndexVar>& getGroupBy() const;
+  const std::vector<Attr>& getAttrs() const;
+
+private:
+  struct Content;
+  std::shared_ptr<Content> content;
+};
+
+std::ostream& operator<<(std::ostream&, const AttrQuery::Attr&);
+std::ostream& operator<<(std::ostream&, const AttrQuery&);
+
+class AttrQueryResult {
+public:
+  AttrQueryResult() = default;
+  AttrQueryResult(ir::Expr resultVar, ir::Expr resultValues);
+
+  ir::Expr getResult(const std::vector<ir::Expr>& indices, 
+                     const std::string& attr) const;
+
+  friend std::ostream& operator<<(std::ostream&, const AttrQueryResult&);
+
+private:
+  ir::Expr resultVar;
+  ir::Expr resultValues;
+};
+
+std::ostream& operator<<(std::ostream&, const AttrQueryResult&);
+
 /// Mode functions implement parts of mode capabilities, such as position
 /// iteration and locate.  The lower machinery requests mode functions from
 /// mode type implementations (`ModeTypeImpl`) and use these to generate code
 /// to iterate over and assemble tensors.
 class ModeFunction {
 public:
   /// Construct an undefined mode function.
@@ -55,39 +101,48 @@
 
 /// The abstract class to inherit from to add a new mode format to the system.
 /// The mode type implementation can then be passed to the `ModeType`
 /// constructor.
 class ModeFormatImpl {
 public:
   ModeFormatImpl(std::string name, bool isFull, bool isOrdered, bool isUnique, 
-                 bool isBranchless, bool isCompact, bool hasCoordValIter, 
-                 bool hasCoordPosIter, bool hasLocate, bool hasInsert, 
-                 bool hasAppend);
+                 bool isBranchless, bool isCompact, bool isZeroless, 
+		 bool isPadded, bool hasCoordValIter, bool hasCoordPosIter, 
+		 bool hasLocate, bool hasInsert, bool hasAppend, 
+		 bool hasSeqInsertEdge, bool hasInsertCoord, 
+		 bool isYieldPosPure);
 
   virtual ~ModeFormatImpl();
 
   /// Create a copy of the mode type with different properties.
   virtual ModeFormat copy(
       std::vector<ModeFormat::Property> properties) const = 0;
 
 
+  virtual std::vector<AttrQuery> attrQueries(
+      std::vector<IndexVar> parentCoords, 
+      std::vector<IndexVar> childCoords) const;
+
+
   /// The coordinate iteration capability's iterator function computes a range
   /// [result[0], result[1]) of coordinates to iterate over.
   /// `coord_iter_bounds(i_{1}, ..., i_{k−1}) -> begin_{k}, end_{k}`
   virtual ModeFunction coordIterBounds(std::vector<ir::Expr> parentCoords,
                                        Mode mode) const;
 
   /// The coordinate iteration capability's access function maps a coordinate
   /// iterator variable to a position (result[0]) and reports if a position
   /// could not be found (result[1]).
   /// `coord_iter_access(p_{k−1}, i_{1}, ..., i_{k}) -> p_{k}, found`
   virtual ModeFunction coordIterAccess(ir::Expr parentPos,
                                        std::vector<ir::Expr> coords,
                                        Mode mode) const;
 
+  virtual ModeFunction coordBounds(ir::Expr parentPos, Mode mode) const;
+
 
   /// The position iteration capability's iterator function computes a range
   /// [result[0], result[1]) of positions to iterate over.
   /// `pos_iter_bounds(p_{k−1}) -> begin_{k}, end_{k}`
   virtual ModeFunction posIterBounds(ir::Expr parentPos, Mode mode) const;
 
   /// The position iteration capability's access function maps a position
@@ -103,15 +158,15 @@
   /// and reports if the coordinate could not be found (result[1]).
   /// `locate(p_{k−1}, i_{1}, ..., i_{k}) -> p_{k}, found`
   virtual ModeFunction locate(ir::Expr parentPos,
                               std::vector<ir::Expr> coords,
                               Mode mode) const;
 
 
-  /// Level functions that implement insert capabilitiy.
+  /// Level functions that implement grouped insert capabilitiy.
   /// @{
   virtual ir::Stmt
   getInsertCoord(ir::Expr p, const std::vector<ir::Expr>& i, Mode mode) const;
 
   virtual ir::Expr getWidth(Mode mode) const;
 
   virtual ir::Stmt
@@ -142,34 +197,70 @@
   virtual ir::Stmt
   getAppendInitLevel(ir::Expr szPrev, ir::Expr sz, Mode mode) const;
 
   virtual ir::Stmt
   getAppendFinalizeLevel(ir::Expr szPrev, ir::Expr sz, Mode mode) const;
   /// @}
 
+  /// Level functions that implement ungrouped insert capabilitiy.
+  /// @{
+  virtual ir::Expr getAssembledSize(ir::Expr prevSize, Mode mode) const;
+
+  virtual ir::Stmt
+  getSeqInitEdges(ir::Expr prevSize, std::vector<AttrQueryResult> queries, 
+                  Mode mode) const;
+  
+  virtual ir::Stmt
+  getSeqInsertEdge(ir::Expr parentPos, std::vector<ir::Expr> coords,
+                   std::vector<AttrQueryResult> queries, Mode mode) const;
+
+  virtual ir::Stmt
+  getInitCoords(ir::Expr prevSize, std::vector<AttrQueryResult> queries, 
+                Mode mode) const;
+
+  virtual ir::Stmt
+  getInitYieldPos(ir::Expr prevSize, Mode mode) const;
+  
+  virtual ModeFunction
+  getYieldPos(ir::Expr parentPos, std::vector<ir::Expr> coords, 
+              Mode mode) const;
+
+  virtual ir::Stmt
+  getInsertCoord(ir::Expr parentPos, ir::Expr pos, std::vector<ir::Expr> coords, 
+                 Mode mode) const;
+
+  virtual ir::Stmt
+  getFinalizeYieldPos(ir::Expr prevSize, Mode mode) const;
+  /// @}
+
   /// Returns arrays associated with a tensor mode
   virtual std::vector<ir::Expr>
   getArrays(ir::Expr tensor, int mode, int level) const = 0;
 
   friend bool operator==(const ModeFormatImpl&, const ModeFormatImpl&);
   friend bool operator!=(const ModeFormatImpl&, const ModeFormatImpl&);
 
   const std::string name;
 
   const bool isFull;
   const bool isOrdered;
   const bool isUnique;
   const bool isBranchless;
   const bool isCompact;
-
+  const bool isZeroless;
+  const bool isPadded;
+  
   const bool hasCoordValIter;
   const bool hasCoordPosIter;
   const bool hasLocate;
   const bool hasInsert;
   const bool hasAppend;
+  const bool hasSeqInsertEdge;
+  const bool hasInsertCoord;
+  const bool isYieldPosPure;
 
 protected:
   /// Check if other mode format is identical. Can assume that this method will 
   /// always be called with an argument that is of the same class.
   virtual bool equals(const ModeFormatImpl& other) const;
 };
```

### Comparing `tensora-0.0.6/src/taco/include/taco/parser/lexer.h` & `tensora-0.0.7/src/taco/include/taco/parser/lexer.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/parser/parser.h` & `tensora-0.0.7/src/taco/include/taco/parser/parser.h`

 * *Files 3% similar despite different names*

```diff
@@ -50,17 +50,21 @@
 
   /// Retrieve the tensor with the given name
   const TensorBase& getTensor(std::string name) const;
 
   /// Retrieve a map from tensor names to tensors.
   const std::map<std::string,TensorBase>& getTensors() const;
 
+  /// Retrieve a list of names in the order they occurred in the expression
+  const std::vector<std::string> getNames() const;
+
 private:
   struct Content;
   std::shared_ptr<Content> content;
+  std::vector<std::string> names;
 
   /// assign ::= access '=' expr
   ///          | access '+=' expr
   TensorBase parseAssign();
 
   /// expr ::= term {('+' | '-') term}
   IndexExpr parseExpr();
```

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/array.h` & `tensora-0.0.7/src/taco/include/taco/storage/array.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/coordinate.h` & `tensora-0.0.7/src/taco/include/taco/storage/coordinate.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/file_io_mtx.h` & `tensora-0.0.7/src/taco/include/taco/storage/file_io_mtx.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/file_io_rb.h` & `tensora-0.0.7/src/taco/include/taco/storage/file_io_rb.h`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 namespace taco {
 class TensorBase;
 class Format;
 
 void readFile(std::istream &hbfile,
               int* nrow, int* ncol,
               int** colptr, int** rowind, double** values);
+template<typename T>
 void writeFile(std::ostream &hbfile, std::string key,
                int nrow, int ncol, int nnzero,
                int ptrsize, int indsize, int valsize,
-               int* colptr, int* rowind, double* values);
+               int* colptr, int* rowind, T* values);
 
 void readHeader(std::istream &hbfile,
                 std::string* title, std::string* key,
                 int* totcrd, int* ptrcrd, int* indcrd, int* valcrd, int* rhscrd,
                 std::string* mxtype, int* nrow,
                 int* ncol, int* nnzero, int* neltvl,
                 std::string* ptrfmt, std::string* indfmt,
@@ -34,16 +35,19 @@
                  std::string mxtype, int nrow, int ncol, int nnzero, int neltvl,
                  std::string ptrfmt, std::string indfmt,
                  std::string valfmt, std::string rhsfmt);
 void readIndices(std::istream &hbfile, int linesize, int indices[]);
 void writeIndices(std::ostream &hbfile, int indsize,
                   int linesize, int indices[]);
 void readValues(std::istream &hbfile, int linesize, double values[]);
+
+template<typename T>
 void writeValues(std::ostream &hbfile, int valuesize,
-                 int valperline, double values[]);
+                             int valperline, T values[]);
+
 // Useless for Taco
 void readRHS();
 void writeRHS();
 
 /// Read an rb matrix from a file.
 TensorBase readRB(std::string filename, const ModeFormat& modetype, 
                   bool pack=true);
```

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/file_io_tns.h` & `tensora-0.0.7/src/taco/include/taco/storage/file_io_tns.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/index.h` & `tensora-0.0.7/src/taco/include/taco/storage/index.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/pack.h` & `tensora-0.0.7/src/taco/include/taco/storage/pack.h`

 * *Files 6% similar despite different names*

```diff
@@ -13,40 +13,43 @@
 #include "taco/format.h"
 #include "taco/storage/typed_vector.h"
 #include "taco/storage/storage.h"
 #include "taco/storage/coordinate.h"
  
 namespace taco {
 
+class Literal;
+
 namespace ir {
 class Stmt;
 }
 
 TensorStorage pack(Datatype                             datatype,
                    const std::vector<int>&              dimensions,
                    const Format&                        format,
                    const std::vector<TypedIndexVector>& coordinates,
-                   const void*                          values);
-
+                   const void*                          values,
+                   const Literal&                       fill);
 
 template<typename V, size_t O, typename C>
 TensorStorage pack(std::vector<int> dimensions, Format format,
-                   const std::vector<std::pair<Coordinates<O,C>,V>>& components){
+                   const std::vector<std::pair<Coordinates<O,C>,V>>& components,
+                   const Literal& fill){
   size_t order = dimensions.size();
   size_t nnz = components.size();
 
   std::vector<TypedIndexVector> coordinates(order,
                                             TypedIndexVector(type<C>(), nnz));
   std::vector<V> values(nnz);
   for (size_t i = 0; i < nnz; i++) {
     values[i] = components[i].second;
     auto& coords = components[i].first;
     for (size_t j = 0; j < order; j++) {
       coordinates[j][i] = coords[j];
     }
   }
 
-  return pack(type<V>(), dimensions, format, coordinates, values.data());
+  return pack(type<V>(), dimensions, format, coordinates, values.data(), fill);
 }
 
 }
 #endif
```

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/storage.h` & `tensora-0.0.7/src/taco/include/taco/storage/storage.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 #ifndef TACO_STORAGE_STORAGE_H
 #define TACO_STORAGE_STORAGE_H
 
 #include <vector>
 #include <memory>
 
+#include "taco/format.h"
+#include "taco/storage/index.h"
+#include "taco/storage/array.h"
+#include "taco/storage/typed_vector.h"
+#include "taco/storage/typed_index.h"
+
 struct taco_tensor_t;
 
 namespace taco {
 class Format;
 class Type;
 class Datatype;
 class Index;
 class Array;
+class Literal;
 
 /// Storage for a tensor object.  Tensor storage consists of a value array that
 /// contains the tensor values and one index per mode.  The type of each
 /// mode index is determined by the mode type in the format, and the
 /// ordering of the mode indices is determined by the format mode ordering.
 class TensorStorage {
 public:
 
   /// Construct tensor storage for the given format.
   TensorStorage(Datatype componentType, const std::vector<int>& dimensions,
-                Format format);
+                Format format, Literal fillVal);
 
   /// Returns the tensor storage format.
   const Format& getFormat() const;
 
   /// Returns the component type of the tensor storage.
   Datatype getComponentType() const;
 
@@ -44,31 +51,37 @@
 
   /// Returns the value array that contains the tensor components.
   const Array& getValues() const;
 
   /// Returns the tensor component value array.
   Array getValues();
 
+  /// Returns the full value attached to the tensor storage
+  Literal getFillValue();
+
   /// Returns the size of the storage in bytes.
   size_t getSizeInBytes();
 
   /// Convert to a taco_tensor_t, whose lifetime is the same as the storage.
   operator struct taco_tensor_t*() const;
 
   /// Set the tensor index, which describes the non-zero values.
   void setIndex(const Index& index);
 
   /// Set the tensor component value array.
   void setValues(const Array& values);
 
+
 private:
   struct Content;
   std::shared_ptr<Content> content;
 };
 
+
+
 /// Compare tensor storage objects.
 bool equals(TensorStorage a, TensorStorage b);
 
 /// Print Storage objects to a stream.
 std::ostream& operator<<(std::ostream&, const TensorStorage&);
 
 }
```

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/typed_index.h` & `tensora-0.0.7/src/taco/include/taco/storage/typed_index.h`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,16 @@
 public:
   /// Create a TypedIndexRef initialized with the value stored at ptr of the size of DataType t
   template<typename T>
   TypedIndexRef(Datatype t, T *ptr) : ptr(reinterpret_cast<IndexTypeUnion *>(ptr)) {
     dType = t;
   }
 
+  TypedIndexRef(const TypedIndexRef& other) = default;
+
   /// Dereferences to a TypedIndexPtr
   TypedIndexPtr operator&() const;
   /// Gets a reference to the stored IndexTypeUnion
   IndexTypeUnion& get();
   /// Gets the value of the stored IndexTypeUnion
   IndexTypeUnion get() const;
   /// Gets the value of this TypedIndexRef as a size_t (for use in indexing)
```

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/typed_value.h` & `tensora-0.0.7/src/taco/include/taco/storage/typed_value.h`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class TypedComponent {
 public:
   /// Gets the DataType of this TypedComponent
   const Datatype& getType() const;
 
 protected:
   /// Gets the value of this TypedComponent as a size_t (for use in indexing)
-  size_t getAsIndex(const ComponentTypeUnion mem) const;
+  size_t getAsIndex(const ComponentTypeUnion &mem) const;
   /// Sets mem to value (ensure that it does not write to bytes past the size of the type in the union)
   void set(ComponentTypeUnion& mem, const ComponentTypeUnion& value);
   /// Sets mem to casted value of integer
   void setInt(ComponentTypeUnion& mem, const int value);
   /// Add the values of two ValueTypeUnion into a result
   void add(ComponentTypeUnion& result, const ComponentTypeUnion& a, const ComponentTypeUnion& b) const;
   /// Add the values of one ValueTypeUnion with an integer constant into a result
@@ -43,15 +43,15 @@
 /// Stores ValueTypeUnion and calls methods on TypedComponent with value
 /// NOTE: The implementations of these methods are very similar to TypedIndexVal in typed_index.h make sure to keep in sync.
 class TypedComponentVal: public TypedComponent {
 public:
   /// Create an undefined type TypedComponentVal
   TypedComponentVal();
   /// Create a TypedComponentVal with DataType type
-  TypedComponentVal(Datatype type);
+  explicit TypedComponentVal(Datatype type);
   /// Create a TypedComponentVal initialized with the value and type of ref
   TypedComponentVal(TypedComponentRef ref);
 
   /// Create a TypedComponentVal initialized with type t and the value of constant
   TypedComponentVal(Datatype t, int constant);
 
   /// Create a TypedComponentVal initialized with the value stored at ptr of the size of DataType t
@@ -160,14 +160,16 @@
 public:
   /// Create a TypedComponentRef initialized with the value stored at ptr of the size of DataType t
   template<typename T>
   TypedComponentRef(Datatype t, T *ptr) : ptr(reinterpret_cast<ComponentTypeUnion *>(ptr)) {
     dType = t;
   }
 
+  TypedComponentRef(const TypedComponentRef& other) = default;
+
   /// Dereferences to a TypedComponentPtr
   TypedComponentPtr operator&() const;
   /// Gets a reference to the stored ValueTypeUnion
   ComponentTypeUnion& get();
   /// Gets the value of the stored ValueTypeUnion
   ComponentTypeUnion get() const;
   /// Gets the value of this TypedComponentRef as a size_t (for use in indexing)
@@ -231,8 +233,7 @@
 /// Compare a TypedComponentVal with a constant
 bool operator<=(const TypedComponentVal& a, const int other);
 /// Compare a TypedComponentVal with a constant
 bool operator!=(const TypedComponentVal& a, const int other);
 
 }
 #endif
-
```

### Comparing `tensora-0.0.6/src/taco/include/taco/storage/typed_vector.h` & `tensora-0.0.7/src/taco/include/taco/storage/typed_vector.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/taco_tensor_t.h` & `tensora-0.0.7/src/taco/include/taco/taco_tensor_t.h`

 * *Files 7% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 /// code.  Note: this file must be valid C99, not C++.
 /// This *must* be kept in sync with the version used in codegen_c.cpp
 /// TODO: Remove `vals_size` after old lowering machinery has been replaced.
 
 #ifndef TACO_TENSOR_T_DEFINED
 #define TACO_TENSOR_T_DEFINED
 
-#include <cstdint>
+#include <stdint.h>
 
 typedef enum { taco_mode_dense, taco_mode_sparse } taco_mode_t;
 
 typedef struct taco_tensor_t {
   int32_t      order;         // tensor order (number of modes)
   int32_t*     dimensions;    // tensor dimensions
   int32_t      csize;         // component size
   int32_t*     mode_ordering; // mode storage ordering
   taco_mode_t* mode_types;    // mode storage types
   uint8_t***   indices;       // tensor index data (per mode)
   uint8_t*     vals;          // tensor values
+  uint8_t*     fill_value;    // tensor fill value
   int32_t      vals_size;     // values array size
 } taco_tensor_t;
 
 taco_tensor_t *init_taco_tensor_t(int32_t order, int32_t csize,
-                        int32_t* dimensions, int32_t* modeOrdering,
-                        taco_mode_t* mode_types);
+                                  int32_t* dimensions, int32_t* modeOrdering,
+                                  taco_mode_t* mode_types, void* fill_ptr);
 
 void deinit_taco_tensor_t(taco_tensor_t* t);
 
 #endif
```

### Comparing `tensora-0.0.6/src/taco/include/taco/target.h` & `tensora-0.0.7/src/taco/include/taco/target.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/type.h` & `tensora-0.0.7/src/taco/include/taco/type.h`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 #include <ostream>
 #include <cstdint>
 #include <vector>
 #include <initializer_list>
 #include "taco/error.h"
 #include <complex>
+#include <memory>
 
 namespace taco {
 
 /// A basic taco type. These can be boolean, integer, unsigned integer, float
 /// or complex float at different precisions.
 class Datatype {
 public:
@@ -195,38 +196,47 @@
   int16_t int16Value;
   int32_t int32Value;
   int64_t int64Value;
 
   IndexTypeUnion() {int32Value = 0;}
 };
 
+class IndexVar;
 
 /// A tensor dimension is the size of a tensor mode.  Tensor dimensions can be
 /// variable or fixed sized, which impacts code generation.  Variable dimensions
 /// are provided to kernels as arguments, while fixed dimensions are compiled
 /// into the kernel.
 class Dimension {
 public:
   /// Create a variable sized dimension.
   Dimension();
 
   /// Create a fixed sized dimension.
   Dimension(size_t size);
 
+  /// Create a dimension sized to an indexvar iteration size
+  explicit Dimension(IndexVar indexVar);
+
   /// True if the dimension is variable size, false otherwise.
   bool isVariable() const;
 
   /// True if the dimension is fixed size, false otherwise.
   bool isFixed() const;
 
   /// Returns the size of the dimension or 0 if it is variable sized.
   size_t getSize() const;
 
+  bool isIndexVarSized() const;
+
+  IndexVar getIndexVarSize() const;
+
 private:
-  size_t size;
+  struct Content;
+  std::shared_ptr<Content> content;
 };
 
 bool operator==(const Dimension&, const Dimension&);
 bool operator!=(const Dimension&, const Dimension&);
 
 /// Print a tensor dimension.
 std::ostream& operator<<(std::ostream&, const Dimension&);
```

### Comparing `tensora-0.0.6/src/taco/include/taco/util/collections.h` & `tensora-0.0.7/src/taco/include/taco/util/collections.h`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,28 @@
     if (!contains(filter, v)) {
       result.push_back(v);
     }
   }
   return result;
 }
 
+template <typename V>
+std::vector<V> removeDuplicates(const std::vector<V>& vector) {
+  std::set<V> seen;
+  std::vector<V> result;
+
+  for(const V& v: vector) {
+    if(!contains(seen, v)) {
+      seen.insert(v);
+      result.push_back(v);
+    }
+  }
+  return result;
+}
+
 template <typename V, typename T>
 std::vector<V> filter(const std::vector<V>& vector, T test) {
   std::vector<V> result;
   for (auto& element : vector) {
     if (test(element)) {
       result.push_back(element);
     }
@@ -115,14 +129,24 @@
     if (test(element)) {
       count++;
     }
   }
   return count;
 }
 
+template <typename K, typename V>
+std::map<K, V> zipToMap(const std::vector<K>& keys, const std::vector<V>& values) {
+  std::map<K, V> result;
+  size_t limit = std::min(keys.size(), values.size());
+  for(size_t i = 0; i < limit; ++i) {
+    result.insert({keys[i], values[i]});
+  }
+  return result;
+}
+
 /**
  * Split the vector into two vectors where elements in the first pass the test
  * and elements in the second do not.
  */
 template <typename V, typename T>
 std::pair<std::vector<V>,std::vector<V>> split(const std::vector<V>& vector,
                                                T test) {
@@ -145,17 +169,17 @@
     if (!test(element)) {
       return false;
     }
   }
   return true;
 }
 
-template <typename V, typename T>
-bool any(const std::vector<V>& vector, T test) {
-  for (auto& element : vector) {
+template <typename C, typename T>
+bool any(const C& collection, T test) {
+  for (auto& element : collection) {
     if (test(element)) {
       return true;
     }
   }
   return false;
 }
```

### Comparing `tensora-0.0.6/src/taco/include/taco/util/comparable.h` & `tensora-0.0.7/src/taco/include/taco/util/comparable.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/util/env.h` & `tensora-0.0.7/src/taco/include/taco/util/env.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/util/fill.h` & `tensora-0.0.7/src/taco/include/taco/util/fill.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/util/intrusive_ptr.h` & `tensora-0.0.7/src/taco/include/taco/util/intrusive_ptr.h`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,19 @@
     ptr = other.ptr;
     if (ptr) {
       acquire(ptr);
     }
     return *this;
   }
 
+  // Special function needed in pybind11 for custom smart pointers
+  const T* get() {
+    return ptr;
+  }
+
   /// Copy assignment operator for managed object
   IntrusivePtr& operator=(T *p) {
     if (ptr) {
       release(ptr);
     }
     this->ptr = p;
     if (ptr) {
```

### Comparing `tensora-0.0.6/src/taco/include/taco/util/scopedmap.h` & `tensora-0.0.7/src/taco/include/taco/util/scopedmap.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #ifndef TACO_UTIL_SCOPEDMAP_H
 #define TACO_UTIL_SCOPEDMAP_H
 
+#include <iostream>
 #include <list>
 #include <map>
 #include <ostream>
 #include "taco/util/collections.h"
 
 #include "taco/error.h"
```

### Comparing `tensora-0.0.6/src/taco/include/taco/util/scopedset.h` & `tensora-0.0.7/src/taco/include/taco/util/scopedset.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/include/taco/util/timers.h` & `tensora-0.0.7/src/taco/include/taco/util/timers.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #ifndef TACO_UTIL_BENCHMARK_H
 #define TACO_UTIL_BENCHMARK_H
 
 #include <chrono>
 #include <algorithm>
+#include <iostream>
 #include <numeric>
+#include <vector>
 #include <cmath>
+#include "taco/error.h"
 
 using namespace std;
 
 namespace taco {
 namespace util {
 
 struct TimeResults {
```

### Comparing `tensora-0.0.6/src/taco/include/taco/util/variadic.h` & `tensora-0.0.7/src/taco/include/taco/util/variadic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #ifndef TACO_UTIL_VARIADIC_H
 #define TACO_UTIL_VARIADIC_H
 
 #include <type_traits>
+#include <vector>
 
 namespace taco {
 namespace util {
 
 // Compare types
 template<class T, class...>
 struct areSame : std::true_type {};
```

### Comparing `tensora-0.0.6/src/taco/misc/mainpage.h` & `tensora-0.0.7/src/taco/misc/mainpage.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/CMakeLists.txt` & `tensora-0.0.7/src/taco/src/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 foreach(dir ${TACO_SRC_DIRS})
   file(GLOB TACO_HEADERS ${TACO_HEADERS} ${dir}/*.h)
   file(GLOB TACO_HEADERS ${TACO_HEADERS} ${TACO_INCLUDE_DIR}/taco/${dir}/*.h)
   file(GLOB TACO_SOURCES ${TACO_SOURCES} ${dir}/*.cpp)
 endforeach()
 
-set(TACO_HEADERS ${TACO_HEADERS})
-set(TACO_SOURCES ${TACO_SOURCES})
+set(TACO_HEADERS ${TACO_HEADERS} ../include/taco/ir_tags.h)
+set(TACO_SOURCES ${TACO_SOURCES} ir_tags.cpp)
 
 add_definitions(${TACO_DEFINITIONS})
 include_directories(${TACO_SRC_DIR})
 add_library(taco ${TACO_LIBRARY_TYPE} ${TACO_HEADERS} ${TACO_SOURCES})
 if (CUDA)
-  include_directories(/usr/local/cuda/include)
-  target_link_libraries(taco INTERFACE /usr/local/cuda/lib64/libcudart.so)
+  include_directories(${CUDA_INCLUDE_DIRS})
+  target_link_libraries(taco PUBLIC ${CUDA_LIBRARIES})
 endif (CUDA)
 install(TARGETS taco DESTINATION lib)
 
 if (LINUX)
   target_link_libraries(taco PRIVATE ${TACO_LIBRARIES} dl)
 else()
   target_link_libraries(taco PRIVATE ${TACO_LIBRARIES})
```

### Comparing `tensora-0.0.6/src/taco/src/codegen/codegen.cpp` & `tensora-0.0.7/src/taco/src/codegen/codegen.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -190,41 +190,79 @@
   ret << "    TACO_DEREF(" << sizeName << ") = sizeof(" << ctxClassName
       << ");" << endl;
   ret << "  }" << endl;
 
   return ret.str();
 }
 
+string CodeGen::printTensorProperty(string varname, const GetProperty* op, bool is_ptr) {
+  stringstream ret;
+  string star = is_ptr ? "*" : "";
+  if (is_ptr) {
+    varname += "_ptr";
+  }
+
+  auto tensor = op->tensor.as<Var>();
+  if (op->property == TensorProperty::Values) {
+    // for the values, it's in the last slot
+    ret << printType(tensor->type, true) << star;
+    ret << " " << varname;
+    return ret.str();
+  } else if (op->property == TensorProperty::ValuesSize) {
+    ret << "int" << star << " " << varname;
+    return ret.str();
+  }
+
+  string tp;
+
+  // for a Dense level, nnz is an int
+  // for a Fixed level, ptr is an int
+  // all others are int*
+  if (op->property == TensorProperty::Dimension) {
+    tp = "int" + star;
+    ret << tp << " " << varname;
+  } else {
+    taco_iassert(op->property == TensorProperty::Indices);
+    tp = "int*" + star;
+    ret << tp << " " << varname;
+  }
+
+  return ret.str();
+}
+
 string CodeGen::unpackTensorProperty(string varname, const GetProperty* op,
                             bool is_output_prop) {
   stringstream ret;
   ret << "  ";
 
   auto tensor = op->tensor.as<Var>();
   if (op->property == TensorProperty::Values) {
     // for the values, it's in the last slot
     ret << printType(tensor->type, true);
-    ret << " " << restrictKeyword() << " " << varname
-        << " = (" << printType(tensor->type, true) << ")(";
+    ret << " " << restrictKeyword() << " " << varname << " = (" << printType(tensor->type, true) << ")(";
     ret << tensor->name << "->vals);\n";
     return ret.str();
   } else if (op->property == TensorProperty::ValuesSize) {
     ret << "int " << varname << " = " << tensor->name << "->vals_size;\n";
     return ret.str();
+  } else if (op->property == TensorProperty::FillValue) {
+    ret << printType(tensor->type, false) << " " << varname << " = ";
+    ret << "*((" <<printType(tensor->type, true) << ")(" << tensor->name << "->fill_value));\n";
+    return ret.str();
   }
 
   string tp;
 
   // for a Dense level, nnz is an int
   // for a Fixed level, ptr is an int
   // all others are int*
   if (op->property == TensorProperty::Dimension) {
     tp = "int";
     ret << tp << " " << varname << " = (int)(" << tensor->name
-        << "->dimensions[" << op->mode << "]);\n";;
+        << "->dimensions[" << op->mode << "]);\n";
   } else {
     taco_iassert(op->property == TensorProperty::Indices);
     tp = "int*";
     auto nm = op->index;
     ret << tp << " " << restrictKeyword() << " " << varname << " = ";
     ret << "(int*)(" << tensor->name << "->indices[" << op->mode;
     ret << "][" << nm << "]);\n";
@@ -243,14 +281,16 @@
   if (property == TensorProperty::Values) {
     ret << tensor->name << "->vals";
     ret << " = (uint8_t*)" << varname << ";\n";
     return ret.str();
   } else if (property == TensorProperty::ValuesSize) {
     ret << tensor->name << "->vals_size = " << varname << ";\n";
     return ret.str();
+  } else if (property == TensorProperty::FillValue) {
+    return "";
   }
 
   string tp;
 
   // for a Dense level, nnz is an int
   // for a Fixed level, ptr is an int
   // all others are int*
@@ -264,14 +304,21 @@
         "[" << mode << "][" << nm << "] = (uint8_t*)(" << varname
         << ");\n";
   }
 
   return ret.str();
 }
 
+string CodeGen::pointTensorProperty(std::string varname) {
+  stringstream ret;
+  ret << "*" + varname + "_ptr";
+  ret << " = " << varname << ";" << endl;
+
+  return ret.str();
+}
 
 // helper to print declarations
 string CodeGen::printDecls(map<Expr, string, ExprCompare> varMap,
                            vector<Expr> inputs, vector<Expr> outputs) {
   stringstream ret;
   unordered_set<string> propsAlreadyGenerated;
 
@@ -313,15 +360,25 @@
 
          return a->index < b->index;
        });
 
   for (auto prop: sortedProps) {
     bool isOutputProp = (find(outputs.begin(), outputs.end(),
                               prop->tensor) != outputs.end());
-    ret << unpackTensorProperty(varMap[prop], prop, isOutputProp);
+    
+    auto var = prop->tensor.as<Var>();
+    if (var->is_parameter) {
+      if (isOutputProp) {
+        ret << "  " << printTensorProperty(varMap[prop], prop, false) << ";" << endl;
+      } else {
+        break; 
+      }
+    } else {
+      ret << unpackTensorProperty(varMap[prop], prop, isOutputProp);
+    }
     propsAlreadyGenerated.insert(varMap[prop]);
   }
 
   return ret.str();
 }
 
 
@@ -355,16 +412,21 @@
          if (get<2>(a) != get<2>(b))
            return get<2>(a) < get<2>(b);
 
          return get<3>(a) < get<3>(b);
        });
 
   for (auto prop: sortedProps) {
-    ret << packTensorProperty(outputProperties[prop], get<0>(prop),
+    auto var = get<0>(prop).as<Var>();
+    if (var->is_parameter) {
+      ret << "  " << pointTensorProperty(outputProperties[prop]);
+    } else {
+      ret << packTensorProperty(outputProperties[prop], get<0>(prop),
                               get<1>(prop), get<2>(prop), get<3>(prop));
+    }
   }
   return ret.str();
 }
 
 // seed the unique names with all C99 keywords
 // from: http://en.cppreference.com/w/c/keyword
 map<string, int> uniqueNameCounters;
@@ -418,54 +480,110 @@
     os << uniqueNameCounters[name]++;
   } else {
     uniqueNameCounters[name] = 0;
   }
   return os.str();
 }
 
+static vector<const GetProperty*> sortProps(std::map<Expr, std::string, ExprCompare> map) {
+  vector<const GetProperty*> sortedProps;
 
-string CodeGen::printFuncName(const Function *func) {
+  for (auto const& p: map) {
+    if (p.first.as<GetProperty>())
+      sortedProps.push_back(p.first.as<GetProperty>());
+  }
+
+  // sort the properties in order to generate them in a canonical order
+  sort(sortedProps.begin(), sortedProps.end(),
+       [&](const GetProperty *a,
+           const GetProperty *b) -> bool {
+
+         // if they're different properties, sort by property
+         if (a->property != b->property)
+           return a->property < b->property;
+
+         // now either the mode gives order, or index #
+         if (a->mode != b->mode)
+           return a->mode < b->mode;
+
+         return a->index < b->index;
+       });
+
+  return sortedProps;
+}
+
+string CodeGen::printFuncName(const Function *func, 
+                              std::map<Expr, std::string, ExprCompare> inputMap, 
+                              std::map<Expr, std::string, ExprCompare> outputMap) {
   stringstream ret;
 
   ret << "int " << func->name << "(";
 
   string delimiter = "";
   const auto returnType = func->getReturnType();
   if (returnType.second != Datatype()) {
     ret << "void **" << ctxName << ", ";
     ret << "char *" << coordsName << ", ";
     ret << printType(returnType.second, true) << valName << ", ";
     ret << "int32_t *" << bufCapacityName;
     delimiter = ", ";
   }
+
+  bool unfoldOutput = false;
   for (size_t i=0; i<func->outputs.size(); i++) {
     auto var = func->outputs[i].as<Var>();
     taco_iassert(var) << "Unable to convert output " << func->outputs[i]
                       << " to Var";
+    if (var->is_parameter) {
+      unfoldOutput = true;
+      break;
+    }
+
     if (var->is_tensor) {
       ret << delimiter << "taco_tensor_t *" << var->name;
     } else {
       auto tp = printType(var->type, var->is_ptr);
       ret << delimiter << tp << " " << var->name;
     }
     delimiter = ", ";
   }
+
+  if (unfoldOutput) {
+    for (auto prop : sortProps(outputMap)) {
+      ret << delimiter << printTensorProperty(outputMap[prop], prop, true);
+      delimiter = ", ";
+    }
+  }
+
+  bool unfoldInput = false;
   for (size_t i=0; i<func->inputs.size(); i++) {
     auto var = func->inputs[i].as<Var>();
     taco_iassert(var) << "Unable to convert output " << func->inputs[i]
                       << " to Var";
+    if (var->is_parameter) {
+      unfoldInput = true;
+      break;
+    }
+
     if (var->is_tensor) {
       ret << delimiter << "taco_tensor_t *" << var->name;
     } else {
       auto tp = printType(var->type, var->is_ptr);
       ret << delimiter << tp << " " << var->name;
     }
     delimiter = ", ";
   }
 
+  if (unfoldInput) {
+    for (auto prop : sortProps(inputMap)) {
+      ret << delimiter << printTensorProperty(inputMap[prop], prop, false);
+      delimiter = ", ";
+    }
+  }
+
   ret << ")";
   return ret.str();
 }
 
 void CodeGen::doIndentStream(stringstream &stream) {
   for (int i=0; i<indent; i++)
     stream << "  ";
```

### Comparing `tensora-0.0.6/src/taco/src/codegen/codegen.h` & `tensora-0.0.7/src/taco/src/codegen/codegen.h`

 * *Files 4% similar despite different names*

```diff
@@ -45,29 +45,32 @@
   std::string printDecls(std::map<Expr, std::string, ExprCompare> varMap,
                          std::vector<Expr> inputs, std::vector<Expr> outputs);
   std::string printPack(std::map<std::tuple<Expr, TensorProperty, int, int>,
           std::string> outputProperties, std::vector<Expr> outputs);
   std::string printCoroutineFinish(int numYields, std::string funcName);
   void printYield(const Yield* op, std::vector<Expr> localVars,
                          std::map<Expr, std::string, ExprCompare> varMap, int labelCount, std::string funcName);
-  std::string printFuncName(const Function *func);
+  std::string printFuncName(const Function *func, 
+          std::map<Expr, std::string, ExprCompare> inputMap={}, 
+          std::map<Expr, std::string, ExprCompare> outputMap={});
 
   void resetUniqueNameCounters();
   std::string genUniqueName(std::string name);
   void doIndentStream(std::stringstream &stream);
   CodeGenType codeGenType;
 
 private:
   virtual std::string restrictKeyword() const { return ""; }
 
-
+  std::string printTensorProperty(std::string varname, const GetProperty* op, bool is_ptr);
   std::string unpackTensorProperty(std::string varname, const GetProperty* op,
                               bool is_output_prop);
   std::string packTensorProperty(std::string varname, Expr tnsr, TensorProperty property,
                             int mode, int index);
+  std::string pointTensorProperty(std::string varname);
 };
 
 
 
 
 } // namespace ir
 } // namespace taco
```

### Comparing `tensora-0.0.6/src/taco/src/codegen/codegen_c.h` & `tensora-0.0.7/src/taco/src/codegen/codegen_c.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #ifndef TACO_BACKEND_C_H
 #define TACO_BACKEND_C_H
-
 #include <map>
 #include <vector>
 
 #include "taco/ir/ir.h"
 #include "taco/ir/ir_printer.h"
 #include "codegen.h"
 
@@ -12,15 +11,15 @@
 namespace ir {
 
 
 class CodeGen_C : public CodeGen {
 public:
   /// Initialize a code generator that generates code to an
   /// output stream.
-  CodeGen_C(std::ostream &dest, OutputKind outputKind);
+  CodeGen_C(std::ostream &dest, OutputKind outputKind, bool simplify=true);
   ~CodeGen_C();
 
   /// Compile a lowered function
   void compile(Stmt stmt, bool isFirst=false);
 
   /// Generate shims that unpack an array of pointers representing
   /// a mix of taco_tensor_t* and scalars into a function call
@@ -36,14 +35,16 @@
   void visit(const For*);
   void visit(const While*);
   void visit(const GetProperty*);
   void visit(const Min*);
   void visit(const Max*);
   void visit(const Allocate*);
   void visit(const Sqrt*);
+  void visit(const Store*);
+  void visit(const Assign*);
 
   std::map<Expr, std::string, ExprCompare> varMap;
   std::vector<Expr> localVars;
   std::ostream &out;
   
   OutputKind outputKind;
```

### Comparing `tensora-0.0.6/src/taco/src/codegen/codegen_cuda.cpp` & `tensora-0.0.7/src/taco/src/codegen/codegen_cuda.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 #include "taco/ir/ir_rewriter.h"
 #include "codegen_cuda.h"
 #include "taco/error.h"
 #include "taco/util/strings.h"
 #include "taco/util/collections.h"
 #include "taco/ir/simplify.h"
 
+#define GEN_TIMING_CODE false
+
 using namespace std;
 
 namespace taco {
   namespace ir {
 
 // Some helper functions
     namespace {
 
-#define CUDA_BLOCK_SIZE 256
-
 // Include stdio.h for printf
 // stdlib.h for malloc/realloc
 // math.h for sqrt
 // MIN preprocessor macro
 // This *must* be kept in sync with taco_tensor_t.h
 const string cHeaders =
   "#ifndef TACO_C_HEADERS\n"
@@ -45,29 +45,123 @@
   "  int32_t      order;         // tensor order (number of modes)\n"
   "  int32_t*     dimensions;    // tensor dimensions\n"
   "  int32_t      csize;         // component size\n"
   "  int32_t*     mode_ordering; // mode storage ordering\n"
   "  taco_mode_t* mode_types;    // mode storage types\n"
   "  uint8_t***   indices;       // tensor index data (per mode)\n"
   "  uint8_t*     vals;          // tensor values\n"
+  "  uint8_t*     fill_value;    // tensor fill value\n"
   "  int32_t      vals_size;     // values array size\n"
   "} taco_tensor_t;\n"
   "#endif\n"
   "#endif\n\n"; // // https://stackoverflow.com/questions/14038589/what-is-the-canonical-way-to-check-for-errors-using-the-cuda-runtime-api
 
 const string gpuAssertMacro =
   "#define gpuErrchk(ans) { gpuAssert((ans), __FILE__, __LINE__); }\n"
   "inline void gpuAssert(cudaError_t code, const char *file, int line, bool abort=true)\n"
   "{\n"
   "  if (code != cudaSuccess)\n"
   "  {\n"
   "    fprintf(stderr,\"GPUassert: %s %s %d\\n\", cudaGetErrorString(code), file, line);\n"
   "    if (abort) exit(code);\n"
   "  }\n"
+  "}\n"
+  "__device__ __host__ int taco_binarySearchAfter(int *array, int arrayStart, int arrayEnd, int target) {\n"
+  "  if (array[arrayStart] >= target) {\n"
+  "    return arrayStart;\n"
+  "  }\n"
+  "  int lowerBound = arrayStart; // always < target\n"
+  "  int upperBound = arrayEnd; // always >= target\n"
+  "  while (upperBound - lowerBound > 1) {\n"
+  "    int mid = (upperBound + lowerBound) / 2;\n"
+  "    int midValue = array[mid];\n"
+  "    if (midValue < target) {\n"
+  "      lowerBound = mid;\n"
+  "    }\n"
+  "    else if (midValue > target) {\n"
+  "      upperBound = mid;\n"
+  "    }\n"
+  "    else {\n"
+  "      return mid;\n"
+  "    }\n"
+  "  }\n"
+  "  return upperBound;\n"
+  "}\n"
+  "__device__ __host__ int taco_binarySearchBefore(int *array, int arrayStart, int arrayEnd, int target) {\n"
+  "  if (array[arrayEnd] <= target) {\n"
+  "    return arrayEnd;\n"
+  "  }\n"
+  "  int lowerBound = arrayStart; // always <= target\n"
+  "  int upperBound = arrayEnd; // always > target\n"
+  "  while (upperBound - lowerBound > 1) {\n"
+  "    int mid = (upperBound + lowerBound) / 2;\n"
+  "    int midValue = array[mid];\n"
+  "    if (midValue < target) {\n"
+  "      lowerBound = mid;\n"
+  "    }\n"
+  "    else if (midValue > target) {\n"
+  "      upperBound = mid;\n"
+  "    }\n"
+  "    else {\n"
+  "      return mid;\n"
+  "    }\n"
+  "  }\n"
+  "  return lowerBound;\n"
+  "}\n"
+  "__global__ void taco_binarySearchBeforeBlock(int * __restrict__ array, int * __restrict__ results, int arrayStart, int arrayEnd, int values_per_block, int num_blocks) {\n"
+  "  int thread = threadIdx.x;\n"
+  "  int block = blockIdx.x;\n"
+  "  int idx = block * blockDim.x + thread;\n"
+  "  if (idx >= num_blocks+1) {\n"
+  "    return;\n"
+  "  }\n"
+  "\n"
+  "  results[idx] = taco_binarySearchBefore(array, arrayStart, arrayEnd, idx * values_per_block);\n"
+  "}\n"
+  "\n"
+  "__host__ int * taco_binarySearchBeforeBlockLaunch(int * __restrict__ array, int * __restrict__ results, int arrayStart, int arrayEnd, int values_per_block, int block_size, int num_blocks){\n"
+  "  int num_search_blocks = (num_blocks + 1 + block_size - 1) / block_size;\n"
+  "  taco_binarySearchBeforeBlock<<<num_search_blocks, block_size>>>(array, results, arrayStart, arrayEnd, values_per_block, num_blocks);\n"
+  "  return results;\n"
+  "}\n"
+  "__global__ void taco_binarySearchIndirectBeforeBlock(int * __restrict__ array, int * __restrict__ results, int arrayStart, int arrayEnd, int * __restrict__ targets, int num_blocks) {\n"
+  "  int thread = threadIdx.x;\n"
+  "  int block = blockIdx.x;\n"
+  "  int idx = block * blockDim.x + thread;\n"
+  "  if (idx >= num_blocks+1) {\n"
+  "    return;\n"
+  "  }\n"
+  "\n"
+  "  results[idx] = taco_binarySearchBefore(array, arrayStart, arrayEnd, targets[idx]);\n"
+  "}\n"
+  "\n"
+  "__host__ int * taco_binarySearchIndirectBeforeBlockLaunch(int * __restrict__ array, int * __restrict__ results, int arrayStart, int arrayEnd, int * __restrict__ targets, int block_size, int num_blocks){\n"
+  "  int num_search_blocks = (num_blocks + 1 + block_size - 1) / block_size;\n"
+  "  taco_binarySearchIndirectBeforeBlock<<<num_search_blocks, block_size>>>(array, results, arrayStart, arrayEnd, targets, num_blocks);\n"
+  "  return results;\n"
+  "}\n"
+  "template<typename T>\n"
+  "__device__ inline void atomicAddWarp(T *array, int index, T val)\n"
+  "{\n"
+  "  int leader_index = __shfl_sync(-1, index, 0);\n"
+  "  int mask = __ballot_sync(-1, leader_index == index);\n"
+  "  if(mask == -1) {\n"
+  "    val += __shfl_down_sync(-1, val, 16);\n"
+  "    val += __shfl_down_sync(-1, val, 8);\n"
+  "    val += __shfl_down_sync(-1, val, 4);\n"
+  "    val += __shfl_down_sync(-1, val, 2);\n"
+  "    val += __shfl_down_sync(-1, val, 1);\n"
+  "    if(threadIdx.x % 32 == 0) {\n"
+  "      atomicAdd(&array[index], val);\n"
+  "    }\n"
+  "  } else {\n"
+  "    atomicAdd(&array[index], val);\n"
+  "  }\n"
   "}\n";
+
 const std::string blue="\033[38;5;67m";
 const std::string nc="\033[0m";
 } // anonymous namespace
 
 // find variables for generating declarations
 // also only generates a single var for each GetProperty
 class CodeGen_CUDA::FindVars : public IRVisitor {
@@ -88,72 +182,83 @@
 
   // TODO: should replace this with an unordered set
   vector<Expr> outputTensors;
 
   // Stop searching for variables at device functions (used to generate kernel launches)
   bool stopAtDeviceFunction;
 
+  bool inBlock;
+
   CodeGen_CUDA *codeGen;
 
   // copy inputs and outputs into the map
   FindVars(vector<Expr> inputs, vector<Expr> outputs, CodeGen_CUDA *codeGen,
            bool stopAtDeviceFunction=false)
   : codeGen(codeGen) {
     for (auto v: inputs) {
       auto var = v.as<Var>();
       taco_iassert(var) << "Inputs must be vars in codegen";
       taco_iassert(varMap.count(var) == 0) <<
-                                           "Duplicate input found in codegen";
+                                           "Duplicate input found in codegen: " << var->name;
       varMap[var] = var->name;
     }
     for (auto v: outputs) {
       auto var = v.as<Var>();
       taco_iassert(var) << "Outputs must be vars in codegen";
       taco_iassert(varMap.count(var) == 0) <<
                                            "Duplicate output found in codegen";
 
       outputTensors.push_back(v);
       varMap[var] = var->name;
     }
     FindVars::stopAtDeviceFunction = stopAtDeviceFunction;
+    inBlock = false;
   }
 
 protected:
   using IRVisitor::visit;
 
   virtual void visit(const For *op) {
     if (!util::contains(localVars, op->var)) {
       localVars.push_back(op->var);
     }
+    if (op->parallel_unit == ParallelUnit::GPUThread && stopAtDeviceFunction) {
+      // Want to collect the start, end, increment for the thread loop, but no other variables
+      taco_iassert(inBlock);
+      inBlock = false;
+    }
     op->var.accept(this);
     op->start.accept(this);
     op->end.accept(this);
     op->increment.accept(this);
-    if (op->accelerator && stopAtDeviceFunction) {
+    if (op->parallel_unit == ParallelUnit::GPUBlock && stopAtDeviceFunction) {
+      inBlock = true;
+    }
+    if (op->parallel_unit == ParallelUnit::GPUThread && stopAtDeviceFunction) {
       return;
     }
     op->contents.accept(this);
   }
 
   virtual void visit(const Var *op) {
-    if (varMap.count(op) == 0) {
-      varMap[op] = codeGen->genUniqueName(op->name);
+    if (varMap.count(op) == 0 && !inBlock) {
+      varMap[op] = op->is_ptr? op->name : codeGen->genUniqueName(op->name);
     }
   }
 
   virtual void visit(const VarDecl *op) {
-    if (!util::contains(localVars, op->var)) {
+    if (!util::contains(localVars, op->var) && !inBlock) {
       localVars.push_back(op->var);
     }
     op->var.accept(this);
     op->rhs.accept(this);
   }
 
   virtual void visit(const GetProperty *op) {
-    if (varMap.count(op) == 0) {
+    if (varMap.count(op) == 0 && !inBlock) {
       auto key =
               tuple<Expr,TensorProperty,int,int>(op->tensor,op->property,
                                                  (size_t)op->mode,
                                                  (size_t)op->index);
       if (canonicalPropertyVar.count(key) > 0) {
         varMap[op] = canonicalPropertyVar[key];
       } else {
@@ -170,23 +275,31 @@
 };
 
 // Finds all for loops tagged with accelerator and adds statements to deviceFunctions
 // Also tracks scope of when device function is called and
 // tracks which variables must be passed to function.
 class CodeGen_CUDA::DeviceFunctionCollector : public IRVisitor {
 public:
-  vector<Stmt> deviceFunctions;
+  vector<Stmt> blockFors;
+  vector<Stmt> threadFors; // contents is device function
+  vector<Stmt> warpFors;
   map<Expr, string, ExprCompare> scopeMap;
 
   // the variables to pass to each device function
   vector<vector<pair<string, Expr>>> functionParameters;
   vector<pair<string, Expr>> currentParameters; // keep as vector so code generation is deterministic
   set<Expr> currentParameterSet;
 
+  set<Expr> variablesDeclaredInKernel;
+
   vector<pair<string, Expr>> threadIDVars;
+  vector<pair<string, Expr>> blockIDVars;
+  vector<pair<string, Expr>> warpIDVars;
+  vector<Expr> numThreads;
+  vector<Expr> numWarps;
 
   CodeGen_CUDA *codeGen;
   // copy inputs and outputs into the map
   DeviceFunctionCollector(vector<Expr> inputs, vector<Expr> outputs, CodeGen_CUDA *codeGen) : codeGen(codeGen)  {
     inDeviceFunction = false;
     for (auto v: inputs) {
       auto var = v.as<Var>();
@@ -207,48 +320,89 @@
 
 protected:
   bool inDeviceFunction;
   using IRVisitor::visit;
 
   virtual void visit(const For *op) {
     // Don't need to find/initialize loop bounds
-    op->var.accept(this);
-    if (op->accelerator) {
+    if (op->parallel_unit == ParallelUnit::GPUBlock) {
+      op->var.accept(this);
       taco_iassert(!inDeviceFunction) << "Nested Device functions not supported";
-      deviceFunctions.push_back(op);
-      threadIDVars.push_back(pair<string, Expr>(scopeMap[op->var], op->var));
+      blockFors.push_back(op);
+      blockIDVars.push_back(pair<string, Expr>(scopeMap[op->var], op->var));
       currentParameters.clear();
       currentParameterSet.clear();
+      variablesDeclaredInKernel.clear();
       inDeviceFunction = true;
     }
+    else if (op->parallel_unit == ParallelUnit::GPUWarp) {
+      taco_iassert(inDeviceFunction) << "Nested Device functions not supported";
+      taco_iassert(blockIDVars.size() == warpIDVars.size() + 1) << "No matching GPUBlock parallelize for GPUWarp";
+      inDeviceFunction = false;
+      op->var.accept(this);
+      inDeviceFunction = true;
+
+      warpFors.push_back(op);
+      warpIDVars.push_back(pair<string, Expr>(scopeMap[op->var], op->var));
+      Expr warpsInBlock = ir::simplify(ir::Div::make(ir::Sub::make(op->end, op->start), op->increment));
+      numWarps.push_back(warpsInBlock);
+    }
+    else if (op->parallel_unit == ParallelUnit::GPUThread) {
+      taco_iassert(inDeviceFunction) << "Nested Device functions not supported";
+      taco_iassert(blockIDVars.size() == threadIDVars.size() + 1) << "No matching GPUBlock parallelize for GPUThread";
+      if (blockIDVars.size() > warpIDVars.size()) {
+        warpFors.push_back(Stmt());
+        warpIDVars.push_back({});
+        numWarps.push_back(0);
+      }
+      inDeviceFunction = false;
+      op->var.accept(this);
+      inDeviceFunction = true;
+
+      threadFors.push_back(op);
+      threadIDVars.push_back(pair<string, Expr>(scopeMap[op->var], op->var));
+      Expr blockSize = ir::simplify(ir::Div::make(ir::Sub::make(op->end, op->start), op->increment));
+      numThreads.push_back(blockSize);
+    }
+    else{
+      op->var.accept(this);
+    }
     op->start.accept(this);
     op->end.accept(this);
     op->increment.accept(this);
     op->contents.accept(this);
-    if (op->accelerator) {
+    if (op->parallel_unit == ParallelUnit::GPUBlock) {
+      taco_iassert(blockIDVars.size() == threadIDVars.size()) << "No matching GPUThread parallelize for GPUBlock";
       inDeviceFunction = false;
       sort(currentParameters.begin(), currentParameters.end());
       functionParameters.push_back(currentParameters);
     }
   }
 
   virtual void visit(const Var *op) {
     if (scopeMap.count(op) == 0) {
       string name = codeGen->genUniqueName(op->name);
       if (!inDeviceFunction) {
         scopeMap[op] = name;
       }
     }
-    else if (scopeMap.count(op) == 1 && inDeviceFunction && currentParameterSet.count(op) == 0 && op != threadIDVars.back().second) {
+    else if (scopeMap.count(op) == 1 && inDeviceFunction && currentParameterSet.count(op) == 0
+            && (threadIDVars.empty() || op != threadIDVars.back().second)
+            && (blockIDVars.empty() || op != blockIDVars.back().second)
+            && (warpIDVars.empty() || op != warpIDVars.back().second)
+            && !variablesDeclaredInKernel.count(op)) {
       currentParameters.push_back(pair<string, Expr>(scopeMap[op], op));
       currentParameterSet.insert(op);
     }
   }
 
   virtual void visit(const VarDecl *op) {
+    if (inDeviceFunction) {
+      variablesDeclaredInKernel.insert(op->var);
+    }
     op->var.accept(this);
     op->rhs.accept(this);
   }
 
   virtual void visit(const GetProperty *op) {
     if (scopeMap.count(op->tensor) == 0 && !inDeviceFunction) {
       auto key =
@@ -292,98 +446,194 @@
   for (size_t i=0; i<currentParameters.size(); i++) {
     auto var = currentParameters[i].second.as<Var>();
     taco_iassert(var) << "Unable to convert output " << currentParameters[i].second
                       << " to Var";
     string varName = currentParameters[i].first;
 
     if (var->is_tensor) {
-      ret << delimiter << "taco_tensor_t *" << varName;
+      ret << delimiter << "taco_tensor_t * __restrict__ " << varName;
     }
     else {
       auto tp = printCUDAType(var->type, var->is_ptr);
-      ret << delimiter << tp << " " << var->name;
+      ret << delimiter << tp << " ";
+      if (!var->is_ptr) {
+        ret << "&";
+      }
+      ret << var->name;
     }
     // No non-tensor parameters
     delimiter = ", ";
   }
   ret << ")";
   return ret.str();
 }
 
-void CodeGen_CUDA::printThreadIDVariable(pair<string, Expr> threadIDVar, Expr start, Expr increment) {
+void CodeGen_CUDA::printThreadIDVariable(pair<string, Expr> threadIDVar, Expr start, Expr increment, Expr numThreads) {
   auto var = threadIDVar.second.as<Var>();
   taco_iassert(var) << "Unable to convert output " << threadIDVar.second
                     << " to Var";
   string varName = threadIDVar.first;
   auto tp = printCUDAType(var->type, var->is_ptr);
   stream << tp << " " << varName << " = ";
   increment = ir::simplify(increment);
   if (!isa<Literal>(increment) || !to<Literal>(increment)->equalsScalar(1)) {
-    stream << "(blockIdx.x * blockDim.x + threadIdx.x) * ";
+    stream << "(threadIdx.x";
+    stream << " % (";
+    numThreads.accept(this);
+    stream << ")) * ";
     increment.accept(this);
   }
   else {
-    stream << "blockIdx.x * blockDim.x + threadIdx.x";
+    stream << "(threadIdx.x";
+    stream << " % (";
+    numThreads.accept(this);
+    stream << "))";
   }
   Expr expr = ir::simplify(start);
   if (!isa<Literal>(expr) || !to<Literal>(expr)->equalsScalar(0)) {
     stream << " + ";
     expr.accept(this);
   }
   stream << ";\n";
 }
 
-void CodeGen_CUDA::printThreadBoundCheck(pair<string, Expr> threadIDVar, Expr end) {
-  taco_iassert(threadIDVar.second.as<Var>()) << "Unable to convert output " << threadIDVar.second
-                                             << " to Var";
-  string varName = threadIDVar.first;
+void CodeGen_CUDA::printWarpIDVariable(pair<string, Expr> warpIDVar, Expr start, Expr increment, Expr warpSize) {
+  auto var = warpIDVar.second.as<Var>();
+  taco_iassert(var) << "Unable to convert output " << warpIDVar.second
+                    << " to Var";
+  string varName = warpIDVar.first;
+  auto tp = printCUDAType(var->type, var->is_ptr);
+  stream << tp << " " << varName << " = ";
+  increment = ir::simplify(increment);
+  if (!isa<Literal>(increment) || !to<Literal>(increment)->equalsScalar(1)) {
+    stream << "(threadIdx.x / ";
+    stream << warpSize << ") * ";
+    increment.accept(this);
+  }
+  else {
+    stream << "(threadIdx.x / ";
+    stream << warpSize;
+    stream << ")";
+  }
+  Expr expr = ir::simplify(start);
+  if (!isa<Literal>(expr) || !to<Literal>(expr)->equalsScalar(0)) {
+    stream << " + ";
+    expr.accept(this);
+  }
+  stream << ";\n";
+}
+
+void CodeGen_CUDA::printBlockIDVariable(pair<string, Expr> blockIDVar, Expr start, Expr increment) {
+  auto var = blockIDVar.second.as<Var>();
+  taco_iassert(var) << "Unable to convert output " << blockIDVar.second
+                    << " to Var";
+  string varName = blockIDVar.first;
+  auto tp = printCUDAType(var->type, var->is_ptr);
+  stream << tp << " " << varName << " = ";
+  increment = ir::simplify(increment);
+  if (!isa<Literal>(increment) || !to<Literal>(increment)->equalsScalar(1)) {
+    stream << "blockIdx.x * ";
+    increment.accept(this);
+  }
+  else {
+    stream << "blockIdx.x";
+  }
+  Expr expr = ir::simplify(start);
+  if (!isa<Literal>(expr) || !to<Literal>(expr)->equalsScalar(0)) {
+    stream << " + ";
+    expr.accept(this);
+  }
+  stream << ";\n";
+}
+
+void CodeGen_CUDA::printThreadBoundCheck(Expr end) {
   end = ir::simplify(end);
-  stream << "if (" << varName << " >= ";
+  stream << "if (threadIdx.x >= ";
   end.accept(this);
   stream << ") {" << "\n";
   indent++;
   doIndent();
   stream << "return;\n";
   indent--;
   doIndent();
   stream << "}" << "\n" << "\n";
 }
 
-void CodeGen_CUDA::printDeviceFuncCall(const vector<pair<string, Expr>> currentParameters, int index, Expr start, Expr end, Expr increment) {
+void CodeGen_CUDA::printDeviceFuncCall(const vector<pair<string, Expr>> currentParameters, Expr blockSize, int index, Expr gridSize) {
+  if (GEN_TIMING_CODE && !emittedTimerStartCode) {
+    doIndent();
+    stream << "float tot_ms;" << endl;
+    doIndent();
+    stream << "cudaEvent_t event1, event2;" << endl;
+    doIndent();
+    stream << "cudaEventCreate(&event1);" << endl;
+    doIndent();
+    stream << "cudaEventCreate(&event2);" << endl;
+    doIndent();
+    stream << "cudaDeviceSynchronize();" << endl;
+    doIndent();
+    stream << "cudaEventRecord(event1,0);" << endl;
+    emittedTimerStartCode = true;
+  }
+
+
   stream << funcName << "DeviceKernel" << index << "<<<";
-  // ensure always rounds up
-  Expr loopIterations = Div::make(Add::make(Sub::make(end, start), Sub::make(increment, Literal::make(1, Int()))), increment);
-  loopIterations = ir::simplify(loopIterations);
-  Expr blockSize = Div::make(Add::make(loopIterations, Literal::make(CUDA_BLOCK_SIZE - 1, Int())), Literal::make(CUDA_BLOCK_SIZE));
-  blockSize = ir::simplify(blockSize);
+  gridSize = ir::simplify(gridSize);
+  gridSize.accept(this);
+  stream << ", ";
   blockSize.accept(this);
-  stream << ", " << CUDA_BLOCK_SIZE << ">>>";
+  stream << ">>>";
   stream << "(";
 
   string delimiter = "";
   for (size_t i=0; i<currentParameters.size(); i++) {
     taco_iassert(currentParameters[i].second.as<Var>()) << "Unable to convert output " << currentParameters[i].second
                                                         << " to Var";
     string varName = currentParameters[i].first;
     stream << delimiter << varName;
 
     delimiter = ", ";
   }
   stream << ");\n";
+
+  if (GEN_TIMING_CODE) {
+    doIndent();
+    stream << "cudaEventRecord(event2,0);\n";
+    doIndent();
+    stream << "cudaEventSynchronize(event1);\n";
+    doIndent();
+    stream << "cudaEventSynchronize(event2);\n";
+    doIndent();
+    stream << "cudaEventElapsedTime(&tot_ms, event1, event2);\n";
+  }
   doIndent();
   stream << "cudaDeviceSynchronize();\n";
+
 }
 
 
 CodeGen_CUDA::CodeGen_CUDA(std::ostream &dest, OutputKind outputKind)
       : CodeGen(dest, false, false, CUDA), out(dest), outputKind(outputKind) {}
 
 CodeGen_CUDA::~CodeGen_CUDA() {}
 
 void CodeGen_CUDA::compile(Stmt stmt, bool isFirst) {
+  deviceFunctionParameters = {};
+  varMap = {};
+  localVars = {};
+  deviceFunctionBlockSizes = {};
+  deviceFunctionGridSizes = {};
+  deviceFunctions = {};
+  scalarVarsPassedToDeviceFunction = {};
+  deviceFunctionLoopDepth = 0;
+  parentParallelUnits = {};
+  parallelUnitSizes = {};
+  parallelUnitIDVars = {};
+  emittedTimerStartCode = false;
+  isHostFunction = true;
   if (isFirst) {
     // output the headers
     out << cHeaders;
     if (outputKind == ImplementationGen) {
       out << endl << gpuAssertMacro;
     }
   }
@@ -392,47 +642,92 @@
   stmt = simplifyFunctionBodies(stmt);
   stmt.accept(this);
 }
 
 void CodeGen_CUDA::printDeviceFunctions(const Function* func) {
   // Collect device functions
   resetUniqueNameCounters();
+  deviceFunctionLoopDepth = 0;
   DeviceFunctionCollector deviceFunctionCollector(func->inputs, func->outputs, this);
   func->body.accept(&deviceFunctionCollector);
-  deviceFunctions = deviceFunctionCollector.deviceFunctions;
+  deviceFunctions = deviceFunctionCollector.blockFors;
   deviceFunctionParameters = deviceFunctionCollector.functionParameters;
+  for (int i = 0; i < (int) deviceFunctionCollector.numThreads.size(); i++) {
+    Expr blockSize = deviceFunctionCollector.numThreads[i];
+    if (deviceFunctionCollector.warpFors[i].defined()) {
+      blockSize = Mul::make(blockSize, deviceFunctionCollector.numWarps[i]);
+    }
+    deviceFunctionBlockSizes.push_back(blockSize);
+
+    const For *blockloop = to<For>(deviceFunctions[i]);
+    Expr gridSize = Div::make(Add::make(Sub::make(blockloop->end, blockloop->start), Sub::make(blockloop->increment, Literal::make(1, Int()))), blockloop->increment);
+    deviceFunctionGridSizes.push_back(gridSize);
+  }
 
   resetUniqueNameCounters();
   for (size_t i = 0; i < deviceFunctions.size(); i++) {
-    const For *forloop = to<For>(deviceFunctions[i]);
-    Stmt function = forloop->contents;
+    const For *blockloop = to<For>(deviceFunctions[i]);
+    taco_iassert(blockloop->parallel_unit == ParallelUnit::GPUBlock);
+    const For *threadloop = to<For>(deviceFunctionCollector.threadFors[i]);
+    taco_iassert(threadloop->parallel_unit == ParallelUnit::GPUThread);
+    Stmt function = blockloop->contents;
     vector<pair<string, Expr>> parameters = deviceFunctionParameters[i];
+
+    // add scalar parameters to set
+    for (auto parameter : parameters) {
+      auto var = parameter.second.as<Var>();
+      if (!var->is_tensor && !var->is_ptr) {
+        scalarVarsPassedToDeviceFunction.insert(parameter.second);
+      }
+    }
+
     // Generate device function header
     doIndent();
     out << printDeviceFuncName(parameters, i);
     out << "{\n";
     indent++;
 
     // Generate device function code
     resetUniqueNameCounters();
     vector<Expr> inputs;
     for (size_t i = 0; i < parameters.size(); i++) {
       inputs.push_back(parameters[i].second);
     }
-    inputs.push_back(deviceFunctionCollector.threadIDVars[i].second);
+
+    parallelUnitIDVars = {{ParallelUnit::GPUBlock, deviceFunctionCollector.blockIDVars[i].second},
+                          {ParallelUnit::GPUThread, deviceFunctionCollector.threadIDVars[i].second}};
+
+    parallelUnitSizes = {{ParallelUnit::GPUBlock, deviceFunctionBlockSizes[i]}};
+
+    if (deviceFunctionCollector.warpFors[i].defined()) {
+      parallelUnitIDVars[ParallelUnit::GPUWarp] = deviceFunctionCollector.warpIDVars[i].second;
+      parallelUnitSizes[ParallelUnit::GPUWarp] = deviceFunctionCollector.numThreads[i];
+    }
+
+    for (auto idVar : parallelUnitIDVars) {
+      inputs.push_back(idVar.second);
+    }
+
     FindVars varFinder(inputs, {}, this);
-    forloop->accept(&varFinder);
+    blockloop->accept(&varFinder);
     varMap = varFinder.varMap;
 
     // Print variable declarations
     out << printDecls(varFinder.varDecls, inputs, {}) << endl;
     doIndent();
-    printThreadIDVariable(deviceFunctionCollector.threadIDVars[i], forloop->start, forloop->increment);
+    printBlockIDVariable(deviceFunctionCollector.blockIDVars[i], blockloop->start, blockloop->increment);
     doIndent();
-    printThreadBoundCheck(deviceFunctionCollector.threadIDVars[i], forloop->end);
+    printThreadIDVariable(deviceFunctionCollector.threadIDVars[i], threadloop->start, threadloop->increment, deviceFunctionCollector.numThreads[i]);
+    if (deviceFunctionCollector.warpFors[i].defined()) {
+      doIndent();
+      const For *warploop = to<For>(deviceFunctionCollector.warpFors[i]);
+      printWarpIDVariable(deviceFunctionCollector.warpIDVars[i], warploop->start, warploop->increment, deviceFunctionCollector.numThreads[i]);
+    }
+    doIndent();
+    printThreadBoundCheck(deviceFunctionBlockSizes[i]);
 
     // output body
     print(function);
 
     // output repack only if we allocated memory
     if (checkForAlloc(func))
       out << endl << printPack(varFinder.outputProperties, func->outputs);
@@ -447,15 +742,17 @@
   // if generating a header, protect the function declaration with a guard
   if (outputKind == HeaderGen) {
     out << "#ifndef TACO_GENERATED_" << func->name << "\n";
     out << "#define TACO_GENERATED_" << func->name << "\n";
   }
   else {
     emittingCoroutine = false;
+    isHostFunction = false;
     printDeviceFunctions(func);
+    isHostFunction = true;
   }
 
   int numYields = countYields(func);
   emittingCoroutine = (numYields > 0);
   labelCount = 0;
 
   // Generate rest of code + calls to device functions
@@ -498,15 +795,20 @@
     out << endl << printPack(varFinder.outputProperties, func->outputs);
 
   if (emittingCoroutine) {
     out << printCoroutineFinish(numYields, funcName);
   }
 
   doIndent();
-  out << "return 0;\n";
+  if (GEN_TIMING_CODE && emittedTimerStartCode && func->name.rfind("compute", 0) == 0) {
+    out << "return (int) (tot_ms * 100000); // returns 10^-8 seconds (assumes tot_ms < 20 seconds)\n";
+  }
+  else {
+    out << "return 0;\n";
+  }
   indent--;
 
   doIndent();
   out << "}\n";
 }
 
 // For Vars, we replace their names with the generated name,
@@ -539,27 +841,65 @@
   ret << "#pragma omp parallel for";
   if (kind == LoopKind::Dynamic) {
     ret << " schedule(dynamic, 16)";
   }
   return ret.str();
 }
 
+static string getAtomicPragma() {
+  return "#pragma omp atomic";
+}
+
+static string getUnrollPragma(size_t unrollFactor) {
+  return "#pragma unroll " + std::to_string(unrollFactor);
+}
+
 // The next two need to output the correct pragmas depending
 // on the loop kind (Serial, Static, Dynamic, Vectorized)
 //
 // Docs for vectorization pragmas:
 // http://clang.llvm.org/docs/LanguageExtensions.html#extensions-for-loop-hint-optimizations
 void CodeGen_CUDA::visit(const For* op) {
+  if (op->parallel_unit != ParallelUnit::NotParallel) {
+    parentParallelUnits.insert(op->parallel_unit);
+  }
+
+  if (!isHostFunction && (op->parallel_unit == ParallelUnit::GPUThread || op->parallel_unit == ParallelUnit::GPUWarp)) {
+    // Don't emit thread loop
+    indent--;
+    op->contents.accept(this);
+    indent++;
+    return;
+  }
+
+  // only first thread
+  if (!isHostFunction && (op->parallel_unit == ParallelUnit::GPUWarpReduction || op->parallel_unit == ParallelUnit::GPUBlockReduction)) {
+    doIndent();
+    if (op->parallel_unit == ParallelUnit::GPUWarpReduction) {
+      stream << "__syncwarp();" << endl;
+    }
+    else if (op->parallel_unit == ParallelUnit::GPUBlockReduction) {
+      stream << "__syncthreads();" << endl;
+    }
+    doIndent();
+    stream << keywordString("if") << " (";
+    op->var.accept(this);
+    stream << " == ";
+    op->start.accept(this);
+    stream << ") {" << endl;
+    indent++;
+  }
+
   for (size_t i = 0; i < deviceFunctions.size(); i++) {
     auto dFunction = deviceFunctions[i].as<For>();
     assert(dFunction);
     if (op == dFunction) {
       // Generate kernel launch
       doIndent();
-      printDeviceFuncCall(deviceFunctionParameters[i], i, op->start, op->end, op->increment);
+      printDeviceFuncCall(deviceFunctionParameters[i], deviceFunctionBlockSizes[i], i, deviceFunctionGridSizes[i]);
       return;
     }
   }
 
   switch (op->kind) {
     case LoopKind::Vectorized:
       doIndent();
@@ -567,15 +907,20 @@
       out << "\n";
       break;
     case LoopKind::Static:
     case LoopKind::Dynamic:
       doIndent();
       out << getParallelizePragma(op->kind);
       out << "\n";
+      break;
     default:
+      if (op->unrollFactor > 0) {
+        doIndent();
+        out << getUnrollPragma(op->unrollFactor) << endl;
+      }
       break;
   }
 
   doIndent();
   stream << keywordString("for") << " (";
   if (!emittingCoroutine) {
     stream << keywordString(printCUDAType(op->var.type(), false)) << " ";
@@ -598,18 +943,34 @@
   }
   else {
     stream << " += ";
     op->increment.accept(this);
   }
   stream << ") {\n";
 
+  if(!isHostFunction) {
+    deviceFunctionLoopDepth++;
+  }
   op->contents.accept(this);
+  if(!isHostFunction) {
+    deviceFunctionLoopDepth--;
+  }
   doIndent();
   stream << "}";
   stream << endl;
+
+  if (!isHostFunction && (op->parallel_unit == ParallelUnit::GPUWarpReduction || op->parallel_unit == ParallelUnit::GPUBlockReduction)) {
+    indent--;
+    doIndent();
+    stream << "}" << endl;
+  }
+
+  if (op->parallel_unit != ParallelUnit::NotParallel) {
+    parentParallelUnits.erase(op->parallel_unit);
+  }
 }
 
 void CodeGen_CUDA::visit(const While* op) {
   // it's not clear from documentation that clang will vectorize
   // while loops
   // however, we'll output the pragmas anyway
   if (op->kind == LoopKind::Vectorized) {
@@ -640,23 +1001,77 @@
   op->operands.back().accept(this);
   for (size_t i=0; i<op->operands.size()-1; i++) {
     stream << ")";
   }
 }
 
 void CodeGen_CUDA::visit(const Max* op) {
-  stream << "TACO_MAX(";
-  op->a.accept(this);
-  stream << ", ";
-  op->b.accept(this);
-  stream << ")";
+  if (op->operands.size() == 1) {
+    op->operands[0].accept(this);
+    return;
+  }
+  for (size_t i=0; i<op->operands.size()-1; i++) {
+    stream << "TACO_MAX(";
+    op->operands[i].accept(this);
+    stream << ",";
+  }
+  op->operands.back().accept(this);
+  for (size_t i=0; i<op->operands.size()-1; i++) {
+    stream << ")";
+  }
 }
 
 void CodeGen_CUDA::visit(const Allocate* op) {
   string elementType = printCUDAType(op->var.type(), false);
+  if (!isHostFunction) {
+    if (parentParallelUnits.count(ParallelUnit::GPUThread)) {
+      // double w_GPUThread[num];
+      // for threads allocate thread local memory
+      doIndent();
+      stream << elementType << " ";
+      op->var.accept(this);
+      stream << "[";
+      op->num_elements.accept(this);
+      stream << "];" << endl;
+      return;
+    }
+    // __shared__ double w_GPUThread[32]; if no warps
+    // __shared__ double w_GPUThread_ALL[32 * # num warps]; if warps
+    // double * w_GPUThread = w_GPUThread_ALL + warp_id * 32;
+    taco_iassert(!op->is_realloc);
+    doIndent();
+    stream << "__shared__ " << elementType << " ";
+    op->var.accept(this);
+    if (parentParallelUnits.count(ParallelUnit::GPUWarp)) {
+      stream << "_ALL";
+    }
+    stream << "[";
+    if (parentParallelUnits.count(ParallelUnit::GPUWarp)) {
+      Expr numElements = Mul::make(op->num_elements, Div::make(parallelUnitSizes[ParallelUnit::GPUBlock], parallelUnitSizes[ParallelUnit::GPUWarp]));
+      ir::simplify(numElements).accept(this);
+    }
+    else {
+      op->num_elements.accept(this);
+    }
+    stream << "];" << endl;
+    if (parentParallelUnits.count(ParallelUnit::GPUWarp)) {
+      doIndent();
+      stream << elementType << " * ";
+      op->var.accept(this);
+
+      stream << " = ";
+      op->var.accept(this);
+      stream << "_ALL + ";
+      parallelUnitIDVars[ParallelUnit::GPUWarp].accept(this);
+      stream << " * ";
+      parallelUnitSizes[ParallelUnit::GPUWarp].accept(this);
+      stream << ";" << endl;
+    }
+    return;
+  }
   string variable_name;
   if (op->is_realloc) {
     // cuda doesn't have realloc
     // void * tmp_realloc_ptr;
     // gpuErrchk(cudaMallocManaged((void**)& tmp_realloc_ptr, new_size);
     // memcpy(tmp_realloc_ptr, var, TACO_MIN(old_size, new_size));
     // cudaFree(var);
@@ -678,14 +1093,28 @@
   stream << ", ";
   stream << "sizeof(" << elementType << ")";
   stream << " * ";
   parentPrecedence = MUL;
   op->num_elements.accept(this);
   parentPrecedence = TOP;
   stream << "));" << endl;
+  // If the operation wants the input cleared, then memset it to zero.
+  if (op->clear) {
+    doIndent();
+    stream << "gpuErrchk(cudaMemset(";
+    op->var.accept(this);
+    stream << variable_name;
+    stream << ", 0, ";
+    stream << "sizeof(" << elementType << ")";
+    stream << " * ";
+    parentPrecedence = MUL;
+    op->num_elements.accept(this);
+    parentPrecedence = TOP;
+    stream << "));" << endl;
+  }
 
   if(op->is_realloc) {
     doIndent();
     stream << "memcpy(" << variable_name << ", ";
     op->var.accept(this);
     stream << ", ";
     stream << "TACO_MIN(";
@@ -703,35 +1132,95 @@
     doIndent();
     op->var.accept(this);
     stream << " = (" << printCUDAType(op->var.type(), true) << ") " << variable_name << ";" << endl;
   }
 
 }
 
+void CodeGen_CUDA::visit(const Free* op) {
+  if (!isHostFunction) {
+    // Don't need to free shared memory
+    return;
+  }
+  doIndent();
+  stream << "cudaFree(";
+  parentPrecedence = Precedence::TOP;
+  op->var.accept(this);
+  stream << ");";
+  stream << endl;
+}
+
 void CodeGen_CUDA::visit(const Sqrt* op) {
   taco_tassert(op->type.isFloat() && op->type.getNumBits() == 64) <<
                                                                   "Codegen doesn't currently support non-double sqrt";
   stream << "sqrt(";
   op->a.accept(this);
   stream << ")";
 }
 
+void CodeGen_CUDA::visit(const Continue*) {
+  doIndent();
+  if(!isHostFunction && deviceFunctionLoopDepth == 0) {
+    // can't break out of kernel
+    stream << "return;" << endl;
+  }
+  else {
+    stream << "break;" << endl;
+  }
+}
+
 void CodeGen_CUDA::visit(const VarDecl* op) {
   if (emittingCoroutine) {
     doIndent();
     op->var.accept(this);
     parentPrecedence = Precedence::TOP;
     stream << " = ";
     op->rhs.accept(this);
     stream << ";";
     stream << endl;
   }
+  // f var can be passed to device function then allocated in uvm
+  else if (scalarVarsPassedToDeviceFunction.count(op->var) && isHostFunction) {
+    // type *x_ptr;
+    // gpuErrchk(cudaMallocManaged((void**)&x_ptr, sizeof(type));
+    // type &x = *x_ptr;
+    // x = rhs;
+    doIndent();
+    stream << keywordString(printCUDAType(op->var.type(), true)) << " ";
+    string varName = varNameGenerator.getUniqueName(util::toString(op->var));
+    varNames.insert({op->var, varName});
+    op->var.accept(this);
+    stream << "_ptr;" << endl;
+    parentPrecedence = Precedence ::TOP;
+
+    doIndent();
+    stream << "gpuErrchk(cudaMallocManaged((void**)&";
+    op->var.accept(this);
+    stream << "_ptr, sizeof(" << keywordString(printCUDAType(op->var.type(), false)) << ")));" << endl;
+
+    doIndent();
+    stream << keywordString(printCUDAType(op->var.type(), false)) << "& ";
+    op->var.accept(this);
+    stream << " = *";
+    op->var.accept(this);
+    stream << "_ptr;" << endl;
+
+    doIndent();
+    op->var.accept(this);
+    stream << " = ";
+    op->rhs.accept(this);
+    stream << ";" << endl;
+  }
   else {
+    bool is_ptr = false;
+    if (isa<Var>(op->var)) {
+      is_ptr = to<Var>(op->var)->is_ptr;
+    }
     doIndent();
-    stream << keywordString(printCUDAType(op->var.type(), false)) << " ";
+    stream << keywordString(printCUDAType(op->var.type(), is_ptr)) << " ";
     string varName = varNameGenerator.getUniqueName(util::toString(op->var));
     varNames.insert({op->var, varName});
     op->var.accept(this);
     parentPrecedence = Precedence::TOP;
     stream << " = ";
     op->rhs.accept(this);
     stream << ";";
@@ -741,16 +1230,17 @@
 
 void CodeGen_CUDA::visit(const Yield* op) {
   printYield(op, localVars, varMap, labelCount, funcName);
 }
 
 // Need to handle some binary ops so that we can add the necessary casts if complex
 // Because c++ does not properly handle double * std::complex<float> or std::complex<float> * std::complex<double>
+// Based on IRPrinter::printBinOp
 void CodeGen_CUDA::printBinCastedOp(Expr a, Expr b, string op, Precedence precedence) {
-  bool parenthesize = precedence > parentPrecedence;
+  bool parenthesize = needsParentheses(precedence);
   if (parenthesize) {
     stream << "(";
   }
   parentPrecedence = precedence;
   Datatype mType = max_type(a.type(), b.type());
   if (mType.isComplex() && mType != a.type()) {
     stream << "(" << printCUDAType(mType, false) << ") ";
@@ -807,20 +1297,29 @@
   }
   else {
     IRPrinter::visit(op);
   }
 }
 
 void CodeGen_CUDA::visit(const Call* op) {
+  if (op->func == "cudaMemset") {
+    IRPrinter::visit(op);
+    return;
+  }
   stream << op->func << "(";
   parentPrecedence = Precedence::CALL;
 
-  // Need to print cast to type so that arguments match
+  // Need to print cast to type so that arguments match.
   if (op->args.size() > 0) {
-    if (op->type != op->args[0].type() || isa<Literal>(op->args[0])) {
+    // However, the binary search arguments take int* as their first
+    // argument. This pointer information isn't carried anywhere in
+    // the argument expressions, so we need to special case and not
+    // emit an invalid cast for that argument.
+    auto opIsBinarySearch = op->func == "taco_binarySearchAfter" || op->func == "taco_binarySearchBefore";
+    if (!opIsBinarySearch && (op->type != op->args[0].type() || isa<Literal>(op->args[0]))) {
       stream << "(" << printCUDAType(op->type, false) << ") ";
     }
     op->args[0].accept(this);
   }
 
   for (size_t i=1; i < op->args.size(); ++i) {
     stream << ", ";
@@ -828,14 +1327,179 @@
       stream << "(" << printCUDAType(op->type, false) << ") ";
     }
     op->args[i].accept(this);
   }
 
   stream << ")";
 }
+
+void CodeGen_CUDA::visit(const Assign* op) {
+  if (GEN_TIMING_CODE && !emittedTimerStartCode && isa<ir::Call>(op->rhs)) {
+    if (to<ir::Call>(op->rhs)->func == "taco_binarySearchBeforeBlockLaunch") {
+      doIndent();
+      stream << "float tot_ms;" << endl;
+      doIndent();
+      stream << "cudaEvent_t event1, event2;" << endl;
+      doIndent();
+      stream << "cudaEventCreate(&event1);" << endl;
+      doIndent();
+      stream << "cudaEventCreate(&event2);" << endl;
+      doIndent();
+      stream << "cudaDeviceSynchronize();" << endl;
+      doIndent();
+      stream << "cudaEventRecord(event1,0);" << endl;
+      emittedTimerStartCode = true;
+    }
+  }
+
+  if (op->use_atomics) {
+    if (isHostFunction) {
+      doIndent();
+      stream << getAtomicPragma() << endl;
+      IRPrinter::visit(op);
+    }
+    else {
+      if (isa<Mul>(op->rhs)) {
+        auto mul = to<Mul>(op->rhs);
+        taco_iassert(mul->a == op->lhs);
+        doIndent();
+        // type atomicOldX = rhs;
+        string oldValueName = genUniqueName("atomicOld");
+        stream << printCUDAType(op->lhs.type(), false);
+        stream << " " << oldValueName << " = ";
+        op->lhs.accept(this);
+        stream << ";";
+
+        doIndent();
+        stream << "atomicCAS(&";
+        op->lhs.accept(this);
+        stream << ", " << oldValueName << ", ";
+        stream << oldValueName << " * ";
+        mul->b.accept(this);
+        stream << ");" << endl;
+      } else if (isa<Add>(op->rhs)) {
+        auto add = to<Add>(op->rhs);
+        taco_iassert(add->a == op->lhs);
+        doIndent();
+        stream << "atomicAdd(&";
+        op->lhs.accept(this);
+        stream << ", ";
+        add->b.accept(this);
+        stream << ");" << endl;
+      } else if (isa<BitOr>(op->rhs)) {
+        auto bitOr = to<BitOr>(op->rhs);
+        taco_iassert(bitOr->a == op->lhs);
+        doIndent();
+        stream << "atomicOr(&";
+        op->lhs.accept(this);
+        stream << ", ";
+        bitOr->b.accept(this);
+        stream << ");" << endl;
+      } else {
+        taco_ierror;
+      }
+    }
+  }
+  else {
+    IRPrinter::visit(op);
+  }
+}
+
+void CodeGen_CUDA::visit(const Store* op) {
+  if (op->use_atomics) {
+    if (isHostFunction) {
+      doIndent();
+      stream << getAtomicPragma() << endl;
+      IRPrinter::visit(op);
+    }
+    else {
+      if (isa<Mul>(op->data)) {
+        auto mul = to<Mul>(op->data);
+        taco_iassert(isa<Load>(mul->a));
+        auto load = to<Load>(mul->a);
+        taco_iassert(load->arr == op->arr && load->loc == op->loc);
+        doIndent();
+        // type atomicOldX = rhs;
+        string oldValueName = genUniqueName("atomicOld");
+        stream << printCUDAType(load->type, false);
+        stream << " " << oldValueName << " = ";
+        op->arr.accept(this);
+        stream << "[";
+        parentPrecedence = Precedence::TOP;
+        op->loc.accept(this);
+        stream << "];";
+
+        doIndent();
+        stream << "atomicCAS(&";
+
+        op->arr.accept(this);
+        stream << "[";
+        parentPrecedence = Precedence::TOP;
+        op->loc.accept(this);
+        stream << "]";
+
+        stream << ", " << oldValueName << ", ";
+        stream << oldValueName << " * ";
+        mul->b.accept(this);
+        stream << ");" << endl;
+      } else if (isa<Add>(op->data)) {
+        auto add = to<Add>(op->data);
+        taco_iassert(isa<Load>(add->a));
+        taco_iassert(to<Load>(add->a)->arr == op->arr && to<Load>(add->a)->loc == op->loc);
+        if (deviceFunctionLoopDepth == 0 || op->atomic_parallel_unit == ParallelUnit::GPUWarp) {
+          // use atomicAddWarp
+          doIndent();
+          stream << "atomicAddWarp<" << printCUDAType(add->b.type(), false) << ">(";
+          op->arr.accept(this);
+          stream << ", ";
+          op->loc.accept(this);
+          stream << ", ";
+          add->b.accept(this);
+          stream << ");" << endl;
+        }
+        else {
+          doIndent();
+          stream << "atomicAdd(&";
+
+          op->arr.accept(this);
+          stream << "[";
+          parentPrecedence = Precedence::TOP;
+          op->loc.accept(this);
+          stream << "]";
+
+          stream << ", ";
+          add->b.accept(this);
+          stream << ");" << endl;
+        }
+      } else if (isa<BitOr>(op->data)) {
+        auto bitOr = to<BitOr>(op->data);
+        taco_iassert(isa<Load>(bitOr->a));
+        taco_iassert(to<Load>(bitOr->a)->arr == op->arr && to<Load>(bitOr->a)->loc == op->loc);
+
+        doIndent();
+        stream << "atomicOr(&";
+
+        op->arr.accept(this);
+        stream << "[";
+        parentPrecedence = Precedence::TOP;
+        op->loc.accept(this);
+        stream << "]";
+
+        stream << ", ";
+        bitOr->b.accept(this);
+        stream << ");" << endl;
+      } else {
+        taco_ierror;
+      }
+    }
+  }
+  else {
+    IRPrinter::visit(op);
+  }
+}
   
 void CodeGen_CUDA::generateShim(const Stmt& func, stringstream &ret) {
   const Function *funcPtr = func.as<Function>();
   ret << "extern \"C\" {\n";
   ret << "  int _shim_" << funcPtr->name << "(void** parameterPack);\n";
   ret << "}\n\n";
```

### Comparing `tensora-0.0.6/src/taco/src/codegen/codegen_cuda.h` & `tensora-0.0.7/src/taco/src/codegen/codegen_cuda.h`

 * *Files 12% similar despite different names*

```diff
@@ -40,27 +40,44 @@
   void visit(const Sub*);
   void visit(const Mul*);
   void visit(const Div*);
   void visit(const VarDecl*);
   void visit(const Literal*);
   void visit(const Yield*);
   void visit(const Call*);
+  void visit(const Store*);
+  void visit(const Assign*);
+  void visit(const Continue*);
+  void visit(const Free* op);
   std::string printDeviceFuncName(const std::vector<std::pair<std::string, Expr>> currentParameters, int index);
-  void printDeviceFuncCall(const std::vector<std::pair<std::string, Expr>> currentParameters, int index, Expr start, Expr end, Expr increment);
-  void printThreadIDVariable(std::pair<std::string, Expr> threadIDVar, Expr start, Expr increment);
-  void printThreadBoundCheck(std::pair<std::string, Expr> threadIDVar, Expr end);
+  void printDeviceFuncCall(const std::vector<std::pair<std::string, Expr>> currentParameters, Expr blockSize, int index, Expr gridSize);
+  void printThreadIDVariable(std::pair<std::string, Expr> threadIDVar, Expr start, Expr increment, Expr numThreads);
+  void printBlockIDVariable(std::pair<std::string, Expr> blockIDVar, Expr start, Expr increment);
+  void printWarpIDVariable(std::pair<std::string, Expr> warpIDVar, Expr start, Expr increment, Expr warpSize);
+  void printThreadBoundCheck(Expr end);
   void printDeviceFunctions(const Function* func);
   void printBinCastedOp(Expr a, Expr b, std::string op, Precedence precedence);
   Stmt simplifyFunctionBodies(Stmt stmt);
 
+  bool isHostFunction=true;
+
   std::map<Expr, std::string, ExprCompare> varMap;
   std::vector<Expr> localVars;
 
   std::vector<std::vector<std::pair<std::string, Expr>>> deviceFunctionParameters;
+  std::vector<Expr> deviceFunctionBlockSizes;
+  std::vector<Expr> deviceFunctionGridSizes;
   std::vector<Stmt> deviceFunctions; // expressions to replace to calls of device function
+  std::set<Expr> scalarVarsPassedToDeviceFunction; // need to be allocated in uvm
+  int deviceFunctionLoopDepth;
+  std::set<ParallelUnit> parentParallelUnits;
+  std::map<ParallelUnit, Expr> parallelUnitSizes;
+  std::map<ParallelUnit, Expr> parallelUnitIDVars;
+
+  bool emittedTimerStartCode = false;
 
   std::ostream &out;
   
   OutputKind outputKind;
 
   std::string funcName;
   int labelCount;
```

### Comparing `tensora-0.0.6/src/taco/src/codegen/module.cpp` & `tensora-0.0.7/src/taco/src/codegen/module.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -17,32 +17,27 @@
 #include "taco/cuda.h"
 
 using namespace std;
 
 namespace taco {
 namespace ir {
 
+std::string Module::chars = "abcdefghijkmnpqrstuvwxyz0123456789";
+std::default_random_engine Module::gen = std::default_random_engine();
+std::uniform_int_distribution<int> Module::randint =
+    std::uniform_int_distribution<int>(0, chars.length() - 1);
+
 void Module::setJITTmpdir() {
   tmpdir = util::getTmpdir();
 }
 
 void Module::setJITLibname() {
-  string chars = "abcdefghijkmnpqrstuvwxyz0123456789";
   libname.resize(12);
   for (int i=0; i<12; i++)
-    libname[i] = chars[rand() % chars.length()];
-}
-
-void Module::reset() {
-  funcs.clear();
-  moduleFromUserSource = false;
-  header.str("");
-  header.clear();
-  source.str("");
-  source.clear();
+    libname[i] = chars[randint(gen)];
 }
 
 void Module::addFunction(Stmt func) {
   funcs.push_back(func);
 }
 
 void Module::compileToSource(string path, string prefix) {
@@ -118,30 +113,37 @@
   string fullpath = prefix + ".so";
   
   string cc;
   string cflags;
   string file_ending;
   string shims_file;
   if (should_use_CUDA_codegen()) {
-    cc = "nvcc";
+    cc = util::getFromEnv("TACO_NVCC", "nvcc");
     cflags = util::getFromEnv("TACO_NVCCFLAGS",
     get_default_CUDA_compiler_flags());
     file_ending = ".cu";
     shims_file = prefix + "_shims.cpp";
   }
   else {
     cc = util::getFromEnv(target.compiler_env, target.compiler);
-    cflags = util::getFromEnv("TACO_CFLAGS",
-    "-O3 -ffast-math -std=c99") + " -shared -fPIC";
+#ifdef TACO_DEBUG
+    // In debug mode, compile the generated code with debug symbols and a
+    // low optimization level.
+    string defaultFlags = "-g -O0 -std=c99";
+#else
+    // Otherwise, use the standard set of optimizing flags.
+    string defaultFlags = "-O3 -ffast-math -std=c99";
+#endif
+    cflags = util::getFromEnv("TACO_CFLAGS", defaultFlags) + " -shared -fPIC";
+#if USE_OPENMP
+    cflags += " -fopenmp";
+#endif
     file_ending = ".c";
     shims_file = "";
   }
-#if USE_OPENMP
-  cflags += " -fopenmp";
-#endif
   
   string cmd = cc + " " + cflags + " " +
     prefix + file_ending + " " + shims_file + " " + 
     "-o " + fullpath + " -lm";
 
   // open the output file & write out the source
   compileToSource(tmpdir, libname);
@@ -155,15 +157,15 @@
     << "\nreturned " << err;
 
   // use dlsym() to open the compiled library
   if (lib_handle) {
     dlclose(lib_handle);
   }
   lib_handle = dlopen(fullpath.data(), RTLD_NOW | RTLD_LOCAL);
-  taco_uassert(lib_handle) << "Failed to load generated code";
+  taco_uassert(lib_handle) << "Failed to load generated code, error is: " << dlerror();
 
   return fullpath;
 }
 
 void Module::setSource(string source) {
   this->source << source;
   moduleFromUserSource = true;
```

### Comparing `tensora-0.0.6/src/taco/src/cuda.cpp` & `tensora-0.0.7/src/taco/src/cuda.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 }
 
 #if CUDA_BUILT
   // https://stackoverflow.com/questions/14038589/what-is-the-canonical-way-to-check-for-errors-using-the-cuda-runtime-api
   #define gpuErrchk(ans) { gpuAssert((ans), __FILE__, __LINE__); }
   inline void gpuAssert(cudaError_t code, const char *file, int line, bool abort=true)
   {
-    if (code != cudaSuccess && code != 29) // 29 is driver is shutting down which is normal behavior 
+    if (code != cudaSuccess && code != cudaErrorCudartUnloading) // cudart unloading is normal behavior
     {
       taco_ierror << "GPUassert: " << code << " " << cudaGetErrorString(code) << " " << file << " " << line;
     }
   }
 #endif
 
 void* cuda_unified_alloc(size_t size) {
```

### Comparing `tensora-0.0.6/src/taco/src/error/error_checks.cpp` & `tensora-0.0.7/src/taco/src/error/error_checks.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include "error_checks.h"
 
+#include <functional>
 #include <map>
 #include <set>
-#include <stack>
-#include <functional>
+#include <tuple>
 
 #include "taco/type.h"
 #include "taco/index_notation/index_notation.h"
 #include "taco/index_notation/index_notation_nodes.h"
 #include "taco/util/strings.h"
 #include "taco/util/collections.h"
 
@@ -22,91 +22,64 @@
     std::function<void(const AccessNode*)>([&](const AccessNode* op) {
       readNodes.push_back(op);
     })
   );
   return readNodes;
 }
 
-bool dimensionsTypecheck(const std::vector<IndexVar>& resultVars,
-                         const IndexExpr& expr,
-                         const Shape& shape) {
-
-  std::map<IndexVar,Dimension> indexVarDims;
-  for (size_t mode = 0; mode < resultVars.size(); mode++) {
-    IndexVar var = resultVars[mode];
-    auto dimension = shape.getDimension(mode);
-    if (util::contains(indexVarDims,var) && indexVarDims.at(var) != dimension) {
-      return false;
-    }
-    else {
-      indexVarDims.insert({var, dimension});
-    }
-  }
-
-  vector<const AccessNode*> readNodes = getAccessNodes(expr);
-  for (auto& readNode : readNodes) {
-    for (size_t mode = 0; mode < readNode->indexVars.size(); mode++) {
-      IndexVar var = readNode->indexVars[mode];
-      Dimension dimension =
-          readNode->tensorVar.getType().getShape().getDimension(mode);
-      if (util::contains(indexVarDims,var) &&
-          indexVarDims.at(var) != dimension) {
-        return false;
-      }
-      else {
-        indexVarDims.insert({var, dimension});
-      }
-    }
-  }
-
-  return true;
-}
-
 static string addDimensionError(const IndexVar& var,
                                 Dimension dimension1, Dimension dimension2) {
   return "Index variable " + util::toString(var) + " is used to index "
          "modes of different dimensions (" + util::toString(dimension1) +
          " and " + util::toString(dimension2) + ").";
 }
 
-std::string dimensionTypecheckErrors(const std::vector<IndexVar>& resultVars,
-                                     const IndexExpr& expr,
-                                     const Shape& shape) {
+std::pair<bool, string> dimensionsTypecheck(const std::vector<IndexVar>& resultVars,
+                                            const IndexExpr& expr,
+                                            const Shape& shape) {
   vector<string> errors;
-
   std::map<IndexVar,Dimension> indexVarDims;
   for (size_t mode = 0; mode < resultVars.size(); mode++) {
     IndexVar var = resultVars[mode];
     auto dimension = shape.getDimension(mode);
-    if (util::contains(indexVarDims,var) && indexVarDims.at(var) != dimension) {
+    if (util::contains(indexVarDims,var) && indexVarDims.at(var) != dimension &&
+        !(indexVarDims.at(var).isIndexVarSized() && indexVarDims.at(var).getIndexVarSize() == var) &&
+        !(dimension.isIndexVarSized() && dimension.getIndexVarSize() == var)) {
       errors.push_back(addDimensionError(var, indexVarDims.at(var), dimension));
-    }
-    else {
+    } else {
       indexVarDims.insert({var, dimension});
     }
   }
 
   vector<const AccessNode*> readNodes = getAccessNodes(expr);
   for (auto& readNode : readNodes) {
     for (size_t mode = 0; mode < readNode->indexVars.size(); mode++) {
       IndexVar var = readNode->indexVars[mode];
-      Dimension dimension =
-          readNode->tensorVar.getType().getShape().getDimension(mode);
-      if (util::contains(indexVarDims,var) &&
-          indexVarDims.at(var) != dimension) {
-        errors.push_back(addDimensionError(var, indexVarDims.at(var),
-                                           dimension));
+      Dimension dimension = readNode->tensorVar.getType().getShape().getDimension(mode);
+
+      // If this access has windowed modes, use the dimensions of those windows
+      // as the shape, rather than the shape of the underlying tensor.
+      auto a = Access(readNode);
+      if (a.isModeWindowed(mode)) {
+        dimension = Dimension(a.getWindowSize(mode));
+      } else if (a.isModeIndexSet(mode)) {
+        dimension = Dimension(a.getIndexSet(mode).size());
       }
-      else {
+
+      if (util::contains(indexVarDims,var) && indexVarDims.at(var) != dimension &&
+        !(indexVarDims.at(var).isIndexVarSized() && indexVarDims.at(var).getIndexVarSize() == var) &&
+        !(dimension.isIndexVarSized() && dimension.getIndexVarSize() == var)) {
+        errors.push_back(addDimensionError(var, indexVarDims.at(var), dimension));
+      } else {
         indexVarDims.insert({var, dimension});
       }
     }
   }
 
-  return util::join(errors, " ");
+  return std::make_pair(errors.empty(), util::join(errors, " "));
 }
 
 static void addEdges(vector<IndexVar> indexVars, vector<int> modeOrdering,
                      map<IndexVar,set<IndexVar>>* successors) {
   if (indexVars.size() == 0) {
     return;
   }
```

### Comparing `tensora-0.0.6/src/taco/src/error/error_messages.cpp` & `tensora-0.0.7/src/taco/src/error/error_messages.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
   "Summations/reductions are not specified and the Einstein summation "
   "convention cannot be applied, because the expression is not of the form "
   "a*...*b + ... + c*...*d.";
 
 const std::string compile_without_expr =
   "The tensor must be assigned to before compile is called.";
 
+const std::string compile_tensor_name_collision =
+  "Tensor name collision.";
+
 const std::string assemble_without_compile =
   "The compile method must be called before assemble.";
 
 const std::string compute_without_compile =
    "The compile method must be called before compute.";
 
 const std::string requires_matrix =
```

### Comparing `tensora-0.0.6/src/taco/src/error.cpp` & `tensora-0.0.7/src/taco/src/error.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 #include <iostream>
 #include <cstdlib>
 
 using namespace std;
 
 namespace taco {
 
+TacoException::TacoException(std::string msg) : message(msg) {}
+
+const char* TacoException::what() const noexcept {
+  return message.c_str();
+}
+
+
 ErrorReport::ErrorReport(const char *file, const char *func, int line,
                          bool condition, const char *conditionString,
                          Kind kind, bool warning)
     : msg(NULL), file(file), func(func), line(line), condition(condition),
       conditionString(conditionString), kind(kind), warning(warning) {
   if (condition) {
     return;
@@ -48,15 +55,14 @@
       }
       (*msg) << endl;
       break;
   }
   (*msg) << " ";
 }
 
-void ErrorReport::explode() {
-  std::cerr << msg->str() << endl;
+void ErrorReport::explodeWithException() {
+  TacoException e = TacoException(msg->str());
   delete msg;
-  if (warning) return;
-  abort();
+  throw e;
 }
 
 }
```

### Comparing `tensora-0.0.6/src/taco/src/format.cpp` & `tensora-0.0.7/src/taco/src/format.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -178,14 +178,24 @@
         }
         break;
       case COMPACT:
         if (!isCompact()) {
           return false;
         }
         break;
+      case ZEROLESS:
+        if (!isZeroless()) {
+          return false;
+        }
+        break;	
+      case PADDED:
+        if (!isPadded()) {
+          return false;
+        }
+        break;	
       case NOT_FULL:
         if (isFull()) {
           return false;
         }
         break;
       case NOT_ORDERED:
         if (isOrdered()) {
@@ -203,14 +213,24 @@
         }
         break;
       case NOT_COMPACT:
         if (isCompact()) {
           return false;
         }
         break;
+      case NOT_ZEROLESS:
+        if (isZeroless()) {
+          return false;
+        }
+        break;
+      case NOT_PADDED:
+        if (isPadded()) {
+          return false;
+        }
+        break;
     }
   }
   return true;
 }
 
 bool ModeFormat::isFull() const {
   taco_iassert(defined());
@@ -233,14 +253,24 @@
 }
 
 bool ModeFormat::isCompact() const {
   taco_iassert(defined());
   return impl->isCompact;
 }
 
+bool ModeFormat::isZeroless() const {
+  taco_iassert(defined());
+  return impl->isZeroless;
+}
+
+bool ModeFormat::isPadded() const {
+  taco_iassert(defined());
+  return impl->isPadded;
+}
+
 bool ModeFormat::hasCoordValIter() const {
   taco_iassert(defined());
   return impl->hasCoordValIter;
 }
 
 bool ModeFormat::hasCoordPosIter() const {
   taco_iassert(defined());
@@ -258,14 +288,36 @@
 }
 
 bool ModeFormat::hasAppend() const {
   taco_iassert(defined());
   return impl->hasAppend;
 }
 
+bool ModeFormat::hasSeqInsertEdge() const {
+  taco_iassert(defined());
+  return impl->hasSeqInsertEdge;
+}
+
+bool ModeFormat::hasInsertCoord() const {
+  taco_iassert(defined());
+  return impl->hasInsertCoord;
+}
+
+bool ModeFormat::isYieldPosPure() const {
+  taco_iassert(defined());
+  return impl->isYieldPosPure;
+}
+
+std::vector<AttrQuery> ModeFormat::getAttrQueries(
+    std::vector<IndexVar> parentCoords, 
+    std::vector<IndexVar> childCoords) const {
+  taco_iassert(defined());
+  return impl->attrQueries(parentCoords, childCoords);
+}
+
 bool ModeFormat::defined() const {
   return impl != nullptr;
 }
 
 bool operator==(const ModeFormat& a, const ModeFormat& b) {
   return (a.defined() && b.defined() && (*a.impl == *b.impl));
 }
```

### Comparing `tensora-0.0.6/src/taco/src/index_notation/index_notation_nodes_abstract.cpp` & `tensora-0.0.7/src/taco/src/index_notation/index_notation_nodes_abstract.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/index_notation/index_notation_printer.cpp` & `tensora-0.0.7/src/taco/src/index_notation/index_notation_printer.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -16,19 +16,26 @@
 void IndexNotationPrinter::print(const IndexStmt& expr) {
   parentPrecedence = Precedence::TOP;
   expr.accept(this);
 }
 
 void IndexNotationPrinter::visit(const AccessNode* op) {
   os << op->tensorVar.getName();
+  if (op->isAccessingStructure) {
+    os << "_struct";
+  }
   if (op->indexVars.size() > 0) {
     os << "(" << util::join(op->indexVars,",") << ")";
   }
 }
 
+void IndexNotationPrinter::visit(const IndexVarNode* op) {
+  os << op->getName();
+}
+
 void IndexNotationPrinter::visit(const LiteralNode* op) {
   switch (op->getDataType().getKind()) {
     case Datatype::Bool:
       os << op->getVal<bool>();
       break;
     case Datatype::UInt8:
       os << op->getVal<uint8_t>();
@@ -77,15 +84,20 @@
   }
 }
 
 void IndexNotationPrinter::visit(const NegNode* op) {
   Precedence precedence = Precedence::NEG;
   bool parenthesize =  precedence > parentPrecedence;
   parentPrecedence = precedence;
-  os << "-";
+  if(op->getDataType().isBool()) {
+    os << "!";
+  } else {
+    os << "-";
+  }
+
   if (parenthesize) {
     os << "(";
   }
   op->a.accept(this);
   if (parenthesize) {
     os << ")";
   }
@@ -149,14 +161,21 @@
   }
   for (size_t i = 1; i < nodes.size(); ++i) {
     stream << sep;
     nodes[i].accept(printer);
   }
 }
 
+void IndexNotationPrinter::visit(const CallNode* op) {
+  parentPrecedence = Precedence::FUNC;
+  os << op->name << "(";
+  acceptJoin(this, os, op->args, ", ");
+  os << ")";
+}
+
 void IndexNotationPrinter::visit(const CallIntrinsicNode* op) {
   parentPrecedence = Precedence::FUNC;
   os << op->func->getName();
   os << "(";
   acceptJoin(this, os, op->args, ", ");
   os << ")";
 }
@@ -174,14 +193,18 @@
     }
     void visit(const MulNode* node) {
       reductionName = "product";
     }
     void visit(const BinaryExprNode* node) {
       reductionName = "reduction(" + node->getOperatorString() + ")";
     }
+
+    void visit(const CallNode* node) {
+      reductionName = node->name + "Reduce";
+    }
   };
   parentPrecedence = Precedence::REDUCTION;
   os << ReductionName().get(op->op) << "(" << op->var << ", ";
   op->a.accept(this);
   os << ")";
 }
 
@@ -193,14 +216,18 @@
       if (!expr.defined()) return "";
       expr.accept(this);
       return operatorName;
     }
     void visit(const BinaryExprNode* node) {
       operatorName = node->getOperatorString();
     }
+
+    void visit(const CallNode* node) {
+      operatorName = node->name;
+    }
   };
 
   op->lhs.accept(this);
   os << " " << OperatorName().get(op->op) << "= ";
   op->rhs.accept(this);
 }
 
@@ -212,22 +239,16 @@
   op->expr.accept(this);
   os << ")";
 }
 
 void IndexNotationPrinter::visit(const ForallNode* op) {
   os << "forall(" << op->indexVar << ", ";
   op->stmt.accept(this);
-  for (auto iter = op->tags.begin(); iter != op->tags.end(); ++iter) {
-    switch (*iter) {
-      case Forall::PARALLELIZE:
-        os << ", PARALLELIZE";
-        break;
-      default:
-        taco_ierror;
-    }
+  if (op->parallel_unit != ParallelUnit::NotParallel) {
+    os << ", " << ParallelUnit_NAMES[(int) op->parallel_unit] << ", " << OutputRaceStrategy_NAMES[(int) op->output_race_strategy];
   }
   os << ")";
 }
 
 void IndexNotationPrinter::visit(const WhereNode* op) {
   os << "where(";
   op->consumer.accept(this);
@@ -240,16 +261,39 @@
   os << "multi(";
   op->stmt1.accept(this);
   os << ", ";
   op->stmt2.accept(this);
   os << ")";
 }
 
+void IndexNotationPrinter::visit(const SuchThatNode* op) {
+  os << "suchthat(";
+  op->stmt.accept(this);
+  os << ", ";
+  for (auto iter = op->predicate.begin(); iter != op->predicate.end(); ++iter) {
+    os << *iter;
+    if (iter + 1 != op->predicate.end()) {
+      os << " and ";
+    }
+  }
+  os << ")";
+}
+
 void IndexNotationPrinter::visit(const SequenceNode* op) {
   os << "sequence(";
   op->definition.accept(this);
   os << ", ";
   op->mutation.accept(this);
   os << ")";
 }
 
+void IndexNotationPrinter::visit(const AssembleNode* op) {
+  os << "assemble(";
+  if (op->queries.defined()) {
+    op->queries.accept(this);
+    os << ", ";
+  }
+  op->compute.accept(this);
+  os << ")";
+}
+
 }
```

### Comparing `tensora-0.0.6/src/taco/src/index_notation/index_notation_rewriter.cpp` & `tensora-0.0.7/src/taco/src/index_notation/index_notation_rewriter.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 
 
 // class ExprRewriter
 void IndexNotationRewriter::visit(const AccessNode* op) {
   expr = op;
 }
 
+void IndexNotationRewriter::visit(const IndexVarNode* op) {
+  expr = op;
+}
+
 template <class T>
 IndexExpr visitUnaryOp(const T *op, IndexNotationRewriter *rw) {
   IndexExpr a = rw->rewrite(op->a);
   if (a == op->a) {
     return op;
   }
   else {
@@ -99,14 +103,36 @@
     expr = op;
   }
   else {
     expr = new CastNode(a, op->getDataType());
   }
 }
 
+void IndexNotationRewriter::visit(const CallNode* op) {
+  std::vector<IndexExpr> args;
+  bool rewritten = false;
+  for(auto& arg : op->args) {
+    IndexExpr rewrittenArg = rewrite(arg);
+    args.push_back(rewrittenArg);
+    if (arg != rewrittenArg) {
+      rewritten = true;
+    }
+  }
+
+  if (rewritten) {
+    const std::map<IndexExpr, IndexExpr> subs = util::zipToMap(op->args, args);
+    IterationAlgebra newAlg = replaceAlgIndexExprs(op->iterAlg, subs);
+    expr = new CallNode(op->name, args, op->defaultLowerFunc, newAlg, op->properties,
+                        op->regionDefinitions);
+  }
+  else {
+    expr = op;
+  }
+}
+
 void IndexNotationRewriter::visit(const CallIntrinsicNode* op) {
   std::vector<IndexExpr> args;
   bool rewritten = false;
   for (auto& arg : op->args) {
     IndexExpr rewrittenArg = rewrite(arg);
     args.push_back(rewrittenArg);
     if (arg != rewrittenArg) {
@@ -128,15 +154,15 @@
   }
   else {
     expr = new ReductionNode(op->op, op->var, a);
   }
 }
 
 void IndexNotationRewriter::visit(const AssignmentNode* op) {
-  // A design decission is to not visit the rhs access expressions or the op,
+  // A design decission is to not visit the lhs access expressions or the op,
   // as these are considered part of the assignment.  When visiting access
   // expressions, therefore, we only visit read access expressions.
   IndexExpr rhs = rewrite(op->rhs);
   if (rhs == op->rhs) {
     stmt = op;
   }
   else {
@@ -155,15 +181,15 @@
 
 void IndexNotationRewriter::visit(const ForallNode* op) {
   IndexStmt s = rewrite(op->stmt);
   if (s == op->stmt) {
     stmt = op;
   }
   else {
-    stmt = new ForallNode(op->indexVar, s, op->tags);
+    stmt = new ForallNode(op->indexVar, s, op->merge_strategy, op->parallel_unit, op->output_race_strategy, op->unrollFactor);
   }
 }
 
 void IndexNotationRewriter::visit(const WhereNode* op) {
   IndexStmt producer = rewrite(op->producer);
   IndexStmt consumer = rewrite(op->consumer);
   if (producer == op->producer && consumer == op->consumer) {
@@ -181,25 +207,47 @@
     stmt = op;
   }
   else {
     stmt = new SequenceNode(definition, mutation);
   }
 }
 
+void IndexNotationRewriter::visit(const AssembleNode* op) {
+  IndexStmt queries = rewrite(op->queries);
+  IndexStmt compute = rewrite(op->compute);
+  if (queries == op->queries && compute == op->compute) {
+    stmt = op;
+  }
+  else {
+    stmt = new AssembleNode(queries, compute, op->results);
+  }
+}
+
 void IndexNotationRewriter::visit(const MultiNode* op) {
   IndexStmt stmt1 = rewrite(op->stmt1);
   IndexStmt stmt2 = rewrite(op->stmt2);
   if (stmt1 == op->stmt1 && stmt2 == op->stmt2) {
     stmt = op;
   }
   else {
     stmt = new MultiNode(stmt1, stmt2);
   }
 }
 
+void IndexNotationRewriter::visit(const SuchThatNode* op) {
+  IndexStmt s = rewrite(op->stmt);
+  if (s == op->stmt) {
+    stmt = op;
+  }
+  else {
+    stmt = new SuchThatNode(s, op->predicate);
+  }
+}
+
+
 
 // Functions
 #define SUBSTITUTE_EXPR                        \
 do {                                           \
   IndexExpr e = op;                            \
   if (util::contains(exprSubstitutions, e)) {  \
     expr = exprSubstitutions.at(e);            \
@@ -231,14 +279,18 @@
 
   using IndexNotationRewriter::visit;
 
   void visit(const AccessNode* op) {
     SUBSTITUTE_EXPR;
   }
 
+  void visit(const IndexVarNode* op) {
+    SUBSTITUTE_EXPR;
+  }
+
   void visit(const LiteralNode* op) {
     SUBSTITUTE_EXPR;
   }
 
   void visit(const NegNode* op) {
     SUBSTITUTE_EXPR;
   }
@@ -259,14 +311,22 @@
     SUBSTITUTE_EXPR;
   }
 
   void visit(const DivNode* op) {
     SUBSTITUTE_EXPR;
   }
 
+  void visit(const CallNode* op) {
+    SUBSTITUTE_EXPR;
+  }
+
+  void visit(const CallIntrinsicNode* op) {
+    SUBSTITUTE_EXPR;
+  }
+
   void visit(const ReductionNode* op) {
     SUBSTITUTE_EXPR;
   }
 
   void visit(const AssignmentNode* op) {
     SUBSTITUTE_STMT;
   }
@@ -283,17 +343,25 @@
     SUBSTITUTE_STMT;
   }
 
   void visit(const SequenceNode* op) {
     SUBSTITUTE_STMT;
   }
 
+  void visit(const AssembleNode* op) {
+    SUBSTITUTE_STMT;
+  }
+
   void visit(const MultiNode* op) {
     SUBSTITUTE_STMT;
   }
+
+  void visit(const SuchThatNode* op) {
+    SUBSTITUTE_STMT;
+  }
 };
 
 struct ReplaceIndexVars : public IndexNotationRewriter {
   const std::map<IndexVar,IndexVar>& substitutions;
   ReplaceIndexVars(const std::map<IndexVar,IndexVar>& substitutions)
       : substitutions(substitutions) {}
 
@@ -308,22 +376,53 @@
         modified = true;
       }
       else {
         indexVars.push_back(var);
       }
     }
     if (modified) {
-      expr = Access(op->tensorVar, indexVars);
+      expr = Access(op->tensorVar, indexVars, op->packageModifiers());
     }
     else {
       expr = op;
     }
   }
 
-  // TODO: Replace in assignments
+  void visit(const AssignmentNode* op) {
+    IndexExpr rhs = rewrite(op->rhs);
+    Access lhs = to<Access>(rewrite(op->lhs));
+    if (rhs == op->rhs && lhs == op->lhs) {
+      stmt = op;
+    }
+    else {
+      stmt = new AssignmentNode(lhs, rhs, op->op);
+    }
+  }
+
+  void visit(const ForallNode* op) {
+    IndexStmt s = rewrite(op->stmt);
+    IndexVar iv = util::contains(substitutions, op->indexVar) 
+                ? substitutions.at(op->indexVar) : op->indexVar;
+    if (s == op->stmt && iv == op->indexVar) {
+      stmt = op;
+    }
+    else {
+      stmt = new ForallNode(iv, s, op->merge_strategy, op->parallel_unit, op->output_race_strategy, 
+                            op->unrollFactor);
+    }
+  }
+
+  void visit(const IndexVarNode* op) {
+    IndexVar var(op);
+    if(util::contains(substitutions, var)) {
+      expr = substitutions.at(var);
+    } else {
+      expr = var;
+    }
+  }
 };
 
 struct ReplaceTensorVars : public IndexNotationRewriter {
   const std::map<TensorVar,TensorVar>& substitutions;
   ReplaceTensorVars(const std::map<TensorVar,TensorVar>& substitutions)
       : substitutions(substitutions) {}
 
@@ -370,8 +469,13 @@
 }
 
 IndexStmt replace(IndexStmt stmt,
                   const std::map<TensorVar,TensorVar>& substitutions) {
   return ReplaceTensorVars(substitutions).rewrite(stmt);
 }
 
+IndexStmt replace(IndexStmt stmt,
+                  const std::map<IndexVar,IndexVar>& substitutions) {
+  return ReplaceIndexVars(substitutions).rewrite(stmt);
+}
+
 }
```

### Comparing `tensora-0.0.6/src/taco/src/index_notation/index_notation_visitor.cpp` & `tensora-0.0.7/src/taco/src/index_notation/index_notation_visitor.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 // class IndexNotationVisitor
 IndexNotationVisitor::~IndexNotationVisitor() {
 }
 
 void IndexNotationVisitor::visit(const AccessNode* op) {
 }
 
+void IndexNotationVisitor::visit(const IndexVarNode *op) {
+}
+
 void IndexNotationVisitor::visit(const LiteralNode* op) {
 }
 
 void IndexNotationVisitor::visit(const NegNode* op) {
   visit(static_cast<const UnaryExprNode*>(op));
 }
 
@@ -62,14 +65,20 @@
   visit(static_cast<const BinaryExprNode*>(op));
 }
 
 void IndexNotationVisitor::visit(const CastNode* op) {
   op->a.accept(this);
 }
 
+void IndexNotationVisitor::visit(const CallNode* op) {
+  for (auto& arg : op->args) {
+    arg.accept(this);
+  }
+}
+
 void IndexNotationVisitor::visit(const CallIntrinsicNode* op) {
   for (auto& arg : op->args) {
     arg.accept(this);
   }
 }
 
 void IndexNotationVisitor::visit(const UnaryExprNode* op) {
@@ -103,13 +112,24 @@
 }
 
 void IndexNotationVisitor::visit(const SequenceNode* op) {
   op->definition.accept(this);
   op->mutation.accept(this);
 }
 
+void IndexNotationVisitor::visit(const AssembleNode* op) {
+  if (op->queries.defined()) {
+    op->queries.accept(this);
+  }
+  op->compute.accept(this);
+}
+
 void IndexNotationVisitor::visit(const MultiNode* op) {
   op->stmt1.accept(this);
   op->stmt2.accept(this);
 }
 
+void IndexNotationVisitor::visit(const SuchThatNode* op) {
+  op->stmt.accept(this);
+}
+
 }
```

### Comparing `tensora-0.0.6/src/taco/src/index_notation/intrinsic.cpp` & `tensora-0.0.7/src/taco/src/index_notation/intrinsic.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/index_notation/kernel.cpp` & `tensora-0.0.7/src/taco/src/index_notation/kernel.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/index_notation/schedule.cpp` & `tensora-0.0.7/src/taco/src/index_notation/schedule.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/ir/ir.cpp` & `tensora-0.0.7/src/taco/src/ir/ir.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,16 @@
     default:
       break;
   }
   taco_ierror << "not a floating point type";
   return 0.0;
 }
 
+
+
 template <typename T> bool compare(const Literal* literal, double val) {
       return literal->getValue<T>() == static_cast<T>(val);
 }
 
 bool Literal::equalsScalar(double scalar) const {
   switch (type.getKind()) {
     case Datatype::Bool:
@@ -237,22 +239,24 @@
     case Datatype::Undefined:
       taco_not_supported_yet;
     break;
   }
   return false;
 }
 
-Expr Var::make(std::string name, Datatype type, bool is_ptr, bool is_tensor) {
+Expr Var::make(std::string name, Datatype type, 
+               bool is_ptr, bool is_tensor, bool is_parameter) {
   Var *var = new Var;
   var->type = type;
   var->name = name;
 
   // TODO: is_ptr and is_tensor should be part of type
   var->is_ptr = is_ptr;
   var->is_tensor = is_tensor;
+  var->is_parameter = is_parameter;
 
   return var;
 }
 
 Expr Neg::make(Expr a) {
   Neg *neg = new Neg;
   neg->a = a;
@@ -275,15 +279,16 @@
 }
 
 Expr Add::make(Expr a, Expr b) {
   return Add::make(a, b, max_expr_type(a, b));
 }
 
 Expr Add::make(Expr a, Expr b, Datatype type) {
-  taco_iassert(!a.type().isBool() && !b.type().isBool()) <<
+  taco_iassert((!a.type().isBool() || (isa<Var>(a) && a.as<Var>()->is_ptr)) &&
+            (!b.type().isBool() || (isa<Var>(b) && b.as<Var>()->is_ptr))) <<
       "Can't do arithmetic on booleans.";
 
   Add *add = new Add;
   add->type = type;
   add->a = a;
   add->b = b;
   return add;
@@ -372,19 +377,27 @@
 Expr Max::make(Expr a, Expr b) {
   return Max::make(a, b, max_expr_type(a, b));
 }
 
 Expr Max::make(Expr a, Expr b, Datatype type) {
   taco_iassert(!a.type().isBool() && !b.type().isBool()) <<
       "Can't do arithmetic on booleans.";
-  
-  Max *max = new Max;
+
+  return Max::make({a, b}, type);
+}
+
+Expr Max::make(std::vector<Expr> operands) {
+  taco_iassert(operands.size() > 0);
+  return Max::make(operands, operands[0].type());
+}
+
+Expr Max::make(std::vector<Expr> operands, Datatype type) {
+  Max* max = new Max;
+  max->operands = operands;
   max->type = type;
-  max->a = a;
-  max->b = b;
   return max;
 }
 
 Expr BitAnd::make(Expr a, Expr b) {
   BitAnd *bitAnd = new BitAnd;
   bitAnd->type = UInt();
   bitAnd->a = a;
@@ -461,14 +474,32 @@
   And *andnode = new And;
   andnode->type = Bool;
   andnode->a = a;
   andnode->b = b;
   return andnode;
 }
 
+Expr BinOp::make(Expr a, Expr b, std::string op) {
+  BinOp *binopnode = new BinOp;
+  binopnode->strMid = op;
+  binopnode->a = a;
+  binopnode->b = b;
+  return binopnode;
+}
+
+Expr BinOp::make(Expr a, Expr b, std::string strStart, std::string strMid, std::string strEnd) {
+  BinOp *binopnode = new BinOp;
+  binopnode->strStart = strStart;
+  binopnode->strMid = strMid;
+  binopnode->strEnd = strEnd;
+  binopnode->a = a;
+  binopnode->b = b;
+  return binopnode;
+}
+
 Expr Cast::make(Expr a, Datatype newType) {
   Cast *cast = new Cast;
   cast->type = newType;
   cast->a = a;
   return cast;
 }
 
@@ -566,19 +597,21 @@
 
   Scope *scope = new Scope;
   scope->scopedStmt = scopedStmt;
   return scope;
 }
 
 // Store to an array
-Stmt Store::make(Expr arr, Expr loc, Expr data) {
+Stmt Store::make(Expr arr, Expr loc, Expr data, bool use_atomics, ParallelUnit atomic_parallel_unit) {
   Store *store = new Store;
   store->arr = arr;
   store->loc = loc;
   store->data = data;
+  store->use_atomics = use_atomics;
+  store->atomic_parallel_unit = atomic_parallel_unit;
   return store;
 }
 
 // Conditional
 Stmt IfThenElse::make(Expr cond, Stmt then) {
   return IfThenElse::make(cond, then, Stmt());
 }
@@ -627,24 +660,25 @@
   sw->cases = scopedCases;
   sw->controlExpr = controlExpr;
   return sw;
 }
 
 // For loop
 Stmt For::make(Expr var, Expr start, Expr end, Expr increment, Stmt body,
-  LoopKind kind, bool accelerator, int vec_width) {
+  LoopKind kind, ParallelUnit parallel_unit, size_t unrollFactor, int vec_width) {
   For *loop = new For;
   loop->var = var;
   loop->start = start;
   loop->end = end;
   loop->increment = increment;
   loop->contents = Scope::make(body);
   loop->kind = kind;
+  loop->unrollFactor = unrollFactor;
   loop->vec_width = vec_width;
-  loop->accelerator = accelerator;
+  loop->parallel_unit = parallel_unit;
   return loop;
 }
 
 // While loop
 Stmt While::make(Expr cond, Stmt contents, LoopKind kind,
   int vec_width) {
   While *loop = new While;
@@ -709,20 +743,22 @@
   VarDecl* decl = new VarDecl;
   decl->var = var;
   decl->rhs = rhs;
   return decl;
 }
 
 // VarAssign
-Stmt Assign::make(Expr lhs, Expr rhs) {
+Stmt Assign::make(Expr lhs, Expr rhs, bool use_atomics, ParallelUnit atomic_parallel_unit) {
   taco_iassert(lhs.as<Var>() || lhs.as<GetProperty>())
     << "Can only assign to a Var or GetProperty";
   Assign *assign = new Assign;
   assign->lhs = lhs;
   assign->rhs = rhs;
+  assign->use_atomics = use_atomics;
+  assign->atomic_parallel_unit = atomic_parallel_unit;
   return assign;
 }
 
 // Yield
 Stmt Yield::make(std::vector<Expr> coords, Expr val) {
   for (auto coord : coords) {
     taco_iassert(coord.as<Var>()) << "Coordinates must be instances of Var";
@@ -730,26 +766,27 @@
   Yield *yield = new Yield;
   yield->coords = coords;
   yield->val = val;
   return yield;
 }
 
 // Allocate
-Stmt Allocate::make(Expr var, Expr num_elements, bool is_realloc, Expr old_elements) {
+Stmt Allocate::make(Expr var, Expr num_elements, bool is_realloc, Expr old_elements, bool clear) {
   taco_iassert(var.as<GetProperty>() ||
                (var.as<Var>() && var.as<Var>()->is_ptr)) <<
       "Can only allocate memory for a pointer-typed Var";
   taco_iassert(num_elements.type().isInt() || num_elements.type().isUInt()) <<
       "Can only allocate an integer-valued number of elements";
   Allocate* alloc = new Allocate;
   alloc->var = var;
   alloc->num_elements = num_elements;
   alloc->is_realloc = is_realloc;
   taco_iassert(!is_realloc || old_elements.ptr != NULL);
   alloc->old_elements = old_elements;
+  alloc->clear = clear;
   return alloc;
 }
 
 // Free
 Stmt Free::make(Expr var) {
   taco_iassert(var.as<GetProperty>() ||
                (var.as<Var>() && var.as<Var>()->is_ptr)) <<
@@ -767,14 +804,24 @@
 }
 
 // BlankLine
 Stmt BlankLine::make() {
   return new BlankLine;
 }
 
+// Continue
+Stmt Continue::make() {
+  return new Continue;
+}
+
+// Break
+Stmt Break::make() {
+  return new Break;
+}
+
 // Print
 Stmt Print::make(std::string fmt, std::vector<Expr> params) {
   Print* pr = new Print;
   pr->fmt = fmt;
   pr->params = params;
   return pr;
 }
@@ -793,14 +840,21 @@
     gp->type = tensor.type();
   else
     gp->type = Int();
   
   return gp;
 }
 
+// Sort
+Stmt Sort::make(std::vector<Expr> args) {
+  Sort* sort = new Sort;
+  sort->args = args;
+  return sort;
+}
+
 
 // GetProperty
 Expr GetProperty::make(Expr tensor, TensorProperty property, int mode) {
   GetProperty* gp = new GetProperty;
   gp->tensor = tensor;
   gp->property = property;
   gp->mode = mode;
@@ -833,14 +887,17 @@
       break;
     case TensorProperty::Values:
       gp->name = tensorVar->name + "_vals";
       break;
     case TensorProperty::ValuesSize:
       gp->name = tensorVar->name + "_vals_size";
       break;
+    case TensorProperty::FillValue:
+      gp->name = tensorVar->name + "_fill_value";
+      break;
   }
   
   return gp;
 }
   
 // visitor methods
 template<> void ExprNode<Literal>::accept(IRVisitorStrict *v)
@@ -881,14 +938,16 @@
     const { v->visit((const Gte*)this); }
 template<> void ExprNode<Lte>::accept(IRVisitorStrict *v)
     const { v->visit((const Lte*)this); }
 template<> void ExprNode<And>::accept(IRVisitorStrict *v)
     const { v->visit((const And*)this); }
 template<> void ExprNode<Or>::accept(IRVisitorStrict *v)
     const { v->visit((const Or*)this); }
+template<> void ExprNode<BinOp>::accept(IRVisitorStrict *v)
+    const { v->visit((const BinOp*)this); }
 template<> void ExprNode<Cast>::accept(IRVisitorStrict *v)
     const { v->visit((const Cast*)this); }
 template<> void ExprNode<Call>::accept(IRVisitorStrict *v)
     const { v->visit((const Call*)this); }
 template<> void StmtNode<IfThenElse>::accept(IRVisitorStrict *v)
     const { v->visit((const IfThenElse*)this); }
 template<> void StmtNode<Case>::accept(IRVisitorStrict *v)
@@ -923,18 +982,24 @@
     const { v->visit((const Allocate*)this); }
 template<> void StmtNode<Free>::accept(IRVisitorStrict *v)
     const { v->visit((const Free*)this); }
 template<> void StmtNode<Comment>::accept(IRVisitorStrict *v)
     const { v->visit((const Comment*)this); }
 template<> void StmtNode<BlankLine>::accept(IRVisitorStrict *v)
     const { v->visit((const BlankLine*)this); }
+template<> void StmtNode<Continue>::accept(IRVisitorStrict *v)
+  const { v->visit((const Continue*)this); }
 template<> void StmtNode<Print>::accept(IRVisitorStrict *v)
     const { v->visit((const Print*)this); }
 template<> void ExprNode<GetProperty>::accept(IRVisitorStrict *v)
     const { v->visit((const GetProperty*)this); }
+template<> void StmtNode<Sort>::accept(IRVisitorStrict *v)
+  const { v->visit((const Sort*)this); }
+template<> void StmtNode<Break>::accept(IRVisitorStrict *v)
+  const { v->visit((const Break*)this); }
 
 // printing methods
 std::ostream& operator<<(std::ostream& os, const Stmt& stmt) {
   if (!stmt.defined()) return os << "Stmt()" << std::endl;
   IRPrinter printer(os);
   stmt.accept(&printer);
   return os;
```

### Comparing `tensora-0.0.6/src/taco/src/ir/ir_generators.cpp` & `tensora-0.0.7/src/taco/src/ir/ir_generators.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#include "ir_generators.h"
+#include "taco/ir/ir_generators.h"
 
 #include "taco/ir/ir.h"
 #include "taco/error.h"
 #include "taco/util/strings.h"
 
 namespace taco {
 namespace ir {
 
-Stmt compoundStore(Expr a, Expr i, Expr val) {
+Stmt compoundStore(Expr a, Expr i, Expr val, bool use_atomics, ParallelUnit atomic_parallel_unit) {
   Expr add = (val.type().getKind() == Datatype::Bool) 
              ? Or::make(Load::make(a, i), val)
              : Add::make(Load::make(a, i), val);
-  return Store::make(a, i, add);
+  return Store::make(a, i, add, use_atomics, atomic_parallel_unit);
 }
 
-Stmt compoundAssign(Expr a, Expr val) {
+Stmt compoundAssign(Expr a, Expr val, bool use_atomics, ParallelUnit atomic_parallel_unit) {
   Expr add = (val.type().getKind() == Datatype::Bool) 
              ? Or::make(a, val) : Add::make(a, val);
-  return Assign::make(a, add);
+  return Assign::make(a, add, use_atomics, atomic_parallel_unit);
 }
 
 Expr conjunction(std::vector<Expr> exprs) {
   taco_iassert(exprs.size() > 0) << "No expressions to and";
   Expr conjunction = exprs[0];
   for (size_t i = 1; i < exprs.size(); i++) {
     conjunction = And::make(conjunction, exprs[i]);
```

### Comparing `tensora-0.0.6/src/taco/src/ir/ir_printer.cpp` & `tensora-0.0.7/src/taco/src/ir/ir_printer.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,19 @@
 }
 
 void IRPrinter::print(Stmt stmt) {
   if (isa<Scope>(stmt)) {
     stmt = to<Scope>(stmt)->scopedStmt;
   }
   if (simplify) {
-    stmt = ir::simplify(stmt);
+    Stmt oldStmt;
+    do {
+      oldStmt = stmt;
+      stmt = ir::simplify(stmt);
+    } while (stmt != oldStmt);
   }
   stmt.accept(this);
 }
 
 void IRPrinter::visit(const Literal* op) {
   if (color) {
     stream << blue ;
@@ -127,15 +131,19 @@
   }
   else {
     stream << op->name;
   }
 }
 
 void IRPrinter::visit(const Neg* op) {
-  stream << "-";
+  if(op->type.isBool()) {
+    stream << "!";
+  } else {
+    stream << "-";
+  }
   parentPrecedence = Precedence::NEG;
   op->a.accept(this);
 }
 
 void IRPrinter::visit(const Sqrt* op) {
   stream << "sqrt(";
   op->a.accept(this);
@@ -168,22 +176,25 @@
     op->operands[i].accept(this);
     if (i < op->operands.size()-1)
       stream << ", ";
   }
   stream << ")";
 }
 
-void IRPrinter::visit(const Max* op){
+void IRPrinter::visit(const Max* op) {
   stream << "max(";
-  op->a.accept(this);
-  stream << ", ";
-  op->b.accept(this);
+  for (size_t i=0; i<op->operands.size(); i++) {
+    op->operands[i].accept(this);
+    if (i < op->operands.size()-1)
+      stream << ", ";
+  }
   stream << ")";
 }
 
+
 void IRPrinter::visit(const BitAnd* op){
   printBinOp(op->a, op->b, "&", Precedence::BAND);
 }
 
 void IRPrinter::visit(const BitOr* op){
   printBinOp(op->a, op->b, "|", Precedence::BOR);
 }
@@ -216,14 +227,22 @@
   printBinOp(op->a, op->b, keywordString("&&"), Precedence::LAND);
 }
 
 void IRPrinter::visit(const Or* op) {
   printBinOp(op->a, op->b, keywordString("||"), Precedence::LOR);
 }
 
+void IRPrinter::visit(const BinOp* op) {
+  stream << op->strStart;
+  op->a.accept(this);
+  stream << op->strMid;
+  op->b.accept(this);
+  stream << op->strEnd;
+}
+
 void IRPrinter::visit(const Cast* op) {
   stream << "(" << keywordString(util::toString(op->type)) << ")";
   parentPrecedence = Precedence::CAST;
   op->a.accept(this);
 }
 
 void IRPrinter::visit(const Call* op) {
@@ -547,14 +566,24 @@
   stream << endl;
 }
 
 void IRPrinter::visit(const BlankLine*) {
   stream << endl;
 }
 
+void IRPrinter::visit(const Continue*) {
+  doIndent();
+  stream << "continue;" << endl;
+}
+
+void IRPrinter::visit(const Break*) {
+  doIndent();
+  stream << "break;" << endl;
+}
+
 void IRPrinter::visit(const Print* op) {
   doIndent();
   stream << "printf(";
   stream << "\"" << op->fmt << "\"";
   for (auto e: op->params) {
     stream << ", ";
     e.accept(this);
@@ -563,14 +592,24 @@
   stream << endl;
 }
 
 void IRPrinter::visit(const GetProperty* op) {
   stream << op->name;
 }
 
+void IRPrinter::visit(const Sort* op) {
+  doIndent();
+  stream << "qsort(";
+  parentPrecedence = Precedence::CALL;
+  acceptJoin(this, stream, op->args, ", ");
+  stream << ", cmp);";
+  stream << endl;
+}
+
+
 void IRPrinter::resetNameCounters() {
   // seed the unique names with all C99 keywords
   // from: http://en.cppreference.com/w/c/keyword
   vector<string> keywords =
     {"auto",
      "break",
      "case",
@@ -613,32 +652,36 @@
 
 void IRPrinter::doIndent() {
   for (int i=0; i<indent; i++)
     stream << "  ";
 }
 
 void IRPrinter::printBinOp(Expr a, Expr b, string op, Precedence precedence) {
-  // Add parentheses if required by C operator precedence or for Boolean 
-  // expressions of form `a || (b && c)` (to avoid C compiler warnings)
-  bool parenthesize = (precedence > parentPrecedence || 
-                       (precedence == Precedence::LAND && 
-                        parentPrecedence == Precedence::LOR));
+  bool parenthesize = needsParentheses(precedence);
   if (parenthesize) {
     stream << "(";
   }
   parentPrecedence = precedence;
   a.accept(this);
   stream << " " << op << " ";
   parentPrecedence = precedence;
   b.accept(this);
   if (parenthesize) {
     stream << ")";
   }
 }
 
+bool IRPrinter::needsParentheses(Precedence precedence) {
+  // Add parentheses if required by C operator precedence or for Boolean
+  // expressions of form `a || (b && c)` (to avoid C compiler warnings)
+  return (precedence >= parentPrecedence ||
+            (precedence == Precedence::LAND &&
+              parentPrecedence == Precedence::LOR));
+}
+
 
 std::string IRPrinter::keywordString(std::string keyword) {
   if (color) {
     return magenta + keyword + nc;
   }
   else {
     return keyword;
```

### Comparing `tensora-0.0.6/src/taco/src/ir/ir_rewriter.cpp` & `tensora-0.0.7/src/taco/src/ir/ir_rewriter.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,29 @@
   }
   else {
     expr = Min::make(operands);
   }
 }
 
 void IRRewriter::visit(const Max* op) {
-  expr = visitBinaryOp(op, this);
+  vector<Expr> operands;
+  bool operandsSame = true;
+  for (const Expr& operand : op->operands) {
+    Expr rewrittenOperand = rewrite(operand);
+    operands.push_back(rewrittenOperand);
+    if (rewrittenOperand != operand) {
+      operandsSame = false;
+    }
+  }
+  if (operandsSame) {
+    expr = op;
+  }
+  else {
+    expr = Max::make(operands);
+  }
 }
 
 void IRRewriter::visit(const BitAnd* op) {
   expr = visitBinaryOp(op, this);
 }
 
 void IRRewriter::visit(const BitOr* op) {
@@ -156,14 +170,24 @@
   expr = visitBinaryOp(op, this);
 }
 
 void IRRewriter::visit(const Or* op) {
   expr = visitBinaryOp(op, this);
 }
 
+void IRRewriter::visit(const BinOp* op) {
+  Expr a = rewrite(op->a);
+  Expr b = rewrite(op->b);
+  if (a == op->a && b == op->b) {
+    expr = op;
+  } else {
+    expr = BinOp::make(op->a, op->b, op->strStart, op->strMid, op->strEnd);
+  }
+}
+
 void IRRewriter::visit(const Cast* op) {
   Expr a = rewrite(op->a);
   if (a == op->a) {
     expr = op;
   }
   else {
     expr = Cast::make(a, op->type);
@@ -269,15 +293,15 @@
   Expr arr  = rewrite(op->arr);
   Expr loc  = rewrite(op->loc);
   Expr data = rewrite(op->data);
   if (arr == op->arr && loc == op->loc && data == op->data) {
     stmt = op;
   }
   else {
-    stmt = Store::make(arr, loc, data);
+    stmt = Store::make(arr, loc, data, op->use_atomics);
   }
 }
 
 void IRRewriter::visit(const For* op) {
   Expr var       = rewrite(op->var);
   Expr start     = rewrite(op->start);
   Expr end       = rewrite(op->end);
@@ -285,15 +309,15 @@
   Stmt contents  = rewrite(op->contents);
   if (var == op->var && start == op->start && end == op->end &&
       increment == op->increment && contents == op->contents) {
     stmt = op;
   }
   else {
     stmt = For::make(var, start, end, increment, contents, op->kind,
-                     op->accelerator, op->vec_width);
+                     op->parallel_unit, op->unrollFactor, op->vec_width);
   }
 }
 
 void IRRewriter::visit(const While* op) {
   Expr cond     = rewrite(op->cond);
   Stmt contents = rewrite(op->contents);
   if (cond == op->cond && contents == op->contents) {
@@ -377,15 +401,15 @@
 void IRRewriter::visit(const Assign* op) {
   Expr lhs = rewrite(op->lhs);
   Expr rhs = rewrite(op->rhs);
   if (lhs == op->lhs && rhs == op->rhs) {
     stmt = op;
   }
   else {
-    stmt = Assign::make(lhs, rhs);
+    stmt = Assign::make(lhs, rhs, op->use_atomics);
   }
 }
 
 void IRRewriter::visit(const Yield* op) {
   std::vector<Expr> coords;
   bool coordsSame = true;
   for (auto& coord : op->coords) {
@@ -407,15 +431,15 @@
 void IRRewriter::visit(const Allocate* op) {
   Expr var          = rewrite(op->var);
   Expr num_elements = rewrite(op->num_elements);
   if (var == op->var && num_elements == op->num_elements) {
     stmt = op;
   }
   else {
-    stmt = Allocate::make(var, num_elements, op->is_realloc, op->old_elements);
+    stmt = Allocate::make(var, num_elements, op->is_realloc, op->old_elements, op->clear);
   }
 }
 
 void IRRewriter::visit(const Free* op) {
   Expr var = rewrite(op->var);
   if (var == op->var) {
     stmt = op;
@@ -429,14 +453,22 @@
   stmt = op;
 }
 
 void IRRewriter::visit(const BlankLine* op) {
   stmt = op;
 }
 
+void IRRewriter::visit(const Continue* op) {
+  stmt = op;
+}
+
+void IRRewriter::visit(const Break* op) {
+  stmt = op;
+}
+
 void IRRewriter::visit(const Print* op) {
   vector<Expr> params;
   bool paramsSame = true;
   for (auto& param : op->params) {
     Expr rewrittenParam = rewrite(param);
     params.push_back(rewrittenParam);
     if (rewrittenParam != param) {
@@ -457,9 +489,27 @@
     expr = op;
   }
   else {
     expr = GetProperty::make(tensor, op->property, op->mode, op->index, op->name);
   }
 }
 
+void IRRewriter::visit(const Sort* op) {
+  std::vector<Expr> args;
+  bool rewritten = false;
+  for (auto& arg : op->args) {
+    Expr rewrittenArg = rewrite(arg);
+    args.push_back(rewrittenArg);
+    if (rewrittenArg != arg) {
+      rewritten = true;
+    }
+  }
+  if (rewritten) {
+    stmt = Sort::make(args);
+  }
+  else {
+    stmt = op;
+  }
+}
+
 
 }}
```

### Comparing `tensora-0.0.6/src/taco/src/ir/ir_verifier.cpp` & `tensora-0.0.7/src/taco/src/ir/ir_verifier.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,21 @@
         messages << "Node: " << (Expr)op << " has operand with incorrect type\n";
       }
       x.accept(this);
     }
   }
   
   void visit(const Max *op) {
-    verify_operand_types_consistent_with_result(op);
-    op->a.accept(this);
-    op->b.accept(this);
+    auto tp = op->type;
+    for (auto &x: op->operands) {
+      if (x.type() != tp) {
+        messages << "Node: " << (Expr)op << " has operand with incorrect type\n";
+      }
+      x.accept(this);
+    }
   }
   
   void visit(const BitAnd *op) {
     // TODO: do we want to enforce integer-ness?
     verify_operand_types_consistent_with_result(op);
     op->a.accept(this);
     op->b.accept(this);
```

### Comparing `tensora-0.0.6/src/taco/src/ir/ir_visitor.cpp` & `tensora-0.0.7/src/taco/src/ir/ir_visitor.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -56,16 +56,17 @@
 void IRVisitor::visit(const Min* op){
   for (auto e: op->operands) {
     e.accept(this);
   }
 }
 
 void IRVisitor::visit(const Max* op){
-  op->a.accept(this);
-  op->b.accept(this);
+  for (auto e: op->operands) {
+    e.accept(this);
+  }
 }
 
 void IRVisitor::visit(const BitAnd* op){
   op->a.accept(this);
   op->b.accept(this);
 }
 
@@ -110,14 +111,19 @@
 }
 
 void IRVisitor::visit(const Or* op){
   op->a.accept(this);
   op->b.accept(this);
 }
 
+void IRVisitor::visit(const BinOp* op) {
+  op->a.accept(this);
+  op->b.accept(this);
+}
+
 void IRVisitor::visit(const Cast* op){
   op->a.accept(this);
 }
 
 void IRVisitor::visit(const Call* op) {
   for (auto& arg : op->args) {
     arg.accept(this);
@@ -223,14 +229,25 @@
 
 void IRVisitor::visit(const Comment*) {
 }
 
 void IRVisitor::visit(const BlankLine*) {
 }
 
+void IRVisitor::visit(const Continue*) {
+}
+
+void IRVisitor::visit(const Break*) {
+}
+
 void IRVisitor::visit(const Print* op) {
   for (auto e: op->params)
     e.accept(this);
 }
 
+void IRVisitor::visit(const Sort* op) {
+  for (auto e: op->args)
+    e.accept(this);
+}
+
 }  // namespace ir
 }  // namespace taco
```

### Comparing `tensora-0.0.6/src/taco/src/ir/simplify.cpp` & `tensora-0.0.7/src/taco/src/ir/simplify.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,37 @@
 #include "taco/util/strings.h"
 #include "taco/util/collections.h"
 #include "taco/util/scopedmap.h"
 
 namespace taco {
 namespace ir {
 
-struct ExpressionSimplifier : IRRewriter {
+struct ExpressionSimplifier : public IRRewriter {
   using IRRewriter::visit;
+
+  void visit(const Cast* op) {
+    Expr a = rewrite(op->a);
+
+    // (T)true == T(1)
+    // (T)false == T(0)
+    if (isa<Literal>(a) && to<Literal>(a)->type.isBool()) {
+      const auto lit = TypedComponentVal(op->type, 
+                                         to<Literal>(a)->getValue<bool>());
+      expr = Literal::make(lit, op->type);
+      return;
+    }
+
+    if (a == op->a) {
+      expr = op;
+    }
+    else {
+      expr = Cast::make(a, op->type);
+    }
+  }
+
   void visit(const Or* op) {
     Expr a = rewrite(op->a);
     Expr b = rewrite(op->b);
 
     // true || b = true
     // false || b = b
     if (isa<Literal>(a)) {
@@ -334,15 +355,15 @@
 
 ir::Stmt simplify(const ir::Stmt& stmt) {
   // Perform copy propagation on variables that are added to a product of zero
   // and never re-assign, e.g. `int B1_pos = (0 * 42) + iB;`. These occur when
   // emitting code for top levels that are dense.
 
   // Identify all loop dependent variables. (This analysis is imprecise.)
-  struct FindLoopDependentVars : IRVisitor {
+  struct FindLoopDependentVars : public IRVisitor {
     std::set<Expr> loopDependentVars;
     std::map<Expr,int> defLevel;
     int loopLevel = 0;
 
     using IRVisitor::visit;
 
     void visit(const For* op) {
@@ -365,15 +386,14 @@
     void visit(const Assign* op) {
       if (util::contains(defLevel, op->lhs) && 
           defLevel.at(op->lhs) < loopLevel) {
         loopDependentVars.insert(op->lhs);
       }
     }
   };
-
   FindLoopDependentVars findLoopDepVars;
   stmt.accept(&findLoopDepVars);
 
   // Copy propagation (remove candidate var definitions and replace uses) and
   // expression simplification. Also identify non-redundant variable 
   // declarations.
   // TODO: Currently does not handle the following pattern:
@@ -385,54 +405,54 @@
   //     ... = b
   //   }
   //   ... = b
   // The use of `b` in the if branch would be rewritten to `a` but not the use
   // in the else branch. To fix this, the visit method for if and case
   // statements would probably need to be overridden so that each branch is
   // evaluated starting with the same `varsToReplace`.
-  struct Simplifier : ExpressionSimplifier {
+  struct Simplifier : public ExpressionSimplifier {
     util::ScopedMap<Expr,std::pair<Expr,Stmt>> varsToReplace;
     std::set<Stmt> necessaryDecls;
     std::multimap<Expr,Expr> dependencies;
     util::ScopedMap<Expr,Stmt> declarations;
     std::set<Expr> loopDependentVars;
 
     using ExpressionSimplifier::visit;
 
     Simplifier(const std::set<Expr>& loopDependentVars) : 
         loopDependentVars(loopDependentVars) {}
 
     void visit(const Scope* scope) {
       declarations.scope();
       varsToReplace.scope();
-      stmt = rewrite(scope->scopedStmt);
+      IRRewriter::visit(scope);
       varsToReplace.unscope();
       declarations.unscope();
     }
 
     void visit(const VarDecl* decl) {
       Expr rhs = rewrite(decl->rhs);
       stmt = (rhs == decl->rhs) ? decl : VarDecl::make(decl->var, rhs);
 
       declarations.insert({decl->var, stmt});
       if (decl->var.type().isInt() && isa<Var>(rhs) && 
           !util::contains(loopDependentVars, decl->var)) {
-        taco_iassert(!varsToReplace.contains(decl->var)) 
-            << "Copy propagation pass currently does not support variables " 
-            << "with same name declared in nested scopes";
+//        TODO: taco_iassert(!varsToReplace.contains(decl->var))
+//            << "Copy propagation pass currently does not support variables "
+//            << "with same name declared in nested scopes: " << decl->var.as<Var>()->name;
         varsToReplace.insert({decl->var, {rhs, stmt}});
         dependencies.insert({rhs, decl->var});
       }
     }
 
     void visit(const Assign* assign) {
       Expr lhs = isa<Var>(assign->lhs) ? assign->lhs : rewrite(assign->lhs);
       Expr rhs = rewrite(assign->rhs);
       stmt = (lhs == assign->lhs && rhs == assign->rhs) ? assign : 
-             Assign::make(lhs, rhs);
+             Assign::make(lhs, rhs, assign->use_atomics);
       
       if (declarations.contains(lhs)) {
         taco_iassert(isa<Var>(lhs));
         necessaryDecls.insert(declarations.get(lhs));
       }
 
       if (!assign->lhs.type().isInt()) {
@@ -460,31 +480,245 @@
     void visit(const Var* var) {
       expr = varsToReplace.contains(var) ? varsToReplace.get(var).first : var;
       if (declarations.contains(expr)) {
         necessaryDecls.insert(declarations.get(expr));
       }
     }
   };
-
   Simplifier copyPropagation(findLoopDepVars.loopDependentVars);
   Stmt simplifiedStmt = copyPropagation.rewrite(stmt);
 
   // Remove redundant variable declarations.
-  struct RemoveRedundantStmts : IRRewriter {
+  struct RemoveRedundantStmts : public IRRewriter {
     std::set<Stmt> necessaryDecls;
     
     using IRRewriter::visit;
 
     RemoveRedundantStmts(const std::set<Stmt>& necessaryDecls) : 
         necessaryDecls(necessaryDecls) {}
 
     void visit(const VarDecl* decl) {
+      if (isa<ir::Call>(decl->rhs)) { // don't remove function calls that might have side effects
+        stmt = decl;
+        return;
+      }
       stmt = util::contains(necessaryDecls, decl)? decl : Block::make();
     }
   };
-
   simplifiedStmt = RemoveRedundantStmts(copyPropagation.necessaryDecls).rewrite(
       simplifiedStmt);
+
+  // Eliminate loops that only increment variables.
+  struct RemoveRedundantLoops : public IRRewriter {
+    using IRRewriter::visit;
+
+    struct DuplicateBody : public IRRewriter {
+      Expr loopCount;
+
+      using IRRewriter::visit;
+
+      DuplicateBody(Expr loopCount) : loopCount(loopCount) {}
+
+      void visit(const Block* op) {
+        std::vector<Stmt> contents;
+        for (auto& content : op->contents) {
+          Stmt rewrittenContent = rewrite(content);
+
+          if (!rewrittenContent.defined()) {
+            stmt = Stmt();
+            return;
+          }
+          
+          contents.push_back(rewrittenContent);
+        }
+        stmt = Block::make(contents);
+      }
+
+      void visit(const Scope* op) {
+        Stmt scopedStmt = rewrite(op->scopedStmt);
+        if (!scopedStmt.defined()) {
+          stmt = Stmt();
+          return;
+        }
+        stmt = Scope::make(scopedStmt);
+      }
+
+      void visit(const Assign* op) {
+        if (isa<Literal>(op->rhs)) {
+          stmt = op;
+          return;
+        }
+
+        if (!isa<Add>(op->rhs)) {
+          stmt = Stmt();
+          return;
+        }
+
+        const auto add = to<Add>(op->rhs);
+        if (add->a != op->lhs || !isa<Literal>(add->b)) {
+          stmt = Stmt();
+          return;
+        }
+
+        Expr inc = simplify(Mul::make(loopCount, add->b));
+        stmt = Assign::make(op->lhs, Add::make(add->a, inc));
+      }
+
+      void visit(const IfThenElse* op) {
+        stmt = Stmt();
+      }
+      void visit(const Case* op) {
+        stmt = Stmt();
+      }
+      void visit(const Switch* op) {
+        stmt = Stmt();
+      }
+      void visit(const Malloc* op) {
+        stmt = Stmt();
+      }
+      void visit(const Store* op) {
+        stmt = Stmt();
+      }
+      void visit(const For* op) {
+        stmt = Stmt();
+      }
+      void visit(const While* op) {
+        stmt = Stmt();
+      }
+      void visit(const Function* op) {
+        stmt = Stmt();
+      }
+      void visit(const VarDecl* op) {
+        stmt = Stmt();
+      }
+      void visit(const Yield* op) {
+        stmt = Stmt();
+      }
+      void visit(const Allocate* op) {
+        stmt = Stmt();
+      }
+      void visit(const Free* op) {
+        stmt = Stmt();
+      }
+      void visit(const Comment* op) {
+        stmt = Stmt();
+      }
+      void visit(const BlankLine* op) {
+        stmt = Stmt();
+      }
+      void visit(const Continue* op) {
+        stmt = Stmt();
+      }
+      void visit(const Print* op) {
+        stmt = Stmt();
+      }
+      void visit(const GetProperty* op) {
+        stmt = Stmt();
+      }
+      void visit(const Sort *op) {
+        stmt = Stmt();
+      }
+      void visit(const Break *op) {
+        stmt = Stmt();
+      }
+    };
+
+    struct CheckModified : public IRVisitor {
+      bool isModified = false;
+      Expr var;
+      
+      using IRVisitor::visit;
+
+      CheckModified(Expr var) : var(var) {}
+
+      void visit(const Assign* op) {
+        if (isa<Var>(op->lhs) && to<Var>(op->lhs) == var) {
+          isModified = true;
+        }
+      }
+    };
+
+    // Replace loops of the form:
+    //
+    //   for (int i = s; i < e; i += c) {
+    //     x += lit;
+    //     y = lit;
+    //   }
+    //
+    // with the following:
+    //
+    //   if (s < e)
+    //     x += lit * (e - s) / c;
+    //     y = lit;
+    void visit(const For* op) {
+      Expr loopCount = simplify(Div::make(Sub::make(op->end, op->start), 
+                                          op->increment));
+      Stmt body = DuplicateBody(loopCount).rewrite(op->contents);
+      if (body.defined()) {
+        stmt = IfThenElse::make(Lt::make(op->start, op->end), body);
+        return;
+      }
+      IRRewriter::visit(op);
+    }
+
+    // Replace loops of the form:
+    //
+    //   while (i < e) {
+    //     x += lit;
+    //     y = lit;
+    //     i++;
+    //   }
+    //
+    // with the following:
+    //
+    //   if (i < e) {
+    //     x += lit * (e - i);
+    //     y = lit;
+    //     i = e;
+    //   }
+    void visit(const While* op) {
+      if (isa<Lt>(op->cond)) {
+        const auto cond = to<Lt>(op->cond);
+        if (isa<Var>(cond->a) && isa<Var>(cond->b)) {
+          Expr iter = to<Var>(cond->a);
+          Expr end = to<Var>(cond->b);
+          CheckModified checkModified(end);
+          op->contents.accept(&checkModified);
+          if (!checkModified.isModified) {
+            Stmt body = op->contents.as<Scope>()->scopedStmt;
+            if (isa<Block>(body)) {
+              auto contents = to<Block>(body)->contents;
+              Stmt last = contents.back();
+              if (isa<Assign>(last)) {
+                const auto assign = to<Assign>(last);
+                if (isa<Add>(assign->rhs) && assign->lhs == iter) {
+                  const auto add = to<Add>(assign->rhs);
+                  if (add->a == assign->lhs && isa<Literal>(add->b)) {
+                    const auto inc = to<Literal>(add->b);
+                    if ((inc->type.isInt()  && inc->equalsScalar(1)) ||
+                        (inc->type.isUInt() && inc->equalsScalar(1))) {
+                      Expr loopCount = simplify(Sub::make(end, iter));
+                      contents.pop_back();
+                      body = Block::make(contents);
+                      body = DuplicateBody(loopCount).rewrite(body);
+                      if (body.defined()) {
+                        body = Block::make(body, Assign::make(iter, end));
+                        stmt = IfThenElse::make(op->cond, body);
+                        return;
+                      }
+                    }
+                  }
+                }
+              }
+            }
+          }
+        }
+      }
+      IRRewriter::visit(op);
+    }
+  };
+  simplifiedStmt = RemoveRedundantLoops().rewrite(simplifiedStmt);
+
   return simplifiedStmt;
 }
 
 }}
```

### Comparing `tensora-0.0.6/src/taco/src/lower/expr_tools.cpp` & `tensora-0.0.7/src/taco/src/lower/expr_tools.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -185,14 +185,23 @@
 
 private:
   set<IndexVar> vars;
   IndexExpr     subExpr;
 
   using IndexExprVisitorStrict::visit;
 
+  void visit(const IndexVarNode* op) {
+    IndexVar var(op);
+    if (util::contains(vars, var)) {
+      subExpr = op;
+      return;
+    }
+    subExpr = IndexExpr();
+  }
+
   void visit(const AccessNode* op) {
     // If any variable is in the set of index variables, then the expression
     // has not been emitted at a previous level, so we keep it.
     for (auto& indexVar : op->indexVars) {
       if (util::contains(vars, indexVar)) {
         subExpr = op;
         return;
@@ -248,14 +257,18 @@
     subExpr = binarySubExpr(op);
   }
 
   void visit(const DivNode* op) {
     subExpr = binarySubExpr(op);
   }
 
+  void visit(const CallNode* op) {
+    taco_not_supported_yet;
+  }
+
   void visit(const CastNode* op) {
     taco_not_supported_yet;
   }
 
   void visit(const CallIntrinsicNode* op) {
     taco_not_supported_yet;
   }
```

### Comparing `tensora-0.0.6/src/taco/src/lower/expr_tools.h` & `tensora-0.0.7/src/taco/src/lower/expr_tools.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/lower/iteration_forest.cpp` & `tensora-0.0.7/src/taco/src/lower/iteration_forest.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/lower/iteration_forest.h` & `tensora-0.0.7/src/taco/src/lower/iteration_forest.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/lower/iteration_graph.cpp` & `tensora-0.0.7/src/taco/src/lower/iteration_graph.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/lower/iteration_graph.h` & `tensora-0.0.7/src/taco/src/lower/iteration_graph.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/lower/iterator.cpp` & `tensora-0.0.7/src/taco/src/lower/iterator.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #include "taco/index_notation/index_notation.h"
 #include "taco/index_notation/index_notation_nodes.h"
 #include "mode_access.h"
 #include "taco/ir/ir.h"
 #include "taco/storage/storage.h"
 #include "taco/storage/array.h"
 #include "taco/util/strings.h"
+#include "taco/lower/mode_format_impl.h"
 
 using namespace std;
 using namespace taco::ir;
 
 namespace taco {
 
 // class Iterator
@@ -24,51 +25,78 @@
   ir::Expr tensor;
   ir::Expr posVar;
   ir::Expr coordVar;
   ir::Expr endVar;
   ir::Expr segendVar;
   ir::Expr validVar;
   ir::Expr beginVar;
+
+  // AccessWindow represents a window (or slice) into a tensor mode, given by
+  // the expressions representing an upper and lower bound. An iterator
+  // is windowed if window is not NULL.
+  struct Window {
+    // windowVar is a Var specific to this iterator. It is intended to
+    // be used as temporary storage to avoid duplicate memory loads of
+    // expressions that are used in window/stride related bounds checking.
+    ir::Expr windowVar;
+    ir::Expr lo;
+    ir::Expr hi;
+    ir::Expr stride;
+    Window(ir::Expr _lo, ir::Expr _hi, ir::Expr _stride, ir::Expr _windowVar) :
+      windowVar(_windowVar), lo(_lo), hi(_hi), stride(_stride) {};
+  };
+  std::unique_ptr<Window> window;
+  Iterator indexSetIterator;
 };
 
 Iterator::Iterator() : content(nullptr) {
 }
 
 Iterator::Iterator(std::shared_ptr<Content> content) : content(content) {
 }
 
-Iterator::Iterator(IndexVar indexVar) : content(new Content) {
+Iterator::Iterator(IndexVar indexVar, bool isFull) : content(new Content) {
   content->indexVar = indexVar;
-  content->coordVar = Var::make(indexVar.getName(), Int());
+  content->coordVar = Var::make(indexVar.getName(), indexVar.getDataType());
+  content->posVar = Var::make(indexVar.getName() + "_pos", indexVar.getDataType());
+
+  if (!isFull) {
+    content->beginVar = Var::make(indexVar.getName() + "_begin", indexVar.getDataType());
+    content->endVar = Var::make(indexVar.getName() + "_end", indexVar.getDataType());
+  }
 }
 
 Iterator::Iterator(ir::Expr tensor) : content(new Content) {
   content->tensor = tensor;
   content->posVar = 0;
   content->coordVar = 0;
   content->endVar = 1;
 }
 
 Iterator::Iterator(IndexVar indexVar, Expr tensor, Mode mode, Iterator parent,
-                   string name) : content(new Content) {
+                   string name, bool useNameForPos) : content(new Content) {
   content->indexVar = indexVar;
 
   content->mode = mode;
   content->parent = parent;
   content->parent.setChild(*this);
 
   string modeName = mode.getName();
   content->tensor = tensor;
 
-  content->posVar   = Var::make("p" + modeName,            Int());
-  content->endVar   = Var::make("p" + modeName + "_end",   Int());
-  content->beginVar = Var::make("p" + modeName + "_begin", Int());
+  string posNamePrefix = "p" + modeName;
+  if (useNameForPos) {
+    posNamePrefix = name;
+  }
+  content->posVar   = Var::make(name,            indexVar.getDataType());
+  content->endVar   = Var::make("p" + modeName + "_end",   indexVar.getDataType());
+  content->beginVar = Var::make("p" + modeName + "_begin", indexVar.getDataType());
 
-  content->coordVar = Var::make(name, Int());
-  content->segendVar = Var::make(modeName + "_segend", Int());
+  content->coordVar = Var::make(name, indexVar.getDataType());
+  content->segendVar = Var::make(modeName + "_segend", indexVar.getDataType());
   content->validVar = Var::make("v" + modeName, Bool);
 }
 
 bool Iterator::isRoot() const {
   return !getParent().defined();
 }
 
@@ -149,15 +177,15 @@
 
 bool Iterator::isModeIterator() const {
   return content->mode.defined();
 }
 
 bool Iterator::isFull() const {
   taco_iassert(defined());
-  if (isDimensionIterator()) return true;
+  if (isDimensionIterator()) return !content->beginVar.defined() && !content->endVar.defined();
   return getMode().defined() && getMode().getModeFormat().isFull();
 }
 
 bool Iterator::isOrdered() const {
   taco_iassert(defined());
   if (isDimensionIterator()) return true;
   return getMode().defined() && getMode().getModeFormat().isOrdered();
@@ -177,14 +205,20 @@
 
 bool Iterator::isCompact() const {
   taco_iassert(defined());
   if (isDimensionIterator()) return true;
   return getMode().defined() && getMode().getModeFormat().isCompact();
 }
 
+bool Iterator::isZeroless() const {
+  taco_iassert(defined());
+  if (isDimensionIterator()) return false;
+  return getMode().defined() && getMode().getModeFormat().isZeroless();
+}
+
 bool Iterator::hasCoordIter() const {
   taco_iassert(defined());
   if (isDimensionIterator()) return false;
   return getMode().defined() && getMode().getModeFormat().hasCoordValIter();
 }
 
 bool Iterator::hasPosIter() const {
@@ -207,19 +241,42 @@
 
 bool Iterator::hasAppend() const {
   taco_iassert(defined());
   if (isDimensionIterator()) return false;
   return getMode().defined() && getMode().getModeFormat().hasAppend();
 }
 
+bool Iterator::hasSeqInsertEdge() const {
+  taco_iassert(defined());
+  if (isDimensionIterator()) return false;
+  return getMode().defined() && getMode().getModeFormat().hasSeqInsertEdge();
+}
+
+bool Iterator::hasInsertCoord() const {
+  taco_iassert(defined());
+  if (isDimensionIterator()) return false;
+  return getMode().defined() && getMode().getModeFormat().hasInsertCoord();
+}
+
+bool Iterator::isYieldPosPure() const {
+  taco_iassert(defined());
+  if (isDimensionIterator()) return false;
+  return getMode().defined() && getMode().getModeFormat().isYieldPosPure();
+}
+
 ModeFunction Iterator::coordBounds(const std::vector<ir::Expr>& coords) const {
   taco_iassert(defined() && content->mode.defined());
   return getMode().getModeFormat().impl->coordIterBounds(coords, getMode());
 }
 
+ModeFunction Iterator::coordBounds(const ir::Expr& parentPos) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->coordBounds(parentPos, getMode());
+}
+
 ModeFunction Iterator::coordAccess(const std::vector<ir::Expr>& coords) const {
   taco_iassert(defined() && content->mode.defined());
   return getMode().getModeFormat().impl->coordIterAccess(getParent().getPosVar(),
                                                    coords, getMode());
 }
 
 ModeFunction Iterator::posBounds(const ir::Expr& parentPos) const {
@@ -300,23 +357,130 @@
 
 Stmt Iterator::getAppendFinalizeLevel(const Expr& szPrev, const Expr& sz) const{
   taco_iassert(defined() && content->mode.defined());
   return getMode().getModeFormat().impl->getAppendFinalizeLevel(szPrev, sz,
                                                               getMode());
 }
 
+Expr Iterator::getAssembledSize(const Expr& prevSize) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->getAssembledSize(prevSize, getMode());
+}
+
+Stmt Iterator::getSeqInitEdges(const Expr& prevSize, 
+    const std::vector<AttrQueryResult>& queries) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->getSeqInitEdges(prevSize, queries, 
+                                                         getMode());
+}
+
+Stmt Iterator::getSeqInsertEdge(const Expr& parentPos, 
+    const std::vector<Expr>& coords, 
+    const std::vector<AttrQueryResult>& queries) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->getSeqInsertEdge(parentPos, coords, 
+                                                          queries, getMode());
+}
+
+Stmt Iterator::getInitCoords(const Expr& prevSize, 
+    const std::vector<AttrQueryResult>& queries) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->getInitCoords(prevSize, queries, 
+                                                       getMode());
+}
+
+Stmt Iterator::getInitYieldPos(const Expr& prevSize) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->getInitYieldPos(prevSize, getMode());
+}
+
+ModeFunction Iterator::getYieldPos(const Expr& parentPos, 
+    const std::vector<Expr>& coords) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->getYieldPos(parentPos, coords, 
+                                                     getMode());
+}
+
+Stmt Iterator::getInsertCoord(const Expr& parentPos, const Expr& pos, 
+    const std::vector<Expr>& coords) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->getInsertCoord(parentPos, pos, coords, 
+                                                        getMode());
+}
+
+Stmt Iterator::getFinalizeYieldPos(const Expr& prevSize) const {
+  taco_iassert(defined() && content->mode.defined());
+  return getMode().getModeFormat().impl->getFinalizeYieldPos(prevSize, 
+                                                             getMode());
+}
+
 bool Iterator::defined() const {
   return content != nullptr;
 }
 
+bool Iterator::isWindowed() const {
+  return this->content->window != nullptr;
+}
+
+ir::Expr Iterator::getWindowLowerBound() const {
+  taco_iassert(this->isWindowed());
+  return this->content->window->lo;
+}
+
+ir::Expr Iterator::getWindowUpperBound() const {
+  taco_iassert(this->isWindowed());
+  return this->content->window->hi;
+}
+
+ir::Expr Iterator::getStride() const {
+  taco_iassert(this->isWindowed());
+  return this->content->window->stride;
+}
+
+ir::Expr Iterator::getWindowVar() const {
+  taco_iassert(this->isWindowed());
+  return this->content->window->windowVar;
+}
+
+bool Iterator::isStrided() const {
+  // It's not necessary but makes things simpler to require a window in order
+  // to have a stride.
+  taco_iassert(this->isWindowed());
+  auto strideLiteral = this->content->window->stride.as<ir::Literal>();
+  return !(strideLiteral != nullptr && strideLiteral->getIntValue() == 1);
+}
+
+void Iterator::setWindowBounds(ir::Expr lo, ir::Expr hi, ir::Expr stride) {
+  auto windowVarName = this->getIndexVar().getName() + this->getMode().getName() + "_window";
+  auto wvar = ir::Var::make(windowVarName, Int());
+  this->content->window = std::make_unique<Content::Window>(Content::Window(lo, hi, stride, wvar));
+}
+
+bool Iterator::hasIndexSet() const {
+  return this->content->indexSetIterator.defined();
+}
+Iterator Iterator::getIndexSetIterator() const {
+  taco_iassert(this->hasIndexSet());
+  return this->content->indexSetIterator;
+}
+
+void Iterator::setIndexSetIterator(Iterator iter) {
+  this->content->indexSetIterator = iter;
+}
+
 bool operator==(const Iterator& a, const Iterator& b) {
   if (a.isDimensionIterator() && b.isDimensionIterator()) {
     return a.getIndexVar() == b.getIndexVar();
   }
-  return a.content == b.content;
+  if (a.content == b.content) {
+    return true;
+  }
+
+  return (a.getIndexVar() == b.getIndexVar() && a.getTensor() == b.getTensor()
+      && a.getParent() == b.getParent());
 }
 
 bool operator<(const Iterator& a, const Iterator& b) {
   if (a == b) return false;
   return a.content < b.content;
 }
 
@@ -336,81 +500,82 @@
 // class Iterators
 struct Iterators::Content {
   map<ModeAccess,Iterator> levelIterators;
   map<Iterator,ModeAccess> modeAccesses;
   map<IndexVar,Iterator>   modeIterators;
 };
 
-
 Iterators::Iterators()
   : content(new Content)
 {
 }
 
 
-static std::map<TensorVar, ir::Expr> createIRTensorVars(IndexStmt stmt)
-{
-  std::map<TensorVar, ir::Expr> tensorVars;
-
-  // Create result and parameter variables
-  vector<TensorVar> results = getResults(stmt);
-  vector<TensorVar> arguments = getArguments(stmt);
-  vector<TensorVar> temporaries = getTemporaries(stmt);
-
-  // Convert tensor results, arguments and temporaries to IR variables
-  map<TensorVar, Expr> resultVars;
-  vector<Expr> resultsIR = createVars(results, &resultVars);
-  tensorVars.insert(resultVars.begin(), resultVars.end());
-  vector<Expr> argumentsIR = createVars(arguments, &tensorVars);
-  vector<Expr> temporariesIR = createVars(temporaries, &tensorVars);
-
-  return tensorVars;
-}
-
-
 Iterators::Iterators(IndexStmt stmt) : Iterators(stmt, createIRTensorVars(stmt))
 {
 }
 
 
 Iterators::Iterators(IndexStmt stmt, const map<TensorVar, Expr>& tensorVars)
 : Iterators()
 {
-  // Create dimension iteratorss
+  ProvenanceGraph provGraph = ProvenanceGraph(stmt);
+  set<IndexVar> underivedAdded;
+  set<IndexVar> computeVars;
+  // Create dimension iterators
   match(stmt,
     function<void(const ForallNode*, Matcher*)>([&](auto n, auto m) {
-      content->modeIterators.insert({n->indexVar, n->indexVar});
+      content->modeIterators.insert({n->indexVar, Iterator(n->indexVar, !provGraph.hasCoordBounds(n->indexVar)
+                                                                              && provGraph.isCoordVariable(n->indexVar))});
+      for (const IndexVar& underived : provGraph.getUnderivedAncestors(n->indexVar)) {
+        if (!underivedAdded.count(underived)) {
+          content->modeIterators.insert({underived, underived});
+          underivedAdded.insert(underived);
+        }
+      }
+
+      // Insert all children of current index variable into iterators as well
+      for (const IndexVar& child : provGraph.getChildren(n->indexVar)) {
+        if (!underivedAdded.count(child)) {
+          content->modeIterators.insert({child, child});
+          underivedAdded.insert(child);
+        }
+      }
+
       m->match(n->stmt);
+    }),
+    function<void(const IndexVarNode*)>([&](const IndexVarNode* var) {
+
     })
   );
 
   // Create access iterators
   match(stmt,
     function<void(const AccessNode*)>([&](auto n) {
       taco_iassert(util::contains(tensorVars, n->tensorVar));
       Expr tensorIR = tensorVars.at(n->tensorVar);
       Format format = n->tensorVar.getFormat();
-      createAccessIterators(Access(n), format, tensorIR);
+      this->createAccessIterators(Access(n), format, tensorIR, provGraph, tensorVars);
     }),
     function<void(const AssignmentNode*, Matcher*)>([&](auto n, auto m) {
       m->match(n->rhs);
-      m->match(n->lhs);
+      m->match(n->lhs); 
     })
   );
 
-  // Reverse the levelITerators map for fast modeAccess lookup
+  // Reverse the levelIterators map for fast modeAccess lookup
   for (auto& iterator : content->levelIterators) {
     content->modeAccesses.insert({iterator.second, iterator.first});
   }
 }
 
 
-void
-Iterators::createAccessIterators(Access access, Format format, Expr tensorIR)
-{
+void Iterators::createAccessIterators(Access access, Format format, Expr tensorIR,
+                                      ProvenanceGraph provGraph,
+                                      const map<TensorVar, Expr> &tensorVars) {
   TensorVar tensorConcrete = access.getTensorVar();
   taco_iassert(tensorConcrete.getOrder() == format.getOrder())
       << tensorConcrete << ", Format" << format;
   Shape shape = tensorConcrete.getType().getShape();
 
   Iterator parent(tensorIR);
   content->levelIterators.insert({{access,0}, parent});
@@ -427,38 +592,81 @@
                       modeNumber, level);
 
     int pos = 0;
     for (auto& modeType : modeTypePack.getModeFormats()) {
       int modeNumber = format.getModeOrdering()[level-1];
       Dimension dim = shape.getDimension(modeNumber);
       IndexVar indexVar = access.getIndexVars()[modeNumber];
+      IndexVar iteratorIndexVar;
+      if (!provGraph.getPosIteratorDescendant(indexVar, &iteratorIndexVar)) {
+        iteratorIndexVar = indexVar;
+      }
+      else if (!provGraph.isPosOfAccess(iteratorIndexVar, access)) {
+        // want to iterate across level as a position variable if has irregular descendant, but otherwise iterate normally
+        iteratorIndexVar = indexVar;
+      }
       Mode mode(tensorIR, dim, level, modeType, modePack, pos,
                 parentModeType);
 
-      string name = indexVar.getName() + tensorConcrete.getName();
-      Iterator iterator(indexVar, tensorIR, mode, parent, name);
+      string name = iteratorIndexVar.getName() + tensorConcrete.getName();
+      Iterator iterator(iteratorIndexVar, tensorIR, mode, parent, name, true);
+
+      // If the access that this iterator corresponds to has a window, then
+      // adjust the iterator appropriately.
+      if (access.isModeWindowed(modeNumber)) {
+        auto lo = ir::Literal::make(access.getWindowLowerBound(modeNumber));
+        auto hi = ir::Literal::make(access.getWindowUpperBound(modeNumber));
+        auto stride = ir::Literal::make(access.getStride(modeNumber));
+        iterator.setWindowBounds(lo, hi, stride);
+      }
+      // If the access that corresponds to this iterator has an index set,
+      // then we need to construct an iterator for the index set.
+      if (access.isModeIndexSet(modeNumber)) {
+        auto tv = access.getModeIndexSetTensor(modeNumber);
+        auto tvVar = tensorVars.at(tv);
+        auto tvFormat = tv.getFormat();
+        auto tvShape = tv.getType().getShape();
+        auto accessIvar = access.getIndexVars()[modeNumber];
+        ModePack tvModePack(1, tvFormat.getModeFormats()[0], tvVar, 0, 1);
+        Mode tvMode(tvVar, tvShape.getDimension(0), 1, tvFormat.getModeFormats()[0], tvModePack, 0, ModeFormat());
+        // Finally, construct the iterator and register it as an indexSetIterator.
+        auto iter = Iterator(accessIvar, tvVar, tvMode, {tvVar}, accessIvar.getName() + tv.getName() + "_filter");
+        iterator.setIndexSetIterator(iter);
+        // Also add the iterator to the modeAccesses map.
+        content->modeAccesses.insert({iter, {access, modeNumber + 1}});
+      }
+
       content->levelIterators.insert({{access,modeNumber+1}, iterator});
+      if (iteratorIndexVar != indexVar) {
+        // add to allowing lowering to find correct iterator for this pos variable
+        content->modeIterators[iteratorIndexVar] = iterator;
+      }
 
       parent = iterator;
       parentModeType = modeType;
       pos++;
       level++;
     }
   }
 }
 
 Iterator Iterators::levelIterator(ModeAccess modeAccess) const
 {
   taco_iassert(content != nullptr);
   taco_iassert(util::contains(content->levelIterators, modeAccess))
       << "Cannot find " << modeAccess << " in "
-      << util::join(content->levelIterators);
+      << util::join(content->levelIterators) << "\n" << modeAccess.getAccess();
   return content->levelIterators.at(modeAccess);
 }
 
+std::map<ModeAccess,Iterator> Iterators::levelIterators() const
+{
+  return content->levelIterators;
+}
+
 
 ModeAccess Iterators::modeAccess(Iterator iterator) const
 {
   taco_iassert(content != nullptr);
   taco_iassert(util::contains(content->modeAccesses, iterator));
   return content->modeAccesses.at(iterator);
 }
@@ -467,14 +675,18 @@
 Iterator Iterators::modeIterator(IndexVar indexVar) const
 {
   taco_iassert(content != nullptr);
   taco_iassert(util::contains(content->modeIterators, indexVar));
   return content->modeIterators.at(indexVar);
 }
 
+std::map<IndexVar, Iterator> Iterators::modeIterators() const {
+  return content->modeIterators;
+}
+
 
 // Free functions
 std::vector<Iterator> getAppenders(const std::vector<Iterator>& iterators) {
   vector<Iterator> appendIterators;
   for (auto& iterator : iterators) {
     if (iterator.hasAppend()) {
       appendIterators.push_back(iterator);
```

### Comparing `tensora-0.0.6/src/taco/src/lower/lower.cpp` & `tensora-0.0.7/src/taco/src/lower/lower.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 #include <map>
 
 #include "taco/index_notation/index_notation.h"
 #include "taco/index_notation/index_notation_nodes.h"
 
 #include "taco/ir/ir.h"
 #include "taco/ir/simplify.h"
-#include "ir/ir_generators.h"
+#include "taco/ir/ir_generators.h"
+#include "taco/ir/ir_printer.h"
 
 #include "taco/lower/lowerer_impl.h"
+#include "taco/lower/lowerer_impl_imperative.h"
 #include "taco/lower/iterator.h"
 #include "mode_access.h"
 
 #include "error/error_checks.h"
 #include "taco/error/error_messages.h"
 #include "taco/util/name_generator.h"
 #include "taco/util/collections.h"
@@ -28,37 +30,40 @@
 using namespace std;
 using namespace taco::ir;
 
 namespace taco {
 
 
 // class Lowerer
-Lowerer::Lowerer() : impl(new LowererImpl()) {
+Lowerer::Lowerer() : impl(new LowererImplImperative()) {
 }
 
 Lowerer::Lowerer(LowererImpl* impl) : impl(impl) {
 }
 
 std::shared_ptr<LowererImpl> Lowerer::getLowererImpl() {
   return impl;
 }
 
-ir::Stmt lower(IndexStmt stmt, std::string name, bool assemble, bool compute,
+ir::Stmt lower(IndexStmt stmt, std::string name, 
+               bool assemble, bool compute, bool pack, bool unpack,
                Lowerer lowerer) {
   string reason;
   taco_iassert(isLowerable(stmt, &reason))
       << "Not lowerable, because " << reason << ": " << stmt;
-  ir::Stmt lowered = lowerer.getLowererImpl()->lower(stmt, name, assemble, compute);
-
-  std::string messages;
-  verify(lowered, &messages);
-  if (!messages.empty()) {
-    std::cerr << "Verifier messages:\n" << messages << "\n";
-  }
   
+  ir::Stmt lowered = lowerer.getLowererImpl()->lower(stmt, name, assemble, compute, pack, unpack);
+
+  // TODO: re-enable this
+  // std::string messages;
+  // verify(lowered, &messages);
+  // if (!messages.empty()) {
+  //   std::cerr << "Verifier messages:\n" << messages << "\n";
+  // }
+
   return lowered;
 }
 
 
 bool isLowerable(IndexStmt stmt, std::string* reason) {
   INIT_REASON(reason);
```

### Comparing `tensora-0.0.6/src/taco/src/lower/lowerer_impl.cpp` & `tensora-0.0.7/src/taco/src/index_notation/provenance_graph.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,1546 +1,1422 @@
-#include "taco/lower/lowerer_impl.h"
-
 #include "taco/index_notation/index_notation.h"
+
+#include <algorithm>
+#include <taco/ir/simplify.h>
+#include "lower/mode_access.h"
+
+#include "error/error_checks.h"
+#include "taco/error/error_messages.h"
+
+#include "taco/index_notation/schedule.h"
+#include "taco/index_notation/transformations.h"
 #include "taco/index_notation/index_notation_nodes.h"
-#include "taco/index_notation/index_notation_visitor.h"
-#include "taco/ir/ir.h"
-#include "ir/ir_generators.h"
-#include "taco/ir/ir_visitor.h"
-#include "taco/ir/simplify.h"
-#include "taco/lower/iterator.h"
-#include "taco/lower/merge_lattice.h"
-#include "mode_access.h"
-#include "taco/util/collections.h"
+#include "taco/index_notation/index_notation_rewriter.h"
+#include "taco/index_notation/index_notation_printer.h"
+#include "taco/lower/lower.h"
+#include "taco/lower/mode_format_impl.h"
+
+#include "taco/util/name_generator.h"
+#include "taco/util/scopedmap.h"
 
 using namespace std;
-using namespace taco::ir;
-using taco::util::combine;
 
 namespace taco {
 
-class LowererImpl::Visitor : public IndexNotationVisitorStrict {
-public:
-  Visitor(LowererImpl* impl) : impl(impl) {}
-  Stmt lower(IndexStmt stmt) {
-    this->stmt = Stmt();
-    impl->accessibleIterators.scope();
-    IndexStmtVisitorStrict::visit(stmt);
-    impl->accessibleIterators.unscope();
-    return this->stmt;
-  }
-  Expr lower(IndexExpr expr) {
-    this->expr = Expr();
-    IndexExprVisitorStrict::visit(expr);
-    return this->expr;
-  }
-private:
-  LowererImpl* impl;
-  Expr expr;
-  Stmt stmt;
-  using IndexNotationVisitorStrict::visit;
-  void visit(const AssignmentNode* node)    { stmt = impl->lowerAssignment(node); }
-  void visit(const YieldNode* node)         { stmt = impl->lowerYield(node); }
-  void visit(const ForallNode* node)        { stmt = impl->lowerForall(node); }
-  void visit(const WhereNode* node)         { stmt = impl->lowerWhere(node); }
-  void visit(const MultiNode* node)         { stmt = impl->lowerMulti(node); }
-  void visit(const SequenceNode* node)      { stmt = impl->lowerSequence(node); }
-  void visit(const AccessNode* node)        { expr = impl->lowerAccess(node); }
-  void visit(const LiteralNode* node)       { expr = impl->lowerLiteral(node); }
-  void visit(const NegNode* node)           { expr = impl->lowerNeg(node); }
-  void visit(const AddNode* node)           { expr = impl->lowerAdd(node); }
-  void visit(const SubNode* node)           { expr = impl->lowerSub(node); }
-  void visit(const MulNode* node)           { expr = impl->lowerMul(node); }
-  void visit(const DivNode* node)           { expr = impl->lowerDiv(node); }
-  void visit(const SqrtNode* node)          { expr = impl->lowerSqrt(node); }
-  void visit(const CastNode* node)          { expr = impl->lowerCast(node); }
-  void visit(const CallIntrinsicNode* node) { expr = impl->lowerCallIntrinsic(node); }
-  void visit(const ReductionNode* node)  {
-    taco_ierror << "Reduction nodes not supported in concrete index notation";
+void IndexVarRel::print(std::ostream& stream) const {
+  if (ptr == nullptr) {
+    stream << "undefined";
   }
-};
-
-LowererImpl::LowererImpl() : visitor(new Visitor(this)) {
-}
-
-
-static void createCapacityVars(const map<TensorVar, Expr>& tensorVars,
-                               map<Expr, Expr>* capacityVars) {
-  for (auto& tensorVar : tensorVars) {
-    Expr tensor = tensorVar.second;
-    Expr capacityVar = Var::make(util::toString(tensor) + "_capacity", Int());
-    capacityVars->insert({tensor, capacityVar});
+  else {
+    switch(getRelType()) {
+      case SPLIT:
+        getNode<SplitRelNode>()->print(stream);
+        break;
+      case DIVIDE:
+        getNode<DivideRelNode>()->print(stream);
+        break;
+      case POS:
+        getNode<PosRelNode>()->print(stream);
+        break;
+      case FUSE:
+        getNode<FuseRelNode>()->print(stream);
+        break;
+      case BOUND:
+        getNode<BoundRelNode>()->print(stream);
+        break;
+      case PRECOMPUTE:
+        getNode<PrecomputeRelNode>()->print(stream);
+        break;
+      default:
+        taco_ierror;
+    }
   }
 }
 
-static void createReducedValueVars(const vector<Access>& inputAccesses,
-                                   map<Access, Expr>* reducedValueVars) {
-  for (const auto& access : inputAccesses) {
-    const TensorVar inputTensor = access.getTensorVar();
-    const std::string name = inputTensor.getName() + "_val";
-    const Datatype type = inputTensor.getType().getDataType();
-    reducedValueVars->insert({access, Var::make(name, type)});
+bool IndexVarRel::equals(const IndexVarRel &rel) const {
+  if (getRelType() != rel.getRelType()) {
+    return false;
+  }
+
+  switch(getRelType()) {
+    case SPLIT:
+      return getNode<SplitRelNode>()->equals(*rel.getNode<SplitRelNode>());
+    case DIVIDE:
+      return getNode<DivideRelNode>()->equals(*rel.getNode<DivideRelNode>());
+    case POS:
+      return getNode<PosRelNode>()->equals(*rel.getNode<PosRelNode>());
+    case FUSE:
+      return getNode<FuseRelNode>()->equals(*rel.getNode<FuseRelNode>());
+    case UNDEFINED:
+      return true;
+    case BOUND:
+      return getNode<BoundRelNode>()->equals(*rel.getNode<BoundRelNode>());
+    case PRECOMPUTE:
+      return getNode<PrecomputeRelNode>()->equals(*rel.getNode<PrecomputeRelNode>());
+    default:
+      taco_ierror;
+      return false;
   }
 }
 
-/// Returns true iff `stmt` modifies an array
-static bool hasStores(Stmt stmt) {
-  struct FindStores : IRVisitor {
-    bool hasStore;
+bool operator==(const IndexVarRel& a, const IndexVarRel& b) {
+  return a.equals(b);
+}
 
-    using IRVisitor::visit;
+std::ostream& operator<<(std::ostream& stream, const IndexVarRel& rel) {
+  rel.print(stream);
+  return stream;
+}
 
-    void visit(const Store* stmt) {
-      hasStore = true;
-    }
+IndexVarRelType IndexVarRel::getRelType() const {
+  if (ptr == NULL) return UNDEFINED;
+  return getNode()->relType;
+}
 
-    bool hasStores(Stmt stmt) {
-      hasStore = false;
-      stmt.accept(this);
-      return hasStore;
-    }
-  };
-  return stmt.defined() && FindStores().hasStores(stmt);
+std::vector<ir::Expr> IndexVarRelNode::computeRelativeBound(std::set<IndexVar> definedVars, std::map<IndexVar, std::vector<ir::Expr>> computedBounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_ierror;
+  return {};
 }
 
-Stmt
-LowererImpl::lower(IndexStmt stmt, string name, bool assemble, bool compute)
-{
-  this->assemble = assemble;
-  this->compute = compute;
-
-  // Create result and parameter variables
-  vector<TensorVar> results = getResults(stmt);
-  vector<TensorVar> arguments = getArguments(stmt);
-  vector<TensorVar> temporaries = getTemporaries(stmt);
-
-  // Convert tensor results and arguments IR variables
-  map<TensorVar, Expr> resultVars;
-  vector<Expr> resultsIR = createVars(results, &resultVars);
-  tensorVars.insert(resultVars.begin(), resultVars.end());
-  vector<Expr> argumentsIR = createVars(arguments, &tensorVars);
-
-  // Create variables for temporaries
-  // TODO Remove this
-  for (auto& temp : temporaries) {
-    ir::Expr irVar = ir::Var::make(temp.getName(), temp.getType().getDataType(),
-                                   true, true);
-    tensorVars.insert({temp, irVar});
-  }
-
-  // Create variables for keeping track of result values array capacity
-  createCapacityVars(resultVars, &capacityVars);
-
-  // Create iterators
-  iterators = Iterators(stmt, tensorVars);
-
-  vector<Access> inputAccesses, resultAccesses;
-  set<Access> reducedAccesses;
-  inputAccesses = getArgumentAccesses(stmt);
-  std::tie(resultAccesses, reducedAccesses) = getResultAccesses(stmt);
-
-  // Create variables that represent the reduced values of duplicated tensor 
-  // components
-  createReducedValueVars(inputAccesses, &reducedValueVars);
-
-  map<TensorVar, Expr> scalars;
-
-  // Define and initialize dimension variables
-  vector<IndexVar> indexVars = getIndexVars(stmt);
-  for (auto& indexVar : indexVars) {
-    Expr dimension;
-    match(stmt,
-      function<void(const AssignmentNode*, Matcher*)>([&](
-          const AssignmentNode* n, Matcher* m) {
-        m->match(n->rhs);
-        if (!dimension.defined()) {
-          auto ivars = n->lhs.getIndexVars();
-          int loc = (int)distance(ivars.begin(),
-                                  find(ivars.begin(),ivars.end(), indexVar));
-          dimension = GetProperty::make(tensorVars.at(n->lhs.getTensorVar()),
-                                        TensorProperty::Dimension, loc);
-        }
-      }),
-      function<void(const AccessNode*)>([&](const AccessNode* n) {
-        auto indexVars = n->indexVars;
-        if (util::contains(indexVars, indexVar)) {
-          int loc = (int)distance(indexVars.begin(),
-                                  find(indexVars.begin(),indexVars.end(),
-                                       indexVar));
-          dimension = GetProperty::make(tensorVars.at(n->tensorVar),
-                                        TensorProperty::Dimension, loc);
-        }
-      })
-    );
-    dimensions.insert({indexVar, dimension});
-  }
+std::vector<ir::Expr> IndexVarRelNode::deriveIterBounds(IndexVar indexVar, std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                                        std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                       std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                       Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_ierror;
+  return {};
+}
 
-  // Define and initialize scalar results and arguments
-  if (generateComputeCode()) {
-    for (auto& result : results) {
-      if (isScalar(result.getType())) {
-        taco_iassert(!util::contains(scalars, result));
-        taco_iassert(util::contains(tensorVars, result));
-        scalars.insert({result, tensorVars.at(result)});
-        header.push_back(defineScalarVariable(result, true));
-      }
-    }
-    for (auto& argument : arguments) {
-      if (isScalar(argument.getType())) {
-        taco_iassert(!util::contains(scalars, argument));
-        taco_iassert(util::contains(tensorVars, argument));
-        scalars.insert({argument, tensorVars.at(argument)});
-        header.push_back(defineScalarVariable(argument, false));
-      }
-    }
-  }
+ir::Expr IndexVarRelNode::recoverVariable(IndexVar indexVar, std::map<IndexVar, ir::Expr> variableNames, Iterators iterators, std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds, std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds, ProvenanceGraph provGraph) const {
+  taco_ierror;
+  return {};
+}
 
-  // Allocate memory for scalar results
-  if (generateAssembleCode()) {
-    for (auto& result : results) {
-      if (result.getOrder() == 0) {
-        Expr resultIR = resultVars.at(result);
-        Expr vals = GetProperty::make(resultIR, TensorProperty::Values);
-        header.push_back(Allocate::make(vals, 1));
-      }
-    }
-  }
+ir::Stmt IndexVarRelNode::recoverChild(IndexVar indexVar, std::map<IndexVar, ir::Expr> variableNames, bool emitVarDecl, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_ierror;
+  return {};
+}
 
-  // Allocate and initialize append and insert mode indices
-  Stmt initializeResults = initResultArrays(resultAccesses, inputAccesses, 
-                                            reducedAccesses);
-
-  // Lower the index statement to compute and/or assemble
-  Stmt body = lower(stmt);
-
-  // Post-process result modes and allocate memory for values if necessary
-  Stmt finalizeResults = finalizeResultArrays(resultAccesses);
-
-  // Store scalar stack variables back to results
-  if (generateComputeCode()) {
-    for (auto& result : results) {
-      if (isScalar(result.getType())) {
-        taco_iassert(util::contains(scalars, result));
-        taco_iassert(util::contains(tensorVars, result));
-        Expr resultIR = scalars.at(result);
-        Expr varValueIR = tensorVars.at(result);
-        Expr valuesArrIR = GetProperty::make(resultIR, TensorProperty::Values);
-        footer.push_back(Store::make(valuesArrIR, 0, varValueIR));
-      }
-    }
-  }
+struct SplitRelNode::Content {
+  IndexVar parentVar;
+  IndexVar outerVar;
+  IndexVar innerVar;
+  size_t splitFactor;
+};
 
-  // Create function
-  return Function::make(name, resultsIR, argumentsIR,
-                        Block::blanks(Block::make(header),
-                                      initializeResults,
-                                      body,
-                                      finalizeResults,
-                                      Block::make(footer)));
+SplitRelNode::SplitRelNode(IndexVar parentVar, IndexVar outerVar, IndexVar innerVar, size_t splitFactor)
+  : IndexVarRelNode(SPLIT), content(new Content) {
+  content->parentVar = parentVar;
+  content->outerVar = outerVar;
+  content->innerVar = innerVar;
+  content->splitFactor = splitFactor;
 }
 
+const IndexVar& SplitRelNode::getParentVar() const {
+  return content->parentVar;
+}
+const IndexVar& SplitRelNode::getOuterVar() const {
+  return content->outerVar;
+}
+const IndexVar& SplitRelNode::getInnerVar() const {
+  return content->innerVar;
+}
+const size_t& SplitRelNode::getSplitFactor() const {
+  return content->splitFactor;
+}
 
-Stmt LowererImpl::lowerAssignment(Assignment assignment)
-{
-  TensorVar result = assignment.getLhs().getTensorVar();
-
-  if (generateComputeCode()) {
-    Expr var = getTensorVar(result);
-    Expr rhs = lower(assignment.getRhs());
-
-    // Assignment to scalar variables.
-    if (isScalar(result.getType())) {
-      if (!assignment.getOperator().defined()) {
-        return Assign::make(var, rhs);
-      }
-      else {
-        taco_iassert(isa<taco::Add>(assignment.getOperator()));
-        return compoundAssign(var, rhs);
-      }
-    }
-    // Assignments to tensor variables (non-scalar).
-    else {
-      Expr values = getValuesArray(result);
-      Expr loc = generateValueLocExpr(assignment.getLhs());
+void SplitRelNode::print(std::ostream &stream) const {
+  stream << "split(" << getParentVar() << ", " << getOuterVar() << ", " << getInnerVar() << ", " << getSplitFactor() << ")";
+}
 
-      Stmt computeStmt;
-      if (!assignment.getOperator().defined()) {
-        computeStmt = Store::make(values, loc, rhs);
-      }
-      else {
-        computeStmt = compoundStore(values, loc, rhs);
-      }
-      taco_iassert(computeStmt.defined());
+bool SplitRelNode::equals(const SplitRelNode &rel) const {
+  return getParentVar() == rel.getParentVar() && getOuterVar() == rel.getOuterVar()
+        && getInnerVar() == rel.getInnerVar() && getSplitFactor() == rel.getSplitFactor();
+}
 
-      return computeStmt;
-    }
-  }
-  // We're only assembling so defer allocating value memory to the end when
-  // we'll know exactly how much we need.
-  else if (generateAssembleCode()) {
-    // TODO
-    return Stmt();
-  }
-  // We're neither assembling or computing so we emit nothing.
-  else {
-    return Stmt();
-  }
-  taco_unreachable;
-  return Stmt();
+std::vector<IndexVar> SplitRelNode::getParents() const {
+  return {getParentVar()};
 }
 
+std::vector<IndexVar> SplitRelNode::getChildren() const {
+  return {getOuterVar(), getInnerVar()};
+}
 
-Stmt LowererImpl::lowerYield(Yield yield) {
-  std::vector<Expr> coords;
-  for (auto& indexVar : yield.getIndexVars()) {
-    coords.push_back(getCoordinateVar(indexVar));
-  }
-  Expr val = lower(yield.getExpr());
-  return ir::Yield::make(coords, val);
+std::vector<IndexVar> SplitRelNode::getIrregulars() const {
+  return {getOuterVar()};
 }
 
+std::vector<ir::Expr> SplitRelNode::computeRelativeBound(std::set<IndexVar> definedVars, std::map<IndexVar, std::vector<ir::Expr>> computedBounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(computedBounds.count(getParentVar()) == 1);
+  std::vector<ir::Expr> parentBound = computedBounds.at(getParentVar());
+  bool outerVarDefined = definedVars.count(getOuterVar());
+  bool innerVarDefined = definedVars.count(getInnerVar());
 
-static pair<vector<Iterator>, vector<Iterator>>
-splitAppenderAndInserters(const vector<Iterator>& results) {
-  vector<Iterator> appenders;
-  vector<Iterator> inserters;
+  if (provGraph.isPosVariable(getParentVar())) {
+    return parentBound; // splitting pos space does not change coordinate bounds
+  }
 
-  // TODO: Choose insert when the current forall is nested inside a reduction
-  for (auto& result : results) {
-    taco_iassert(result.hasAppend() || result.hasInsert())
-        << "Results must support append or insert";
+  ir::Expr splitFactorLiteral = ir::Literal::make(getSplitFactor(), variableExprs[getParentVar()].type());
 
-    if (result.hasAppend()) {
-      appenders.push_back(result);
-    }
-    else {
-      taco_iassert(result.hasInsert());
-      inserters.push_back(result);
-    }
+  if (!outerVarDefined && !innerVarDefined) {
+    return parentBound;
+  }
+  else if(outerVarDefined && !innerVarDefined) {
+    // outerVar constrains space to a length splitFactor strip starting at outerVar * splitFactor
+    ir::Expr minBound = parentBound[0];
+    minBound = ir::Add::make(minBound, ir::Mul::make(variableExprs[getOuterVar()], splitFactorLiteral));
+    ir::Expr maxBound = ir::Min::make(parentBound[1], ir::Add::make(minBound, splitFactorLiteral));
+    return {minBound, maxBound};
+  }
+  else if(!outerVarDefined && innerVarDefined) {
+    // when innerVar is defined first does not limit coordinate space
+    return parentBound;
+  }
+  else {
+    taco_iassert(outerVarDefined && innerVarDefined);
+    // outerVar and innervar constrains space to a length 1 strip starting at outerVar * splitFactor + innerVar
+    ir::Expr minBound = parentBound[0];
+    minBound = ir::Add::make(minBound, ir::Add::make(ir::Mul::make(variableExprs[getOuterVar()], splitFactorLiteral), variableExprs[getInnerVar()]));
+    ir::Expr maxBound = ir::Min::make(parentBound[1], ir::Add::make(minBound, ir::Literal::make(1, variableExprs[getParentVar()].type())));
+    return {minBound, maxBound};
   }
-
-  return {appenders, inserters};
 }
 
-
-Stmt LowererImpl::lowerForall(Forall forall)
-{
-  MergeLattice lattice = MergeLattice::make(forall, iterators);
-
-  vector<Access> resultAccesses;
-  set<Access> reducedAccesses;
-  std::tie(resultAccesses, reducedAccesses) = getResultAccesses(forall);
-
-  // Pre-allocate/initialize memory of value arrays that are full below this
-  // loops index variable
-  Stmt preInitValues = initResultArrays(forall.getIndexVar(), resultAccesses,
-                                        getArgumentAccesses(forall), 
-                                        reducedAccesses);
-
-  Stmt loops;
-  // Emit a loop that iterates over over a single iterator (optimization)
-  if (lattice.iterators().size() == 1 && lattice.iterators()[0].isUnique()) {
-    taco_iassert(lattice.points().size() == 1);
-
-    MergePoint point = lattice.points()[0];
-    Iterator iterator = lattice.iterators()[0];
-
-    vector<Iterator> locators = point.locators();
-    vector<Iterator> appenders;
-    vector<Iterator> inserters;
-    tie(appenders, inserters) = splitAppenderAndInserters(point.results());
-
-    // Emit dimension coordinate iteration loop
-    if (iterator.isDimensionIterator()) {
-      loops = lowerForallDimension(forall, point.locators(),
-                                   inserters, appenders, reducedAccesses);
+std::vector<ir::Expr> SplitRelNode::deriveIterBounds(taco::IndexVar indexVar,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                                     std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                                     Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getOuterVar() || indexVar == getInnerVar());
+  taco_iassert(parentIterBounds.size() == 1);
+  taco_iassert(parentIterBounds.count(getParentVar()) == 1);
+
+  std::vector<ir::Expr> parentBound = parentIterBounds.at(getParentVar());
+  Datatype splitFactorType = parentBound[0].type();
+  if (indexVar == getOuterVar()) {
+    ir::Expr minBound = ir::Div::make(parentBound[0], ir::Literal::make(getSplitFactor(), splitFactorType));
+    ir::Expr maxBound = ir::Div::make(ir::Add::make(parentBound[1], ir::Literal::make(getSplitFactor()-1, splitFactorType)), ir::Literal::make(getSplitFactor(), splitFactorType));
+    return {minBound, maxBound};
+  }
+  else if (indexVar == getInnerVar()) {
+    ir::Expr minBound = 0;
+    ir::Expr maxBound = ir::Literal::make(getSplitFactor(), splitFactorType);
+    return {minBound, maxBound};
+  }
+  taco_ierror;
+  return {};
+}
+
+ir::Expr SplitRelNode::recoverVariable(taco::IndexVar indexVar,
+                                       std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                       Iterators iterators, std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds, std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getParentVar());
+  taco_iassert(variableNames.count(getParentVar()) && variableNames.count(getOuterVar()) && variableNames.count(getInnerVar()));
+  Datatype splitFactorType = variableNames[getParentVar()].type();
+  return ir::Add::make(ir::Mul::make(variableNames[getOuterVar()], ir::Literal::make(getSplitFactor(), splitFactorType)), variableNames[getInnerVar()]);
+}
+
+ir::Stmt SplitRelNode::recoverChild(taco::IndexVar indexVar,
+                                       std::map<taco::IndexVar, taco::ir::Expr> variableNames, bool emitVarDecl, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getOuterVar() || indexVar == getInnerVar());
+  taco_iassert(variableNames.count(getParentVar()) && variableNames.count(getOuterVar()) && variableNames.count(getInnerVar()));
+  Datatype splitFactorType = variableNames[getParentVar()].type();
+  if (indexVar == getOuterVar()) {
+    // outerVar = parentVar - innerVar
+    ir::Expr subStmt = ir::Sub::make(variableNames[getParentVar()], variableNames[getInnerVar()]);
+    if (emitVarDecl) {
+      return ir::Stmt(ir::VarDecl::make(variableNames[getOuterVar()], subStmt));
     }
-    // Emit position iteration loop
-    else if (iterator.hasPosIter()) {
-      loops = lowerForallPosition(forall, iterator, locators,
-                                 inserters, appenders, reducedAccesses);
-    }
-    // Emit coordinate iteration loop
     else {
-      taco_iassert(iterator.hasCoordIter());
-//      taco_not_supported_yet
-      loops = Stmt();
+      return ir::Stmt(ir::Assign::make(variableNames[getOuterVar()], subStmt));
     }
   }
-  // Emit general loops to merge multiple iterators
   else {
-    loops = lowerMergeLattice(lattice, getCoordinateVar(forall.getIndexVar()),
-                              forall.getStmt(), reducedAccesses);
-  }
-//  taco_iassert(loops.defined());
-
-  if (!generateComputeCode() && !hasStores(loops)) {
-    // If assembly loop does not modify output arrays, then it can be safely 
-    // omitted.
-    loops = Stmt();
+    // innerVar = parentVar - outerVar * splitFactor
+    ir::Expr subStmt = ir::Sub::make(variableNames[getParentVar()],
+                                     ir::Mul::make(variableNames[getOuterVar()], ir::Literal::make(getSplitFactor(), splitFactorType)));
+    if (emitVarDecl) {
+      return ir::Stmt(ir::VarDecl::make(variableNames[getInnerVar()], subStmt));
+    }
+    else {
+      return ir::Stmt(ir::Assign::make(variableNames[getInnerVar()], subStmt));
+    }
   }
+}
 
-  return Block::blanks(preInitValues,
-                       loops);
+bool operator==(const SplitRelNode& a, const SplitRelNode& b) {
+  return a.equals(b);
 }
 
+struct DivideRelNode::Content {
+  IndexVar parentVar;
+  IndexVar outerVar;
+  IndexVar innerVar;
+  size_t divFactor;
+};
 
-Stmt LowererImpl::lowerForallDimension(Forall forall,
-                                       vector<Iterator> locators,
-                                       vector<Iterator> inserters,
-                                       vector<Iterator> appenders,
-                                       set<Access> reducedAccesses)
-{
-  Expr coordinate = getCoordinateVar(forall.getIndexVar());
+DivideRelNode::DivideRelNode(IndexVar parentVar, IndexVar outerVar, IndexVar innerVar, size_t divFactor)
+  : IndexVarRelNode(DIVIDE), content(new Content) {
+  content->parentVar = parentVar;
+  content->outerVar = outerVar;
+  content->innerVar = innerVar;
+  content->divFactor = divFactor;
+}
 
-  Stmt body = lowerForallBody(coordinate, forall.getStmt(),
-                              locators, inserters, appenders, reducedAccesses);
+const IndexVar& DivideRelNode::getParentVar() const {
+  return content->parentVar;
+}
+const IndexVar& DivideRelNode::getOuterVar() const {
+  return content->outerVar;
+}
+const IndexVar& DivideRelNode::getInnerVar() const {
+  return content->innerVar;
+}
+const size_t& DivideRelNode::getDivFactor() const {
+  return content->divFactor;
+}
 
-  Stmt posAppend = generateAppendPositions(appenders);
+void DivideRelNode::print(std::ostream &stream) const {
+  stream << "divide(" << getParentVar() << ", " << getOuterVar() << ", " << getInnerVar() << ", " << getDivFactor() << ")";
+}
 
-  // Emit loop with preamble and postamble
-  Expr dimension = getDimension(forall.getIndexVar());
-  bool parallelize = forall.getTags().count(Forall::PARALLELIZE);
-  return Block::blanks(For::make(coordinate, 0, dimension, 1, body,
-                                 parallelize ? LoopKind::Runtime : LoopKind::Serial, parallelize),
-                       posAppend);
+bool DivideRelNode::equals(const DivideRelNode &rel) const {
+  return getParentVar() == rel.getParentVar() && getOuterVar() == rel.getOuterVar() &&
+    getInnerVar() == rel.getInnerVar() && getDivFactor() == rel.getDivFactor();
 }
 
+std::vector<IndexVar> DivideRelNode::getParents() const {
+  return {getParentVar()};
+}
 
-Stmt LowererImpl::lowerForallCoordinate(Forall forall, Iterator iterator,
-                                        vector<Iterator> locators,
-                                        vector<Iterator> inserters,
-                                        vector<Iterator> appenders,
-                                        set<Access> reducedAccesses) {
-  taco_not_supported_yet;
-  return Stmt();
+std::vector<IndexVar> DivideRelNode::getChildren() const {
+  return {getOuterVar(), getInnerVar()};
 }
 
-Stmt LowererImpl::lowerForallPosition(Forall forall, Iterator iterator,
-                                      vector<Iterator> locators,
-                                      vector<Iterator> inserters,
-                                      vector<Iterator> appenders,
-                                      set<Access> reducedAccesses)
-{
-  Expr coordinate = getCoordinateVar(forall.getIndexVar());
-  Expr coordinateArray= iterator.posAccess(iterator.getPosVar(), 
-                                           coordinates(iterator)).getResults()[0];
-  Stmt declareCoordinate = VarDecl::make(coordinate, coordinateArray);
-
-  Stmt body = lowerForallBody(coordinate, forall.getStmt(),
-                              locators, inserters, appenders, reducedAccesses);
-
-  // Code to append positions
-  Stmt posAppend = generateAppendPositions(appenders);
-
-  // Code to compute iteration bounds
-  Stmt boundsCompute;
-  Expr startBound, endBound;
-  Expr parentPos = iterator.getParent().getPosVar();
-  if (iterator.getParent().isRoot() || iterator.getParent().isUnique()) {
-    // E.g. a compressed mode without duplicates
-    ModeFunction bounds = iterator.posBounds(parentPos);
-    boundsCompute = bounds.compute();
-    startBound = bounds[0];
-    endBound = bounds[1];
-  } else {
-    taco_iassert(iterator.isOrdered() && iterator.getParent().isOrdered());
-    taco_iassert(iterator.isCompact() && iterator.getParent().isCompact());
+std::vector<IndexVar> DivideRelNode::getIrregulars() const {
+  return {getOuterVar()};
+}
 
-    // E.g. a compressed mode with duplicates. Apply iterator chaining
-    Expr parentSegend = iterator.getParent().getSegendVar();
-    ModeFunction startBounds = iterator.posBounds(parentPos);
-    ModeFunction endBounds = iterator.posBounds(ir::Sub::make(parentSegend, 1));
-    boundsCompute = Block::make(startBounds.compute(), endBounds.compute());
-    startBound = startBounds[0];
-    endBound = endBounds[1];
-  }
-  bool parallelize = forall.getTags().count(Forall::PARALLELIZE);
-  // Loop with preamble and postamble
-  return Block::blanks(boundsCompute,
-                       For::make(iterator.getPosVar(), startBound, endBound, 1,
-                                 Block::make(declareCoordinate, body),
-                                 parallelize ? LoopKind::Runtime : LoopKind::Serial, parallelize),
-                       posAppend);
-
-}
-
-Stmt LowererImpl::lowerMergeLattice(MergeLattice lattice, Expr coordinate,
-                                    IndexStmt statement, 
-                                    const std::set<Access>& reducedAccesses)
-{
-  vector<Iterator> appenders = filter(lattice.results(),
-                                      [](Iterator it){return it.hasAppend();});
-
-  Stmt iteratorVarInits = codeToInitializeIteratorVars(lattice.iterators());
-
-  vector<Stmt> mergeLoopsVec;
-  for (MergePoint point : lattice.points()) {
-    // Each iteration of this loop generates a while loop for one of the merge
-    // points in the merge lattice.
-    IndexStmt zeroedStmt = zero(statement, getExhaustedAccesses(point,lattice));
-    MergeLattice sublattice = lattice.subLattice(point);
-    Stmt mergeLoop = lowerMergePoint(sublattice, coordinate, zeroedStmt, reducedAccesses);
-    mergeLoopsVec.push_back(mergeLoop);
-  }
-  Stmt mergeLoops = Block::make(mergeLoopsVec);
-
-  // Append position to the pos array
-  Stmt appendPositions = generateAppendPositions(appenders);
-
-  return Block::blanks(iteratorVarInits,
-                       mergeLoops,
-                       appendPositions);
-}
-
-Stmt LowererImpl::lowerMergePoint(MergeLattice pointLattice,
-                                  ir::Expr coordinate, IndexStmt statement,
-                                  const std::set<Access>& reducedAccesses)
-{
-  MergePoint point = pointLattice.points().front();
-
-  vector<Iterator> iterators = point.iterators();
-  vector<Iterator> mergers = point.mergers();
-  vector<Iterator> rangers = point.rangers();
-  vector<Iterator> locators = point.locators();
-
-  taco_iassert(iterators.size() > 0);
-  taco_iassert(mergers.size() > 0);
-  taco_iassert(rangers.size() > 0);
-
-  // Load coordinates from position iterators
-  Stmt loadPosIterCoordinates;
-  if (iterators.size() > 1) {
-    vector<Stmt> loadPosIterCoordinateStmts;
-    auto posIters = filter(iterators, [](Iterator it){return it.hasPosIter();});
-    for (auto& posIter : posIters) {
-      taco_tassert(posIter.hasPosIter());
-      ModeFunction posAccess = posIter.posAccess(posIter.getPosVar(), 
-                                                 coordinates(posIter));
-      loadPosIterCoordinateStmts.push_back(posAccess.compute());
-      loadPosIterCoordinateStmts.push_back(VarDecl::make(posIter.getCoordVar(),
-                                                          posAccess[0]));
-    }
-    loadPosIterCoordinates = Block::make(loadPosIterCoordinateStmts);
-  }
-
-  // Merge iterator coordinate variables
-  Stmt resolveCoordinate;
-  if (mergers.size() == 1) {
-    Iterator merger = mergers[0];
-    if (merger.hasPosIter()) {
-      // Just one position iterator so it is the resolved coordinate
-      ModeFunction posAccess = merger.posAccess(merger.getPosVar(), 
-                                                coordinates(merger));
-      resolveCoordinate = Block::make(posAccess.compute(),
-                                          VarDecl::make(coordinate,
-                                                        posAccess[0]));
-    }
-    else if (merger.hasCoordIter()) {
-      taco_not_supported_yet;
-    }
-    else if (merger.isDimensionIterator()) {
-      // Just one dimension iterator so resolved coordinate already exist and we
-      // do nothing
-    }
-    else {
-      taco_ierror << "Unexpected type of single iterator " << merger;
-    }
-  }
-  else {
-    // Multiple position iterators so the smallest is the resolved coordinate
-    resolveCoordinate = VarDecl::make(coordinate,
-                                      Min::make(coordinates(mergers)));
-  }
-
-  // Locate positions
-  Stmt loadLocatorPosVars = declLocatePosVars(locators);
-
-  // Deduplication loops
-  auto dupIters = filter(iterators, [](Iterator it){return !it.isUnique() && 
-                                                           it.hasPosIter();});
-  bool alwaysReduce = (mergers.size() == 1 && mergers[0].hasPosIter());
-  Stmt deduplicationLoops = reduceDuplicateCoordinates(coordinate, dupIters, 
-                                                       alwaysReduce);
-
-  // One case for each child lattice point lp
-  Stmt caseStmts = lowerMergeCases(coordinate, statement, pointLattice, 
-                                   reducedAccesses);
-
-  // Increment iterator position variables
-  Stmt incIteratorVarStmts = codeToIncIteratorVars(coordinate, iterators);
-
-  /// While loop over rangers
-  return While::make(checkThatNoneAreExhausted(rangers),
-                     Block::make(loadPosIterCoordinates,
-                                 resolveCoordinate,
-                                 loadLocatorPosVars,
-                                 deduplicationLoops,
-                                 caseStmts,
-                                 incIteratorVarStmts));
-}
-
-Stmt LowererImpl::lowerMergeCases(ir::Expr coordinate, IndexStmt stmt,
-                                  MergeLattice lattice,
-                                  const std::set<Access>& reducedAccesses)
-{
-  vector<Stmt> result;
-
-  vector<Iterator> appenders;
-  vector<Iterator> inserters;
-  tie(appenders, inserters) = splitAppenderAndInserters(lattice.results());
-
-  // Just one iterator so no conditionals
-  if (lattice.iterators().size() == 1) {
-    Stmt body = lowerForallBody(coordinate, stmt, {}, inserters, 
-                                appenders, reducedAccesses);
-    result.push_back(body);
-  }
-  else {
-    vector<pair<Expr,Stmt>> cases;
-    for (MergePoint point : lattice.points()) {
+std::vector<ir::Expr> DivideRelNode::computeRelativeBound(std::set<IndexVar> definedVars, std::map<IndexVar, std::vector<ir::Expr>> computedBounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(computedBounds.count(getParentVar()) == 1);
+  std::vector<ir::Expr> parentBound = computedBounds.at(getParentVar());
+  bool outerVarDefined = definedVars.count(getOuterVar());
+  bool innerVarDefined = definedVars.count(getInnerVar());
 
-      // Construct case expression
-      vector<Expr> coordComparisons;
-      for (Iterator iterator : point.rangers()) {
-        coordComparisons.push_back(Eq::make(iterator.getCoordVar(),coordinate));
-      }
+  if (provGraph.isPosVariable(getParentVar()) || !outerVarDefined) {
+    return parentBound; // splitting pos space does not change coordinate bounds
+  }
 
-      // Construct case body
-      IndexStmt zeroedStmt = zero(stmt, getExhaustedAccesses(point, lattice));
-      Stmt body = lowerForallBody(coordinate, zeroedStmt, {},
-                                  inserters, appenders, reducedAccesses);
+  auto divFactorType = variableExprs[getParentVar()].type();
+  auto divFactor = ir::Literal::make(getDivFactor(), divFactorType);
+  auto divFactorMinusOne = ir::Literal::make(getDivFactor() - 1, divFactorType);
+  auto dimLen = ir::Div::make(ir::Add::make(parentBound[1], divFactorMinusOne), divFactor);
 
-      cases.push_back({conjunction(coordComparisons), body});
-    }
-    result.push_back(Case::make(cases, lattice.exact()));
+  if(!innerVarDefined) {
+    // outerVar constraints the space to a length parentBounds / divFactor strip starting at
+    // outerVar * parentBounds / divFactor.
+    auto lower = ir::Mul::make(variableExprs[getOuterVar()], dimLen);
+    auto upper = ir::Mul::make(ir::Add::make(variableExprs[getOuterVar()], 1), dimLen);
+    return {lower, upper};
+  } else {
+    taco_iassert(outerVarDefined && innerVarDefined);
+    // outerVar and innerVar constrain space to a length 1 strip starting at
+    // outerVar * parentBounds + innerVar.
+    auto lower = ir::Add::make(ir::Mul::make(variableExprs[getOuterVar()], dimLen), variableExprs[getInnerVar()]);
+    auto upper = ir::Min::make(parentBound[1], ir::Add::make(lower, 1));
+    return {lower, upper};
   }
+}
 
-  return Block::make(result);
+std::vector<ir::Expr> DivideRelNode::deriveIterBounds(taco::IndexVar indexVar,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                                     std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                                     Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getOuterVar() || indexVar == getInnerVar());
+  taco_iassert(parentIterBounds.size() == 1);
+  taco_iassert(parentIterBounds.count(getParentVar()) == 1);
+
+  std::vector<ir::Expr> parentBound = parentIterBounds.at(getParentVar());
+  Datatype divFactorType = parentBound[0].type();
+  auto divFactor = ir::Literal::make(getDivFactor(), divFactorType);
+  if (indexVar == getOuterVar()) {
+    // The loop has been divided into divFactor pieces, so the outer variable
+    // ranges from 0 to divFactor.
+    ir::Expr minBound = 0;
+    ir::Expr maxBound = divFactor;
+    return {minBound, maxBound};
+  }
+  else if (indexVar == getInnerVar()) {
+    // The inner loop ranges over a chunk of size parentBound / divFactor.
+    ir::Expr minBound = ir::Div::make(parentBound[0], divFactor);
+    ir::Expr maxBound = ir::Div::make(ir::Add::make(parentBound[1], ir::Literal::make(getDivFactor()-1, divFactorType)), divFactor);
+    return {minBound, maxBound};
+  }
+  taco_ierror;
+  return {};
+}
+
+ir::Expr DivideRelNode::recoverVariable(taco::IndexVar indexVar,
+                                       std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                       Iterators iterators, std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds, std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getParentVar());
+  taco_iassert(variableNames.count(getParentVar()) && variableNames.count(getOuterVar()) && variableNames.count(getInnerVar()));
+  // Extract divFactor and divFactor - 1.
+  Datatype divFactorType = variableNames[getParentVar()].type();
+  auto divFactor = ir::Literal::make(getDivFactor(), divFactorType);
+  auto divFactorMinusOne = ir::Literal::make(getDivFactor() - 1, divFactorType);
+  // Get the size of the dimension being iterated over.
+  auto parentBounds = parentIterBounds.at(getParentVar());
+  auto dimSize = ir::Sub::make(parentBounds[1], parentBounds[0]);
+  // The bounds for the dimension are adjusted so that dimensions that aren't
+  // divisible by divFactor have the last piece included.
+  auto bounds = ir::Div::make(ir::Add::make(dimSize, divFactorMinusOne), divFactor);
+  return ir::Add::make(ir::Mul::make(variableNames[getOuterVar()], bounds), variableNames[getInnerVar()]);
+}
+
+ir::Stmt DivideRelNode::recoverChild(taco::IndexVar indexVar,
+                                    std::map<taco::IndexVar, taco::ir::Expr> variableNames, bool emitVarDecl, Iterators iterators, ProvenanceGraph provGraph) const {
+  // We need bounds on the parent in order to recover the different
+  // child values, but it doesn't seem like we have access to them here.
+  taco_not_supported_yet;
+  return ir::Stmt();
 }
 
+bool operator==(const DivideRelNode& a, const DivideRelNode& b) {
+  return a.equals(b);
+}
 
-Stmt LowererImpl::lowerForallBody(Expr coordinate, IndexStmt stmt,
-                                  vector<Iterator> locators,
-                                  vector<Iterator> inserters,
-                                  vector<Iterator> appenders,
-                                  const set<Access>& reducedAccesses) {
-  Stmt initVals = resizeAndInitValues(appenders, reducedAccesses);
+struct PosRelNode::Content {
+  Content(IndexVar parentVar, IndexVar posVar, Access access) : parentVar(parentVar), posVar(posVar), access(access) {}
+  IndexVar parentVar;
+  IndexVar posVar;
+  Access access;
+};
 
-  // Inserter positions
-  Stmt declInserterPosVars = declLocatePosVars(inserters);
+PosRelNode::PosRelNode(IndexVar i, IndexVar ipos, const Access& access)
+  : IndexVarRelNode(POS), content(new Content(i, ipos, access)) {
+}
 
-  // Locate positions
-  Stmt declLocatorPosVars = declLocatePosVars(locators);
+const IndexVar& PosRelNode::getParentVar() const {
+  return content->parentVar;
+}
 
-  // Code of loop body statement
-  Stmt body = lower(stmt);
+const IndexVar& PosRelNode::getPosVar() const {
+  return content->posVar;
+}
 
-  // Code to append coordinates
-  Stmt appendCoords = appendCoordinate(appenders, coordinate);
+const Access& PosRelNode::getAccess() const {
+  return content->access;
+}
 
-  // TODO: Emit code to insert coordinates
+void PosRelNode::print(std::ostream &stream) const {
+  stream << "pos(" << getParentVar() << ", " << getPosVar() << ", " << getAccess() << ")";
+}
 
-  return Block::make(initVals,
-                     declInserterPosVars,
-                     declLocatorPosVars,
-                     body,
-                     appendCoords);
+bool PosRelNode::equals(const PosRelNode &rel) const {
+  return getParentVar() == rel.getParentVar() && getPosVar() == rel.getPosVar()
+         && getAccess() == rel.getAccess();
 }
 
+std::vector<IndexVar> PosRelNode::getParents() const {
+  return {getParentVar()};
+}
 
-Stmt LowererImpl::lowerWhere(Where where) {
-  TensorVar temporary = where.getTemporary();
+std::vector<IndexVar> PosRelNode::getChildren() const {
+  return {getPosVar()};
+}
 
-  // Declare and initialize the where statement's temporary
-  Stmt initializeTemporary;
-  if (isScalar(temporary.getType())) {
-    initializeTemporary = defineScalarVariable(temporary, true);
-  }
-  else {
-    if (generateComputeCode()) {
-      Expr values = ir::Var::make(temporary.getName(),
-                                  temporary.getType().getDataType(),
-                                  true, false);
+std::vector<IndexVar> PosRelNode::getIrregulars() const {
+  return {getPosVar()};
+}
 
-      Expr size = ir::Mul::make((uint64_t)3, Sizeof::make(values.type()));
-      Stmt allocate = VarDecl::make(values, Malloc::make(size));
-      this->header.push_back(allocate);
+std::vector<ir::Expr> PosRelNode::computeRelativeBound(std::set<IndexVar> definedVars, std::map<IndexVar, std::vector<ir::Expr>> computedBounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(computedBounds.count(getParentVar()) == 1);
+  std::vector<ir::Expr> parentCoordBound = computedBounds.at(getParentVar());
+  return parentCoordBound;
+}
 
-      Stmt free = Free::make(values);
-      this->footer.push_back(free);
+std::vector<ir::Expr> PosRelNode::deriveIterBounds(taco::IndexVar indexVar,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                                     std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                                     Iterators iterators,
+                                                     ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getPosVar());
+  taco_iassert(parentCoordBounds.count(getParentVar()) == 1);
+  std::vector<ir::Expr> parentCoordBound = parentCoordBounds.at(getParentVar());
 
-      /// Make a struct object that lowerAssignment and lowerAccess can read
-      /// temporary value arrays from.
-      TemporaryArrays arrays;
-      arrays.values = values;
-      this->temporaryArrays.insert({temporary, arrays});
+  if (provGraph.getUnderivedAncestors(indexVar).size() > 1) {
+    // has fused take iterbounds instead
+    // TODO: need to search segments by multiple underived for now just assume complete iteration
+    Iterator accessIterator = getAccessIterator(iterators, provGraph);
+    Iterator rootIterator = accessIterator;
+    while(!rootIterator.isRoot()) {
+      rootIterator = rootIterator.getParent();
     }
+    ir::Expr parentSize = 1; // to find size of segment walk down sizes of iterator chain
+    while (rootIterator != accessIterator) {
+      rootIterator = rootIterator.getChild();
+      if (rootIterator.hasAppend()) {
+        parentSize = rootIterator.getSize(parentSize);
+      } else if (rootIterator.hasInsert()) {
+        parentSize = ir::Mul::make(parentSize, rootIterator.getWidth());
+      }
+    }
+    return {ir::Literal::make(0), parentSize};
   }
 
-  Stmt producer = lower(where.getProducer());
-  Stmt consumer = lower(where.getConsumer());
-  return Block::make(initializeTemporary, producer, consumer);
+  // locate position var for segment based on coordinate getParentVar()
+  ir::Expr posVarExpr = variableNames[getPosVar()];
+  return locateBounds(parentCoordBound, posVarExpr.type(), iterators, provGraph);
 }
 
+std::vector<ir::Expr> PosRelNode::locateBounds(std::vector<ir::Expr> coordBounds,
+                                                   Datatype boundType,
+                                                   Iterators iterators,
+                                                   ProvenanceGraph provGraph) const {
+  Iterator accessIterator = getAccessIterator(iterators, provGraph);
+  ir::Expr parentPos = accessIterator.getParent().getPosVar();
+  ModeFunction segment_bounds = accessIterator.posBounds(parentPos);
+  vector<ir::Expr> binarySearchArgsStart = {
+          getAccessCoordArray(iterators, provGraph),
+          segment_bounds[0], // arrayStart
+          segment_bounds[1], // arrayEnd
+          coordBounds[0]
+  };
 
-Stmt LowererImpl::lowerSequence(Sequence sequence) {
-  Stmt definition = lower(sequence.getDefinition());
-  Stmt mutation = lower(sequence.getMutation());
-  return Block::make(definition, mutation);
-}
-
+  vector<ir::Expr> binarySearchArgsEnd = {
+          getAccessCoordArray(iterators, provGraph),
+          segment_bounds[0], // arrayStart
+          segment_bounds[1], // arrayEnd
+          coordBounds[1]
+  };
 
-Stmt LowererImpl::lowerMulti(Multi multi) {
-  Stmt stmt1 = lower(multi.getStmt1());
-  Stmt stmt2 = lower(multi.getStmt2());
-  return Block::make(stmt1, stmt2);
+  ir::Expr start = ir::Call::make("taco_binarySearchAfter", binarySearchArgsStart, boundType);
+  // simplify start when this is 0
+  ir::Expr simplifiedParentBound = ir::simplify(coordBounds[0]);
+  if (isa<ir::Literal>(simplifiedParentBound) && to<ir::Literal>(simplifiedParentBound)->equalsScalar(0)) {
+    start = segment_bounds[0];
+  }
+  ir::Expr end = ir::Call::make("taco_binarySearchAfter", binarySearchArgsEnd, boundType);
+  // simplify end -> A1_pos[1] when parentBound[1] is max coord dimension
+  simplifiedParentBound = ir::simplify(coordBounds[1]);
+  if (isa<ir::GetProperty>(simplifiedParentBound) && to<ir::GetProperty>(simplifiedParentBound)->property == ir::TensorProperty::Dimension) {
+    end = segment_bounds[1];
+  }
+  return {start, end};
 }
 
+Iterator PosRelNode::getAccessIterator(Iterators iterators, ProvenanceGraph provGraph) const {
 
-Expr LowererImpl::lowerAccess(Access access) {
-  TensorVar var = access.getTensorVar();
-
-  if (isScalar(var.getType())) {
-    return getTensorVar(var);
+  // when multiple underived ancestors, match iterator with max mode (iterate bottom level)
+  vector<IndexVar> underivedParentAncestors = provGraph.getUnderivedAncestors(getParentVar());
+  int max_mode = 0;
+  for (IndexVar underivedParent : underivedParentAncestors) {
+    size_t mode_index = 0; // which of the access index vars match?
+    for (auto var : getAccess().getIndexVars()) {
+      if (var == underivedParent) {
+        break;
+      }
+      mode_index++;
+    }
+    taco_iassert(mode_index < getAccess().getIndexVars().size());
+    int mode = getAccess().getTensorVar().getFormat().getModeOrdering()[mode_index];
+    if (mode > max_mode) {
+      max_mode = mode;
+    }
   }
 
-  return getIterators(access).back().isUnique()
-         ? Load::make(getValuesArray(var), generateValueLocExpr(access))
-         : getReducedValueVar(access);
+  // can't use default level iterator access function because mapping contents rather than pointer which is default to allow repeated operands
+  std::map<ModeAccess, Iterator> levelIterators = iterators.levelIterators();
+  ModeAccess modeAccess = ModeAccess(getAccess(), max_mode+1);
+  for (auto levelIterator : levelIterators) {
+    if (::taco::equals(levelIterator.first.getAccess(), modeAccess.getAccess()) && levelIterator.first.getModePos() == modeAccess.getModePos()) {
+      return levelIterator.second;
+    }
+  }
+  taco_ierror;
+  return Iterator();
 }
 
-
-Expr LowererImpl::lowerLiteral(Literal literal) {
-  switch (literal.getDataType().getKind()) {
-    case Datatype::Bool:
-      return ir::Literal::make(literal.getVal<bool>());
-    case Datatype::UInt8:
-      return ir::Literal::make((unsigned long long)literal.getVal<uint8_t>());
-    case Datatype::UInt16:
-      return ir::Literal::make((unsigned long long)literal.getVal<uint16_t>());
-    case Datatype::UInt32:
-      return ir::Literal::make((unsigned long long)literal.getVal<uint32_t>());
-    case Datatype::UInt64:
-      return ir::Literal::make((unsigned long long)literal.getVal<uint64_t>());
-    case Datatype::UInt128:
-      taco_not_supported_yet;
-      break;
-    case Datatype::Int8:
-      return ir::Literal::make((int)literal.getVal<int8_t>());
-    case Datatype::Int16:
-      return ir::Literal::make((int)literal.getVal<int16_t>());
-    case Datatype::Int32:
-      return ir::Literal::make((int)literal.getVal<int32_t>());
-    case Datatype::Int64:
-      return ir::Literal::make((long long)literal.getVal<int64_t>());
-    case Datatype::Int128:
-      taco_not_supported_yet;
-      break;
-    case Datatype::Float32:
-      return ir::Literal::make(literal.getVal<float>());
-    case Datatype::Float64:
-      return ir::Literal::make(literal.getVal<double>());
-    case Datatype::Complex64:
-      return ir::Literal::make(literal.getVal<std::complex<float>>());
-    case Datatype::Complex128:
-      return ir::Literal::make(literal.getVal<std::complex<double>>());
-    case Datatype::Undefined:
-      taco_unreachable;
-      break;
-  }
-  return ir::Expr();
+ir::Expr PosRelNode::getAccessCoordArray(Iterators iterators, ProvenanceGraph provGraph) const {
+  return getAccessIterator(iterators, provGraph).getMode().getModePack().getArray(1);
 }
 
 
-Expr LowererImpl::lowerNeg(Neg neg) {
-  return ir::Neg::make(lower(neg.getA()));
-}
+ir::Expr PosRelNode::recoverVariable(taco::IndexVar indexVar,
+                                       std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                       Iterators iterators,
+                                       std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                       std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                       ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getParentVar());
+  taco_iassert(variableNames.count(getParentVar()) == 1 && variableNames.count(getPosVar()) == 1);
+  taco_iassert(parentCoordBounds.count(getParentVar()) == 1);
 
+  ir::Expr coord_array = getAccessCoordArray(iterators, provGraph);
 
-Expr LowererImpl::lowerAdd(Add add) {
-  Expr a = lower(add.getA());
-  Expr b = lower(add.getB());
-  return (add.getDataType().getKind() == Datatype::Bool)
-         ? ir::Or::make(a, b) : ir::Add::make(a, b);
-}
+  Iterator accessIterator = getAccessIterator(iterators, provGraph);
+  ir::Expr parentPos = accessIterator.getParent().getPosVar();
+  ModeFunction segment_bounds = accessIterator.posBounds(parentPos);
+
+  // positions should be with respect to entire array not just segment so don't need to offset variable when projecting.
+  ir::Expr project_result = ir::Load::make(coord_array, variableNames.at(getPosVar()));
 
+  // but need to subtract parentvars start corodbound
+  ir::Expr parent_value = ir::Sub::make(project_result, parentCoordBounds[getParentVar()][0]);
 
-Expr LowererImpl::lowerSub(Sub sub) {
-  return ir::Sub::make(lower(sub.getA()), lower(sub.getB()));
+  return parent_value;
 }
 
+ir::Stmt PosRelNode::recoverChild(taco::IndexVar indexVar,
+                                    std::map<taco::IndexVar, taco::ir::Expr> variableNames, bool emitVarDecl, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getPosVar());
+  taco_iassert(variableNames.count(getParentVar()) && variableNames.count(getPosVar()));
+  // locate position var for segment based on coordinate getParentVar()
+  ir::Expr posVarExpr = variableNames[getPosVar()];
 
-Expr LowererImpl::lowerMul(Mul mul) {
-  Expr a = lower(mul.getA());
-  Expr b = lower(mul.getB());
-  return (mul.getDataType().getKind() == Datatype::Bool)
-         ? ir::And::make(a, b) : ir::Mul::make(a, b);
+  Iterator accessIterator = getAccessIterator(iterators, provGraph);
+  ir::Expr parentPos = accessIterator.getParent().getPosVar();
+  ModeFunction segment_bounds = accessIterator.posBounds(parentPos);
+  vector<ir::Expr> binarySearchArgs = {
+          getAccessCoordArray(iterators, provGraph),
+          segment_bounds[0], // arrayStart
+          segment_bounds[1], // arrayEnd
+          variableNames[getParentVar()]
+  };
+  return ir::VarDecl::make(posVarExpr, ir::Call::make("taco_binarySearchAfter", binarySearchArgs, posVarExpr.type()));
 }
 
-
-Expr LowererImpl::lowerDiv(Div div) {
-  return ir::Div::make(lower(div.getA()), lower(div.getB()));
+bool operator==(const PosRelNode& a, const PosRelNode& b) {
+  return a.equals(b);
 }
 
+struct FuseRelNode::Content {
+  IndexVar outerParentVar;
+  IndexVar innerParentVar;
+  IndexVar fusedVar;
+};
 
-Expr LowererImpl::lowerSqrt(Sqrt sqrt) {
-  return ir::Sqrt::make(lower(sqrt.getA()));
+FuseRelNode::FuseRelNode(IndexVar outerParentVar, IndexVar innerParentVar, IndexVar fusedVar)
+  : IndexVarRelNode(FUSE), content(new Content) {
+  content->outerParentVar = outerParentVar;
+  content->innerParentVar = innerParentVar;
+  content->fusedVar = fusedVar;
 }
 
+const IndexVar& FuseRelNode::getOuterParentVar() const {
+  return content->outerParentVar;
+}
+const IndexVar& FuseRelNode::getInnerParentVar() const {
+  return content->innerParentVar;
+}
+const IndexVar& FuseRelNode::getFusedVar() const {
+  return content->fusedVar;
+}
 
-Expr LowererImpl::lowerCast(Cast cast) {
-  return ir::Cast::make(lower(cast.getA()), cast.getDataType());
+void FuseRelNode::print(std::ostream &stream) const {
+  stream << "fuse(" << getOuterParentVar() << ", " << getInnerParentVar() << ", " << getFusedVar() << ")";
 }
 
+bool FuseRelNode::equals(const FuseRelNode &rel) const {
+  return getOuterParentVar() == rel.getOuterParentVar() && getInnerParentVar() == rel.getInnerParentVar()
+         && getFusedVar() == rel.getFusedVar();
+}
 
-Expr LowererImpl::lowerCallIntrinsic(CallIntrinsic call) {
-  std::vector<Expr> args;
-  for (auto& arg : call.getArgs()) {
-    args.push_back(lower(arg));
-  }
-  return call.getFunc().lower(args);
+std::vector<IndexVar> FuseRelNode::getParents() const {
+  return {getOuterParentVar(), getInnerParentVar()};
 }
 
+std::vector<IndexVar> FuseRelNode::getChildren() const {
+  return {getFusedVar()};
+}
 
-Stmt LowererImpl::lower(IndexStmt stmt) {
-  return visitor->lower(stmt);
+std::vector<IndexVar> FuseRelNode::getIrregulars() const {
+  return {getFusedVar()};
 }
 
+std::vector<ir::Expr> FuseRelNode::computeRelativeBound(std::set<IndexVar> definedVars, std::map<IndexVar, std::vector<ir::Expr>> computedBounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(computedBounds.count(getOuterParentVar()) && computedBounds.count(getInnerParentVar()));
+  return combineParentBounds(computedBounds[getOuterParentVar()], computedBounds[getInnerParentVar()]);
+}
 
-Expr LowererImpl::lower(IndexExpr expr) {
-  return visitor->lower(expr);
+std::vector<ir::Expr> FuseRelNode::deriveIterBounds(taco::IndexVar indexVar,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                                     std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                                     Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getFusedVar());
+  taco_iassert(parentIterBounds.count(getOuterParentVar()) && parentIterBounds.count(getInnerParentVar()));
+  return combineParentBounds(parentIterBounds[getOuterParentVar()], parentIterBounds[getInnerParentVar()]);
 }
 
+ir::Expr FuseRelNode::recoverVariable(taco::IndexVar indexVar,
+                                       std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                       Iterators iterators, std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds, std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds, ProvenanceGraph provGraph) const {
+  taco_iassert(variableNames.count(indexVar));
+  taco_iassert(parentIterBounds.count(getInnerParentVar()));
+  ir::Expr innerSize = ir::Sub::make(parentIterBounds[getInnerParentVar()][1], parentIterBounds[getInnerParentVar()][0]);
 
-bool LowererImpl::generateAssembleCode() const {
-  return this->assemble;
+  if (indexVar == getOuterParentVar()) {
+    // getOuterVar() = getFusedVar() / innerSize
+    return ir::Div::make(variableNames[getFusedVar()], innerSize);
+  }
+  else if (indexVar == getInnerParentVar()) {
+    if (provGraph.hasPosDescendant(getFusedVar()) && provGraph.isCoordVariable(getInnerParentVar())) {
+      // getFusedVar() < innerSize (due to pos)
+      return variableNames[getFusedVar()];
+    }
+    // getInnerVar() = getFusedVar() % innerSize
+    return ir::Rem::make(variableNames[getFusedVar()], innerSize);
+  }
+  else {
+    taco_unreachable;
+    return ir::Expr();
+  }
 }
 
+ir::Stmt FuseRelNode::recoverChild(taco::IndexVar indexVar,
+                                    std::map<taco::IndexVar, taco::ir::Expr> variableNames, bool emitVarDecl, Iterators iterators, ProvenanceGraph provGraph) const {
+//  taco_iassert(indexVar == fusedVar);
+//  taco_iassert(variableNames.count(indexVar) && variableNames.count(outerParentVar) && variableNames.count(innerParentVar));
+//  taco_iassert(parentCoordBounds.count(innerParentVar));
+//  ir::Expr innerSize = ir::Sub::make(parentCoordBounds[innerParentVar][1], parentCoordBounds[innerParentVar][0]);
+//  return ir::Add::make(ir::Mul::make(variableNames[outerParentVar], innerSize), variableNames[innerParentVar]);
+  taco_not_supported_yet; // TODO: need to add parentIterBounds to recoverChild parameters
+  return ir::Stmt();
+}
+
+// Combine two bounds
+// if (i, j) where i in [a, b) and j in [c, d)
+// then combined bound is [a * (d - c) + c, b * (d - c) + c)
+// this results in (b - a) * (d - c) iterations while still being
+// properly offset in cases where a != 0 or c != 0
+std::vector<ir::Expr> FuseRelNode::combineParentBounds(std::vector<ir::Expr> outerParentBound, std::vector<ir::Expr> innerParentBound) const {
+  ir::Expr innerSize = ir::Sub::make(innerParentBound[1], innerParentBound[0]);
+  ir::Expr minBound = ir::Add::make(ir::Mul::make(outerParentBound[0], innerSize), innerParentBound[0]);
+  ir::Expr maxBound = ir::Add::make(ir::Mul::make(outerParentBound[1], innerSize), innerParentBound[0]);
+  return {minBound, maxBound};
+}
+
+bool operator==(const FuseRelNode& a, const FuseRelNode& b) {
+  return a.equals(b);
+}
+
+// BoundRelNode
+struct BoundRelNode::Content {
+  IndexVar parentVar;
+  IndexVar boundVar;
+  size_t bound;
+  BoundType boundType;
+};
 
-bool LowererImpl::generateComputeCode() const {
-  return this->compute;
+BoundRelNode::BoundRelNode(taco::IndexVar parentVar, taco::IndexVar boundVar, size_t bound,
+                           taco::BoundType boundType) : IndexVarRelNode(BOUND), content(new Content) {
+  content->parentVar = parentVar;
+  content->boundVar = boundVar;
+  content->bound = bound;
+  content->boundType = boundType;
 }
 
-
-Expr LowererImpl::getTensorVar(TensorVar tensorVar) const {
-  taco_iassert(util::contains(this->tensorVars, tensorVar)) << tensorVar;
-  return this->tensorVars.at(tensorVar);
+const IndexVar& BoundRelNode::getParentVar() const {
+  return content->parentVar;
+}
+const IndexVar& BoundRelNode::getBoundVar() const {
+  return content->boundVar;
+}
+const size_t& BoundRelNode::getBound() const {
+  return content->bound;
+}
+const BoundType& BoundRelNode::getBoundType() const {
+  return content->boundType;
 }
 
+void BoundRelNode::print(std::ostream &stream) const {
+  stream << "bound(" << getParentVar() << ", " << getBoundVar() << ", " << getBound() << ", " << BoundType_NAMES[(int) getBoundType()] << ")";
+}
 
-Expr LowererImpl::getCapacityVar(Expr tensor) const {
-  taco_iassert(util::contains(this->capacityVars, tensor)) << tensor;
-  return this->capacityVars.at(tensor);
+bool BoundRelNode::equals(const BoundRelNode &rel) const {
+  return getParentVar() == rel.getParentVar() &&
+    getBoundVar() == rel.getBoundVar() && getBound() == rel.getBound() &&
+    getBoundType() == rel.getBoundType();
 }
 
+std::vector<IndexVar> BoundRelNode::getParents() const {
+  return {getParentVar()};
+}
 
-ir::Expr LowererImpl::getValuesArray(TensorVar var) const
-{
-  return (util::contains(temporaryArrays, var))
-         ? temporaryArrays.at(var).values
-         : GetProperty::make(getTensorVar(var), TensorProperty::Values);
+std::vector<IndexVar> BoundRelNode::getChildren() const {
+  return {getBoundVar()};
 }
 
+std::vector<IndexVar> BoundRelNode::getIrregulars() const {
+  return {getBoundVar()};
+}
 
-Expr LowererImpl::getDimension(IndexVar indexVar) const {
-  taco_iassert(util::contains(this->dimensions, indexVar)) << indexVar;
-  return this->dimensions.at(indexVar);
+std::vector<ir::Expr> BoundRelNode::computeRelativeBound(std::set<IndexVar> definedVars, std::map<IndexVar, std::vector<ir::Expr>> computedBounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators, ProvenanceGraph provGraph) const {
+  // coordinate bounds stay unchanged, only iteration bounds change
+  taco_iassert(computedBounds.count(getParentVar()) == 1);
+  std::vector<ir::Expr> parentCoordBound = computedBounds.at(getParentVar());
+  return parentCoordBound;
 }
 
+std::vector<ir::Expr> BoundRelNode::deriveIterBounds(taco::IndexVar indexVar,
+                                                   std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                                   std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                                   std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                                   Iterators iterators,
+                                                   ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getBoundVar());
+  taco_iassert(parentCoordBounds.count(getParentVar()) == 1);
+  std::vector<ir::Expr> parentCoordBound = parentCoordBounds.at(getParentVar());
 
-std::vector<Iterator> LowererImpl::getIterators(Access access) const {
-  vector<Iterator> result;
-  TensorVar tensor = access.getTensorVar();
-  for (int i = 0; i < tensor.getOrder(); i++) {
-    int mode = tensor.getFormat().getModeOrdering()[i];
-    result.push_back(iterators.levelIterator(ModeAccess(access, mode+1)));
+  if (getBoundType() == BoundType::MaxExact) {
+    return {parentCoordBound[0], ir::Literal::make(getBound(), parentCoordBound[1].type())};
+  }
+  else {
+    taco_not_supported_yet;
   }
-  return result;
+  return {};
 }
 
-
-set<Access> LowererImpl::getExhaustedAccesses(MergePoint point,
-                                              MergeLattice lattice) const
-{
-  set<Access> exhaustedAccesses;
-  for (auto& iterator : lattice.exhausted(point)) {
-    exhaustedAccesses.insert(iterators.modeAccess(iterator).getAccess());
-  }
-  return exhaustedAccesses;
+ir::Expr BoundRelNode::recoverVariable(taco::IndexVar indexVar,
+                                     std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                     Iterators iterators,
+                                     std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                     std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                     ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getParentVar());
+  taco_iassert(variableNames.count(getBoundVar()) == 1);
+  return variableNames[getBoundVar()];
 }
 
+ir::Stmt BoundRelNode::recoverChild(taco::IndexVar indexVar,
+                                  std::map<taco::IndexVar, taco::ir::Expr> variableNames, bool emitVarDecl, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getBoundVar());
+  taco_iassert(variableNames.count(getParentVar()) && variableNames.count(getBoundVar()));
+  ir::Expr boundVarExpr = variableNames[getBoundVar()];
+  return ir::VarDecl::make(boundVarExpr, variableNames[getParentVar()]);
+}
 
-Expr LowererImpl::getReducedValueVar(Access access) const {
-  return this->reducedValueVars.at(access);
+bool operator==(const BoundRelNode& a, const BoundRelNode& b) {
+  return a.equals(b);
 }
 
+// PrecomputeRelNode
+struct PrecomputeRelNode::Content {
+  IndexVar parentVar;
+  IndexVar precomputeVar;
+};
 
-Expr LowererImpl::getCoordinateVar(IndexVar indexVar) const {
-  return this->iterators.modeIterator(indexVar).getCoordVar();
+PrecomputeRelNode::PrecomputeRelNode(taco::IndexVar parentVar, taco::IndexVar precomputeVar)
+  : IndexVarRelNode(PRECOMPUTE), content (new Content) {
+  content->parentVar = parentVar;
+  content->precomputeVar = precomputeVar;
 }
 
+const IndexVar& PrecomputeRelNode::getParentVar() const {
+  return content->parentVar;
+}
 
-Expr LowererImpl::getCoordinateVar(Iterator iterator) const {
-  if (iterator.isDimensionIterator()) {
-    return iterator.getCoordVar();
-  }
-  return this->getCoordinateVar(iterator.getIndexVar());
+const IndexVar& PrecomputeRelNode::getPrecomputeVar() const {
+  return content->precomputeVar;
 }
 
 
-vector<Expr> LowererImpl::coordinates(Iterator iterator) const {
-  taco_iassert(iterator.defined());
+void PrecomputeRelNode::print(std::ostream &stream) const {
+  stream << "precompute(" << getParentVar() << ", " << getPrecomputeVar() << ")";
+}
 
-  vector<Expr> coords;
-  do {
-    coords.push_back(getCoordinateVar(iterator));
-    iterator = iterator.getParent();
-  } while (!iterator.isRoot());
-  auto reverse = util::reverse(coords);
-  return vector<Expr>(reverse.begin(), reverse.end());
+bool PrecomputeRelNode::equals(const PrecomputeRelNode &rel) const {
+  return getParentVar() == rel.getParentVar() && getPrecomputeVar() == rel.getPrecomputeVar();
 }
 
+std::vector<IndexVar> PrecomputeRelNode::getParents() const {
+  return {getParentVar()};
+}
 
-vector<Expr> LowererImpl::coordinates(vector<Iterator> iterators)
-{
-  taco_iassert(all(iterators, [](Iterator iter){ return iter.defined(); }));
-  vector<Expr> result;
-  for (auto& iterator : iterators) {
-    result.push_back(iterator.getCoordVar());
-  }
-  return result;
+std::vector<IndexVar> PrecomputeRelNode::getChildren() const {
+  return {getPrecomputeVar()};
 }
 
+std::vector<IndexVar> PrecomputeRelNode::getIrregulars() const {
+  return {getPrecomputeVar()};
+}
 
-/// Returns true iff a result mode is assembled by inserting a sparse set of 
-/// result coordinates (e.g., compressed to dense).
-static 
-bool hasSparseInserts(const std::vector<Iterator>& resultIterators,
-                      const std::multimap<IndexVar, Iterator>& inputIterators) {
-  for (const auto& resultIterator : resultIterators) {
-    if (resultIterator.hasInsert()) {
-      const auto indexVar = resultIterator.getIndexVar();
-      const auto accessedInputs = inputIterators.equal_range(indexVar);
-      for (auto inputIterator = accessedInputs.first; 
-           inputIterator != accessedInputs.second; ++inputIterator) {
-        if (!inputIterator->second.isFull()) {
-          return true;
-        }
-      }
-    }
-  }
-  return false;
+std::vector<ir::Expr> PrecomputeRelNode::computeRelativeBound(std::set<IndexVar> definedVars, std::map<IndexVar, std::vector<ir::Expr>> computedBounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(computedBounds.count(getParentVar()) == 1);
+  std::vector<ir::Expr> parentCoordBound = computedBounds.at(getParentVar());
+  return parentCoordBound;
 }
 
+std::vector<ir::Expr> PrecomputeRelNode::deriveIterBounds(taco::IndexVar indexVar,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                                     std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                                     std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                                     Iterators iterators,
+                                                     ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getPrecomputeVar());
+  taco_iassert(parentIterBounds.count(getParentVar()) == 1);
+  std::vector<ir::Expr> parentIterBound = parentIterBounds.at(getParentVar());
+  return parentIterBound;
+}
 
-Stmt LowererImpl::initResultArrays(vector<Access> writes, 
-                                   vector<Access> reads,
-                                   set<Access> reducedAccesses) {
-  multimap<IndexVar, Iterator> readIterators;
-  for (auto& read : reads) {
-    for (auto& readIterator : getIterators(read)) {
-      readIterators.insert({readIterator.getIndexVar(), readIterator});
-    }
-  }
+ir::Expr PrecomputeRelNode::recoverVariable(taco::IndexVar indexVar,
+                                       std::map<taco::IndexVar, taco::ir::Expr> variableNames,
+                                       Iterators iterators,
+                                       std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds,
+                                       std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds,
+                                       ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getParentVar());
+  taco_iassert(variableNames.count(getPrecomputeVar()) == 1);
+  return variableNames[getPrecomputeVar()];
+}
 
-  std::vector<Stmt> result;
-  for (auto& write : writes) {
-    if (write.getTensorVar().getOrder() == 0) continue;
-
-    std::vector<Stmt> initArrays;
-
-    const auto iterators = getIterators(write);
-    taco_iassert(!iterators.empty());
-
-    Expr tensor = getTensorVar(write.getTensorVar());
-    Expr valuesArr = GetProperty::make(tensor, TensorProperty::Values);
-
-    Expr parentSize = 1;
-    if (generateAssembleCode()) {
-      for (const auto& iterator : iterators) {
-        Expr size;
-        Stmt init;
-        // Initialize data structures for storing levels
-        if (iterator.hasAppend()) {
-          size = 0;
-          init = iterator.getAppendInitLevel(parentSize, size);
-        } else if (iterator.hasInsert()) {
-          size = simplify(ir::Mul::make(parentSize, iterator.getWidth()));
-          init = iterator.getInsertInitLevel(parentSize, size);
-        } else {
-          taco_ierror << "Write iterator supports neither append nor insert";
-        }
-        initArrays.push_back(init);
+ir::Stmt PrecomputeRelNode::recoverChild(taco::IndexVar indexVar,
+                                    std::map<taco::IndexVar, taco::ir::Expr> variableNames, bool emitVarDecl, Iterators iterators, ProvenanceGraph provGraph) const {
+  taco_iassert(indexVar == getPrecomputeVar());
+  taco_iassert(variableNames.count(getParentVar()) && variableNames.count(getPrecomputeVar()));
+  ir::Expr boundVarExpr = variableNames[getPrecomputeVar()];
+  return ir::VarDecl::make(boundVarExpr, variableNames[getParentVar()]);
+}
 
-        // Declare position variable of append modes that are not above a 
-        // branchless mode (if mode below is branchless, then can share same 
-        // position variable)
-        if (iterator.hasAppend() && (iterator.isLeaf() || 
-            !iterator.getChild().isBranchless())) {
-          initArrays.push_back(VarDecl::make(iterator.getPosVar(), 0));
-        }
+bool operator==(const PrecomputeRelNode& a, const PrecomputeRelNode& b) {
+  return a.equals(b);
+}
 
-        parentSize = size;
-      }
+// class ProvenanceGraph
+ProvenanceGraph::ProvenanceGraph(IndexStmt concreteStmt) {
+  // Add all nodes (not all nodes may be scheduled)
+  match(concreteStmt,
+        std::function<void(const ForallNode*)>([&](const ForallNode* op) {
+          nodes.insert(op->indexVar);
+        })
+  );
 
-      // Pre-allocate memory for the value array if computing while assembling
-      if (generateComputeCode()) {
-        taco_iassert(!iterators.empty());
-        
-        Expr capacityVar = getCapacityVar(tensor);
-        Expr allocSize = isValue(parentSize, 0) 
-                         ? DEFAULT_ALLOC_SIZE : parentSize;
-        initArrays.push_back(VarDecl::make(capacityVar, allocSize));
-        initArrays.push_back(Allocate::make(valuesArr, capacityVar));
-      }
+  // Get SuchThat node with relations
+  if (!isa<SuchThat>(concreteStmt)) {
+    // No relations defined
+    return;
+  }
 
-      taco_iassert(!initArrays.empty());
-      result.push_back(Block::make(initArrays));
+  SuchThat suchThat = to<SuchThat>(concreteStmt);
+  vector<IndexVarRel> relations = suchThat.getPredicate();
+
+  for (IndexVarRel rel : relations) {
+    std::vector<IndexVar> parents = rel.getNode()->getParents();
+    std::vector<IndexVar> children = rel.getNode()->getChildren();
+    for (IndexVar parent : parents) {
+      nodes.insert(parent);
+      childRelMap[parent] = rel;
+      childrenMap[parent] = children;
     }
-    else if (generateComputeCode()) {
-      Iterator lastAppendIterator;
-      // Compute size of values array
-      for (auto& iterator : iterators) {
-        if (iterator.hasAppend()) {
-          lastAppendIterator = iterator;
-          parentSize = iterator.getSize(parentSize);
-        } else if (iterator.hasInsert()) {
-          parentSize = ir::Mul::make(parentSize, iterator.getWidth());
-        } else {
-          taco_ierror << "Write iterator supports neither append nor insert";
-        }
-        parentSize = simplify(parentSize);
-      }
 
-      // Declare position variable for the last append level
-      if (lastAppendIterator.defined()) {
-        result.push_back(VarDecl::make(lastAppendIterator.getPosVar(), 0));
-      }
+    for (IndexVar child : children) {
+      nodes.insert(child);
+      parentRelMap[child] = rel;
+      parentsMap[child] = parents;
     }
+  }
+}
 
-    if (generateComputeCode() && iterators.back().hasInsert() && 
-        !isValue(parentSize, 0) && 
-        (hasSparseInserts(iterators, readIterators) || 
-         util::contains(reducedAccesses, write))) {
-      // Zero-initialize values array if size statically known and might not 
-      // assign to every element in values array during compute
-      Expr size = generateAssembleCode() ? getCapacityVar(tensor) : parentSize;
-      result.push_back(zeroInitValues(tensor, 0, size));
-    }
-  }
-  return result.empty() ? Stmt() : Block::blanks(result);
+std::vector<IndexVar> ProvenanceGraph::getChildren(IndexVar indexVar) const {
+  if (childrenMap.count(indexVar)) {
+    return childrenMap.at(indexVar);
+  }
+  return {};
 }
 
+std::vector<IndexVar> ProvenanceGraph::getParents(IndexVar indexVar) const {
+  if (parentsMap.count(indexVar)) {
+    return parentsMap.at(indexVar);
+  }
+  return {};
+}
 
-ir::Stmt LowererImpl::finalizeResultArrays(std::vector<Access> writes) {
-  if (!generateAssembleCode()) {
-    return Stmt();
-  }
-
-  std::vector<Stmt> result;
-  for (auto& write : writes) {
-    if (write.getTensorVar().getOrder() == 0) continue;
-
-    const auto iterators = getIterators(write);
-    taco_iassert(!iterators.empty());
-      
-    Expr parentSize = 1;
-    for (const auto& iterator : iterators) {
-      Expr size;
-      Stmt finalize;
-      // Post-process data structures for storing levels
-      if (iterator.hasAppend()) {
-        size = iterator.getPosVar();
-        finalize = iterator.getAppendFinalizeLevel(parentSize, size);
-      } else if (iterator.hasInsert()) {
-        size = simplify(ir::Mul::make(parentSize, iterator.getWidth()));
-        finalize = iterator.getInsertFinalizeLevel(parentSize, size);
-      } else {
-        taco_ierror << "Write iterator supports neither append nor insert";
-      }
-      result.push_back(finalize);
-      parentSize = size;
-    }
+std::vector<IndexVar> ProvenanceGraph::getFullyDerivedDescendants(IndexVar indexVar) const {
+  // DFS to find all fully derived children
+  std::vector<IndexVar> children = getChildren(indexVar);
+  if (children.empty()) {
+    return {indexVar};
+  }
 
-    if (!generateComputeCode()) {
-      // Allocate memory for values array after assembly if not also computing
-      Expr tensor = getTensorVar(write.getTensorVar());
-      Expr valuesArr = GetProperty::make(tensor, TensorProperty::Values);
-      result.push_back(Allocate::make(valuesArr, parentSize));
-    }
+  std::vector<IndexVar> fullyDerivedChildren;
+  for (IndexVar child : children) {
+    std::vector<IndexVar> childFullyDerived = getFullyDerivedDescendants(child);
+    fullyDerivedChildren.insert(fullyDerivedChildren.end(), childFullyDerived.begin(), childFullyDerived.end());
   }
-  return result.empty() ? Stmt() : Block::blanks(result);
+  return fullyDerivedChildren;
 }
 
-Stmt LowererImpl::defineScalarVariable(TensorVar var, bool zero) {
-  Datatype type = var.getType().getDataType();
-  Expr varValueIR = Var::make(var.getName() + "_val", type, false, false);
-  Expr init = (zero) ? ir::Literal::zero(type)
-                     : Load::make(GetProperty::make(tensorVars.at(var),
-                                                    TensorProperty::Values));
-  tensorVars.find(var)->second = varValueIR;
-  return VarDecl::make(varValueIR, init);
+std::vector<IndexVar> ProvenanceGraph::getUnderivedAncestors(IndexVar indexVar) const {
+  // DFS to find all underived parents
+  std::vector<IndexVar> parents = getParents(indexVar);
+  if (parents.empty()) {
+    return {indexVar};
+  }
+
+  std::vector<IndexVar> underivedParents;
+  for (IndexVar parent : parents) {
+    std::vector<IndexVar> parentUnderived = getUnderivedAncestors(parent);
+    underivedParents.insert(underivedParents.end(), parentUnderived.begin(), parentUnderived.end());
+  }
+  return underivedParents;
 }
 
-static
-vector<Iterator> getIteratorsFrom(IndexVar var, 
-                                  const vector<Iterator>& iterators) {
-  vector<Iterator> result;
-  bool found = false;
-  for (Iterator iterator : iterators) {
-    if (var == iterator.getIndexVar()) found = true;
-    if (found) {
-      result.push_back(iterator);
+bool ProvenanceGraph::getIrregularDescendant(IndexVar indexVar, IndexVar *irregularChild) const {
+  if (isFullyDerived(indexVar) && isIrregular(indexVar)) {
+    *irregularChild = indexVar;
+    return true;
+  }
+  for (IndexVar child : getChildren(indexVar)) {
+    if (getIrregularDescendant(child, irregularChild)) {
+      return true;
     }
   }
-  return result;
+  return false;
 }
 
+// A pos Iterator Descendant is first innermost variable that is pos
+bool ProvenanceGraph::getPosIteratorAncestor(IndexVar indexVar, IndexVar *irregularChild) const {
+  if (!isPosVariable(indexVar)) {
+    return false;
+  }
 
-Stmt LowererImpl::initResultArrays(IndexVar var, vector<Access> writes, 
-                                   vector<Access> reads,
-                                   set<Access> reducedAccesses) {
-  if (!generateAssembleCode()) {
-    return Stmt();
+  if (isUnderived(indexVar)) {
+    return false;
   }
 
-  multimap<IndexVar, Iterator> readIterators;
-  for (auto& read : reads) {
-    for (auto& readIterator : getIteratorsFrom(var, getIterators(read))) {
-      readIterators.insert({readIterator.getIndexVar(), readIterator});
+  for (IndexVar parent : getParents(indexVar)) {
+    if (isCoordVariable(parent)) {
+      *irregularChild = indexVar;
+      return true;
+    }
+    if (getPosIteratorAncestor(parent, irregularChild)) {
+      return true;
     }
   }
+  return false;
+}
 
-  vector<Stmt> result;
-  for (auto& write : writes) {
-    Expr tensor = getTensorVar(write.getTensorVar());
-    Expr values = GetProperty::make(tensor, TensorProperty::Values);
-
-    vector<Iterator> iterators = getIteratorsFrom(var, getIterators(write));
+// A pos Iterator Descendant is first innermost variable that is pos
+bool ProvenanceGraph::getPosIteratorDescendant(IndexVar indexVar, IndexVar *irregularChild) const {
+  if (isPosVariable(indexVar)) {
+    *irregularChild = indexVar;
+    return true;
+  }
 
-    if (iterators.empty()) {
-      continue;
-    }
+  if (isFullyDerived(indexVar)) {
+    return false;
+  }
 
-    Iterator resultIterator = iterators.front();
+  if (childRelMap.at(indexVar).getRelType() == FUSE && isPosVariable(getChildren(indexVar)[0])) { // can't gain pos by fusing with pos variable
+    return false;
+  }
 
-    // Initialize begin var
-    if (resultIterator.hasAppend() && !resultIterator.isBranchless()) {
-      Expr begin = resultIterator.getBeginVar();
-      result.push_back(VarDecl::make(begin, resultIterator.getPosVar()));
+  if (getChildren(indexVar).size() == 1) {
+    return getPosIteratorDescendant(getChildren(indexVar)[0], irregularChild);
+  }
+  for (IndexVar child : getChildren(indexVar)) {
+    if (!util::contains(childRelMap.at(indexVar).getNode()->getIrregulars(), child)) { // is irregularity not maintained through relationship
+      return getPosIteratorDescendant(child, irregularChild);
     }
+  }
+  return false;
+}
 
-    const bool isTopLevel = (iterators.size() == write.getIndexVars().size());
-    if (resultIterator.getParent().hasAppend() || isTopLevel) {
-      Expr resultParentPos = resultIterator.getParent().getPosVar();
-      Expr resultParentPosNext = simplify(ir::Add::make(resultParentPos, 1));
-      Expr initBegin = resultParentPos;
-      Expr initEnd = resultParentPosNext;
-      Expr stride = 1;
-
-      Iterator initIterator;
-      for (Iterator iterator : iterators) {
-        if (!iterator.hasInsert()) {
-          initIterator = iterator;
-          break;
-        }
-
-        stride = simplify(ir::Mul::make(stride, iterator.getWidth()));
-        initBegin = simplify(ir::Mul::make(resultParentPos, stride));
-        initEnd = simplify(ir::Mul::make(resultParentPosNext, stride));
+bool ProvenanceGraph::getPosIteratorFullyDerivedDescendant(IndexVar indexVar, IndexVar *irregularChild) const {
+  if (isFullyDerived(indexVar) || childRelMap.at(indexVar).getRelType() == PRECOMPUTE) {
+    if (isPosVariable(indexVar)) {
+      *irregularChild = indexVar;
+      return true;
+    }
+    return false;
+  }
 
-        // Initialize data structures for storing insert mode
-        result.push_back(iterator.getInsertInitCoords(initBegin, initEnd));
-      }
+  if (childRelMap.at(indexVar).getRelType() == FUSE && isPosVariable(indexVar)) { // can't iterate pos through fuse
+    return false;
+  }
 
-      if (initIterator.defined()) {
-        // Initialize data structures for storing edges of next append mode
-        taco_iassert(initIterator.hasAppend());
-        result.push_back(initIterator.getAppendInitEdges(initBegin, initEnd));
-      } else if (generateComputeCode() && !isTopLevel) {
-        if (isa<ir::Mul>(stride)) {
-          Expr strideVar = Var::make(util::toString(tensor) + "_stride", Int());
-          result.push_back(VarDecl::make(strideVar, stride));
-          stride = strideVar;
-        } 
-
-        // Resize values array if not large enough
-        Expr capacityVar = getCapacityVar(tensor);
-        Expr size = simplify(ir::Mul::make(resultParentPosNext, stride));
-        result.push_back(atLeastDoubleSizeIfFull(values, capacityVar, size));
-
-        if (hasSparseInserts(iterators, readIterators) || 
-            util::contains(reducedAccesses, write)) {
-          // Zero-initialize values array if might not assign to every element 
-          // in values array during compute
-          result.push_back(zeroInitValues(tensor, resultParentPos, stride));
-        }
-      }
+  if (getChildren(indexVar).size() == 1) {
+    return getPosIteratorFullyDerivedDescendant(getChildren(indexVar)[0], irregularChild);
+  }
+  for (IndexVar child : getChildren(indexVar)) {
+    if (!util::contains(childRelMap.at(indexVar).getNode()->getIrregulars(), child)) { // is irregularity not maintained through relationship
+      return getPosIteratorFullyDerivedDescendant(child, irregularChild); // TODO: need new classification rather than reusing irregular
     }
   }
-  return result.empty() ? Stmt() : Block::make(result);
+  return false;
 }
 
-
-Stmt LowererImpl::resizeAndInitValues(const std::vector<Iterator>& appenders, 
-                                      const std::set<Access>& reducedAccesses) {
-  if (!generateComputeCode()) {
-    return Stmt();
+bool ProvenanceGraph::isIrregular(IndexVar indexVar) const {
+  if (isUnderived(indexVar)) {
+    return true;
+  }
+
+  IndexVarRel rel = parentRelMap.at(indexVar);
+  std::vector<IndexVar> irregulars = rel.getNode()->getIrregulars();
+  auto it = std::find (irregulars.begin(), irregulars.end(), indexVar);
+  if (it == irregulars.end()) {
+    // variable does not maintain irregular status through relationship
+    return false;
+  }
+
+  for (const IndexVar& parent : getParents(indexVar)) {
+    if (isIrregular(parent)) {
+      return true;
+    }
   }
+  return false;
+}
 
-  std::function<Expr(Access)> getTensor = [&](Access access) {
-    return getTensorVar(access.getTensorVar());
-  };
-  const auto reducedTensors = util::map(reducedAccesses, getTensor);
-
-  std::vector<Stmt> result;
+bool ProvenanceGraph::isUnderived(taco::IndexVar indexVar) const {
+  return getParents(indexVar).empty();
+}
 
-  for (auto& appender : appenders) {
-    if (!appender.isLeaf()) {
-      continue;
+bool ProvenanceGraph::isDerivedFrom(taco::IndexVar indexVar, taco::IndexVar ancestor) const {
+  for (IndexVar parent : getParents(indexVar)) {
+    if (parent == ancestor) {
+      return true;
+    }
+    if(isDerivedFrom(parent, ancestor)) {
+      return true;
     }
+  }
+  return false;
+}
 
-    Expr tensor = appender.getTensor(); 
-    Expr values = GetProperty::make(tensor, TensorProperty::Values);
-    Expr capacity = getCapacityVar(appender.getTensor());
-    Expr pos = appender.getIteratorVar();
+bool ProvenanceGraph::isFullyDerived(taco::IndexVar indexVar) const {
+  return getChildren(indexVar).empty();
+}
 
-    if (generateAssembleCode()) {
-      result.push_back(doubleSizeIfFull(values, capacity, pos));
+bool ProvenanceGraph::isAvailable(IndexVar indexVar, std::set<IndexVar> defined) const {
+  for (const IndexVar& parent : getParents(indexVar)) {
+    if (!defined.count(parent)) {
+      return false;
     }
+  }
+  return true;
+}
 
-    if (util::contains(reducedTensors, tensor)) {
-      Expr zero = ir::Literal::zero(tensor.type());
-      result.push_back(Store::make(values, pos, zero));
+bool ProvenanceGraph::isRecoverable(taco::IndexVar indexVar, std::set<taco::IndexVar> defined) const {
+  // all children are either defined or recoverable from their children
+  // This checks the definedVars list to determine where in the statement the variables are trying to be
+  // recovered from ( either on the producer or consumer side of a where stmt or not in a where stmt)
+  vector<IndexVar> producers;
+  vector<IndexVar> consumers;
+  for (auto& def : defined) {
+    if (childRelMap.count(def) && childRelMap.at(def).getRelType() == IndexVarRelType::PRECOMPUTE) {
+      consumers.push_back(def);
+    }
+    if (parentRelMap.count(def) && parentRelMap.at(def).getRelType() == IndexVarRelType::PRECOMPUTE) {
+      producers.push_back(def);
     }
   }
 
-  return result.empty() ? Stmt() : Block::make(result);
+  return isRecoverablePrecompute(indexVar, defined, producers, consumers);
 }
 
-
-Stmt LowererImpl::zeroInitValues(Expr tensor, Expr begin, Expr size) {
-  Expr lower = simplify(ir::Mul::make(begin, size));
-  Expr upper = simplify(ir::Mul::make(ir::Add::make(begin, 1), size));
-  Expr p = Var::make("p" + util::toString(tensor), Int());
-  Expr values = GetProperty::make(tensor, TensorProperty::Values);
-  Stmt zeroInit = Store::make(values, p, ir::Literal::zero(tensor.type()));
-  LoopKind parallel = (isa<ir::Literal>(size) && 
-                       to<ir::Literal>(size)->getIntValue() < (1 << 10))
-                      ? LoopKind::Serial : LoopKind::Static;
-  return For::make(p, lower, upper, 1, zeroInit, parallel, false);
+bool ProvenanceGraph::isRecoverablePrecompute(taco::IndexVar indexVar, std::set<taco::IndexVar> defined,
+                                              vector<IndexVar> producers, vector<IndexVar> consumers) const {
+  vector<IndexVar> childPrecompute;
+  if (std::find(consumers.begin(), consumers.end(), indexVar) != consumers.end()) {
+    return true;
+  }
+  if (!producers.empty() && (childRelMap.count(indexVar) &&
+                             childRelMap.at(indexVar).getRelType() == IndexVarRelType::PRECOMPUTE)) {
+    auto precomputeChild = getChildren(indexVar)[0];
+    if (std::find(producers.begin(), producers.end(), precomputeChild) != producers.end()) {
+      return true;
+    }
+    return isRecoverablePrecompute(precomputeChild, defined, producers, consumers);
+  }
+  for (const IndexVar& child : getChildren(indexVar)) {
+    if (!defined.count(child) && (isFullyDerived(child) ||
+                                  !isRecoverablePrecompute(child, defined, producers, consumers))) {
+      return false;
+    }
+  }
+  return true;
 }
 
-
-Stmt LowererImpl::declLocatePosVars(vector<Iterator> locators) {
-  vector<Stmt> result;
-  for (Iterator& locator : locators) {
-    accessibleIterators.insert(locator);
-
-    bool doLocate = true;
-    for (Iterator ancestorIterator = locator.getParent();
-         !ancestorIterator.isRoot() && ancestorIterator.hasLocate();
-         ancestorIterator = ancestorIterator.getParent()) {
-      if (!accessibleIterators.contains(ancestorIterator)) {
-        doLocate = false;
+bool ProvenanceGraph::isChildRecoverable(taco::IndexVar indexVar, std::set<taco::IndexVar> defined) const {
+  // at most 1 unknown in relation
+  int count_unknown = 0;
+  for (const IndexVar& parent : getParents(indexVar)) {
+    if (!defined.count(parent)) {
+      count_unknown++;
+    }
+    for (const IndexVar& sibling : getChildren(parent)) {
+      if (!defined.count(sibling)) {
+        count_unknown++;
       }
     }
+  }
+  return count_unknown <= 1;
+}
 
-    if (doLocate) {
-      Iterator locateIterator = locator;
-      do {
-        ModeFunction locate = locateIterator.locate(coordinates(locateIterator));
-        taco_iassert(isValue(locate.getResults()[1], true));
-        Stmt declarePosVar = VarDecl::make(locateIterator.getPosVar(),
-                                           locate.getResults()[0]);
-        result.push_back(declarePosVar);
+// in terms of joined spaces
+void ProvenanceGraph::addRelativeBoundsToMap(IndexVar indexVar, std::set<IndexVar> alreadyDefined, std::map<IndexVar, std::vector<ir::Expr>> &bounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators) const {
+  // derive bounds of parents and use to construct bounds
+  if (isUnderived(indexVar)) {
+    taco_iassert(bounds.count(indexVar));
+    return; // underived bound should already be in bounds
+  }
 
-        if (locateIterator.isLeaf()) {
-          break;
-        }
-        
-        locateIterator = locateIterator.getChild();
-      } while (accessibleIterators.contains(locateIterator));
-    }
-  }
-  return result.empty() ? Stmt() : Block::make(result);
+  for (IndexVar parent : getParents(indexVar)) {
+    addRelativeBoundsToMap(parent, alreadyDefined, bounds, variableExprs, iterators);
+  }
+
+  IndexVarRel rel = parentRelMap.at(indexVar);
+  bounds[indexVar] = rel.getNode()->computeRelativeBound(alreadyDefined, bounds, variableExprs, iterators, *this);
 }
 
+void ProvenanceGraph::computeBoundsForUnderivedAncestors(IndexVar indexVar, std::map<IndexVar, std::vector<ir::Expr>> relativeBounds, std::map<IndexVar, std::vector<ir::Expr>> &computedBounds) const {
+  std::vector<IndexVar> underivedAncestors = getUnderivedAncestors(indexVar);
+  // taco_iassert(underivedAncestors.size() == 1); // TODO: fuse
 
-Stmt LowererImpl::reduceDuplicateCoordinates(Expr coordinate, 
-                                             vector<Iterator> iterators,
-                                             bool alwaysReduce) {
-  vector<Stmt> result;
-  for (Iterator& iterator : iterators) {
-    taco_iassert(!iterator.isUnique() && iterator.hasPosIter());
-
-    Access access = this->iterators.modeAccess(iterator).getAccess();
-    Expr iterVar = iterator.getIteratorVar();
-    Expr segendVar = iterator.getSegendVar();
-    Expr reducedVal = iterator.isLeaf() ? getReducedValueVar(access) : Expr();
-    Expr tensorVar = getTensorVar(access.getTensorVar());
-    Expr tensorVals = GetProperty::make(tensorVar, TensorProperty::Values);
-
-    // Initialize variable storing reduced component value.
-    if (reducedVal.defined()) {
-      Expr reducedValInit = alwaysReduce 
-                          ? Load::make(tensorVals, iterVar)
-                          : ir::Literal::zero(reducedVal.type());
-      result.push_back(VarDecl::make(reducedVal, reducedValInit));
-    }
-
-    if (iterator.isLeaf()) {
-      // If iterator is over bottommost coordinate hierarchy level and will 
-      // always advance (i.e., not merging with another iterator), then we don't 
-      // need a separate segend variable.
-      segendVar = iterVar;
-      if (alwaysReduce) {
-        result.push_back(compoundAssign(segendVar, 1));
-      }
-    } else {
-      Expr segendInit = alwaysReduce ? ir::Add::make(iterVar, 1) : iterVar;
-      result.push_back(VarDecl::make(segendVar, segendInit));
-    } 
-    
-    vector<Stmt> dedupStmts;
-    if (reducedVal.defined()) {
-      Expr partialVal = Load::make(tensorVals, segendVar);
-      dedupStmts.push_back(compoundAssign(reducedVal, partialVal));
-    }
-    dedupStmts.push_back(compoundAssign(segendVar, 1));
-    Stmt dedupBody = Block::make(dedupStmts);
-
-    ModeFunction posAccess = iterator.posAccess(segendVar, 
-                                                coordinates(iterator));
-    // TODO: Support access functions that perform additional computations 
-    //       and/or might access invalid positions.
-    taco_iassert(!posAccess.compute().defined());
-    taco_iassert(to<ir::Literal>(posAccess.getResults()[1])->getBoolValue());
-    Expr nextCoord = posAccess.getResults()[0];
-    Expr withinBounds = Lt::make(segendVar, iterator.getEndVar());
-    Expr isDuplicate = Eq::make(posAccess.getResults()[0], coordinate);
-    result.push_back(While::make(And::make(withinBounds, isDuplicate),
-                                 Block::make(dedupStmts)));
-  }
-  return result.empty() ? Stmt() : Block::make(result);
+  computedBounds[underivedAncestors[0]] = relativeBounds[indexVar];
 }
 
-
-Stmt LowererImpl::codeToInitializeIteratorVars(vector<Iterator> iterators) {
-  vector<Stmt> result;
-  for (Iterator iterator : iterators) {
-    taco_iassert(iterator.hasPosIter() || iterator.hasCoordIter() ||
-                 iterator.isDimensionIterator());
-
-    Expr iterVar = iterator.getIteratorVar();
-    Expr endVar = iterator.getEndVar();
-    if (iterator.hasPosIter()) {
-      Expr parentPos = iterator.getParent().getPosVar();
-      if (iterator.getParent().isRoot() || iterator.getParent().isUnique()) {
-        // E.g. a compressed mode without duplicates
-        ModeFunction bounds = iterator.posBounds(parentPos);
-        result.push_back(bounds.compute());
-        result.push_back(VarDecl::make(iterVar, bounds[0]));
-        result.push_back(VarDecl::make(endVar, bounds[1]));
-      } else {
-        taco_iassert(iterator.isOrdered() && iterator.getParent().isOrdered());
-        taco_iassert(iterator.isCompact() && iterator.getParent().isCompact());
-
-        // E.g. a compressed mode with duplicates. Apply iterator chaining
-        Expr parentSegend = iterator.getParent().getSegendVar();
-        ModeFunction startBounds = iterator.posBounds(parentPos);
-        ModeFunction endBounds = iterator.posBounds(ir::Sub::make(parentSegend, 1));
-        result.push_back(startBounds.compute());
-        result.push_back(VarDecl::make(iterVar, startBounds[0]));
-        result.push_back(endBounds.compute());
-        result.push_back(VarDecl::make(endVar, endBounds[1]));
+std::map<IndexVar, std::vector<ir::Expr>> ProvenanceGraph::deriveCoordBounds(std::vector<IndexVar> derivedVarOrder, std::map<IndexVar, std::vector<ir::Expr>> underivedBounds, std::map<IndexVar, ir::Expr> variableExprs, Iterators iterators) const {
+  std::map<IndexVar, std::vector<ir::Expr>> computedCoordbounds = underivedBounds;
+  std::set<IndexVar> defined;
+  for (IndexVar indexVar : derivedVarOrder) {
+    if (indexVar != derivedVarOrder.back()) {
+      for (auto recoverable : newlyRecoverableParents(indexVar, defined)) {
+        defined.insert(recoverable);
       }
+      defined.insert(indexVar);
     }
-    else if (iterator.hasCoordIter()) {
-      // E.g. a hasmap mode
-      vector<Expr> coords = coordinates(iterator);
-      coords.erase(coords.begin());
-      ModeFunction bounds = iterator.coordBounds(coords);
-      result.push_back(bounds.compute());
-      result.push_back(VarDecl::make(iterVar, bounds[0]));
-      result.push_back(VarDecl::make(endVar, bounds[1]));
-    }
-    else if (iterator.isDimensionIterator()) {
-      // A dimension
-      Expr coord = coordinates(vector<Iterator>({iterator}))[0];
-      result.push_back(VarDecl::make(coord, 0));
+    if (isUnderived(indexVar)) {
+      continue; // underived indexvar can't constrain bounds
     }
+
+    // add all relative coord bounds of nodes along derivation path to map.
+    std::map<IndexVar, std::vector<ir::Expr>> relativeBounds = underivedBounds;
+    addRelativeBoundsToMap(indexVar, defined, relativeBounds, variableExprs, iterators);
+
+    // modify bounds for affected underived
+    computeBoundsForUnderivedAncestors(indexVar, relativeBounds, computedCoordbounds);
   }
-  return result.empty() ? Stmt() : Block::make(result);
+  return computedCoordbounds;
 }
 
+std::vector<ir::Expr> ProvenanceGraph::deriveIterBounds(IndexVar indexVar, std::vector<IndexVar> derivedVarOrder, std::map<IndexVar, std::vector<ir::Expr>> underivedBounds,
+                                                  std::map<taco::IndexVar, taco::ir::Expr> variableNames, Iterators iterators) const {
+  // strategy is to start with underived variable bounds and propagate through each step on return call.
+  // Define in IndexVarRel a function that takes in an Expr and produces an Expr for bound
+  // for split: outer: Div(expr, splitfactor), Div(expr, splitfactor), inner: 0, splitfactor
+  // what about for reordered split: same loop bounds just reordered loops (this might change for different tail strategies)
 
-Stmt LowererImpl::codeToIncIteratorVars(Expr coordinate, vector<Iterator> iterators) {
-  if (iterators.size() == 1) {
-    Expr ivar = iterators[0].getIteratorVar();
+  if (isUnderived(indexVar)) {
+    taco_iassert(underivedBounds.count(indexVar) == 1);
+    return underivedBounds[indexVar];
+  }
 
-    if (iterators[0].isUnique()) {
-      return compoundAssign(ivar, 1); 
-    }
+  std::vector<IndexVar> derivedVarOrderExceptLast = derivedVarOrder;
+  if (!derivedVarOrderExceptLast.empty()) {
+    derivedVarOrderExceptLast.pop_back();
+  }
+  taco_iassert(std::find(derivedVarOrderExceptLast.begin(), derivedVarOrderExceptLast.end(), indexVar) == derivedVarOrderExceptLast.end());
 
-    // If iterator is over bottommost coordinate hierarchy level with 
-    // duplicates and iterator will always advance (i.e., not merging with 
-    // another iterator), then deduplication loop will take care of 
-    // incrementing iterator variable.
-    return iterators[0].isLeaf() 
-           ? Stmt()
-           : Assign::make(ivar, iterators[0].getSegendVar());
+  std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds;
+  std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds;
+  for (const IndexVar& parent : getParents(indexVar)) {
+    parentIterBounds[parent] = deriveIterBounds(parent, derivedVarOrder, underivedBounds, variableNames, iterators);
+    vector<IndexVar> underivedParentAncestors = getUnderivedAncestors(parent);
+    // TODO: this is okay for now because we don't need parentCoordBounds for fused taco_iassert(underivedParentAncestors.size() == 1);
+    IndexVar underivedParent = underivedParentAncestors[0];
+    parentCoordBounds[parent] = deriveCoordBounds(derivedVarOrderExceptLast, underivedBounds, variableNames, iterators)[underivedParent];
   }
 
-  vector<Stmt> result;
+  IndexVarRel rel = parentRelMap.at(indexVar);
+  return rel.getNode()->deriveIterBounds(indexVar, parentIterBounds, parentCoordBounds, variableNames, iterators, *this);
+}
 
-  // We emit the level iterators before the mode iterator because the coordinate
-  // of the mode iterator is used to conditionally advance the level iterators.
+bool ProvenanceGraph::hasCoordBounds(IndexVar indexVar) const {
+  return !isUnderived(indexVar) && isCoordVariable(indexVar);
+}
 
-  auto levelIterators =
-      filter(iterators, [](Iterator it){return !it.isDimensionIterator();});
-  for (auto& iterator : levelIterators) {
-    Expr ivar = iterator.getIteratorVar();
-    if (iterator.isUnique()) {
-      Expr increment = iterator.isFull()
-                     ? 1
-                     : ir::Cast::make(Eq::make(iterator.getCoordVar(), 
-                                               coordinate),
-                                      ivar.type());
-      result.push_back(compoundAssign(ivar, increment));
-    } else if (!iterator.isLeaf()) {
-      result.push_back(Assign::make(ivar, iterator.getSegendVar()));
+// position variable if any pos relationship parent
+bool ProvenanceGraph::isPosVariable(taco::IndexVar indexVar) const {
+  if (isUnderived(indexVar)) return false;
+  if (parentRelMap.at(indexVar).getRelType() == POS) return true;
+  for (const IndexVar& parent : getParents(indexVar)) {
+    if (isPosVariable(parent)) {
+      return true;
     }
   }
+  return false;
+}
 
-  auto modeIterators =
-      filter(iterators, [](Iterator it){return it.isDimensionIterator();});
-  for (auto& iterator : modeIterators) {
-    taco_iassert(iterator.isFull());
-    Expr ivar = iterator.getIteratorVar();
-    result.push_back(compoundAssign(ivar, 1));
+bool ProvenanceGraph::isPosOfAccess(IndexVar indexVar, Access access) const {
+  if (isUnderived(indexVar)) return false;
+  if (parentRelMap.at(indexVar).getRelType() == POS) {
+    return equals(parentRelMap.at(indexVar).getNode<PosRelNode>()->getAccess(), access);
+  }
+  else if (parentRelMap.at(indexVar).getRelType() == FUSE) {
+    return false; // lose pos of access status through fuse
+  }
+  for (const IndexVar& parent : getParents(indexVar)) {
+    if (isPosOfAccess(parent, access)) {
+      return true;
+    }
   }
-
-  return Block::make(result);
+  return false;
 }
 
-
-static
-bool isLastAppender(Iterator iter) {
-  taco_iassert(iter.hasAppend());
-  while (!iter.isLeaf()) {
-    iter = iter.getChild();
-    if (iter.hasAppend()) {
+bool ProvenanceGraph::hasPosDescendant(taco::IndexVar indexVar) const {
+  if (isPosVariable(indexVar)) return true;
+  if (isFullyDerived(indexVar)) return false;
+  IndexVarRel rel = childRelMap.at(indexVar);
+  if (rel.getRelType() == FUSE) {
+    vector<IndexVar> partners = getParents(getChildren(indexVar)[0]);
+    if ((indexVar == partners[0] && isPosVariable(partners[1])) || (indexVar == partners[1] && isPosVariable(partners[0]))) {
+      // can't get pos descendant from being fused with an already pos variable (need to be turned pos along derivation path)
       return false;
     }
   }
-  return true;
+  for (auto child : getChildren(indexVar)) {
+    if (hasPosDescendant(child)) return true;
+  }
+  return false;
 }
 
+bool ProvenanceGraph::isCoordVariable(taco::IndexVar indexVar) const {
+  return !isPosVariable(indexVar);
+}
 
-Stmt LowererImpl::appendCoordinate(vector<Iterator> appenders, Expr coord) {
-  vector<Stmt> result;
-  for (auto& appender : appenders) {
-    Expr pos = appender.getPosVar();
-    Iterator appenderChild = appender.getChild();
-
-    if (appenderChild.defined() && appenderChild.isBranchless()) {
-      // Already emitted assembly code for current level when handling 
-      // branchless child level, so don't emit code again.
-      continue;
-    }
-
-    vector<Stmt> appendStmts;
-
-    if (generateAssembleCode()) {
-      appendStmts.push_back(appender.getAppendCoord(pos, coord));
-      while (!appender.isRoot() && appender.isBranchless()) {
-        // Need to append result coordinate to parent level as well if child 
-        // level is branchless (so child coordinates will have unique parents).
-        appender = appender.getParent();
-        if (!appender.isRoot()) {
-          taco_iassert(appender.hasAppend()) << "Parent level of branchless, "
-              << "append-capable level must also be append-capable";
-          taco_iassert(!appender.isUnique()) << "Need to be able to insert " 
-              << "duplicate coordinates to level, but level is declared unique";
+bool ProvenanceGraph::hasExactBound(IndexVar indexVar) const {
+  if (isUnderived(indexVar)) {
+    return false;
+  }
 
-          Expr coord = getCoordinateVar(appender);
-          appendStmts.push_back(appender.getAppendCoord(pos, coord));
+  IndexVarRel rel = parentRelMap.at(indexVar);
+  if(rel.getRelType() == BOUND)
+  {
+    return rel.getNode<BoundRelNode>()->getBoundType() == BoundType::MaxExact;
+  }
+  // TODO: include non-irregular variables
+  return false;
+}
+
+std::vector<IndexVar> ProvenanceGraph::newlyRecoverableParents(taco::IndexVar indexVar,
+                                                   std::set<taco::IndexVar> previouslyDefined) const {
+  // for each parent is it not recoverable with previouslyDefined, but yes with previouslyDefined+indexVar
+  if (isUnderived(indexVar)) {
+    return {};
+  }
+
+  std::set<taco::IndexVar> defined = previouslyDefined;
+  defined.insert(indexVar);
+
+  std::vector<IndexVar> newlyRecoverable;
+
+  for (const IndexVar& parent : getParents(indexVar)) {
+    if (parentRelMap.at(indexVar).getRelType() == FUSE) {
+      IndexVar irregularDescendant;
+      if (getIrregularDescendant(indexVar, &irregularDescendant) && isPosVariable(irregularDescendant) && isCoordVariable(parent)) { // Fused Pos case needs to be tracked with special while loop
+        if (parent == getParents(indexVar)[0]) {
+          continue;
         }
       }
-    } 
-    
-    if (generateAssembleCode() || isLastAppender(appender)) {
-      appendStmts.push_back(compoundAssign(pos, 1));
-
-      Stmt appendCode = Block::make(appendStmts);
-      if (appenderChild.defined() && appenderChild.hasAppend()) {
-        // Emit guard to avoid appending empty slices to result.
-        // TODO: Users should be able to configure whether to append zeroes.
-        Expr shouldAppend = Lt::make(appenderChild.getBeginVar(), 
-                                     appenderChild.getPosVar());
-        appendCode = IfThenElse::make(shouldAppend, appendCode);
-      }
-      result.push_back(appendCode);
+    }
+
+    if (!isRecoverable(parent, previouslyDefined) && isRecoverable(parent, defined)) {
+      newlyRecoverable.push_back(parent);
+      std::vector<IndexVar> parentRecoverable = newlyRecoverableParents(parent, previouslyDefined);
+      newlyRecoverable.insert(newlyRecoverable.end(), parentRecoverable.begin(), parentRecoverable.end());
     }
   }
-  return result.empty() ? Stmt() : Block::make(result);
+  return newlyRecoverable;
 }
 
+std::vector<IndexVar> ProvenanceGraph::derivationPath(taco::IndexVar ancestor, taco::IndexVar indexVar) const {
+  if (ancestor == indexVar) {
+    return {indexVar};
+  }
 
-Stmt LowererImpl::generateAppendPositions(vector<Iterator> appenders) {
-  vector<Stmt> result;
-  if (generateAssembleCode()) {
-    for (Iterator appender : appenders) {
-      if (!appender.isBranchless()) {
-        Expr pos = [](Iterator appender) {
-          // Get the position variable associated with the appender. If a mode 
-          // is above a branchless mode, then the two modes can share the same 
-          // position variable.
-          while (!appender.isLeaf() && appender.getChild().isBranchless()) {
-            appender = appender.getChild();
-          }
-          return appender.getPosVar();
-        }(appender);
-        Expr beginPos = appender.getBeginVar();
-        Expr parentPos = appender.getParent().getPosVar();
-        result.push_back(appender.getAppendEdges(parentPos, beginPos, pos));
-      }
+  for (IndexVar child : getChildren(ancestor)) {
+    std::vector<IndexVar> childResult = derivationPath(child, indexVar);
+    if (!childResult.empty()) {
+      childResult.insert(childResult.begin(), ancestor);
+      return childResult;
     }
   }
-  return result.empty() ? Stmt() : Block::make(result);
+  // wrong path taken
+  return {};
 }
 
-
-Expr LowererImpl::generateValueLocExpr(Access access) const {
-  if (isScalar(access.getTensorVar().getType())) {
-    return ir::Literal::make(0);
+ir::Expr ProvenanceGraph::recoverVariable(taco::IndexVar indexVar,
+                                           std::vector<IndexVar> definedVarOrder,
+                                           std::map<IndexVar, std::vector<ir::Expr>> underivedBounds,
+                                           std::map<taco::IndexVar, taco::ir::Expr> childVariables,
+                                           Iterators iterators) const {
+  if (isFullyDerived(indexVar)) {
+    return ir::Expr();
   }
-  Iterator it = getIterators(access).back();
-  return it.getPosVar();
-}
 
+  IndexVarRel rel = childRelMap.at(indexVar);
 
-Expr LowererImpl::checkThatNoneAreExhausted(std::vector<Iterator> iterators)
-{
-  taco_iassert(!iterators.empty());
-  if (iterators.size() == 1 && iterators[0].isFull()) {
-    Expr dimension = getDimension(iterators[0].getIndexVar());
-    return Lt::make(iterators[0].getIteratorVar(), dimension);
+  std::map<IndexVar, std::vector<ir::Expr>> parentCoordBounds;
+  std::map<IndexVar, std::vector<ir::Expr>> parentIterBounds;
+  for (IndexVar parent : rel.getNode()->getParents()) {
+    vector<IndexVar> underivedParentAncestors = getUnderivedAncestors(parent);
+    //TODO: taco_iassert(underivedParentAncestors.size() == 1);
+    IndexVar underivedParent = underivedParentAncestors[0];
+    parentIterBounds[parent] = deriveIterBounds(parent, definedVarOrder, underivedBounds, childVariables, iterators);
+    parentCoordBounds[parent] = deriveCoordBounds(definedVarOrder, underivedBounds, childVariables, iterators)[underivedParent];
   }
 
-  vector<Expr> result;
-  for (const auto& iterator : iterators) {
-    taco_iassert(!iterator.isFull()) << iterator
-        << " - full iterators do not need to partake in merge loop bounds";
-    Expr iterUnexhausted = Lt::make(iterator.getIteratorVar(),
-                                    iterator.getEndVar());
-    result.push_back(iterUnexhausted);
+  return rel.getNode()->recoverVariable(indexVar, childVariables, iterators, parentIterBounds, parentCoordBounds, *this);
+}
+
+ir::Stmt ProvenanceGraph::recoverChild(taco::IndexVar indexVar,
+                                        std::map<taco::IndexVar, taco::ir::Expr> relVariables, bool emitVarDecl, Iterators iterators) const {
+  if (isUnderived(indexVar)) {
+    return ir::Stmt();
   }
 
-  return (!result.empty())
-         ? conjunction(result)
-         : Lt::make(iterators[0].getIteratorVar(), iterators[0].getEndVar());
+  IndexVarRel rel = parentRelMap.at(indexVar);
+  return rel.getNode()->recoverChild(indexVar, relVariables, emitVarDecl, iterators, *this);
+}
+
+std::set<IndexVar> ProvenanceGraph::getAllIndexVars() const {
+  return nodes;
+}
+
+bool ProvenanceGraph::isDivided(IndexVar indexVar) const {
+  // See if the indexVar has any children. If so, look at the relation that
+  // created the parent-child relationship. If it is a divide, return true.
+  auto children = this->getChildren(indexVar);
+  if (children.size() > 0) {
+    auto rel = this->childRelMap.at(indexVar);
+    if (rel.getRelType() == DIVIDE) {
+      return true;
+    }
+  }
+  return false;
 }
 
 }
```

### Comparing `tensora-0.0.6/src/taco/src/lower/mode.cpp` & `tensora-0.0.7/src/taco/src/lower/mode.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/lower/mode_access.h` & `tensora-0.0.7/src/taco/src/lower/mode_access.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/lower/mode_format_compressed.cpp` & `tensora-0.0.7/src/taco/src/lower/mode_format_compressed.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 #include "taco/lower/mode_format_compressed.h"
 
-#include "ir/ir_generators.h"
+#include "taco/ir/ir_generators.h"
 #include "taco/ir/simplify.h"
 #include "taco/util/strings.h"
 
 using namespace std;
 using namespace taco::ir;
 
 namespace taco {
 
 CompressedModeFormat::CompressedModeFormat() : 
-    CompressedModeFormat(false, true, true) {
+    CompressedModeFormat(false, true, true, false) {
 }
 
 CompressedModeFormat::CompressedModeFormat(bool isFull, bool isOrdered,
-                                       bool isUnique, long long allocSize) :
+                                           bool isUnique, bool isZeroless, 
+                                           long long allocSize) :
     ModeFormatImpl("compressed", isFull, isOrdered, isUnique, false, true,
-                   false, true, false, false, true), 
+                   isZeroless, false, false, true, false, false, true, true,  
+                   true, false), 
     allocSize(allocSize) {
 }
 
 ModeFormat CompressedModeFormat::copy(
     vector<ModeFormat::Property> properties) const {
   bool isFull = this->isFull;
   bool isOrdered = this->isOrdered;
   bool isUnique = this->isUnique;
+  bool isZeroless = this->isZeroless;  
   for (const auto property : properties) {
     switch (property) {
       case ModeFormat::FULL:
         isFull = true;
         break;
       case ModeFormat::NOT_FULL:
         isFull = false;
@@ -41,100 +44,128 @@
         break;
       case ModeFormat::UNIQUE:
         isUnique = true;
         break;
       case ModeFormat::NOT_UNIQUE:
         isUnique = false;
         break;
+      case ModeFormat::ZEROLESS:
+        isZeroless = true;
+        break;
+      case ModeFormat::NOT_ZEROLESS:
+        isZeroless = false;
+        break;			
       default:
         break;
     }
   }
   const auto compressedVariant = 
-      std::make_shared<CompressedModeFormat>(isFull, isOrdered, isUnique);
+      std::make_shared<CompressedModeFormat>(isFull, isOrdered, isUnique, 
+                                             isZeroless);
   return ModeFormat(compressedVariant);
 }
 
+std::vector<AttrQuery> CompressedModeFormat::attrQueries(
+    vector<IndexVar> parentCoords, vector<IndexVar> childCoords) const {
+  std::vector<IndexVar> groupBy(parentCoords.begin(), parentCoords.end() - 1);
+
+  std::vector<IndexVar> aggregatedCoords = {parentCoords.back()};
+  if (!isUnique) {
+    aggregatedCoords.insert(aggregatedCoords.end(), childCoords.begin(), 
+                            childCoords.end());
+  }
+
+  return {AttrQuery(groupBy, {std::make_tuple("nnz", AttrQuery::COUNT, aggregatedCoords)})};
+}
+
 ModeFunction CompressedModeFormat::posIterBounds(Expr parentPos, 
                                                  Mode mode) const {
   Expr pbegin = Load::make(getPosArray(mode.getModePack()), parentPos);
   Expr pend = Load::make(getPosArray(mode.getModePack()),
-                         Add::make(parentPos, 1));
+                         ir::Add::make(parentPos, 1));
   return ModeFunction(Stmt(), {pbegin, pend});
 }
 
+ModeFunction CompressedModeFormat::coordBounds(Expr parentPos,
+                                                 Mode mode) const {
+  Expr pend = Load::make(getPosArray(mode.getModePack()),
+                         ir::Add::make(parentPos, 1));
+  Expr coordend = Load::make(getCoordArray(mode.getModePack()), ir::Sub::make(pend, 1));
+  return ModeFunction(Stmt(), {0, coordend});
+}
+
 ModeFunction CompressedModeFormat::posIterAccess(ir::Expr pos,
                                                  std::vector<ir::Expr> coords,
                                                  Mode mode) const {
   taco_iassert(mode.getPackLocation() == 0);
 
   Expr idxArray = getCoordArray(mode.getModePack());
   Expr stride = (int)mode.getModePack().getNumModes();
-  Expr idx = Load::make(idxArray, Mul::make(pos, stride));
+  Expr idx = Load::make(idxArray, ir::Mul::make(pos, stride));
   return ModeFunction(Stmt(), {idx, true});
 }
 
 Stmt CompressedModeFormat::getAppendCoord(Expr p, Expr i, Mode mode) const {
   taco_iassert(mode.getPackLocation() == 0);
 
   Expr idxArray = getCoordArray(mode.getModePack());
   Expr stride = (int)mode.getModePack().getNumModes();
-  Stmt storeIdx = Store::make(idxArray, Mul::make(p, stride), i);
+  Stmt storeIdx = Store::make(idxArray, ir::Mul::make(p, stride), i);
 
   if (mode.getModePack().getNumModes() > 1) {
     return storeIdx;
   }
 
   Stmt maybeResizeIdx = doubleSizeIfFull(idxArray, getCoordCapacity(mode), p);
   return Block::make({maybeResizeIdx, storeIdx});
 }
 
 Stmt CompressedModeFormat::getAppendEdges(Expr pPrev, Expr pBegin, Expr pEnd, 
                                           Mode mode) const {
   Expr posArray = getPosArray(mode.getModePack());
   ModeFormat parentModeType = mode.getParentModeType();
   Expr edges = (!parentModeType.defined() || parentModeType.hasAppend())
-               ? pEnd : Sub::make(pEnd, pBegin);
-  return Store::make(posArray, Add::make(pPrev, 1), edges);
+               ? pEnd : ir::Sub::make(pEnd, pBegin);
+  return Store::make(posArray, ir::Add::make(pPrev, 1), edges);
 }
 
 Expr CompressedModeFormat::getSize(ir::Expr szPrev, Mode mode) const {
   return Load::make(getPosArray(mode.getModePack()), szPrev);
 }
 
 Stmt CompressedModeFormat::getAppendInitEdges(Expr pPrevBegin, 
     Expr pPrevEnd, Mode mode) const {
-  if (isa<Literal>(pPrevBegin)) {
-    taco_iassert(to<Literal>(pPrevBegin)->equalsScalar(0));
+  if (isa<ir::Literal>(pPrevBegin)) {
+    taco_iassert(to<ir::Literal>(pPrevBegin)->equalsScalar(0));
     return Stmt();
   }
 
   Expr posArray = getPosArray(mode.getModePack());
   Expr posCapacity = getPosCapacity(mode);
   ModeFormat parentModeType = mode.getParentModeType();
   if (!parentModeType.defined() || parentModeType.hasAppend()) {
     return doubleSizeIfFull(posArray, posCapacity, pPrevEnd);
   }
 
   Expr pVar = Var::make("p" + mode.getName(), Int());
-  Expr lb = Add::make(pPrevBegin, 1);
-  Expr ub = Add::make(pPrevEnd, 1);
+  Expr lb = ir::Add::make(pPrevBegin, 1);
+  Expr ub = ir::Add::make(pPrevEnd, 1);
   Stmt initPos = For::make(pVar, lb, ub, 1, Store::make(posArray, pVar, 0));
   Stmt maybeResizePos = atLeastDoubleSizeIfFull(posArray, posCapacity, pPrevEnd);
   return Block::make({maybeResizePos, initPos});
 }
 
 Stmt CompressedModeFormat::getAppendInitLevel(Expr szPrev, Expr sz,
                                               Mode mode) const {
-  const bool szPrevIsZero = isa<Literal>(szPrev) && 
-                            to<Literal>(szPrev)->equalsScalar(0);
+  const bool szPrevIsZero = isa<ir::Literal>(szPrev) && 
+                            to<ir::Literal>(szPrev)->equalsScalar(0);
 
-  Expr defaultCapacity = Literal::make(allocSize, Datatype::Int32); 
+  Expr defaultCapacity = ir::Literal::make(allocSize, Datatype::Int32); 
   Expr posArray = getPosArray(mode.getModePack());
-  Expr initCapacity = szPrevIsZero ? defaultCapacity : Add::make(szPrev, 1);
+  Expr initCapacity = szPrevIsZero ? defaultCapacity : ir::Add::make(szPrev, 1);
   Expr posCapacity = initCapacity;
   
   std::vector<Stmt> initStmts;
   if (szPrevIsZero) {
     posCapacity = getPosCapacity(mode);
     initStmts.push_back(VarDecl::make(posCapacity, initCapacity));
   }
@@ -157,32 +188,92 @@
 
   return Block::make(initStmts);
 }
 
 Stmt CompressedModeFormat::getAppendFinalizeLevel(Expr szPrev, 
     Expr sz, Mode mode) const {
     ModeFormat parentModeType = mode.getParentModeType();
-  if ((isa<Literal>(szPrev) && to<Literal>(szPrev)->equalsScalar(1)) || 
+  if ((isa<ir::Literal>(szPrev) && to<ir::Literal>(szPrev)->equalsScalar(1)) || 
       !parentModeType.defined() || parentModeType.hasAppend()) {
     return Stmt();
   }
 
   Expr csVar = Var::make("cs" + mode.getName(), Int());
   Stmt initCs = VarDecl::make(csVar, 0);
   
   Expr pVar = Var::make("p" + mode.getName(), Int());
   Expr loadPos = Load::make(getPosArray(mode.getModePack()), pVar);
-  Stmt incCs = Assign::make(csVar, Add::make(csVar, loadPos));
+  Stmt incCs = Assign::make(csVar, ir::Add::make(csVar, loadPos));
   Stmt updatePos = Store::make(getPosArray(mode.getModePack()), pVar, csVar);
   Stmt body = Block::make({incCs, updatePos});
-  Stmt finalizeLoop = For::make(pVar, 1, Add::make(szPrev, 1), 1, body);
+  Stmt finalizeLoop = For::make(pVar, 1, ir::Add::make(szPrev, 1), 1, body);
 
   return Block::make({initCs, finalizeLoop});
 }
 
+Expr CompressedModeFormat::getAssembledSize(Expr prevSize, Mode mode) const {
+  return Load::make(getPosArray(mode.getModePack()), prevSize);
+}
+
+Stmt CompressedModeFormat::getSeqInitEdges(Expr prevSize, 
+    std::vector<AttrQueryResult> queries, Mode mode) const {
+  Expr posArray = getPosArray(mode.getModePack());
+  return Block::make({Allocate::make(posArray, ir::Add::make(prevSize, 1)),
+                      Store::make(posArray, 0, 0)});
+}
+
+Stmt CompressedModeFormat::getSeqInsertEdge(Expr parentPos, 
+    std::vector<Expr> coords, std::vector<AttrQueryResult> queries, 
+    Mode mode) const {
+  Expr posArray = getPosArray(mode.getModePack());
+  Expr prevPos = Load::make(posArray, parentPos);
+  Expr nnz = queries[0].getResult(coords, "nnz");
+  Expr pos = ir::Add::make(prevPos, nnz);
+  return Store::make(posArray, ir::Add::make(parentPos, 1), pos);
+}
+
+Stmt CompressedModeFormat::getInitCoords(Expr prevSize, 
+    std::vector<AttrQueryResult> queries, Mode mode) const {
+  Expr posArray = getPosArray(mode.getModePack());
+  Expr crdArray = getCoordArray(mode.getModePack());
+  return Allocate::make(crdArray, Load::make(posArray, prevSize));
+}
+
+Stmt CompressedModeFormat::getInitYieldPos(Expr prevSize, Mode mode) const {
+  return Stmt();
+}
+
+ModeFunction CompressedModeFormat::getYieldPos(Expr parentPos, 
+    std::vector<Expr> coords, Mode mode) const {
+  Expr ptrArr = getPosArray(mode.getModePack());
+  Expr loadPtr = Load::make(ptrArr, parentPos);
+  Expr pVar = Var::make("p" + mode.getName(), Int());
+  Stmt getPtr = VarDecl::make(pVar, loadPtr);
+  Stmt incPtr = Store::make(ptrArr, parentPos, ir::Add::make(loadPtr, 1));
+  return ModeFunction(Block::make(getPtr, incPtr), {pVar});
+}
+
+Stmt CompressedModeFormat::getInsertCoord(Expr parentPos, Expr pos, 
+    std::vector<Expr> coords, Mode mode) const {
+  taco_iassert(mode.getPackLocation() == 0);
+  Expr crdArray = getCoordArray(mode.getModePack());
+  Expr stride = (int)mode.getModePack().getNumModes();
+  return Store::make(crdArray, ir::Mul::make(pos, stride), coords.back());
+}
+
+Stmt CompressedModeFormat::getFinalizeYieldPos(Expr prevSize, Mode mode) const {
+  Expr posArr = getPosArray(mode.getModePack());
+  Expr pVar = Var::make("p", Int());
+  Stmt resetLoop = For::make(pVar, 0, prevSize, 1, 
+      Store::make(posArr, ir::Sub::make(prevSize, pVar), 
+                  Load::make(posArr, 
+                             ir::Sub::make(ir::Sub::make(prevSize, pVar), 1))));
+  return Block::make(resetLoop, Store::make(posArr, 0, 0));
+}
+
 vector<Expr> CompressedModeFormat::getArrays(Expr tensor, int mode, 
                                              int level) const {
   std::string arraysName = util::toString(tensor) + std::to_string(level);
   return {GetProperty::make(tensor, TensorProperty::Indices,
                             level - 1, 0, arraysName + "_pos"),
           GetProperty::make(tensor, TensorProperty::Indices,
                             level - 1, 1, arraysName + "_crd")};
@@ -216,8 +307,17 @@
     mode.addVar(varName, idxCapacity);
     return idxCapacity;
   }
 
   return mode.getVar(varName);
 }
 
+Expr CompressedModeFormat::getWidth(Mode mode) const {
+  return ir::Literal::make(allocSize, Datatype::Int32);
+}
+
+bool CompressedModeFormat::equals(const ModeFormatImpl& other) const {
+  return ModeFormatImpl::equals(other) && 
+         (dynamic_cast<const CompressedModeFormat&>(other).allocSize == allocSize);
+}
+
 }
```

### Comparing `tensora-0.0.6/src/taco/src/lower/mode_format_dense.cpp` & `tensora-0.0.7/src/taco/src/lower/mode_format_dense.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 #include "taco/lower/mode_format_dense.h"
 
 using namespace std;
 using namespace taco::ir;
 
 namespace taco {
 
-DenseModeFormat::DenseModeFormat() : DenseModeFormat(true, true) {
+DenseModeFormat::DenseModeFormat() : DenseModeFormat(true, true, false) {
 }
 
-DenseModeFormat::DenseModeFormat(const bool isOrdered, const bool isUnique) : 
-    ModeFormatImpl("dense", true, isOrdered, isUnique, false, true, false,
-                   false, true, true, false) {
+DenseModeFormat::DenseModeFormat(const bool isOrdered, const bool isUnique, 
+                                 const bool isZeroless) : 
+    ModeFormatImpl("dense", true, isOrdered, isUnique, false, true, isZeroless, 
+                   true, false, false, true, true, false, false, false, true) {
 }
 
 ModeFormat DenseModeFormat::copy(
     std::vector<ModeFormat::Property> properties) const {
   bool isOrdered = this->isOrdered;
   bool isUnique = this->isUnique;
+  bool isZeroless = this->isZeroless;  
   for (const auto property : properties) {
     switch (property) {
       case ModeFormat::ORDERED:
         isOrdered = true;
         break;
       case ModeFormat::NOT_ORDERED:
         isOrdered = false;
         break;
       case ModeFormat::UNIQUE:
         isUnique = true;
         break;
       case ModeFormat::NOT_UNIQUE:
         isUnique = false;
         break;
+      case ModeFormat::ZEROLESS:
+        isZeroless = true;
+        break;
+      case ModeFormat::NOT_ZEROLESS:
+        isZeroless = false;
+        break;	
       default:
         break;
     }
   }
-  return ModeFormat(std::make_shared<DenseModeFormat>(isOrdered, isUnique));
+  return ModeFormat(
+      std::make_shared<DenseModeFormat>(isOrdered, isUnique, isZeroless));  
 }
 
 ModeFunction DenseModeFormat::locate(ir::Expr parentPos,
                                    std::vector<ir::Expr> coords,
                                    Mode mode) const {
-  Expr pos = Add::make(Mul::make(parentPos, getWidth(mode)), coords.back());
+  Expr pos = ir::Add::make(ir::Mul::make(parentPos, getWidth(mode)), coords.back());
   return ModeFunction(Stmt(), {pos, true});
 }
 
 Stmt DenseModeFormat::getInsertCoord(Expr p, 
     const std::vector<Expr>& i, Mode mode) const {
   return Stmt();
 }
@@ -67,14 +76,23 @@
 }
 
 Stmt DenseModeFormat::getInsertFinalizeLevel(Expr szPrev, 
     Expr sz, Mode mode) const {
   return Stmt();
 }
 
+Expr DenseModeFormat::getAssembledSize(Expr prevSize, Mode mode) const {
+  return ir::Mul::make(prevSize, getWidth(mode));
+}
+
+ModeFunction DenseModeFormat::getYieldPos(Expr parentPos, 
+    std::vector<Expr> coords, Mode mode) const {
+  return locate(parentPos, coords, mode);
+}
+
 vector<Expr> DenseModeFormat::getArrays(Expr tensor, int mode, 
                                         int level) const {
   return {GetProperty::make(tensor, TensorProperty::Dimension, mode)};
 }
 
 Expr DenseModeFormat::getSizeArray(ModePack pack) const {
   return pack.getArray(0);
```

### Comparing `tensora-0.0.6/src/taco/src/lower/tensor_path.cpp` & `tensora-0.0.7/src/taco/src/lower/tensor_path.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/lower/tensor_path.h` & `tensora-0.0.7/src/taco/src/lower/tensor_path.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/parser/lexer.cpp` & `tensora-0.0.7/src/taco/src/parser/lexer.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/parser/parser.cpp` & `tensora-0.0.7/src/taco/src/parser/parser.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -163,18 +163,19 @@
   IndexExpr rewrittenLhs = rewriter.rewrite(lhs);
 
   for (auto& tensor : rewriter.tensors) {
     content->tensors.at(tensor.first) = tensor.second;
   }
   content->resultTensor = content->tensors.at(lhs.getTensorVar().getName());
 
-  Assignment assignment = Assignment(content->resultTensor.getTensorVar(),
-                                     lhs.getIndexVars(), rhs,
-                                     accumulate ? new AddNode : IndexExpr());
-  content->resultTensor.setAssignment(assignment);
+  if(accumulate) {
+    content->resultTensor(lhs.getIndexVars()) += rhs;
+  }else{
+    content->resultTensor(lhs.getIndexVars()) = rhs;
+  }
   return content->resultTensor;
 }
 
 IndexExpr Parser::parseExpr() {
   IndexExpr expr = parseTerm();
   while (content->currentToken == Token::add ||
          content->currentToken == Token::sub) {
@@ -265,20 +266,25 @@
       return IndexExpr(float_value);
     }
     default:
       return parseAccess();
   }
 }
 
+const std::vector<std::string> Parser::getNames() const{
+  return names;
+}
+
 Access Parser::parseAccess() {
   if(content->currentToken != Token::identifier) {
     throw ParseError("Expected tensor name");
   }
   string tensorName = content->lexer.getIdentifier();
   consume(Token::identifier);
+  names.push_back(tensorName);
 
   vector<IndexVar> varlist;
   if (content->currentToken == Token::underscore) {
     consume(Token::underscore);
     if (content->currentToken == Token::lcurly) {
       consume(Token::lcurly);
       varlist = parseVarList();
```

### Comparing `tensora-0.0.6/src/taco/src/storage/array.cpp` & `tensora-0.0.7/src/taco/src/storage/array.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/storage/file_io_rb.cpp` & `tensora-0.0.7/src/taco/src/storage/file_io_rb.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -82,18 +82,19 @@
     (*values) = (double*)malloc(nnzero * sizeof(double));
   }
   readValues(hbfile, valcrd, *values);
 
   readRHS();
 }
 
+template<typename T>
 void writeFile(std::ostream &hbfile, std::string key,
                int nrow, int ncol, int nnzero,
                int ptrsize, int indsize, int valsize,
-               int* colptr, int* rowind, double* values){
+               int* colptr, int* rowind, T* values){
 
   std::string title="CSC Matrix written by taco";
   int neltvl = 0;
   char mxtype[4] = "RUA";
   /*
     First Character:
     R Real matrix
@@ -277,21 +278,23 @@
     while(iss >> ptr) {
       values[ptr_ind] = std::stod(ptr);
       ptr_ind++;
     }
   }
 }
 
+template<typename T>
 void writeValues(std::ostream &hbfile, int valuesize,
-                 int valperline, double values[]){
+                 int valperline, T values[]){
   for (auto i = 1; i <= valuesize; i++) {
-    if (std::floor(values[i-1]) == values[i-1])
-      hbfile << values[i-1] << ".0 ";
+    auto val = static_cast<double>(values[i-1]);
+    if (std::floor(val) == val)
+      hbfile << val << ".0 ";
     else
-      hbfile << values[i-1] << " ";
+      hbfile << val << " ";
     if (i%valperline==0)
       hbfile << "\n";
   }
   if (valuesize%valperline != 0)
     hbfile << "\n";
 }
 
@@ -353,21 +356,22 @@
 
   std::fstream file;
   util::openStream(file, filename, fstream::out);
   writeRB(file, tensor);
   file.close();
 }
 
-void writeRB(std::ostream& stream, const TensorBase& tensor) {
+template<typename T>
+void writeRBTyped(std::ostream& stream, const TensorBase& tensor) {
   taco_uassert(tensor.getFormat() == CSC) <<
       "writeRB: the format of tensor " << tensor.getName() << " must be CSC";
 
   auto storage = tensor.getStorage();
   auto index = storage.getIndex();
-  double *values = (double*)storage.getValues().getData();
+  T *values = (T*)storage.getValues().getData();
 
   auto modeIndex = index.getModeIndex(1);
   auto colptr = modeIndex.getIndexArray(0);
   auto rowidx = modeIndex.getIndexArray(1);
 
   int nrow = tensor.getDimension(0);
   int ncol = tensor.getDimension(1);
@@ -380,8 +384,31 @@
   writeFile(stream,const_cast<char*> (key.c_str()),
             nrow,ncol,nnzero,
             static_cast<int>(colptr.getSize()),
             static_cast<int>(rowidx.getSize()), nnzero,
             (int*)colptr.getData(), (int*)rowidx.getData(), values);
 }
 
+void writeRB(std::ostream& stream, const TensorBase& tensor) {
+  switch(tensor.getComponentType().getKind()) {
+    case Datatype::Bool: writeRBTyped<bool>(stream, tensor); break;
+    case Datatype::UInt8: writeRBTyped<uint8_t>(stream, tensor); break;
+    case Datatype::UInt16: writeRBTyped<uint16_t>(stream, tensor); break;
+    case Datatype::UInt32: writeRBTyped<uint32_t>(stream, tensor); break;
+    case Datatype::UInt64: writeRBTyped<uint64_t>(stream, tensor); break;
+//    case Datatype::UInt128: writeRBTyped<unsigned long long>(stream, tensor); break;
+    case Datatype::Int8: writeRBTyped<int8_t>(stream, tensor); break;
+    case Datatype::Int16: writeRBTyped<int16_t>(stream, tensor); break;
+    case Datatype::Int32: writeRBTyped<int32_t>(stream, tensor); break;
+    case Datatype::Int64: writeRBTyped<int64_t>(stream, tensor); break;
+//    case Datatype::Int128: writeRBTyped<long long>(stream, tensor); break;
+    case Datatype::Float32: writeRBTyped<float>(stream, tensor); break;
+    case Datatype::Float64: writeRBTyped<double>(stream, tensor); break;
+//    case Datatype::Complex64: writeRBTyped<std::complex<float>>(stream, tensor); break;
+//    case Datatype::Complex128: writeRBTyped<std::complex<double>>(stream, tensor); break;
+    case Datatype::Undefined: taco_ierror; break;
+    default:
+      taco_unreachable;
+  }
+}
+
 }
```

### Comparing `tensora-0.0.6/src/taco/src/storage/index.cpp` & `tensora-0.0.7/src/taco/src/storage/index.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/storage/pack.cpp` & `tensora-0.0.7/src/taco/src/storage/pack.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 #include "taco/storage/pack.h"
 
 #include <climits>
 
 #include "taco/format.h"
 #include "taco/error.h"
 #include "taco/ir/ir.h"
+#include "taco/index_notation/index_notation.h"
 #include "taco/storage/storage.h"
 #include "taco/storage/index.h"
 #include "taco/storage/array.h"
 #include "taco/util/collections.h"
 
 using namespace std;
 
 namespace taco {
 
 #define PACK_NEXT_LEVEL(cend) {                                          \
   if (i + 1 == modeTypes.size()) {                                       \
     if (cbegin < cend) {                                                  \
       memcpy(&values[valuesIndex], &vals[cbegin*dataType.getNumBytes()], dataType.getNumBytes()); \
     }                                                                     \
-    else {                                                                 \
+    else if (fill == nullptr){                                                                 \
       memset(&values[valuesIndex], 0, dataType.getNumBytes());             \
+    } else {                                                               \
+      memcpy(&values[valuesIndex], fill, dataType.getNumBytes());           \
     }                                                                       \
     valuesIndex += dataType.getNumBytes();                                \
   } else {                                                               \
-    valuesIndex = packTensor(dimensions, coords, vals, cbegin, (cend), modeTypes, i+1, \
+    valuesIndex = packTensor(dimensions, coords, vals, fill, cbegin, (cend), modeTypes, i+1, \
     indices, values, dataType, valuesIndex);                             \
   }                                                                      \
 }
 
 
 /// Count unique entries (assumes the values are sorted)
 static TypedIndexVector getUniqueEntries(TypedIndexVector v, 
@@ -52,15 +55,15 @@
 }
 
 /// Pack tensor coordinates into an index structure and value array.  The
 /// indices consist of one index per tensor mode, and each index contains
 /// [0,2] index arrays.
 static int packTensor(const vector<int>& dimensions,
                       const vector<TypedIndexVector>& coords,
-                      char* vals,
+                      char* vals, const void* fill,
                       size_t begin, size_t end,
                       const vector<ModeFormat>& modeTypes, size_t i,
                       std::vector<std::vector<TypedIndexVector>>* indices,
                       char* values, Datatype dataType, int valuesIndex) {
   auto& modeType    = modeTypes[i];
   auto& levelCoords = coords[i];
   auto& index       = (*indices)[i];
@@ -115,24 +118,27 @@
 /// Pack tensor coordinates into a format. The coordinates must be stored as a
 /// structure of arrays, that is one vector per axis coordinate and one vector
 /// for the values. The coordinates must be sorted lexicographically.
 TensorStorage pack(Datatype                             componentType,
                    const std::vector<int>&              dimensions,
                    const Format&                        format,
                    const std::vector<TypedIndexVector>& coordinates,
-                   const void *                         values) {
+                   const void *                         values,
+                   const Literal&                       fill) {
+
   taco_iassert(dimensions.size() == (size_t)format.getOrder());
   taco_iassert(coordinates.size() == (size_t)format.getOrder());
   taco_iassert(sameSize(coordinates));
   taco_iassert(dimensions.size() > 0) << "Scalar packing not supported";
+  taco_iassert(fill.getDataType() == componentType) << "Component type must match value type";
 
   size_t order = dimensions.size();
   size_t numCoordinates = coordinates[0].size();
 
-  TensorStorage storage(componentType, dimensions, format);
+  TensorStorage storage(componentType, dimensions, format, fill);
 
   // Create vectors to store pointers to indices/index sizes
   vector<vector<TypedIndexVector>> indices;
   indices.reserve(order);
 
   long long int maxSize = 1;
   for (size_t i=0; i < order; ++i) {
@@ -151,15 +157,16 @@
       maxSize = numCoordinates;
     } else {
       taco_not_supported_yet;
     }
   }
 
   void* vals = malloc(maxSize * componentType.getNumBytes());
-  int actual_size = packTensor(dimensions, coordinates, (char *) values, 0,
+  const void* fillData = storage.getFillValue().defined()? storage.getFillValue().getValPtr() : nullptr;
+  int actual_size = packTensor(dimensions, coordinates, (char *) values, fillData, 0,
                                numCoordinates, format.getModeFormats(), 0,
                                &indices, (char *)vals, componentType, 0);
   vals = realloc(vals, actual_size);
 
   // Create a tensor index
   vector<ModeIndex> modeIndices;
   for (size_t i = 0; i < order; i++) {
```

### Comparing `tensora-0.0.6/src/taco/src/storage/storage.cpp` & `tensora-0.0.7/src/taco/src/storage/storage.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 #include "taco/type.h"
 #include "taco/format.h"
 #include "taco/error.h"
 #include "taco/storage/index.h"
 #include "taco/storage/array.h"
 #include "taco/util/strings.h"
+#include "taco/index_notation/index_notation.h"
 
 using namespace std;
 
 namespace taco {
 
 // class Storage
 struct TensorStorage::Content {
@@ -22,20 +23,26 @@
   Format        format;
 
   taco_tensor_t *tensorData;
 
   Index         index;
   Array         values;
 
-  Content(Datatype componentType, vector<int> dimensions, Format format)
+  Literal       fillValue;
+
+  Content(Datatype componentType, vector<int> dimensions, Format format, Literal fill)
       : componentType(componentType), dimensions(dimensions), format(format),
         index(format) {
     int order = (int)dimensions.size();
 
+    taco_iassert(fill.getDataType() == componentType) << "Fill value must be of same type as data array";
     taco_iassert(order <= INT_MAX && componentType.getNumBits() <= INT_MAX);
+    taco_uassert(order == format.getOrder()) <<
+        "The number of format mode types (" << format.getOrder() << ") " <<
+        "must match the tensor order (" << dimensions.size() << ").";
     vector<int32_t> dimensionsInt32(order);
     vector<int32_t> modeOrdering(order);
     vector<taco_mode_t> modeTypes(order);
     for (int i=0; i < order; ++i) {
       dimensionsInt32[i] = dimensions[i];
       modeOrdering[i] = format.getModeOrdering()[i];
       auto modeType  = format.getModeFormats()[i];
@@ -46,27 +53,28 @@
       } else if (modeType.getName() == Singleton.getName()) {
         modeTypes[i] = taco_mode_sparse;
       } else {
         taco_not_supported_yet;
       }
     }
 
+    fillValue = fill;
     tensorData = init_taco_tensor_t(order, componentType.getNumBits(),
-                       dimensionsInt32.data(), modeOrdering.data(),
-                       modeTypes.data());
+                                    dimensionsInt32.data(), modeOrdering.data(),
+                                    modeTypes.data(), fill.getValPtr());
   }
 
   ~Content() {
     deinit_taco_tensor_t(tensorData);
   }
 };
 
-TensorStorage::TensorStorage(Datatype componentType,
-                             const vector<int>& dimensions, Format format)
-    : content(new Content(componentType, dimensions, format)) {
+TensorStorage::TensorStorage(Datatype componentType, const vector<int>& dimensions,
+                             Format format, Literal fillVal)
+    : content(new Content(componentType, dimensions, format, fillVal)) {
 }
 
 const Format& TensorStorage::getFormat() const {
   return content->format;
 }
 
 Datatype TensorStorage::getComponentType() const {
@@ -93,14 +101,18 @@
   return content->values;
 }
 
 Array TensorStorage::getValues() {
   return content->values;
 }
 
+Literal TensorStorage::getFillValue() {
+  return content->fillValue;
+}
+
 size_t TensorStorage::getSizeInBytes() {
   size_t indexSizeInBytes = 0;
   const auto& index = getIndex();
   for (int i = 0; i < index.numModeIndices(); i++) {
     const auto& modeIndex = index.getModeIndex(i);
     for (int j = 0; j < modeIndex.numIndexArrays(); j++) {
       const auto& indexArray = modeIndex.getIndexArray(j);
@@ -155,14 +167,15 @@
     }
     else {
       taco_not_supported_yet;
     }
   }
 
   tensorData->vals  = (uint8_t*)getValues().getData();
+  tensorData->fill_value = (uint8_t*) content->fillValue.getValPtr();
 
   return content->tensorData;
 }
 
 void TensorStorage::setIndex(const Index& index) {
   content->index = index;
 }
```

### Comparing `tensora-0.0.6/src/taco/src/storage/typed_index.cpp` & `tensora-0.0.7/src/taco/src/storage/typed_index.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/storage/typed_value.cpp` & `tensora-0.0.7/src/taco/src/storage/typed_value.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ////////// TypedComponent
 
 const Datatype& TypedComponent::getType() const {
   return dType;
 }
 
-size_t TypedComponent::getAsIndex(const ComponentTypeUnion mem) const {
+size_t TypedComponent::getAsIndex(const ComponentTypeUnion &mem) const {
   switch (dType.getKind()) {
     case Datatype::Bool: return (size_t) mem.boolValue;
     case Datatype::UInt8: return (size_t) mem.uint8Value;
     case Datatype::UInt16: return (size_t) mem.uint16Value;
     case Datatype::UInt32: return (size_t) mem.uint32Value;
     case Datatype::UInt64: return (size_t) mem.uint64Value;
     case Datatype::UInt128: return (size_t) mem.uint128Value;
```

### Comparing `tensora-0.0.6/src/taco/src/target.cpp` & `tensora-0.0.7/src/taco/src/target.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/type.cpp` & `tensora-0.0.7/src/taco/src/type.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include "taco/type.h"
 
 #include "taco/error/error_messages.h"
 #include "taco/util/collections.h"
 #include "taco/util/strings.h"
+#include "taco/index_notation/index_notation.h"
 
 #include <ostream>
 #include <set>
 #include <complex>
 
 using namespace std;
 
@@ -213,32 +214,57 @@
       return Datatype(Datatype::Complex128);
   }
 }
   
 Datatype Complex64  = Datatype(Datatype::Complex64);
 Datatype Complex128 = Datatype(Datatype::Complex128);
 
+struct Dimension::Content {
+  size_t size;
+  IndexVar indexVar;
+  bool indexVarDefined;
+};
+
 // class Dimension
-Dimension::Dimension() : size(0) {
+Dimension::Dimension() : content(new Content) {
+  content->size = 0;
+  content->indexVarDefined = false;
 }
 
-Dimension::Dimension(size_t size) : size(size) {
+Dimension::Dimension(size_t size) : content(new Content) {
   taco_iassert(size > 0) << "Cannot create a dimension of size 0";
+  content->size = size;
+  content->indexVarDefined = false;
+}
+
+Dimension::Dimension(IndexVar indexVar) : content(new Content) {
+  content->size = 0;
+  content->indexVarDefined = true;
+  content->indexVar = indexVar;
 }
 
 bool Dimension::isVariable() const {
-  return getSize() == 0;
+  return getSize() == 0 && !content->indexVarDefined;
 }
 
 bool Dimension::isFixed() const {
   return getSize() > 0;
 }
 
 size_t Dimension::getSize() const {
-  return size;
+  return content->size;
+}
+
+bool Dimension::isIndexVarSized() const {
+  return content->indexVarDefined;
+}
+
+IndexVar Dimension::getIndexVarSize() const {
+  taco_iassert(content->indexVarDefined);
+  return content->indexVar;
 }
 
 bool operator==(const Dimension& a, const Dimension& b) {
   if (a.isFixed() != b.isFixed()) return false;
   if (a.isFixed() && b.isFixed() && a.getSize() != b.getSize()) return false;
   return true;
 }
```

### Comparing `tensora-0.0.6/src/taco/src/util/env.cpp` & `tensora-0.0.7/src/taco/src/util/env.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/util/files.cpp` & `tensora-0.0.7/src/taco/src/util/files.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/src/util/name_generator.cpp` & `tensora-0.0.7/src/taco/src/util/name_generator.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,18 @@
   return prefix + to_string(uniqueCount());
 }
 
 string uniqueName(const string& prefix) {
   return prefix + to_string(uniqueCount());
 }
 
+int getUniqueId() {
+  return uniqueCount();
+}
+
 
 // class NameGenerator
 NameGenerator::NameGenerator() {
 }
 
 NameGenerator::NameGenerator(std::vector<std::string> reserved) {
   for (auto& str : reserved) {
```

### Comparing `tensora-0.0.6/src/taco/src/util/strings.cpp` & `tensora-0.0.7/src/taco/src/util/strings.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/data/qcd/theta.ttx` & `tensora-0.0.7/src/taco/test/data/qcd/theta.ttx`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/data/qcd/z.ttx` & `tensora-0.0.7/src/taco/test/data/qcd/z.ttx`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/data/rua_32.mtx` & `tensora-0.0.7/src/taco/test/data/rua_32.mtx`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/data/rua_32.rb` & `tensora-0.0.7/src/taco/test/data/rua_32.rb`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/expr_factory.cpp` & `tensora-0.0.7/src/taco/test/expr_factory.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/expr_factory.h` & `tensora-0.0.7/src/taco/test/expr_factory.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/gtest/LICENSE` & `tensora-0.0.7/src/taco/test/gtest/LICENSE`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/gtest/gtest-all.cc` & `tensora-0.0.7/src/taco/test/gtest/gtest-all.cc`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/gtest/gtest.h` & `tensora-0.0.7/src/taco/test/gtest/gtest.h`

 * *Files 0% similar despite different names*

```diff
@@ -11221,14 +11221,15 @@
 namespace internal {
 
 // Used in the Values() function to provide polymorphic capabilities.
 template <typename T1>
 class ValueArray1 {
  public:
   explicit ValueArray1(T1 v1) : v1_(v1) {}
+  ValueArray1(const ValueArray1& other) = default;
 
   template <typename T>
   operator ParamGenerator<T>() const { return ValuesIn(&v1_, &v1_ + 1); }
 
  private:
   // No implementation - assignment is unsupported.
   void operator=(const ValueArray1& other);
@@ -11236,14 +11237,15 @@
   const T1 v1_;
 };
 
 template <typename T1, typename T2>
 class ValueArray2 {
  public:
   ValueArray2(T1 v1, T2 v2) : v1_(v1), v2_(v2) {}
+  ValueArray2(const ValueArray2& other) = default;
 
   template <typename T>
   operator ParamGenerator<T>() const {
     const T array[] = {static_cast<T>(v1_), static_cast<T>(v2_)};
     return ValuesIn(array);
   }
 
@@ -11255,14 +11257,15 @@
   const T2 v2_;
 };
 
 template <typename T1, typename T2, typename T3>
 class ValueArray3 {
  public:
   ValueArray3(T1 v1, T2 v2, T3 v3) : v1_(v1), v2_(v2), v3_(v3) {}
+  ValueArray3(const ValueArray3& other) = default;
 
   template <typename T>
   operator ParamGenerator<T>() const {
     const T array[] = {static_cast<T>(v1_), static_cast<T>(v2_),
         static_cast<T>(v3_)};
     return ValuesIn(array);
   }
@@ -11277,14 +11280,15 @@
 };
 
 template <typename T1, typename T2, typename T3, typename T4>
 class ValueArray4 {
  public:
   ValueArray4(T1 v1, T2 v2, T3 v3, T4 v4) : v1_(v1), v2_(v2), v3_(v3),
       v4_(v4) {}
+  ValueArray4(const ValueArray4& other) = default;
 
   template <typename T>
   operator ParamGenerator<T>() const {
     const T array[] = {static_cast<T>(v1_), static_cast<T>(v2_),
         static_cast<T>(v3_), static_cast<T>(v4_)};
     return ValuesIn(array);
   }
@@ -11300,14 +11304,15 @@
 };
 
 template <typename T1, typename T2, typename T3, typename T4, typename T5>
 class ValueArray5 {
  public:
   ValueArray5(T1 v1, T2 v2, T3 v3, T4 v4, T5 v5) : v1_(v1), v2_(v2), v3_(v3),
       v4_(v4), v5_(v5) {}
+  ValueArray5(const ValueArray5& other) = default;
 
   template <typename T>
   operator ParamGenerator<T>() const {
     const T array[] = {static_cast<T>(v1_), static_cast<T>(v2_),
         static_cast<T>(v3_), static_cast<T>(v4_), static_cast<T>(v5_)};
     return ValuesIn(array);
   }
@@ -11382,14 +11387,16 @@
     typename T6, typename T7, typename T8>
 class ValueArray8 {
  public:
   ValueArray8(T1 v1, T2 v2, T3 v3, T4 v4, T5 v5, T6 v6, T7 v7,
       T8 v8) : v1_(v1), v2_(v2), v3_(v3), v4_(v4), v5_(v5), v6_(v6), v7_(v7),
       v8_(v8) {}
 
+  ValueArray8(const ValueArray8& other) = default;
+
   template <typename T>
   operator ParamGenerator<T>() const {
     const T array[] = {static_cast<T>(v1_), static_cast<T>(v2_),
         static_cast<T>(v3_), static_cast<T>(v4_), static_cast<T>(v5_),
         static_cast<T>(v6_), static_cast<T>(v7_), static_cast<T>(v8_)};
     return ValuesIn(array);
   }
@@ -11674,14 +11681,16 @@
  public:
   ValueArray16(T1 v1, T2 v2, T3 v3, T4 v4, T5 v5, T6 v6, T7 v7, T8 v8, T9 v9,
       T10 v10, T11 v11, T12 v12, T13 v13, T14 v14, T15 v15, T16 v16) : v1_(v1),
       v2_(v2), v3_(v3), v4_(v4), v5_(v5), v6_(v6), v7_(v7), v8_(v8), v9_(v9),
       v10_(v10), v11_(v11), v12_(v12), v13_(v13), v14_(v14), v15_(v15),
       v16_(v16) {}
 
+  ValueArray16(const ValueArray16& other) = default;
+
   template <typename T>
   operator ParamGenerator<T>() const {
     const T array[] = {static_cast<T>(v1_), static_cast<T>(v2_),
         static_cast<T>(v3_), static_cast<T>(v4_), static_cast<T>(v5_),
         static_cast<T>(v6_), static_cast<T>(v7_), static_cast<T>(v8_),
         static_cast<T>(v9_), static_cast<T>(v10_), static_cast<T>(v11_),
         static_cast<T>(v12_), static_cast<T>(v13_), static_cast<T>(v14_),
```

### Comparing `tensora-0.0.6/src/taco/test/test.cpp` & `tensora-0.0.7/src/taco/test/test.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#include <functional>
+
 #include "test.h"
 #include "taco/tensor.h"
 
 #include "taco/util/strings.h"
 #include "taco/storage/storage.h"
 
 int main(int argc, char **argv) {
@@ -47,8 +49,22 @@
 ostream& operator<<(ostream& os, const NotationTest& test) {
   os << endl;
   os << "Expected: " << test.expected << endl;
   os << "Actual:   " << test.actual << endl;
   return os;
 }
 
+void ASSERT_THROWS_EXCEPTION_WITH_ERROR(std::function<void()> f, std::string err) {
+  EXPECT_THROW({
+    try {
+      f();
+    } catch (TacoException& e) {
+      // Catch and inspect the exception to make sure that err is within it.
+      auto s = std::string(e.what());
+      ASSERT_TRUE(s.find(err) != std::string::npos);
+      // Throw the exception back up to gtest.
+      throw;
+    }
+  }, TacoException);
+}
+
 }}
```

### Comparing `tensora-0.0.6/src/taco/test/test.h` & `tensora-0.0.7/src/taco/test/test.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #ifndef TEST_H
 #define TEST_H
 
 #include "gtest/gtest.h"
 
+#include <functional>
 #include <iostream>
 #include <vector>
 #include <memory>
 
 #include "taco/format.h"
 #include "taco/tensor.h"
 #include "taco/error.h"
@@ -89,14 +90,18 @@
   }
 
   auto nnz = index.getSize();
   ASSERT_EQ(expectedValues.size(), nnz);
   ASSERT_ARRAY_EQ(expectedValues, {(double*)storage.getValues().getData(),nnz});
 }
 
+// ASSERT_THROWS_EXCEPTION_WITH_ERROR asserts that the input function throws
+// a TacoException with the input string err contained within the body.
+void ASSERT_THROWS_EXCEPTION_WITH_ERROR(std::function<void()> f, std::string err);
+
 struct NotationTest {
   NotationTest(IndexStmt actual, IndexStmt expected)
       : actual(actual), expected(expected) {}
   IndexStmt actual;
   IndexStmt expected;
 };
 ostream& operator<<(ostream&, const NotationTest&);
```

### Comparing `tensora-0.0.6/src/taco/test/test_tensors.cpp` & `tensora-0.0.7/src/taco/test/test_tensors.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -133,14 +133,24 @@
   return TensorData<double>({5}, {
     {{0}, 1000},
     {{3}, 2000},
     {{4}, 3000}
   });
 }
 
+TensorData<double> d5e_data() {
+  return TensorData<double>({5}, {
+    {{0}, 1},
+    {{1}, 2},
+    {{2}, 3},
+    {{3}, 4},
+    {{4}, 5}
+  });
+}
+
 TensorData<double> d8a_data() {
   return TensorData<double>({8}, {
     {{0}, 1},
     {{1}, 2},
     {{2}, 3},
     {{5}, 4}
   });
@@ -324,14 +334,31 @@
     {{1,2,0}, 6},
     {{1,2,2}, 7},
     {{2,1,2}, 8},
     {{2,2,1}, 9},
   });
 }
 
+TensorData<double> d355a_data() {
+  return TensorData<double>({3,5,5}, {
+    {{0,0,0}, 1},
+    {{0,1,1}, 2},
+    {{0,2,1}, 3},
+    {{0,3,1}, 4},
+    {{0,4,1}, 5},
+    {{1,0,1}, 6},
+    {{1,1,0}, 7},
+    {{1,2,0}, 8},
+    {{1,4,2}, 9},
+    {{2,1,2}, 10},
+    {{2,2,3}, 11},
+    {{2,4,4}, 12},
+  });
+}
+
 TensorData<double> d32b_data() {
   return TensorData<double>({3,2}, {
     {{0,0}, 10},
     {{0,1}, 11},
     {{1,0}, 20},
     {{1,1}, 21},
     {{2,0}, 30},
@@ -402,14 +429,18 @@
   return d5c_data().makeTensor(name, format);
 }
 
 Tensor<double> d5d(std::string name, Format format) {
   return d5d_data().makeTensor(name, format);
 }
 
+Tensor<double> d5e(std::string name, Format format) {
+  return d5e_data().makeTensor(name, format);
+}
+
 Tensor<double> d8a(std::string name, Format format) {
   return d8a_data().makeTensor(name, format);
 }
 
 Tensor<double> d8b(std::string name, Format format) {
   return d8b_data().makeTensor(name, format);
 }
@@ -482,14 +513,18 @@
   return d233c_data().makeTensor(name, format);
 }
 
 Tensor<double> d333a(std::string name, Format format) {
   return d333a_data().makeTensor(name, format);
 }
 
+Tensor<double> d355a(std::string name, Format format) {
+  return d355a_data().makeTensor(name, format);
+}
+
 Tensor<double> d32b(std::string name, Format format) {
   return d32b_data().makeTensor(name, format);
 }
 
 Tensor<double> d3322a(std::string name, Format format) {
   return d3322a_data().makeTensor(name, format);
 }
```

### Comparing `tensora-0.0.6/src/taco/test/test_tensors.h` & `tensora-0.0.7/src/taco/test/test_tensors.h`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 TensorData<double> d4a_data();
 TensorData<double> d4b_data();
 
 TensorData<double> d5a_data();
 TensorData<double> d5b_data();
 TensorData<double> d5c_data();
 TensorData<double> d5d_data();
+TensorData<double> d5e_data();
 
 TensorData<double> d8a_data();
 TensorData<double> d8b_data();
 TensorData<double> d8c_data();
 
 TensorData<double> dla_data();
 TensorData<double> dlb_data();
@@ -123,14 +124,16 @@
 
 TensorData<double> d233a_data();
 TensorData<double> d233b_data();
 TensorData<double> d233c_data();
 
 TensorData<double> d333a_data();
 
+TensorData<double> d355a_data();
+
 TensorData<double> d32b_data();
 TensorData<double> d3322a_data();
 
 Tensor<double> da(std::string name, Format format);
 Tensor<double> db(std::string name, Format format);
 
 Tensor<double> d1a(std::string name, Format format);
@@ -142,14 +145,15 @@
 Tensor<double> d4a(std::string name, Format format);
 Tensor<double> d4b(std::string name, Format format);
 
 Tensor<double> d5a(std::string name, Format format);
 Tensor<double> d5b(std::string name, Format format);
 Tensor<double> d5c(std::string name, Format format);
 Tensor<double> d5d(std::string name, Format format);
+Tensor<double> d5e(std::string name, Format format);
 
 Tensor<double> d8a(std::string name, Format format);
 Tensor<double> d8b(std::string name, Format format);
 Tensor<double> d8c(std::string name, Format format);
 Tensor<double> d8d(std::string name, Format format);
 
 Tensor<double> dla(std::string name, Format format);
@@ -171,14 +175,16 @@
 
 Tensor<double> d233a(std::string name, Format format);
 Tensor<double> d233b(std::string name, Format format);
 Tensor<double> d233c(std::string name, Format format);
 
 Tensor<double> d333a(std::string name, Format format);
 
+Tensor<double> d355a(std::string name, Format format);
+
 Tensor<double> d32b(std::string name, Format format);
 Tensor<double> d3322a(std::string name, Format format);
 
 Tensor<double> d33a_CSR(std::string name);
 Tensor<double> d33a_CSC(std::string name);
 Tensor<double> d35a_CSR(std::string name);
 Tensor<double> d35a_CSC(std::string name);
```

### Comparing `tensora-0.0.6/src/taco/test/tests-api.cpp` & `tensora-0.0.7/src/taco/test/tests-api.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,16 @@
   ASSERT_ARRAY_EQ(GetParam().getExpectedIndices()[1][1],
                   {(int*)index.getModeIndex(1).getIndexArray(1).getData(),
                    index.getModeIndex(1).getIndexArray(1).getSize()});
 
   ASSERT_ARRAY_EQ(GetParam().getExpectedValues(),
                   {(double*)storage.getValues().getData(),
                    storage.getIndex().getSize()});
+
+  ASSERT_TRUE(equals(tensor.getFillValue(), Literal::zero(tensor.getComponentType())));
 }
 
 TEST_P(apiwrb, api) {
   TensorBase tensor = GetParam().getTensor(CSC);
 
   auto storage = tensor.getStorage();
   if (tensor.getFormat() == taco::CSC) {
```

### Comparing `tensora-0.0.6/src/taco/test/tests-copyprop.cpp` & `tensora-0.0.7/src/taco/test/tests-copyprop.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/tests-error.cpp` & `tensora-0.0.7/src/taco/test/tests-error.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -7,35 +7,42 @@
 using namespace taco;
 
 const IndexVar i("i"), j("j"), k("k");
 
 TEST(error, expr_dimension_mismatch_freevar) {
   Tensor<double> a({3}, Format({Sparse}, {0}));
   Tensor<double> b({5}, Format({Sparse}, {0}));
-  ASSERT_DEATH(a(i) = b(i), error::expr_dimension_mismatch);
+  ASSERT_THROW(a(i) = b(i), taco::TacoException);
 }
 
 TEST(error, expr_dimension_mismatch_sumvar) {
   Tensor<double> a({5}, Format({Sparse}, {0}));
   Tensor<double> B({5,4}, Format({Sparse,Sparse}, {0,1}));
   Tensor<double> c({3}, Format({Sparse}, {0}));
-  ASSERT_DEATH(a(i) = B(i,j)*c(j), error::expr_dimension_mismatch);
+  ASSERT_THROW(a(i) = B(i,j)*c(j), taco::TacoException);
 }
 
 TEST(error, compile_without_expr) {
   Tensor<double> a({5}, Sparse);
-  ASSERT_DEATH(a.compile(), error::compile_without_expr);
+  ASSERT_THROW(a.compile(), taco::TacoException);
+}
+
+TEST(error, compile_tensor_name_collision) {
+  Tensor<double> a("a", {5}, Sparse);
+  Tensor<double> b("a", {5}, Sparse); // name should be "b"
+  a(i) = b(i);
+  ASSERT_THROW(a.compile(), taco::TacoException);
 }
 
 TEST(error, assemble_without_compile) {
   Tensor<double> a({5}, Sparse);
   Tensor<double> b({5}, Sparse);
   a(i) = b(i);
-  ASSERT_DEATH(a.assemble(), error::assemble_without_compile);
+  ASSERT_THROW(a.assemble(), taco::TacoException);
 }
 
 TEST(error, compute_without_compile) {
   Tensor<double> a({5}, Sparse);
   Tensor<double> b({5}, Sparse);
   a(i) = b(i);
-  ASSERT_DEATH(a.compute(), error::compute_without_compile);
+  ASSERT_THROW(a.compute(), taco::TacoException);
 }
```

### Comparing `tensora-0.0.6/src/taco/test/tests-expr.cpp` & `tensora-0.0.7/src/taco/test/tests-expr.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -156,7 +156,49 @@
   a.evaluate();
   ASSERT_EQ(a.begin()->second, 40.0);
 
   a = 42.0;
   a.evaluate();
   ASSERT_EQ(a.begin()->second, 42.0);
 }
+
+TEST(expr, indexVarSimple) {
+  Tensor<int> a("actual", {3,3}, Dense);
+  a(i, j) = i + j;
+  a.evaluate();
+
+  Tensor<int> expected("expected", a.getDimensions(), Dense);
+
+  for(int i = 0; i < a.getDimensions()[0]; ++i) {
+    for(int j = 0; j < a.getDimensions()[1]; ++j) {
+      expected.insert({i, j}, i+j);
+    }
+  }
+  expected.pack();
+
+  ASSERT_TENSOR_EQ(expected, a);
+}
+
+TEST(expr, indexVarMix) {
+  Tensor<int> a("actual", {3, 3}, dense);
+  Tensor<int> b("input", {3, 3}, compressed);
+
+  Tensor<int> expected("expected", a.getDimensions(), Dense);
+  const int n = a.getDimensions()[0];
+  const int m = a.getDimensions()[1];
+
+  for(int i = 0; i < n; ++i) {
+    b.insert({i, i}, 2);
+  }
+  b.pack();
+
+  a(i, j) = b(i, j) * (i * m + j);
+  a.evaluate();
+
+  for(int i = 0; i < n; ++i) {
+    int flattened_idx = i * m + i;
+    expected.insert({i, i}, 2 * flattened_idx);
+  }
+  expected.pack();
+
+  ASSERT_TENSOR_EQ(expected, a);
+}
```

### Comparing `tensora-0.0.6/src/taco/test/tests-expr_storage.cpp` & `tensora-0.0.7/src/taco/test/tests-expr_storage.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,21 @@
 
 struct expr : public TestWithParam<TestData> {};
 
 TEST_P(expr, storage) {
   Tensor<double> tensor = GetParam().tensor;
   packOperands(tensor);
 
+  taco_set_num_threads(2);
+
   tensor.compile();
   tensor.assemble();
   tensor.compute();
+  
+  taco_set_num_threads(1);
 
   SCOPED_TRACE(toString(tensor.getAssignment()));
 
   auto& expectedIndices = GetParam().expectedIndices;
   auto& expectedValues = GetParam().expectedValues;
   ASSERT_COMPONENTS_EQUALS(expectedIndices, expectedValues, tensor);
 }
@@ -949,14 +953,33 @@
                       }
                     },
                     {88.2, 96.4, 0.0, 0.0, 319.4, 335.8}
                     )
            )
 );
 
+Format ell({Dense, Dense, Singleton({ModeFormat::UNIQUE, ModeFormat::PADDED})});
+
+INSTANTIATE_TEST_CASE_P(espmv, expr,
+    Values(
+           TestData(Tensor<double>("a",{5},Format({Dense})),
+                    {i},
+                    d355a("B", ell)(j,i,k) *
+                    d5e("c",Format({Dense}))(k),
+                    {
+                      {
+                        // Dense index
+                        {5}
+                      },
+                    },
+                    {13,41,58,8,97}
+                    )
+           )
+);
+
 INSTANTIATE_TEST_CASE_P(matrix_sum, expr,
     Values(
            TestData(Tensor<double>("a",{},Format()),
                     {},
                     d33a("B",Format({Dense, Dense}))(k,l),
                     {},
                     {9.0}
```

### Comparing `tensora-0.0.6/src/taco/test/tests-format.cpp` & `tensora-0.0.7/src/taco/test/tests-format.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/tests-index.cpp` & `tensora-0.0.7/src/taco/test/tests-index.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/tests-indexexpr.cpp` & `tensora-0.0.7/src/taco/test/tests-indexexpr.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -69,7 +69,16 @@
   IndexExpr expr = b(i) / 2;
   ASSERT_TRUE(isa<Div>(expr));
   ASSERT_TRUE(isa<DivNode>(expr.ptr));
   Div div = to<Div>(expr);
   ASSERT_TRUE(equals(div.getA(), b(i)));
   ASSERT_TRUE(equals(div.getB(), Literal(2)));
 }
+
+TEST(indexexpr, indexvar) {
+  IndexExpr expr = i;
+  ASSERT_TRUE(isa<IndexVar>(expr));
+  ASSERT_TRUE(isa<IndexVarNode>(expr.ptr));
+  IndexVar var = to<IndexVar>(expr);
+  ASSERT_EQ(type<int>(), var.getDataType());
+  ASSERT_EQ("i", var.getName());
+}
```

### Comparing `tensora-0.0.6/src/taco/test/tests-indexstmt.cpp` & `tensora-0.0.7/src/taco/test/tests-indexstmt.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/tests-io.cpp` & `tensora-0.0.7/src/taco/test/tests-io.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/tests-lower.cpp` & `tensora-0.0.7/src/taco/test/tests-lower.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 #include <cmath>
 
 #include "taco/lower/lower.h"
 #include "taco/ir/ir.h"
 #include "taco/index_notation/index_notation.h"
 #include "taco/index_notation/index_notation_rewriter.h"
 #include "taco/index_notation/index_notation_nodes.h"
+#include "taco/index_notation/tensor_operator.h"
 #include "taco/index_notation/kernel.h"
 #include "taco/codegen/module.h"
 #include "taco/storage/storage.h"
 #include "taco/storage/pack.h"
 #include "taco/lower/lower.h"
 #include "taco/format.h"
 #include "taco/util/strings.h"
 
+#include "op_factory.h"
+
 namespace taco {
 namespace test {
 
 static const Dimension n;
 static const Type vectype(Float64, {n});
 static const Type mattype(Float64, {n,n});
 static const Type tentype(Float64, {n,n,n});
@@ -35,14 +38,21 @@
 static TensorVar tj("tj", Float64);
 
 static TensorVar a("a", vectype, Format());
 static TensorVar b("b", vectype, Format());
 static TensorVar c("c", vectype, Format());
 static TensorVar d("d", vectype, Format());
 
+static const Type intvectype(Int32, {n});
+static TensorVar ai("ai", intvectype, Format());
+static TensorVar bi("bi", intvectype, Format());
+static TensorVar ci("ci", intvectype, Format());
+
+static TensorVar fill_10("fillA", vectype, Format(), Literal((double) 10));
+
 static TensorVar w("w", vectype, dense);
 
 static TensorVar A("A", mattype, Format());
 static TensorVar B("B", mattype, Format());
 static TensorVar C("C", mattype, Format());
 static TensorVar D("D", mattype, Format());
 
@@ -76,15 +86,15 @@
       }
     }
     return dims;
   }
 
   TensorStorage getResult(TensorVar var, Format format) const {
     auto dimensions = getDimensions(var);
-    TensorStorage storage(type<double>(), dimensions, format);
+    TensorStorage storage(type<double>(), dimensions, format, var.getFill());
 
     // TODO: Get rid of this and lower to use dimensions instead
     vector<taco::ModeIndex> modeIndices(format.getOrder());
     for (int i = 0; i < format.getOrder(); ++i) {
       if (format.getModeFormats()[i] == dense) {
         const size_t idx = format.getModeOrdering()[i];
         modeIndices[i] = taco::ModeIndex({taco::makeArray({dimensions[idx]})});
@@ -93,49 +103,51 @@
     storage.setIndex(taco::Index(format, modeIndices));
 
     return storage;
   }
 
   static
   TensorStorage pack(Format format, const vector<int>& dims,
-                     const vector<pair<vector<int>,double>>& components){
+                     const vector<pair<vector<int>,double>>& components,
+                     Literal fill){
     size_t order = dims.size();
     size_t num = components.size();
     if (order == 0) {
-      TensorStorage storage = TensorStorage(type<double>(), {}, format);
+      TensorStorage storage = TensorStorage(type<double>(), {}, format, fill);
       Array array = makeArray(type<double>(), 1);
       *((double*)array.getData()) = components[0].second;
       storage.setValues(array);
       return storage;
     }
     else {
       vector<TypedIndexVector> coords;
       for (size_t i=0; i < order; ++i) {
         coords.push_back(TypedIndexVector(type<int>(), num));
       }
       vector<double> values(num);
       for (size_t i=0; i < components.size(); ++i) {
         auto& coordinates = components[i].first;
+        std::vector<int> ordering = format.getModeOrdering();
         for (size_t j=0; j < coordinates.size(); ++j) {
           coords[j][i] = coordinates[j];
         }
         values[i] = components[i].second;
       }
-      return taco::pack(type<double>(), dims, format, coords, values.data());
+      return taco::pack(type<double>(), dims, format, coords, values.data(), fill);
     }
   }
 
   TensorStorage getArgument(TensorVar var, Format format) const {
     taco_iassert(contains(inputs, var)) << var;
-    return pack(format, getDimensions(var), inputs.at(var));
+    return pack(format, getDimensions(var), inputs.at(var), var.getFill());
   }
 
   TensorStorage getExpected(TensorVar var, Format format) const {
     taco_iassert(contains(expected, var)) << var;
-    return pack(format, getDimensions(var), expected.at(var));
+    return pack(format, getDimensions(var), expected.at(var), var.getFill());
   }
 };
 
 std::ostream& operator<<(std::ostream& os, const TestCase& testcase) {
   os << endl << " Inputs:";
   for (auto& input : testcase.inputs) {
     os << endl << "  " << input.first.getName() << ":";
@@ -195,15 +207,15 @@
     if (contains(formats, var)) {
       format = formats.at(var);
     }
     else {
       // Default format is dense in all dimensions
       format = Format(vector<ModeFormatPack>(var.getOrder(), dense));
     }
-    formatted.insert({var, TensorVar(var.getName(), var.getType(), format)});
+    formatted.insert({var, TensorVar(var.getName(), var.getType(), format, var.getFill())});
   }
   return formatted;
 }
 
 static void verifyResults(const vector<TensorVar>& results,
                           const vector<TensorStorage>& arguments,
                           const map<TensorVar,TensorVar>& varsFormatted,
@@ -217,14 +229,32 @@
     Tensor<double> expected(expectedStorage.getDimensions(), format);
     actual.setStorage(actualStorage);
     expected.setStorage(expectedStorage);
     ASSERT_TENSOR_EQ(expected, actual);
   }
 }
 
+static void verifyResultsInt(const vector<TensorVar>& results,
+                          const vector<TensorStorage>& arguments,
+                          const map<TensorVar,TensorVar>& varsFormatted,
+                          const map<TensorVar, TensorStorage>& expected) {
+  for (size_t i = 0; i < results.size(); i++) {
+    TensorVar result = results[i];
+    TensorStorage actualStorage = arguments[i];
+    TensorStorage expectedStorage = expected.at(result);
+    Format format = varsFormatted.at(result).getFormat();
+    Tensor<int> actual(actualStorage.getDimensions(), format);
+    Tensor<int> expected(expectedStorage.getDimensions(), format);
+    actual.setStorage(actualStorage);
+    expected.setStorage(expectedStorage);
+    ASSERT_TENSOR_EQ(expected, actual);
+  }
+}
+
+
 TEST_P(lower, compile) {
   map<TensorVar,TensorVar> varsFormatted =
       formatVars(getTensorVars(get<0>(GetParam()).stmt),
                  get<1>(GetParam()).formats);
 
   IndexStmt stmt = replace(get<0>(GetParam()).stmt, varsFormatted);
   ASSERT_TRUE(isLowerable(stmt)) << stmt;
@@ -255,21 +285,27 @@
       expected.insert({result, testCase.getExpected(result, format)});
     }
 
     {
       SCOPED_TRACE("Separate Assembly and Compute\n");
       ASSERT_TRUE(kernel.assemble(arguments));
       ASSERT_TRUE(kernel.compute(arguments));
-      verifyResults(results, arguments, varsFormatted, expected);
+      if (results[0].getType().getDataType().isInt())
+        verifyResultsInt(results, arguments, varsFormatted, expected);
+      else
+        verifyResults(results, arguments, varsFormatted, expected);
     }
 
     {
       SCOPED_TRACE("Fused Assembly and Compute\n");
       ASSERT_TRUE(kernel(arguments));
-      verifyResults(results, arguments, varsFormatted, expected);
+      if (results[0].getType().getDataType().isInt())
+        verifyResultsInt(results, arguments, varsFormatted, expected);
+      else
+        verifyResults(results, arguments, varsFormatted, expected);
     }
   }
 }
 
 #define TEST_STMT(name, statement, formats, testcases) \
 INSTANTIATE_TEST_CASE_P(name, lower,                   \
 Combine(Values(Test(statement, testcases)), formats));
@@ -693,24 +729,24 @@
   {
     TestCase({{B, {{{0,0}, 42.0}, {{0,2}, 2.0}, {{1,1}, 3.0}, {{3,3}, 4.0}}},
               {c, {{{2}, 1.0}, {{3}, 2.0}}}},
              {{a, {{{0}, 2.0}, {{3}, 8.0}}}})
   }
 )
 
-TEST_STMT(DISABLED_where_spmm,
+TEST_STMT(where_spmm,
   forall(i,
          where(forall(j,
                       A(i,j) = w(j)),
                forall(k,
                       forall(j,
                              w(j) += B(i,k) * C(k,j))))),
   Values(
-//         Formats({{A,Format({dense,dense})},
-//                  {B,Format({dense,dense})}, {C,Format({dense,dense})}}),
+         Formats({{A,Format({dense,dense})},
+                  {B,Format({dense,dense})}, {C,Format({dense,dense})}}),
          Formats({{A,Format({dense,sparse})},
                   {B,Format({dense,sparse})}, {C,Format({dense,sparse})}})
          ),
   {
     TestCase({{B, { {{0,1}, 2.0}, {{2,0},  3.0}, {{2,2}, 4.0}} },
               {C, { {{0,0},10.0}, {{0,1}, 20.0}, {{2,1},30.0}} }},
              {{A, { {{2,0},30.0}, {{2,1},180.0} }}})
@@ -1552,8 +1588,269 @@
          ),
   {
     TestCase({{b, {{{0}, 1.0}, {{2}, 0.0}, {{4}, 1.0}}}},
              {{a, {{{1}, 1.0}, {{2}, 1.0}, {{3}, 1.0}}}})
   }
 )
 
+//TEST_STMT(vector_add_fill,
+//          forall(i,
+//                 fill_10(i) = b(i) * c(i)
+//          ),
+//          Values(
+//                  Formats({{fill_10, dense}, {b,sparse}, {c, sparse}}),
+//                  Formats({{fill_10, sparse}, {b,sparse}, {c, sparse}})
+//          ),
+//          {
+//            TestCase(
+//                    {{b, {{{0}, 2.0}}},
+//                     {c, {{{0}, 3.0}, {{1}, 6.0}}}},
+//
+//                    {{fill_10, {{{0}, 5.0}, {{1}, 6.0}}}})
+//          }
+//)
+
+// Test tensorOps
+
+Func testOp("testOp", MulAdd(), BC_BD_CD());
+
+TEST_STMT(testOp1,
+          forall(i,
+                 a(i) = testOp(b(i), c(i), d(i))
+          ),
+          Values(
+                  Formats({{a,sparse}, {b,sparse}, {c,sparse}, {d, sparse}}),
+                  Formats({{a,dense}, {b,dense}, {c,dense}, {d, dense}}),
+                  Formats({{a,dense}, {b,sparse}, {c,dense}, {d, sparse}}),
+                  Formats({{a,dense}, {b,sparse}, {c,dense}, {d, dense}}),
+                  Formats({{a,dense}, {b,sparse}, {c,sparse}, {d, sparse}})
+          ),
+          {
+            TestCase(
+                     {{b, {{{0}, 2.0}, {{1}, 2.0}, {{4}, 4.0}}},
+                      {c, {{{0}, 3.0}, {{2}, 3.0}, {{4}, 6.0}}},
+                      {d, {{{1}, 1.0}, {{2}, 4.0}, {{4}, 5.0}}}},
+
+                     {{a, {{{0}, 6.0}, {{1}, 1.0}, {{2}, 4.0}}}})
+          }
+)
+
+
+Func specialOp("specialOp", GeneralAdd(), BC_BD_CD(), {{{0, 1}, MulRegionDef()}, {{0, 2}, SubRegionDef()}});
+TEST_STMT(lowerSpecialRegions1,
+          forall(i,
+                     forall(j,
+                       A(i, j) = specialOp(B(i, j), C(i, j), D(i, j))
+          )),
+          Values(
+                  Formats({{A, Format({dense,dense})}, {B, Format({dense,dense})}, {C, Format({dense,dense})},
+                           {D, Format({dense,dense})}}),
+                  Formats({{A, Format({dense,sparse})}, {B, Format({dense,sparse})}, {C, Format({dense,sparse})},
+                           {D, Format({dense,sparse})}}),
+                  Formats({{A, Format({sparse,sparse})}, {B, Format({sparse,sparse})}, {C, Format({sparse,sparse})},
+                           {D, Format({sparse,sparse})}})
+          ),
+          {
+            TestCase(
+            {{B, {{{0, 1}, 2.0}, {{1, 1}, 3.0}, {{1, 2}, 2.0}, {{4, 3}, 4.0}}},
+              {C, {{{0, 1}, 3.0}, {{2, 1}, 3.0}, {{2, 2}, 4.0}, {{4, 3}, 6.0}}},
+              {D, {{{1, 2}, 1.0}, {{2, 1}, 4.0}, {{3, 3}, 5.0}, {{4, 3}, 5.0}}}},
+
+            {{A, {{{0, 1}, 6.0}, {{1, 2}, -1.0}, {{2, 1}, 7.0}}}})
+          }
+)
+
+Func compUnion("compUnion", GeneralAdd(), ComplementUnion());
+TEST_STMT(lowerCompUnion,
+          forall(i,
+                 forall(j,
+                        A(i, j) = compUnion(B(i, j), C(i, j), D(i, j))
+                 )),
+          Values(
+                  Formats({{A, Format({dense,dense})}, {B, Format({dense,dense})}, {C, Format({dense,dense})},
+                           {D, Format({dense,dense})}}),
+                  Formats({{A, Format({dense,sparse})}, {B, Format({dense,sparse})}, {C, Format({dense,sparse})},
+                           {D, Format({dense,sparse})}}),
+                  Formats({{A, Format({sparse,sparse})}, {B, Format({sparse,sparse})}, {C, Format({sparse,sparse})},
+                           {D, Format({sparse,sparse})}})
+          ),
+          {
+            TestCase(
+            {{B, {{{0, 1}, 2.0}, {{1, 1}, 3.0}, {{1, 2}, 2.0}, {{4, 3}, 4.0}}},
+              {C, {{{0, 1}, 3.0}, {{2, 1}, 3.0}, {{2, 2}, 4.0}, {{4, 3}, 6.0}}},
+              {D, {{{1, 2}, 1.0}, {{2, 1}, 4.0}, {{3, 3}, 5.0}, {{4, 3}, 5.0}}}},
+
+            {{A, {{{0, 1}, 5.0}, {{1, 2}, 3.0}, {{2, 1}, 7.0},
+                  {{2, 2}, 4.0}, {{3, 3}, 5.0}, {{4, 3}, 15.0}}}})
+          }
+)
+
+Func scOr("Or", OrImpl(), {Annihilator((double)1), Identity(Literal((double)0))});
+Func scAnd("And", AndImpl(), {Annihilator((double)0), Identity((double)1)});
+Func bfsMaskOp("bfsMask", BfsLower(), BfsMaskAlg());
+
+TEST_STMT(BoolRing,
+          forall(i,
+                 forall(j,
+                        Assignment(a(i), bfsMaskOp(scAnd(B(i, j), c(j)), c(i)), scOr())
+                 )),
+          Values(
+                  Formats({{a, Format({dense})}, {B, Format({dense,sparse})}, {c, Format({dense})}})
+          ),
+          {
+            TestCase(
+            {{B, {{{0, 1}, 1.0}, {{1, 1}, 1.0}, {{1, 2}, 1.0}, {{3, 1}, 1.0}, {{4, 3}, 1.0}}},
+              {c, {{{1}, 1.0}}}},
+
+            {{a, {{{0}, 1.0}, {{3}, 1.0}}}})
+          }
+)
+
+TEST_STMT(BoolRing2,
+          forall(j,
+                 forall(i,
+                        Assignment(a(i), bfsMaskOp(scAnd(B(i, j), c(j)), c(i)), scOr())
+                 )),
+          Values(
+                  Formats({{a, Format({dense})}, {B, Format({dense,sparse}, {1, 0})}, {c, Format({sparse})}})
+          ),
+          {
+            TestCase(
+            {{B, {{{1, 0}, 1.0}, {{1, 1}, 1.0}, {{1, 3}, 1.0}, {{2, 1}, 1.0}, {{3, 4}, 1.0}}},
+              {c, {{{1}, 1.0}}}},
+
+            {{a, {{{0}, 1.0}, {{3}, 1.0}}}})
+          }
+)
+
+TEST_STMT(BoolRing3,
+          forall(j,
+                 forall(i,
+                        Assignment(a(i), scAnd(B(i, j), c(j)), scOr())
+                 )),
+          Values(
+                  Formats({{a, Format({dense})}, {B, Format({dense,sparse}, {1, 0})}, {c, Format({sparse})}})
+          ),
+          {
+            TestCase(
+            {{B, {{{1, 0}, 1.0}, {{1, 1}, 1.0}, {{1, 3}, 1.0}, {{2, 1}, 1.0}, {{3, 4}, 1.0}}},
+              {c, {{{1}, 1.0}}}},
+
+            {{a, {{{0}, 1.0}, {{1}, 1.0}, {{3}, 1.0}}}})
+          }
+)
+
+Func customMin("Min", MinImpl(), {Identity(std::numeric_limits<double>::infinity()) });
+Func Plus("Plus", GeneralAdd(), {Annihilator(std::numeric_limits<double>::infinity())});
+
+static TensorVar a_inf("a", vectype, Format(), std::numeric_limits<double>::infinity());
+static TensorVar c_inf("c", vectype, Format(), std::numeric_limits<double>::infinity());
+static TensorVar B_inf("B", mattype, Format(), std::numeric_limits<double>::infinity());
+
+TEST_STMT(MinPlusRing,
+          forall(i,
+                 forall(j,
+                        Assignment(a_inf(i), Plus(B_inf(i, j), c_inf(j)), customMin())
+                 )),
+          Values(
+                  Formats({{a_inf, Format({dense})}, {B_inf, Format({dense,sparse})}, {c_inf, Format({dense})}})
+          ),
+          {
+            TestCase(
+            {{B_inf, {{{0, 1}, 3.0}, {{1, 1}, 4.0}, {{1, 2}, 2.0}, {{3,2}, 5.0}, {{4, 3}, 1.0}}},
+              {c_inf, {{{1}, 1.0}, {{2}, 6.0}}}},
+
+            {{a_inf, {{{0}, 4.0}, {{1}, 5.0}, {{3}, 11.0}}}})
+          }
+)
+
+Func sparsify("sparsify", identityFunc(), [](const std::vector<IndexExpr>& v) {return Union(v[0], Complement(v[1]));});
+
+TEST_STMT(SparsifyTest,
+          forall(i,
+                        a(i) = sparsify(b(i), i)
+                 ),
+          Values(
+                  Formats({{a, Format({sparse})}, {b, Format({dense})} })
+          ),
+          {
+            TestCase(
+            {{b, {{{0}, 3.0}, {{2}, 4.0}, {{4}, 2.0}}}},
+
+            {{a, {{{0}, 3.0}, {{2}, 4.0}, {{4}, 2.0}}}})
+          }
+)
+
+Func xorOp("xor", GeneralAdd(), xorGen());
+
+TEST_STMT(XorTest,
+          forall(i,
+                 c(i) = xorOp(a(i), b(i))
+          ),
+          Values(
+                  Formats({{a, Format({sparse})}, {b, Format({sparse})}, {c, Format({sparse})} })
+          ),
+          {
+            TestCase(
+            {{a, {{{0}, 3.0}, {{2}, 4.0}, {{4}, 2.0}}},
+             {b, {{{1}, 5.0}, {{2}, 4.0}, {{4}, 2.0}}}},
+
+            {{c, {{{0}, 3.0}, {{1}, 5.0}}}})
+          }
+)
+
+struct RightShift{
+  ir::Expr operator()(const std::vector<ir::Expr> &v) {
+    if (v.size() == 1)
+      return v[0];
+
+    ir::Expr shift = ir::BinOp::make(v[0], v[1], " >> ");
+    for (size_t idx = 2; idx < v.size(); ++idx) {
+      shift = ir::BinOp::make(shift, v[idx], " >> ");
+    }
+    return shift;
+  }
+};
+
+struct rightShiftAlgebra {
+  IterationAlgebra operator()(const std::vector<IndexExpr>& regions) {
+    IterationAlgebra un = Union(regions[0], regions[1]);
+    return Intersect(un, regions[0]);
+  }
+};
+
+Func rightShiftOp("rightShift", RightShift(), rightShiftAlgebra());
+
+TEST_STMT(DISABLED_RightShiftTest,
+          forall(i,
+                 ci(i) = rightShiftOp(ai(i), bi(i))
+          ),
+          Values(
+            Formats({{ai, Format({sparse})}, {bi, Format({sparse})}, {ci, Format({sparse})} })
+          ),
+          {
+            TestCase(
+            {{ai, {{{0}, 3}, {{2}, 40}, {{4}, 2}}},
+              {bi, {{{1}, 5}, {{2}, 4}, {{4}, 2}}}},
+
+            {{ci, {{{0}, 3}, {{2}, 44}, {{4}, 4}}}})
+          }
+)
+
+TEST_STMT(XorTestOrder2,
+          forall(i, forall(j,
+                                     C(i, j) = xorOp(A(i, j), B(i, j)))
+          ),
+          Values(
+            Formats({{A, Format({sparse, sparse})}, {B, Format({sparse, sparse})}, {C, Format({sparse, sparse})} })
+          ),
+          {
+            TestCase(
+            {{B, {{{0, 1}, 2.0}, {{1, 1}, 3.0}, {{1, 2}, 2.0}, {{4, 3}, 4.0}}},
+              {A, {{{0, 1}, 3.0}, {{1, 3}, 5.0}, {{2, 1}, 3.0}, {{2, 2}, 4.0}, {{4, 3}, 6.0}}}},
+
+            {{C, {{{1, 1}, 3.0}, {{1, 2}, 2.0}, {{1, 3}, 5.0}, {{2, 1}, 3.0},
+                  {{2, 2}, 4.0}}}})
+          }
+)
+
 }}
```

### Comparing `tensora-0.0.6/src/taco/test/tests-parafac.cpp` & `tensora-0.0.7/src/taco/test/tests-parafac.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/tests-qcd.cpp` & `tensora-0.0.7/src/taco/test/tests-qcd.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -30,29 +30,35 @@
   Tensor<double> tau("tau");
   Tensor<double> z = read(qcdTestData("z.ttx"), Dense);
   Tensor<double> theta = read(qcdTestData("theta.ttx"), Dense);
 
   tau = z(i) * z(j) * theta(i,j) * theta(i,j);
 
   tau.evaluate();
+  // Using -O0 to compile the generated kernel yields a slightly different
+  // answer than using -O3.
+#ifdef TACO_DEBUG
+  ASSERT_DOUBLE_EQ(0.41212798763234648, getScalarValue(tau));
+#else
   ASSERT_DOUBLE_EQ(0.41212798763234737, getScalarValue(tau));
+#endif
 }
 
 TEST(qcd, mul2) {
   Tensor<double> tau("tau");
   Tensor<double> z = read(qcdTestData("z.ttx"), Dense);
   Tensor<double> theta = read(qcdTestData("theta.ttx"), Dense);
 
   tau = z(i) * z(j) * theta(i,j) * theta(i,j) * theta(i,j);
 
   tau.evaluate();
   ASSERT_DOUBLE_EQ(0.4120590379120669, getScalarValue(tau));
 }
 
-TEST(qcd, mul3) {
+TEST(DISABLED_qcd, mul3) {
   Tensor<double> tau("tau");
   Tensor<double> z = read(qcdTestData("z.ttx"), Dense);
   Tensor<double> theta = read(qcdTestData("theta.ttx"), Dense);
 
   tau = z(i) * z(j) * z(k) * theta(i,j) * theta(i,k);
 
   tau.evaluate();
```

### Comparing `tensora-0.0.6/src/taco/test/tests-storage.cpp` & `tensora-0.0.7/src/taco/test/tests-storage.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/tests-storage_alloc.cpp` & `tensora-0.0.7/src/taco/test/tests-storage_alloc.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,26 @@
 
 struct alloc : public TestWithParam<TestData> {};
 
 TEST_P(alloc, storage) {
   Tensor<double> tensor = GetParam().tensor;
   packOperands(tensor);
 
-  tensor.compile(GetParam().assembleWhileCompute);
+  tensor.setAssembleWhileCompute(GetParam().assembleWhileCompute);
+  tensor.compile();
   tensor.assemble();
   tensor.compute();
 
   auto& expectedIndices = GetParam().expectedIndices;
   auto& expectedValues = GetParam().expectedValues;
   ASSERT_COMPONENTS_EQUALS(expectedIndices, expectedValues, tensor);
 }
 
 IndexVar i("i"), j("j"), m("m"), n("n"), k("k"), l("l");
-ModeFormat SparseSmall(std::make_shared<CompressedModeFormat>(false, true, true, 
+ModeFormat SparseSmall(std::make_shared<CompressedModeFormat>(false, true, true, false,
                                                           32));
 
 IndexArray dlab_indices() {
   IndexArray indices;
   for (int i = 0; i < 10000; ++i) {
     if (i % 2 == 0 || i % 3 == 0) {
       indices.push_back(i);
```

### Comparing `tensora-0.0.6/src/taco/test/tests-tensor_types.cpp` & `tensora-0.0.7/src/taco/test/tests-tensor_types.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/taco/test/tests-transformation.cpp` & `tensora-0.0.7/src/taco/test/tests-transformation.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -175,16 +175,39 @@
                                                S(i,j,k) = T(i,j,k)
                                                ))),
                           forall(j,
                                  forall(i,
                                         forall(k,
                                                S(i,j,k) = T(i,j,k)
                                                )))
-                          )
-         )
+                          ),
+         TransformationTest(Reorder({j, i, k}),
+                            forall(i,
+                                   forall(j,
+                                          forall(k,
+                                                 S(i,j,k) = T(i,j,k)
+                                          ))),
+                            forall(j,
+                                   forall(i,
+                                          forall(k,
+                                                 S(i,j,k) = T(i,j,k)
+                                          )))
+         ),
+         TransformationTest(Reorder({k, j, i}),
+                            forall(i,
+                                   forall(j,
+                                          forall(k,
+                                                 S(i,j,k) = T(i,j,k)
+                                          ))),
+                            forall(k,
+                                   forall(j,
+                                          forall(i,
+                                                 S(i,j,k) = T(i,j,k)
+                                          )))
+         ))
 );
 
 static Assignment elmul = (a(i) = b(i) * c(i));
 
 INSTANTIATE_TEST_CASE_P(precompute, apply,
   Values(
          TransformationTest(Precompute(elmul.getRhs(), i, iw, w),
@@ -196,44 +219,39 @@
                             )
   )
 );
 
 INSTANTIATE_TEST_CASE_P(parallelize, precondition, Values(
   PreconditionTest(Parallelize(i),
                    forall(i, a(i) = b(i))),
-
   PreconditionTest(Parallelize(i),
                    forall(i, w(i) = a(i) + b(i)) ),
-
   PreconditionTest(Parallelize(i),
                    forall(i, forall(j, W(i, j) = D(i, j) * E(i, j)))),
   PreconditionTest(Parallelize(i),
                    forall(i, forall(j, A(i, j) = W(i, j)))),
   PreconditionTest(Parallelize(i),
-                   forall(i, forall(j, E(i, j) = W(i, j)))))
-
-  /*, TODO: add precondition when lowering supports reductions
-   PreconditionTest(Parallelize(j),
-   forall(i, forall(j, w(j) = W(i, j)))
-   )*/
+                   forall(i, forall(j, E(i, j) = W(i, j)))),
+  PreconditionTest(Parallelize(i),
+                   forall(i, forall(j, w(j) = W(i, j)))))
 );
 
 INSTANTIATE_TEST_CASE_P(parallelize, apply,
                         Values(
                                 TransformationTest(Parallelize(i),
                                                    forall(i, w(i) = b(i)),
-                                                   forall(i, w(i) = b(i), {Forall::PARALLELIZE})
+                                                   forall(i, w(i) = b(i), MergeStrategy::TwoFinger, ParallelUnit::DefaultUnit, OutputRaceStrategy::NoRaces)
                                 ),
                                 TransformationTest(Parallelize(i),
                                                    forall(i, forall(j, W(i,j) = A(i,j))),
-                                                   forall(i, forall(j, W(i,j) = A(i,j)), {Forall::PARALLELIZE})
+                                                   forall(i, forall(j, W(i,j) = A(i,j)), MergeStrategy::TwoFinger, ParallelUnit::DefaultUnit, OutputRaceStrategy::NoRaces)
                                 ),
                                 TransformationTest(Parallelize(j),
                                                    forall(i, forall(j, W(i,j) = A(i,j))),
-                                                   forall(i, forall(j, W(i,j) = A(i,j), {Forall::PARALLELIZE}))
+                                                   forall(i, forall(j, W(i,j) = A(i,j), MergeStrategy::TwoFinger, ParallelUnit::DefaultUnit, OutputRaceStrategy::NoRaces))
                                 )
                         )
 );
 
 
 struct reorderLoopsTopologically : public TestWithParam<NotationTest> {};
 
@@ -242,16 +260,16 @@
   ASSERT_NOTATION_EQ(GetParam().expected, actual);
 }
 
 INSTANTIATE_TEST_CASE_P(misc, reorderLoopsTopologically, Values(
   NotationTest(forall(i, w(i) = b(i)),
                   forall(i, w(i) = b(i))),
 
-  NotationTest(forall(i, w(i) = b(i), {Forall::PARALLELIZE}),
-                  forall(i, w(i) = b(i), {Forall::PARALLELIZE})),
+  NotationTest(forall(i, w(i) = b(i), MergeStrategy::TwoFinger, ParallelUnit::DefaultUnit, OutputRaceStrategy::NoRaces),
+                  forall(i, w(i) = b(i), MergeStrategy::TwoFinger, ParallelUnit::DefaultUnit, OutputRaceStrategy::NoRaces)),
 
   NotationTest(forall(i, forall(j, W(i,j) = A(i,j))),
                   forall(i, forall(j, W(i,j) = A(i,j)))),
 
   NotationTest(forall(j, forall(i, W(i,j) = A(i,j))),
                   forall(i, forall(j, W(i,j) = A(i,j)))),
 
@@ -306,31 +324,28 @@
                       where(forall(j,
                                    A(i,j) = w(j)),
                             forall(k,
                                    forall(j,
                                           w(j) += B(i,k) * C(k,j))))))
 ));
 
-/*
 TEST(schedule, workspace_spmspm) {
   TensorBase A("A", Float(64), {3,3}, Format({dense,compressed}));
   TensorBase B = d33a("B", Format({dense,compressed}));
   TensorBase C = d33b("C", Format({dense,compressed}));
   B.pack();
   C.pack();
 
   IndexVar i, j, k;
   IndexExpr matmul = B(i,k) * C(k,j);
   A(i,j) = matmul;
 
   A.evaluate();
 
-  std::cout << A << std::endl;
   Tensor<double> E("e", {3,3}, Format({dense,compressed}));
   E.insert({2,0}, 30.0);
   E.insert({2,1}, 180.0);
   E.pack();
   ASSERT_TENSOR_EQ(E,A);
 }
-*/
 
 }
```

### Comparing `tensora-0.0.6/src/taco/test/tests-type.cpp` & `tensora-0.0.7/src/taco/test/tests-type.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/tensora/compile.py` & `tensora-0.0.7/src/tensora/compile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ['taco_kernel', 'allocate_taco_structure', 'taco_structure_to_cffi', 'take_ownership_of_arrays',
-           'tensor_cdefs']
+           'tensor_cdefs', 'take_ownership_of_tensor_members']
 
 import re
 import subprocess
 import tempfile
 from pathlib import Path
 from typing import List, Tuple, FrozenSet, Any
 from weakref import WeakKeyDictionary
@@ -207,15 +207,14 @@
     memory_holder['mode_types'] = cffi_mode_types
     cffi_tensor.mode_types = cffi_mode_types
 
     converted_levels = []
     memory_holder_levels = []
     memory_holder_levels_arrays = []
     for mode in mode_types:
-        converted_arrays = []
         if mode == tensor_lib.taco_mode_dense:
             converted_arrays = []
         elif mode == tensor_lib.taco_mode_sparse:
             converted_arrays = [tensor_cdefs.NULL, tensor_cdefs.NULL]
         cffi_level = tensor_cdefs.new('int32_t*[]', converted_arrays)
         memory_holder_levels.append(cffi_level)
         memory_holder_levels_arrays.append(converted_arrays)
@@ -321,15 +320,15 @@
 
     The `evaluate` function created by taco `malloc`s several arrays on the output tensor, namely the `pos` and `crd`
     arrays of compressed levels and the `vals` array. This function looks up the tensor in `global_weakkeydict` and
     attaches the allocated arrays so that they get deallocated when the tensor is garbage collected. This function must
     be called on the output tensor of any evaluated taco kernel.
 
     Args:
-        cffi_tensor: A cffi taco_tensor_t*.
+        cffi_tensor: A cffi taco_tensor_t or taco_tensor_t*.
     """
 
     memory_holder = global_weakkeydict[cffi_tensor]
 
     order = cffi_tensor.order
 
     modes = cffi_tensor.mode_types[0:order]
@@ -341,9 +340,70 @@
         if mode == tensor_lib.taco_mode_sparse:
             memory_holder['**indices'][i_dimension][0] = tensor_cdefs.gc(cffi_levels[i_dimension][0], tensor_lib.free)
             memory_holder['**indices'][i_dimension][1] = tensor_cdefs.gc(cffi_levels[i_dimension][1], tensor_lib.free)
 
     memory_holder['vals'] = tensor_cdefs.gc(cffi_tensor.vals, tensor_lib.free)
 
 
+def take_ownership_of_tensor_members(cffi_tensor) -> None:
+    """Take ownership of taco tensor whose members were allocated elsewhere.
+
+    This is not needed by pure Tensora. But some low-level programs might
+    allocate members of a tensor and return it to Python. If the taco_tensor_t
+    will be owned by Python, then this function can be used to take ownership of
+    all the memory of all members of the taco_tensor_t so that it is freed when
+    the cffi object is freed.
+
+    Args:
+        cffi_tensor: A cffi taco_tensor_t or taco_tensor_t*.
+    """
+    # This mayor may not have been called by take_ownership_of_tensor first, so
+    # an entry in global_weakkeydict may or may not already exist.
+    memory_holder = global_weakkeydict.get(cffi_tensor, {})
+
+    # First, take ownership of everything that is owned after taco_structure_to_cffi
+    order = cffi_tensor.order
+
+    memory_holder['dimensions'] = tensor_cdefs.gc(cffi_tensor.dimensions, tensor_lib.free)
+
+    memory_holder['mode_ordering'] = tensor_cdefs.gc(cffi_tensor.mode_ordering, tensor_lib.free)
+
+    memory_holder['mode_types'] = tensor_cdefs.gc(cffi_tensor.mode_types, tensor_lib.free)
+
+    memory_holder_levels = []
+    memory_holder_levels_arrays = []
+    for i_dimension, mode in enumerate(cffi_tensor.mode_types[0:order]):
+        memory_holder_levels.append(tensor_cdefs.gc(cffi_tensor.indices[i_dimension], tensor_lib.free))
+        if mode == tensor_lib.taco_mode_dense:
+            memory_holder_levels_arrays.append([])
+        elif mode == tensor_lib.taco_mode_sparse:
+            # It does not matter what the values are here. They will be overwritten in take_ownership_of_arrays.
+            memory_holder_levels_arrays.append([tensor_cdefs.NULL, tensor_cdefs.NULL])
+    memory_holder['indices'] = tensor_cdefs.gc(cffi_tensor.indices, tensor_lib.free)
+    memory_holder['*indices'] = memory_holder_levels
+    memory_holder['**indices'] = memory_holder_levels_arrays
+
+    global_weakkeydict[cffi_tensor] = memory_holder
+
+    # Second, defer to take_ownership_of_arrays to take ownership of everything else
+    # This function assumes that the memory holder has already been assigned to
+    # the weak key dictionary.
+    take_ownership_of_arrays(cffi_tensor)
+
+
+def take_ownership_of_tensor(cffi_tensor) -> None:
+    """Take ownership of taco tensor that was allocated elsewhere entirely.
+
+    This is not needed by pure Tensora. But some low-level programs might
+    allocate a taco tensor and return it to Python. If the taco_tensor_t will be
+    owned by Python, then this function can be used to take ownership of all the
+    memory so that it is freed when the cffi object is freed.
+
+    Args:
+        cffi_tensor: A cffi taco_tensor_t*.
+    """
+    global_weakkeydict[cffi_tensor] = {'tensor': tensor_cdefs.gc(cffi_tensor, tensor_lib.free)}
+    take_ownership_of_tensor_members(cffi_tensor)
+
+
 def weakly_increasing(list: List[int]):
     return all(x <= y for x, y in zip(list, list[1:]))
```

### Comparing `tensora-0.0.6/src/tensora/expression/ast.py` & `tensora-0.0.7/src/tensora/expression/ast.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/tensora/expression/parser.py` & `tensora-0.0.7/src/tensora/expression/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __all__ = ['parse_assignment']
 
 from functools import reduce
 
-from parsita import TextParsers, lit, reg, rep, rep1sep, Result
+from parsita import ParserContext, lit, reg, rep, rep1sep, Result
 from parsita.util import splat
 
 from .ast import Assignment, Add, Subtract, Multiply, Tensor, Scalar, Integer, Float
 
 
 def make_expression(first, rest):
     value = first
@@ -14,15 +14,15 @@
         if op == '+':
             value = Add(value, term)
         else:
             value = Subtract(value, term)
     return value
 
 
-class TensorExpressionParsers(TextParsers):
+class TensorExpressionParsers(ParserContext, whitespace=r'[ ]*'):
     name = reg(r'[A-Za-z][A-Za-z0-9]*')
 
     # taco does not support negatives or exponents
     floating_point = reg(r'[0-9]+\.[0-9]+') > (lambda x: Float(float(x)))
     integer = reg(r'[0-9]+') > (lambda x: Integer(int(x)))
     number = floating_point | integer
```

### Comparing `tensora-0.0.6/src/tensora/format/format.py` & `tensora-0.0.7/src/tensora/format/format.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/src/tensora/format/parser.py` & `tensora-0.0.7/src/tensora/format/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 __all__ = ['parse_format']
 
-from parsita import TextParsers, reg, lit, rep, eof, Result, Success, Failure
+from parsita import ParserContext, reg, lit, rep, eof, Result, Success, Failure, ParseError, StringReader
 from parsita.util import constant
 
 from .format import Mode, Format
 
 
 def make_format_with_orderings(dims):
     modes = []
     orderings = []
     for mode, ordering in dims:
         modes.append(mode)
         orderings.append(ordering)
     return Format(tuple(modes), tuple(orderings))
 
 
-class FormatTextParsers(TextParsers, whitespace=None):
+class FormatTextParsers(ParserContext):
     integer = reg(r'[0-9]+') > int
     dense = lit('d') > constant(Mode.dense)
     compressed = lit('s') > constant(Mode.compressed)
     mode = dense | compressed
 
     # Use eof to ensure each parser goes to end
     format_without_orderings = rep(mode) << eof > (lambda modes: Format(tuple(modes), tuple(range(len(modes)))))
@@ -29,13 +29,15 @@
 
 
 def parse_format(format: str) -> Result[Format]:
     parse_result = FormatTextParsers.format.parse(format)
     if isinstance(parse_result, Failure):
         return parse_result
     elif isinstance(parse_result, Success):
-        parse_value = parse_result.value
+        parse_value = parse_result.unwrap()
         if set(range(parse_value.order)) != set(parse_value.ordering):
-            return Failure(f'Format ordering must be some order of the set {set(range(parse_value.order))} not '
-                           f'{parse_value.ordering}')
+            return Failure(ParseError(
+                StringReader(format),
+                f'format ordering as some order of the set {set(range(parse_value.order))}'
+            ))
         else:
             return parse_result
```

### Comparing `tensora-0.0.6/src/tensora/function.py` & `tensora-0.0.7/src/tensora/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,19 +118,19 @@
     return cachable_tensor_method(assignment, tuple(input_formats.items()), output_format)
 
 
 @lru_cache()
 def cachable_tensor_method(assignment: str, input_formats: Tuple[Tuple[str, str], ...], output_format: str
                            ) -> PureTensorMethod:
     from .expression.parser import parse_assignment
-    parsed_assignment = parse_assignment(assignment).or_die()
+    parsed_assignment = parse_assignment(assignment).unwrap()
 
-    parsed_input_formats = {name: parse_format(format).or_die() for name, format in input_formats}
+    parsed_input_formats = {name: parse_format(format).unwrap() for name, format in input_formats}
 
-    parsed_output = parse_format(output_format).or_die()
+    parsed_output = parse_format(output_format).unwrap()
 
     if parsed_assignment.is_mutating():
         raise NotImplementedError(f'Mutating tensor assignments like {assignment} not implemented yet.')
     else:
         return PureTensorMethod(parsed_assignment, parsed_input_formats, parsed_output)
```

### Comparing `tensora-0.0.6/src/tensora/tensor.py` & `tensora-0.0.7/src/tensora/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         if dimensions is None:
             dimensions = default_aos_dimensions(coordinates)
 
         if format is None:
             coordinates = list(coordinates)
             format = default_format_given_nnz(dimensions, len(coordinates))
         elif isinstance(format, str):
-            format = parse_format(format).or_die()
+            format = parse_format(format).unwrap()
 
         # Reorder with first level first, etc.
         level_dimensions = tuple(dimensions[i] for i in format.ordering)
         level_coordinates = [tuple(coordinate[i] for i in format.ordering) for coordinate in coordinates]
 
         tree = coordinates_to_tree(level_coordinates, values)
```

### Comparing `tensora-0.0.6/src/tensora.egg-info/PKG-INFO` & `tensora-0.0.7/src/tensora.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,180 @@
 Metadata-Version: 2.1
 Name: tensora
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library for dense and sparse tensors built on the tensor algebra compiler.
 Home-page: https://github.com/drhagen/tensora
 Author: David Hagen
 Author-email: david@drhagen.com
 License: MIT
-Description: # Tensora
-        
-        A fast and easy-to-use dense/sparse tensor library for Python. Evaluate arbitrary tensor expressions with tensors in a variety of sparsity formats.
-        
-        Tensors are n-dimensional generalizations of matrices. Instead of being confined to 1 or 2 dimensions, tensors may have 3, 4, or more dimensions. They are useful in a variety of applications. NumPy is the best known tensor library in Python; its central `ndarray` object is an example of a dense tensor. 
-        
-        In a dense tensor, each element is explicitly stored in memory. If the vast majority of elements are zero, then this is an inefficient layout, taking far more memory to store and far more time to operate on. There are many different sparse tensor formats, each one better or worse depending on which elements of the tensor are nonzero.
-        
-        Many tensor kernels (functions that perform a specific algebraic calculation between tensors with specific sparse formats) have been written to solve specific problems. Recently, the [Tensor Algebra Compiler](http://tensor-compiler.org/) (taco) was invented to automate the construction and optimization of tensor kernels for arbitrary algebraic expressions for arbitrary sparse formats. taco takes an algebraic expression and description of the format of each tensor in the expression and returns a C function that efficiently evaluates the given expression for those tensor arguments.
-        
-        Tensora is a Python wrapper around taco. Tensora has a central class `Tensor` that simply has a pointer to a taco tensor held in C memory, managed by the `cffi` package. Tensora exposes functions that take a string of an algebraic expression and return a Python function the performs that operation in fast C code. In order to do that, the string is parsed and passed to taco; the C code generated by taco is compiled "on the fly" by `cffi` and then wrapped by code that provides good error handling.
-        
-        **This package is highly experimental. Do not trust the results without independently verifying the output for any particular problem.** This is mostly because the underlying taco compiler is itself highly experimental. Much of Tensora's test suite is skipped because of known underlying bugs in the generated kernels. As the research on taco improves, the test suite of Tensora will be expanded and the documentation improved.
-        
-        
-        ## Getting started
-        
-        Tensora can be installed with `pip` from PyPI:
-         
-        ```bash
-        pip install tensora
-        ```
-        
-        The class `Tensor` and the function `evaluate` together provide the porcelain interface for Tensora.
-        
-        Here is an example of multiplying a sparse matrix in CSR format with a dense vector:
-        
-        ```python
-        from tensora import Tensor, evaluate
-        
-        elements = {
-            (1,0): 2.0,
-            (0,1): -2.0,
-            (1,2): 4.0, 
-        }
-        
-        A = Tensor.from_dok(elements, dimensions=(2,3), format='ds')
-        x = Tensor.from_lol([0, -1, 2])
-        
-        y = evaluate('y(i) = A(i,j) * x(j)', 'd', A=A, x=x)
-        
-        assert y == Tensor.from_lol([2,8])
-        ``` 
-        
-        
-        ## Creating `Tensor`s
-        
-        Creating a `Tensor` is best done via the `Tensor.from_*` methods. These methods convert a variety of data types into a `Tensor`. Most of the conversion methods optionally take both `dimensions` and `format` to determine the dimensions and format of the resulting tensor. 
-        
-        ### `from_lol`: list of lists
-        
-        ```python
-        Tensor.from_lol(lol, *, 
-                        dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
-        ```
-        
-        Convert a dense list of lists to a `Tensor`.
-        
-        * `lol` is a list of lists, possibly deeply nested. That is, `lol` is a `float`, a `List[float]`, a `List[List[float]]`, etc. to an arbitrary depth of `List`s. The values are read in row-major format, meaning the top-level list is the first dimension and the deepest list (the one containing actual scalars) is the last dimension. All lists at the same level must have the same length. For those familiar, this is identical to the NumPy behavior when constructing an array from lists of lists via `numpy.array`.
-        
-        * `dimensions` has a default value that is inferred from the structure of `lol`. If provided, it must be consistent with the structure of `lol`. Providing the dimensions is typically only useful when one or more non-final dimensions may have size zero. For example, `Tensor.from_lol([[], []])` has dimensions of `(2,0)`, while `Tensor.from_lol([[], []], dimensions=(2,0,3))` has dimensions of `(2,0,3)`.
-        
-        * `format` has a default value of all dense dimensions.
-        
-        ### `from_dok`: dictionary of keys
-        
-        ```python
-        Tensor.from_dok(dok: Dict[Tuple[int, ...], float], *, 
-                        dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
-        ```
-        
-        Convert a dictionary of keys to a `Tensor`.
-        
-        * `dok` is a Python dictionary where each key is the coordinate of one non-zero value and the value of the entry is the value of the tensor at that coordinate. All coordinates not mentioned are implicitly zero.
-        
-        * `dimensions` has a default value that is the largest size in each dimension found among the coordinates.
-        
-        * `format` has a default value of dense dimensions as long as the number of nonzeros is larger than the product of those dimensions and then sparse dimensions after that. The default value is subject to change with experience.
-        
-        ### `from_aos`: array of structs
-        
-        ```python
-        Tensor.from_aos(aos: Iterable[Tuple[int, ...]], values: Iterable[float], *, 
-                        dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
-        ```
-        
-        Convert a list of coordinates and a corresponding list of values to a `Tensor`.
-        
-        * `aos` is an iterable of the coordinates of the non-zero values.
-        
-        * `values` must be the same length as `aos` and each value is the non-zero value at the corresponding coordinate.
-        
-        * `dimensions` has the same default as `Tensor.from_dok`, the largest size in each dimension.
-        
-        * `format`has the same default as `Tensor.from_dok`, dense for an many dimensions as needed to fit the non-zeros.
-        
-        ### `from_soa`: struct of arrays
-        
-        ```python
-        Tensor.from_soa(soa: Tuple[Iterable[int], ...], values: Iterable[float], *, 
-                        dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
-        ```
-        
-        Convert lists of indexes for each dimension and a corresponding list of values to a `Tensor`.
-        
-        * `soa` is a tuple of iterables, where each iterable is all the indexes of the corresponding dimension. All iterables must be the same length.
-        
-        * `values` must be the same length as the iterables in coordinates and each value is the non-zero value at the corresponding coordinate.
-        
-        * `dimensions` has the same default as `Tensor.from_dok`, the largest size in each dimension.
-        
-        * `format`has the same default as `Tensor.from_dok`, dense for an many dimensions as needed to fit the non-zeros.
-        
-        ### `from_numpy`: convert a NumPy array
-        
-        ```python
-        Tensor.from_numpy(array: numpy.ndarray, *, 
-                          format: Union[Format, str] = None)
-        ```
-        
-        Convert a NumPy array to a `Tensor`.
-        
-        * `array` is any `NumPy.ndarray`. The resulting `Tensor` will have the same order, dimensions, and values of this array. 
-        
-        * `format` has a default value of all dense dimensions.
-        
-        ### `from_scipy_sparse`: convert a SciPy sparse matrix
-        
-        ```python
-        Tensor.from_scipy_sparse(data: scipy.sparse.spmatrix, *, 
-                                 format: Union[Format, str] = None)
-        ```
-        
-        Convert a SciPy sparse matrix to a `Tensor`.
-        
-        * `matrix` is any `SciPy.sparse.spmatrix`. The resulting `Tensor` will have the same order, dimensions, and values of this matrix. The tensor will always have order 2.
-        
-        * `format` has a default value of `ds` for `csr_matrix` and `d1s0` for `csc_matrix` and also `ds` for the other sparse matrix types, though that is subject to changes as taco adds new format mode types.
-        
-        
-        ## Evaluating expressions
-        
-        Taco generates kernels for algebraic expressions of tensor kernels. Tensora wraps this process with the `evaluate` function.
-        
-        ```python
-        evaluate(assignment: str, output_format: str, **inputs: Tensor)
-        ``` 
-        
-        * `assignment` is parsable as an algebraic tensor assignment.
-        
-        * `output_format` is the desired format of the output tensor.
-        
-        * `inputs` is all the inputs to the expression. There must be one named argument for each variable name in `assignment`. The dimensions of the tensors in `inputs` must be consistent with `assignment` and with each other.
 Keywords: tensor sparse matrix array
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: numpy
 Provides-Extra: scipy
+License-File: LICENSE
+
+# Tensora
+
+A fast and easy-to-use dense/sparse tensor library for Python. Evaluate arbitrary tensor expressions with tensors in a variety of sparsity formats.
+
+Tensors are n-dimensional generalizations of matrices. Instead of being confined to 1 or 2 dimensions, tensors may have 3, 4, or more dimensions. They are useful in a variety of applications. NumPy is the best known tensor library in Python; its central `ndarray` object is an example of a dense tensor. 
+
+In a dense tensor, each element is explicitly stored in memory. If the vast majority of elements are zero, then this is an inefficient layout, taking far more memory to store and far more time to operate on. There are many different sparse tensor formats, each one better or worse depending on which elements of the tensor are nonzero.
+
+Many tensor kernels (functions that perform a specific algebraic calculation between tensors with specific sparse formats) have been written to solve specific problems. Recently, the [Tensor Algebra Compiler](http://tensor-compiler.org/) (taco) was invented to automate the construction and optimization of tensor kernels for arbitrary algebraic expressions for arbitrary sparse formats. taco takes an algebraic expression and description of the format of each tensor in the expression and returns a C function that efficiently evaluates the given expression for those tensor arguments.
+
+Tensora is a Python wrapper around taco. Tensora has a central class `Tensor` that simply has a pointer to a taco tensor held in C memory, managed by the `cffi` package. Tensora exposes functions that take a string of an algebraic expression and return a Python function the performs that operation in fast C code. In order to do that, the string is parsed and passed to taco; the C code generated by taco is compiled "on the fly" by `cffi` and then wrapped by code that provides good error handling.
+
+**This package is highly experimental. Do not trust the results without independently verifying the output for any particular problem.** This is mostly because the underlying taco compiler is itself highly experimental. Much of Tensora's test suite is skipped because of known underlying bugs in the generated kernels. As the research on taco improves, the test suite of Tensora will be expanded and the documentation improved.
+
+
+## Getting started
+
+Tensora can be installed with `pip` from PyPI:
+ 
+```bash
+pip install tensora
+```
+
+The class `Tensor` and the function `evaluate` together provide the porcelain interface for Tensora.
+
+Here is an example of multiplying a sparse matrix in CSR format with a dense vector:
+
+```python
+from tensora import Tensor, evaluate
+
+elements = {
+    (1,0): 2.0,
+    (0,1): -2.0,
+    (1,2): 4.0, 
+}
+
+A = Tensor.from_dok(elements, dimensions=(2,3), format='ds')
+x = Tensor.from_lol([0, -1, 2])
+
+y = evaluate('y(i) = A(i,j) * x(j)', 'd', A=A, x=x)
+
+assert y == Tensor.from_lol([2,8])
+``` 
+
+
+## Creating `Tensor`s
+
+Creating a `Tensor` is best done via the `Tensor.from_*` methods. These methods convert a variety of data types into a `Tensor`. Most of the conversion methods optionally take both `dimensions` and `format` to determine the dimensions and format of the resulting tensor. 
+
+### `from_lol`: list of lists
+
+```python
+Tensor.from_lol(lol, *, 
+                dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
+```
+
+Convert a dense list of lists to a `Tensor`.
+
+* `lol` is a list of lists, possibly deeply nested. That is, `lol` is a `float`, a `List[float]`, a `List[List[float]]`, etc. to an arbitrary depth of `List`s. The values are read in row-major format, meaning the top-level list is the first dimension and the deepest list (the one containing actual scalars) is the last dimension. All lists at the same level must have the same length. For those familiar, this is identical to the NumPy behavior when constructing an array from lists of lists via `numpy.array`.
+
+* `dimensions` has a default value that is inferred from the structure of `lol`. If provided, it must be consistent with the structure of `lol`. Providing the dimensions is typically only useful when one or more non-final dimensions may have size zero. For example, `Tensor.from_lol([[], []])` has dimensions of `(2,0)`, while `Tensor.from_lol([[], []], dimensions=(2,0,3))` has dimensions of `(2,0,3)`.
+
+* `format` has a default value of all dense dimensions.
+
+### `from_dok`: dictionary of keys
+
+```python
+Tensor.from_dok(dok: Dict[Tuple[int, ...], float], *, 
+                dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
+```
+
+Convert a dictionary of keys to a `Tensor`.
+
+* `dok` is a Python dictionary where each key is the coordinate of one non-zero value and the value of the entry is the value of the tensor at that coordinate. All coordinates not mentioned are implicitly zero.
+
+* `dimensions` has a default value that is the largest size in each dimension found among the coordinates.
+
+* `format` has a default value of dense dimensions as long as the number of nonzeros is larger than the product of those dimensions and then sparse dimensions after that. The default value is subject to change with experience.
+
+### `from_aos`: array of structs
+
+```python
+Tensor.from_aos(aos: Iterable[Tuple[int, ...]], values: Iterable[float], *, 
+                dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
+```
+
+Convert a list of coordinates and a corresponding list of values to a `Tensor`.
+
+* `aos` is an iterable of the coordinates of the non-zero values.
+
+* `values` must be the same length as `aos` and each value is the non-zero value at the corresponding coordinate.
+
+* `dimensions` has the same default as `Tensor.from_dok`, the largest size in each dimension.
+
+* `format`has the same default as `Tensor.from_dok`, dense for an many dimensions as needed to fit the non-zeros.
+
+### `from_soa`: struct of arrays
+
+```python
+Tensor.from_soa(soa: Tuple[Iterable[int], ...], values: Iterable[float], *, 
+                dimensions: Tuple[int, ...] = None, format: Union[Format, str] = None)
+```
+
+Convert lists of indexes for each dimension and a corresponding list of values to a `Tensor`.
+
+* `soa` is a tuple of iterables, where each iterable is all the indexes of the corresponding dimension. All iterables must be the same length.
+
+* `values` must be the same length as the iterables in coordinates and each value is the non-zero value at the corresponding coordinate.
+
+* `dimensions` has the same default as `Tensor.from_dok`, the largest size in each dimension.
+
+* `format`has the same default as `Tensor.from_dok`, dense for an many dimensions as needed to fit the non-zeros.
+
+### `from_numpy`: convert a NumPy array
+
+```python
+Tensor.from_numpy(array: numpy.ndarray, *, 
+                  format: Union[Format, str] = None)
+```
+
+Convert a NumPy array to a `Tensor`.
+
+* `array` is any `NumPy.ndarray`. The resulting `Tensor` will have the same order, dimensions, and values of this array. 
+
+* `format` has a default value of all dense dimensions.
+
+### `from_scipy_sparse`: convert a SciPy sparse matrix
+
+```python
+Tensor.from_scipy_sparse(data: scipy.sparse.spmatrix, *, 
+                         format: Union[Format, str] = None)
+```
+
+Convert a SciPy sparse matrix to a `Tensor`.
+
+* `matrix` is any `SciPy.sparse.spmatrix`. The resulting `Tensor` will have the same order, dimensions, and values of this matrix. The tensor will always have order 2.
+
+* `format` has a default value of `ds` for `csr_matrix` and `d1s0` for `csc_matrix` and also `ds` for the other sparse matrix types, though that is subject to changes as taco adds new format mode types.
+
+
+## Evaluating expressions
+
+Taco generates kernels for algebraic expressions of tensor kernels. Tensora wraps this process with the `evaluate` function.
+
+```python
+evaluate(assignment: str, output_format: str, **inputs: Tensor)
+``` 
+
+* `assignment` is parsable as an algebraic tensor assignment.
+
+* `output_format` is the desired format of the output tensor.
+
+* `inputs` is all the inputs to the expression. There must be one named argument for each variable name in `assignment`. The dimensions of the tensors in `inputs` must be consistent with `assignment` and with each other.
```

### Comparing `tensora-0.0.6/tests/test_combinatorically.py` & `tensora-0.0.7/tests/test_combinatorically.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,18 +67,16 @@
     assert_same_as_dense('out(i,k) = in1(i,j) * in2(j,k)', format_out, in1=(dense1, format1), in2=(dense2, format2))
 
 
 @pytest.mark.parametrize('dense1', [[[0, 2, 4], [0, -1, 0]], [[0, 0, 0], [0, 0, 0]]])
 @pytest.mark.parametrize('dense2', [[-1, 3.5, 0], [0, 0, 0]])
 @pytest.mark.parametrize('format1', ['ss', 'dd', 'sd', 'ds', 's1s0', 'd1d0', 's1d0', 'd1s0'])
 @pytest.mark.parametrize('format2', ['s', 'd'])
-@pytest.mark.parametrize('format_out', ['s', 'd'])
+@pytest.mark.parametrize('format_out', ['d'])
 def test_matrix_vector_product(dense1, dense2, format1, format2, format_out):
-    if format_out == 's':
-        pytest.skip('taco fails when output is sparse')
     assert_same_as_dense('out(i) = in1(i,j) * in2(j)', format_out, in1=(dense1, format1), in2=(dense2, format2))
 
 
 @pytest.mark.parametrize('dense1', [[[0, 2, 4], [0, -1, 0]], [[0, 0, 0], [0, 0, 0]]])
 @pytest.mark.parametrize('dense2', [[[-1, 3.5], [0, 0], [4, 0]], [[0, 0], [0, 0], [0, 0]]])
 @pytest.mark.parametrize('dense3', [[[-3, 0], [7, 0]], [[0, 0], [0, 0]]])
 @pytest.mark.parametrize('format1', ['dd', 'ds'])
```

### Comparing `tensora-0.0.6/tests/test_expression.py` & `tensora-0.0.7/tests/test_expression.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     ('ab2(i) = (a(i) + b(i)) * 2.0',
      Assignment(Tensor('ab2', ['i']), Multiply(Add(Tensor('a', ['i']), Tensor('b', ['i'])), Float(2.0)))),
 ]
 
 
 @pytest.mark.parametrize('string,assignment', assignment_strings)
 def test_assignment_parsing(string, assignment):
-    actual = parse_assignment(string).or_die()
+    actual = parse_assignment(string).unwrap()
     assert actual == assignment
 
 
 @pytest.mark.parametrize('string,assignment', assignment_strings)
 def test_assignment_deparsing(string, assignment):
     deparsed = assignment.deparse()
     assert deparsed == string
 
 
 def parse(string):
-    return parse_assignment(string).or_die()
+    return parse_assignment(string).unwrap()
 
 
 def test_assignment_to_string():
     string = 'A(i) = 2 * B(i,j) * (C(j) + D(j))'
     assert str(parse(string)) == string
```

### Comparing `tensora-0.0.6/tests/test_format.py` & `tensora-0.0.7/tests/test_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ('d1s0', Format((Mode.dense, Mode.compressed), (1, 0))),
     ('d1s0s2', Format((Mode.dense, Mode.compressed, Mode.compressed), (1, 0, 2))),
 ]
 
 
 @pytest.mark.parametrize('string,format', format_strings)
 def test_parse_format(string, format):
-    actual = parse_format(string).or_die()
+    actual = parse_format(string).unwrap()
     assert actual == format
 
 
 @pytest.mark.parametrize('string,format', format_strings)
 def test_deparse_format(string, format):
     actual = format.deparse()
     assert actual == string
```

### Comparing `tensora-0.0.6/tests/test_from_data.py` & `tensora-0.0.7/tests/test_from_data.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/tests/test_function.py` & `tensora-0.0.7/tests/test_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from random import randrange
 
-import pytest
 from multiprocessing.pool import ThreadPool
 from tensora import Tensor, tensor_method, evaluate
 
 
 def test_csr_matrix_vector_product():
     A = Tensor.from_aos(
         [[1, 0], [0, 1], [1, 2]],
@@ -61,15 +60,14 @@
     assert actual == expected
 
     actual = evaluate('y(i) = A(i,j) * x(j)', 'd', A=A, x=x)
 
     assert actual == expected
 
 
-@pytest.mark.skip('taco fails on sparse outputs')
 def test_csr_matrix_plus_csr_matrix():
     A = Tensor.from_aos(
         [[1, 0], [0, 1], [1, 2]],
         [2.0, -2.0, 4.0],
         dimensions=(2, 3), format='ds'
     )
 
@@ -87,15 +85,15 @@
 
     function = tensor_method('C(i,j) = A(i,j) + B(i,j)', dict(A='ds', B='ds'), 'ds')
 
     actual = function(A, B)
 
     assert actual == expected
 
-    actual = evaluate('C(i,j) = A(i,j) * B(i,j)', 'ds', A=A, B=B)
+    actual = evaluate('C(i,j) = A(i,j) + B(i,j)', 'ds', A=A, B=B)
 
     assert actual == expected
 
 
 def test_multithread_evaluation():
     # As of version 1.14.4 of cffi, the FFI.compile method is not thread safe. This tests that evaluation of different
     # kernels is thread safe.
```

### Comparing `tensora-0.0.6/tests/test_numpy.py` & `tensora-0.0.7/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/tests/test_operators.py` & `tensora-0.0.7/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.6/tests/test_tensor.py` & `tensora-0.0.7/tests/test_tensor.py`

 * *Files identical despite different names*

