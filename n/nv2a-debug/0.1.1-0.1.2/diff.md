# Comparing `tmp/nv2a_debug-0.1.1.tar.gz` & `tmp/nv2a_debug-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nv2a_debug-0.1.1.tar", last modified: Thu Jun 15 07:57:05 2023, max compression
+gzip compressed data, was "nv2a_debug-0.1.2.tar", last modified: Fri Jun 16 02:59:31 2023, max compression
```

## Comparing `nv2a_debug-0.1.1.tar` & `nv2a_debug-0.1.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/build_cffi.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.673933 nv2a_debug-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/src/nv2adbg/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_code_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_file_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_input_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_output_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_program_inputs_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_program_outputs_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_program_vertex_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_register_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_shader_program.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8002 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/py_nv2a_vsh_emu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/tests/test__code_panel_build_ancestor_root_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/tests/test__code_panel_build_contributing_source_segments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/githooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3097 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/githooks/pre-commit
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/disassembler/
--rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/disassembler/test_main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/emulator/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/emulator/test_main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/operations/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.356826 nv2a_debug-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-16 02:59:31.356826 nv2a_debug-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/build_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-16 02:59:31.356826 nv2a_debug-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.348826 nv2a_debug-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.352825 nv2a_debug-0.1.2/src/nv2a_debug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-16 02:59:31.000000 nv2a_debug-0.1.2/src/nv2a_debug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-16 02:59:31.000000 nv2a_debug-0.1.2/src/nv2a_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:59:31.000000 nv2a_debug-0.1.2/src/nv2a_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 02:59:31.000000 nv2a_debug-0.1.2/src/nv2a_debug.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 02:59:31.000000 nv2a_debug-0.1.2/src/nv2a_debug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 02:59:31.000000 nv2a_debug-0.1.2/src/nv2a_debug.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.352825 nv2a_debug-0.1.2/src/nv2adbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_code_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_file_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_input_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_output_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_program_inputs_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_program_outputs_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_program_vertex_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_register_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/_shader_program.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8442 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/py_nv2a_vsh_emu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/src/nv2adbg/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.352825 nv2a_debug-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/tests/test__code_panel_build_ancestor_root_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-16 02:59:27.000000 nv2a_debug-0.1.2/tests/test__code_panel_build_contributing_source_segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.348826 nv2a_debug-0.1.2/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.352825 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.348826 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.352825 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.352825 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/githooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3097 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/githooks/pre-commit
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.356826 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.348826 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.356826 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/disassembler/
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/disassembler/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.356826 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/emulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/emulator/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:59:31.356826 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 02:59:28.000000 nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/operations/test_main.cpp
```

### Comparing `nv2a_debug-0.1.1/LICENSE` & `nv2a_debug-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/PKG-INFO` & `nv2a_debug-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nv2a_debug
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simulator/debugger for the Xbox nv2a vertex shader
 Home-page: https://github.com/abaire/nv2a_vsh_debug
 Author: Erik Abair
 Author-email: erik.abair@bearbrains.work
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/abaire/nv2a_vsh_debug/issues
 Platform: UNKNOWN
```

### Comparing `nv2a_debug-0.1.1/README.md` & `nv2a_debug-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/build_cffi.py` & `nv2a_debug-0.1.2/build_cffi.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/setup.cfg` & `nv2a_debug-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nv2a_debug
-version = 0.1.1
+version = 0.1.2
 author = Erik Abair
 author_email = erik.abair@bearbrains.work
 description = Simulator/debugger for the Xbox nv2a vertex shader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/abaire/nv2a_vsh_debug
 project_urls =
```

### Comparing `nv2a_debug-0.1.1/src/nv2a_debug.egg-info/PKG-INFO` & `nv2a_debug-0.1.2/src/nv2a_debug.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nv2a-debug
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simulator/debugger for the Xbox nv2a vertex shader
 Home-page: https://github.com/abaire/nv2a_vsh_debug
 Author: Erik Abair
 Author-email: erik.abair@bearbrains.work
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/abaire/nv2a_vsh_debug/issues
 Platform: UNKNOWN
```

### Comparing `nv2a_debug-0.1.1/src/nv2a_debug.egg-info/SOURCES.txt` & `nv2a_debug-0.1.2/src/nv2a_debug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_code_panel.py` & `nv2a_debug-0.1.2/src/nv2adbg/_code_panel.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_editor.py` & `nv2a_debug-0.1.2/src/nv2adbg/_editor.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_error_message.py` & `nv2a_debug-0.1.2/src/nv2adbg/_error_message.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_file_menu.py` & `nv2a_debug-0.1.2/src/nv2adbg/_file_menu.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_input_panel.py` & `nv2a_debug-0.1.2/src/nv2adbg/_input_panel.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_output_panel.py` & `nv2a_debug-0.1.2/src/nv2adbg/_output_panel.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_program_inputs_viewer.py` & `nv2a_debug-0.1.2/src/nv2adbg/_program_inputs_viewer.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_program_outputs_viewer.py` & `nv2a_debug-0.1.2/src/nv2adbg/_program_outputs_viewer.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_program_vertex_viewer.py` & `nv2a_debug-0.1.2/src/nv2adbg/_program_vertex_viewer.py`

 * *Files 11% similar despite different names*

```diff
@@ -99,27 +99,21 @@
         try:
             self._row_index_to_vertex_id.clear()
             self._vertex_table.clear()
             if not self._program or not self._program.mesh_inputs_file:
                 self._active_content = "no-content"
                 return
 
-            deduped_vertices = {}
-            for vertex in self._program.vertex_inputs:
-                deduped_vertices[int(vertex["IDX"])] = vertex
+            ordered_vertices = self._program.get_deduped_ordered_vertices()
 
-            for row, vertex_idx in enumerate(sorted(deduped_vertices.keys())):
-                vertex = deduped_vertices[vertex_idx]
+            for row, vertex in enumerate(ordered_vertices):
                 self._row_index_to_vertex_id[row] = int(vertex["VTX"])
                 self._vertex_table.add_row(
-                    vertex_idx,
-                    *[
-                        _render_vertex(deduped_vertices[vertex_idx], f"v{idx}")
-                        for idx in range(0, 16)
-                    ],
+                    vertex["IDX"],
+                    *[_render_vertex(vertex, f"v{idx}") for idx in range(0, 16)],
                 )
 
             self._active_content = "content"
 
         except query.NoMatches:
             # The table is not loaded yet.
             pass
```

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_register_view.py` & `nv2a_debug-0.1.2/src/nv2adbg/_register_view.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/_shader_program.py` & `nv2a_debug-0.1.2/src/nv2adbg/_shader_program.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,14 +103,21 @@
             if self._vertex_inputs:
                 self._active_vertex = self._vertex_inputs[0]
 
     @property
     def vertex_inputs(self):
         return self._vertex_inputs
 
+    def get_deduped_ordered_vertices(self) -> List[Dict]:
+        deduped_vertices = {}
+        for vertex in self._vertex_inputs:
+            deduped_vertices[int(vertex["IDX"])] = vertex
+
+        return [deduped_vertices[idx] for idx in sorted(deduped_vertices.keys())]
+
     @property
     def constants_file(self) -> str:
         return self._renderdoc_constants_csv
 
     @constants_file.setter
     def constants_file(self, val: str):
         self._renderdoc_constants_csv = val
@@ -118,19 +125,22 @@
             with open(val, newline="", encoding="ascii") as csvfile:
                 self._constants = list(csv.DictReader(csvfile))
         else:
             self._constants = []
 
     def set_active_vertex_index(self, index: int) -> bool:
         """Selects a new vertex to use as inputs. Returns True if the shader was rebuilt as a result."""
-        active_vertex = self._vertex_inputs[index]
-        if active_vertex == self._active_vertex:
+        return self.set_active_vertex(self._vertex_inputs[index])
+
+    def set_active_vertex(self, vertex: Dict) -> bool:
+        """Selects a new vertex to use as inputs. Returns True if the shader was rebuilt as a result."""
+        if vertex == self._active_vertex:
             return False
 
-        self._active_vertex = active_vertex
+        self._active_vertex = vertex
         self.build_shader()
         return True
 
     def build_shader(self):
         self._shader = simulator.Shader()
         self._shader.set_initial_state(self._inputs)
```

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/debugger.py` & `nv2a_debug-0.1.2/src/nv2adbg/debugger.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,30 +135,14 @@
     def _on__program_vertex_viewer_active_vertex_changed(
         self, event: _ProgramVertexViewer.ActiveVertexChanged
     ):
         del event
         self.set_shader_trace(self._program.shader_trace)
 
 
-# def _export(self):
-#     # TODO: Pop a text input dialog and capture a filename.
-#     filename = ""
-#     for index in range(1000):
-#         filename = f"export{index:04}.vsh"
-#         if not os.path.exists(filename):
-#             break
-#     if os.path.exists(filename):
-#         raise Exception("Failed to find an unused export filename.")
-#
-#     def resolve(input):
-#         return self._program.shader.initial_state.get(input)
-#
-#     self._editor.export(filename, resolve)
-
-
 def _emit_input_template():
     ctx = simulator.Context()
     values = ctx.to_dict(True)
     json.dump(values, sys.stdout, indent=2, sort_keys=True)
 
 
 def _main(args):
@@ -194,20 +178,44 @@
         args.source, args.inputs, args.renderdoc_mesh, args.renderdoc_constants
     )
 
     if args.json:
         json.dump(program.shader_trace.to_dict(), sys.stdout, indent=2, sort_keys=True)
         return 0
 
+    if args.simulate:
+        _dump_all_results(program)
+        return 0
+
     app = _App(program)
     app.run()
 
     return 0
 
 
+def _dump_all_results(program: _ShaderProgram) -> None:
+    all_results = []
+    ordered_vertices = program.get_deduped_ordered_vertices()
+    print(
+        f"Simulating {len(ordered_vertices)} runs, this may take some time...",
+        file=sys.stderr,
+    )
+
+    for vertex in ordered_vertices:
+        program.set_active_vertex(vertex)
+        result = {
+            "vertex": vertex,
+            "input": program.shader_trace.inputs,
+            "output": program.shader_trace.output,
+        }
+        all_results.append(result)
+
+    json.dump(all_results, sys.stdout, indent=2, sort_keys=True)
+
+
 def entrypoint():
     """The main entrypoint for this program."""
 
     def _parse_args():
         parser = argparse.ArgumentParser()
 
         parser.add_argument(
@@ -242,24 +250,31 @@
             help="Emit a template JSON file that may be used to modify the inputs to the shader.",
         )
 
         parser.add_argument(
             "-j",
             "--json",
             action="store_true",
-            help="Emit a JSON document capturing the context at each instruction in the source.",
+            help="Emit a JSON document capturing the context at each instruction in the source. Requires <source>.",
         )
 
         parser.add_argument(
             "-v",
             "--verbose",
             help="Enables verbose logging information",
             action="store_true",
         )
 
+        parser.add_argument(
+            "-s",
+            "--simulate",
+            action="store_true",
+            help="Emit a JSON document capturing the end results for each vertex in the mesh. Requires <source>.",
+        )
+
         return parser.parse_args()
 
     sys.exit(_main(_parse_args()))
 
 
 if __name__ == "__main__":
     entrypoint()
```

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/py_nv2a_vsh_emu.py` & `nv2a_debug-0.1.2/src/nv2adbg/py_nv2a_vsh_emu.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,16 +225,15 @@
         """Returns a dictionary representation of this state."""
 
         def retrieve_regs(prefix: str, source, count: int) -> List:
             regs = []
             for i in range(count):
                 register = [f"{prefix}{i}"]
                 offset = i * 4
-                for component in range(4):
-                    register.append(source[offset + component])
+                register.extend(source[offset : offset + 4])
                 regs.append(register)
             return regs
 
         ret = {
             "input": retrieve_regs("v", self._state.input_regs, 16),
             "constant": retrieve_regs("c", self._state.context_regs, 192),
         }
```

### Comparing `nv2a_debug-0.1.1/src/nv2adbg/simulator.py` & `nv2a_debug-0.1.2/src/nv2adbg/simulator.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/tests/test__code_panel_build_ancestor_root_segments.py` & `nv2a_debug-0.1.2/tests/test__code_panel_build_ancestor_root_segments.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/tests/test__code_panel_build_contributing_source_segments.py` & `nv2a_debug-0.1.2/tests/test__code_panel_build_contributing_source_segments.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/CMakeLists.txt` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/LICENSE` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/LICENSE`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/githooks/pre-commit` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/githooks/pre-commit`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp` & `nv2a_debug-0.1.2/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp`

 * *Files identical despite different names*

