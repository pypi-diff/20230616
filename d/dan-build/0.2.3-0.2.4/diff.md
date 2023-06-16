# Comparing `tmp/dan-build-0.2.3.tar.gz` & `tmp/dan-build-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.2.3.tar", last modified: Sat May 20 13:57:28 2023, max compression
+gzip compressed data, was "dan-build-0.2.4.tar", last modified: Fri Jun 16 06:05:16 2023, max compression
```

## Comparing `dan-build-0.2.3.tar` & `dan-build-0.2.4.tar`

### file list

```diff
@@ -1,97 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.105941 dan-build-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 13:57:20.000000 dan-build-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-20 13:57:28.105941 dan-build-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-20 13:57:20.000000 dan-build-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.093941 dan-build-0.2.3/completion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/completion/bash/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-20 13:57:20.000000 dan-build-0.2.3/completion/bash/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 13:57:20.000000 dan-build-0.2.3/completion/bash/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/completion/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-20 13:57:20.000000 dan-build-0.2.3/completion/zsh/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 13:57:20.000000 dan-build-0.2.3/completion/zsh/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/dan/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/vscode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/dan/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cmake/configure_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/dan/conan/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/conan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/conan/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/aiofiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/win.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/cxx/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/compile_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/cxx/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/data/detect.cmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/data/empty.c
--rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/msvc_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/cxx/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/support/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/unix_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/io/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/io/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/io/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/pkgconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/pkgconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/pkgconfig/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/pkgconfig/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/pkgconfig/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/src/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/src/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/src/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/src/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.105941 dan-build-0.2.3/dan_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-20 13:57:20.000000 dan-build-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:57:28.105941 dan-build-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.105941 dan-build-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-20 13:57:20.000000 dan-build-0.2.3/tests/test_cxx_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-20 13:57:20.000000 dan-build-0.2.3/tests/test_cxx_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-20 13:57:20.000000 dan-build-0.2.3/tests/test_cxx_smc_catch2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.952009 dan-build-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 06:05:02.000000 dan-build-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-16 06:05:16.948009 dan-build-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-16 06:05:02.000000 dan-build-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.932009 dan-build-0.2.4/completion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.936009 dan-build-0.2.4/completion/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-16 06:05:02.000000 dan-build-0.2.4/completion/bash/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-16 06:05:02.000000 dan-build-0.2.4/completion/bash/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.936009 dan-build-0.2.4/completion/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-16 06:05:02.000000 dan-build-0.2.4/completion/zsh/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 06:05:02.000000 dan-build-0.2.4/completion/zsh/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.936009 dan-build-0.2.4/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.940009 dan-build-0.2.4/dan/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.940009 dan-build-0.2.4/dan/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cmake/configure_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.940009 dan-build-0.2.4/dan/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/conan/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.944009 dan-build-0.2.4/dan/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/aiofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16928 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/win.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.944009 dan-build-0.2.4/dan/cxx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/compile_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.944009 dan-build-0.2.4/dan/cxx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/data/detect.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/data/empty.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24471 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/msvc_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.944009 dan-build-0.2.4/dan/cxx/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/support/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/unix_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/io/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/io/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan/pkgconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/pkgconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/pkgconfig/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan/pkgconfig/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/pkgconfig/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/src/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/src/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/src/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-16 06:05:02.000000 dan-build-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:05:16.952009 dan-build-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_cxx_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_cxx_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_cxx_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_cxx_src_catch2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_python_errors.py
```

### Comparing `dan-build-0.2.3/LICENSE` & `dan-build-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/PKG-INFO` & `dan-build-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.3/README.md` & `dan-build-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/completion/bash/dan-io.sh` & `dan-build-0.2.4/completion/bash/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/completion/bash/dan.sh` & `dan-build-0.2.4/completion/bash/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/completion/zsh/dan-io.sh` & `dan-build-0.2.4/completion/zsh/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/completion/zsh/dan.sh` & `dan-build-0.2.4/completion/zsh/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/cli/click.py` & `dan-build-0.2.4/dan/cli/click.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/cli/io.py` & `dan-build-0.2.4/dan/cli/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import asyncio
 import fnmatch
 import os
+import contextlib
 
 from dan.cli import click
 from dan.core.requirements import parse_package
 from dan.make import Make
 
 _make : Make = None
 async def get_make():
@@ -18,14 +19,15 @@
         (source_path / 'dan-build.py').touch()
         make = Make(source_path / 'build', quiet=True)
         make.config.source_path = str(source_path)
         make.config.build_path = str(source_path / 'build')
         make.config.toolchain = 'default'
         await make._config.save()
         await make.initialize()
+        _make = make
     return _make
 
 
 _repositories = None
 async def get_repositories():
     global _repositories
     if _repositories is None:
@@ -40,80 +42,92 @@
 async def get_repository(name = None):
     from dan.io.repositories import get_repo_instance
     await get_make()
     repo = get_repo_instance(name)
     await repo.build()
     return repo
 
+
+@contextlib.asynccontextmanager
+async def make_context():
+    make = await get_make()
+    with make.context:
+        yield
+
+
 @click.group()
 def cli():
     pass
 
 @cli.group()
 def ls():
     """Inspect stuff"""
     pass
 
 
 @ls.command()
 async def repositories():
     """List available repositories"""
-    repos = await get_repositories()
-    for repo in repos:
-        click.echo(repo.name)
+    async with make_context():
+        repos = await get_repositories()
+        for repo in repos:
+            click.echo(repo.name)
 
 @ls.command()
 async def libraries():
     """List available libraries"""
-    repos = await get_repositories()
-    for repo in repos:
-        for name, lib in repo.installed.items():
-            click.echo(f'{name} = {lib.version}')
+    async with make_context():
+        repos = await get_repositories()
+        for repo in repos:
+            for name, lib in repo.installed.items():
+                click.echo(f'{name} = {lib.version}')
 
 @ls.command()
 @click.argument('LIBRARY')
 async def versions(library: str):
     """Get LIBRARY's available versions"""
-    package, library, repository = parse_package(library)
-    repo = await get_repository(repository)
-    if repo is None:
-        click.logger.error(f'cannot find repository {repository}')
-        return -1
-
-    lib = repo.find(library, package)
-    if lib is None:
-        if repository is None:
-            repository = repo.name
-        if package is None:
-            package = library
-        click.logger.error(f'cannot find {package}:{library}@{repository}')
-        return -1
-    
-    from dan.src.github import GitHubReleaseSources
-    
-    sources: GitHubReleaseSources = lib.get_dependency(GitHubReleaseSources)
-    available_versions = await sources.available_versions()
-    available_versions = sorted(available_versions.keys())
-    for v in available_versions:
-        if v == lib.version:
-            click.echo(f' - {v} (default)')
-        else:
-            click.echo(f' - {v}')
+    async with make_context():
+        package, library, repository = parse_package(library)
+        repo = await get_repository(repository)
+        if repo is None:
+            click.logger.error(f'cannot find repository {repository}')
+            return -1
+
+        lib = repo.find(library, package)
+        if lib is None:
+            if repository is None:
+                repository = repo.name
+            if package is None:
+                package = library
+            click.logger.error(f'cannot find {package}:{library}@{repository}')
+            return -1
+        
+        from dan.src.github import GitHubReleaseSources
+        
+        sources: GitHubReleaseSources = lib.get_dependency(GitHubReleaseSources)
+        available_versions = await sources.available_versions()
+        available_versions = sorted(available_versions.keys())
+        for v in available_versions:
+            if v == lib.version:
+                click.echo(f' - {v} (default)')
+            else:
+                click.echo(f' - {v}')
 
 @cli.command()
 @click.argument('NAME')
 async def search(name):
     """Search for NAME in repositories"""
-    name = f'*{name}*'
-    repos = await get_repositories()
-    for repo in repos:
-        installed = repo.installed
-        for libname, lib in installed.items():
-            if fnmatch.fnmatch(libname, name):
-                click.echo(f'{libname} = {lib.version}')
+    async with make_context():
+        name = f'*{name}*'
+        repos = await get_repositories()
+        for repo in repos:
+            installed = repo.installed
+            for libname, lib in installed.items():
+                if fnmatch.fnmatch(libname, name):
+                    click.echo(f'{libname} = {lib.version}')
 
 
 def main():
     import sys
     try:
         cli(auto_envvar_prefix='DAN')
     except Exception as err:
@@ -123,7 +137,10 @@
         click.logger.debug(' '.join(traceback.format_tb(tb)))
         try:
             # wait asyncio loop to terminate
             asyncio.get_running_loop().run_until_complete()
         except Exception:
             pass
         return -1
+
+if __name__ == '__main__':
+    main()
```

### Comparing `dan-build-0.2.3/dan/cli/main.py` & `dan-build-0.2.4/dan/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import os
 import sys
-import logging
+from dan import logging
 import asyncio
 
 from dan.core.find import find_file
 from dan.core.pathlib import Path
 from dan.cli import click
 
+from dan.core import diagnostics
 from dan.core.cache import Cache
-from dan.cxx.targets import Executable
 from dan.core.settings import Settings
+from dan.cxx.targets import Executable
 
 
-from dan.make import ConfigCache, InstallMode, Make
+from dan.make import InstallMode, Make
 from dan.cli.vscode import Code
 
 
 _minimal_options = [
-    click.option('--build-path', '-B', 'path', help='Path where dan has been initialized.',
+    click.option('--build-path', '-B', help='Path where dan has been initialized.',
                  type=click.Path(resolve_path=True, path_type=Path), required=True, default='build', envvar='DAN_BUILD_PATH'),
-
 ]
 
 _common_opts = [
     *_minimal_options,
     click.option('--quiet', '-q', is_flag=True,
                  help='Dont print informations (errors only).', envvar='DAN_QUIET'),
     click.option('--verbose', '-v', is_flag=True,
                  help='Pring debug informations.', envvar='DAN_VERBOSE'),
     click.option('--jobs', '-j',
                  help='Maximum jobs.', default=None, type=int, envvar='DAN_JOBS'),
     click.option('--no-progress', is_flag=True,
                  help='Disable progress bars', envvar='DAN_NOPROGRESS'),
-    click.argument('TARGETS', nargs=-1),
 ]
 _base_help_ = '''
   PATH          Either build or source directory.
   [TARGETS...]  Targets to process.
 '''
 
 
@@ -68,89 +67,95 @@
         if self._make is None:
             self._make = Make(*self._make_args, **self._make_kwds)
         return self._make
 
 
 pass_context = click.make_pass_decorator(CommandsContext)
 
+@pass_context
+def show_diags(ctx: CommandsContext):
+    if diagnostics.enabled:
+        diags = ctx.make.diagnostics
+        if diags:
+            click.echo(f'DIAGNOSTICS: {diags.to_json()}')
 
 @click.group()
 @click.version_option(package_name='dan-build')
 @click.option('--quiet', '-q', is_flag=True,
               help='Dont print informations (errors only)')
 @click.option('--verbose', '-v', is_flag=True,
               help='Pring debug informations')
 @click.option('--jobs', '-j',
               help='Maximum jobs', default=None, type=int)
 @click.pass_context
-def cli(ctx, **kwds):
+def cli(ctx: click.AsyncContext, **kwds):
     ctx.obj = CommandsContext(**kwds)
+    ctx.call_on_close(show_diags)
 
 
 def available_toolchains():
     from dan.cxx.detect import get_toolchains
-    return ['default', *[name for name in get_toolchains()['toolchains'].keys()]]
+    return ['default', *[name for name in get_toolchains(create=False)['toolchains'].keys()]]
 
 
 _toolchain_choice = click.Choice(available_toolchains(), case_sensitive=False)
 
 
 @cli.command()
 @click.option('--verbose', '-v', is_flag=True,
               help='Pring debug informations')
 @click.option('--toolchain', '-t', help='The toolchain to use',
               type=_toolchain_choice)
 @click.option('--setting', '-s', 'settings', help='Set or change a setting', multiple=True, type=click.SettingsParamType(Settings))
 @click.option('--option', '-o', 'options', help='Set or change an option', multiple=True)
 @click.option('--build-path', '-B', help='Path where dan has been initialized.',
-              type=click.Path(resolve_path=True, path_type=Path), required=True, default='build')
+              type=click.Path(resolve_path=True, path_type=Path), required=True, default='build', envvar='DAN_BUILD_PATH')
 @click.option('--source-path', '-S', help='Path where source is located.',
               type=click.Path(resolve_path=True, path_type=Path), required=True, default='.')
-async def configure(verbose: bool, toolchain: str, settings: tuple[str], options: tuple[str], build_path: Path, source_path: Path):
+@pass_context
+async def configure(ctx: CommandsContext, toolchain: str, settings: tuple[str], options: tuple[str], source_path: Path, **kwds):
     """Configure dan project"""
-    logging.getLogger().setLevel(logging.DEBUG if verbose else logging.INFO)
-    config = ConfigCache(build_path / Make._config_name, )
-    config.data.source_path = config.data.source_path if hasattr(
-        config, 'source_path') else str(source_path)
-    config.data.build_path = str(build_path)
-    click.logger.info(f'source path: {config.data.source_path}')
-    click.logger.info(f'build path: {config.data.build_path}')
-    config.data.toolchain = toolchain or config.data.toolchain or click.prompt('Toolchain', type=_toolchain_choice, default='default')
-    await config.save()
-    Cache.ignore(config)
-    del config
-
-    if len(settings) or len(options):
-        make = Make(build_path, None, verbose, False)
-        await make.initialize()
+    ctx(**kwds)  # update kwds
+    if toolchain is None and ctx.make.config.toolchain is None:
+        toolchain = click.prompt('Toolchain', type=_toolchain_choice, default='default')
 
-        if len(options):
-            await make.apply_options(*options)
+    await ctx.make.configure(source_path, toolchain)
 
-        if len(settings):
-            await make.apply_settings(*settings)
+    if len(settings):
+        await ctx.make.apply_settings(*settings)
 
-        await make.cache.save()
+    # NOTE: intializing make after applying setting
+    #       to check settings are valid implicitly (cache save skipped)
+    await ctx.make.initialize()
+
+    if len(options):
+        await ctx.make.apply_options(*options)
 
 
 @cli.command()
 @click.option('--for-install', is_flag=True, help='Build for install purpose (will update rpaths [posix only])')
 @common_opts
+@click.option('--force', '-f', is_flag=True,
+              help='Clean before building')
+@click.argument('TARGETS', nargs=-1)
 @pass_context
-async def build(ctx: CommandsContext, **kwds):
+async def build(ctx: CommandsContext, force=False, **kwds):
     """Build targets"""
     ctx(**kwds)  # update kwds
+    if force:
+        await ctx.make.clean()
     await ctx.make.build()
-    from dan.cxx import target_toolchain
-    target_toolchain.compile_commands.update()
+    # from dan.cxx import target_toolchain
+    # target_toolchain.compile_commands.update()
 
 
 @cli.command()
 @common_opts
 @click.argument('MODE', type=click.Choice([v.name for v in InstallMode]), default=InstallMode.user.name)
+@click.argument('TARGETS', nargs=-1)
 @pass_context
 async def install(ctx: CommandsContext, mode: str, **kwargs):
     """Install targets"""
     ctx(**kwargs)
     mode = InstallMode[mode]
     await ctx.make.install(mode)
 
@@ -200,14 +205,15 @@
     """Inspect stuff"""
     pass
 
 @ls.command()
 @click.option('-a', '--all', 'all', is_flag=True, help='Show all targets (not only defaulted ones)')
 @click.option('-t', '--type', 'show_type', is_flag=True, help='Show target\'s type')
 @common_opts
+@click.argument('TARGETS', nargs=-1)
 @pass_context
 async def targets(ctx: CommandsContext, all: bool, show_type: bool, **kwargs):
     """List targets"""
     kwargs['quiet'] = True
     ctx(**kwargs)
     await ctx.make.initialize()
     out = []
@@ -217,14 +223,15 @@
         else:
             out.append(target.fullname)
     click.echo('\n'.join(out))
 
 
 @ls.command()
 @common_opts
+@click.argument('TARGETS', nargs=-1)
 @pass_context
 async def tests(ctx: CommandsContext, **kwargs):
     """List tests"""
     kwargs['quiet'] = True
     ctx(**kwargs)
     await ctx.make.initialize()
     for t in ctx.make.tests:
@@ -232,14 +239,15 @@
             for c in t.cases:
                 click.echo(f'{t.fullname}:{c.name}')
         else:
             click.echo(t.fullname)
 
 @ls.command()
 @common_opts
+@click.argument('TARGETS', nargs=-1)
 @pass_context
 async def options(ctx: CommandsContext, **kwargs):
     """List tests"""
     kwargs['quiet'] = True
     ctx(**kwargs)
     await ctx.make.initialize()
     for o in ctx.make.all_options:
@@ -254,138 +262,167 @@
     kwargs['quiet'] = True
     for name, _ in Make.toolchains()['toolchains'].items():
         click.echo(name)
 
 
 @cli.command()
 @common_opts
-async def clean(**kwargs):
+@click.argument('TARGETS', nargs=-1)
+@pass_context
+async def clean(ctx, **kwargs):
     """Clean generated stuff"""
-    await Make(**kwargs).clean()
+    ctx(**kwargs)
+    await ctx.make.clean()
 
 
 @cli.command()
 @common_opts
-async def run(**kwargs):
+@click.argument('TARGETS', nargs=-1)
+@pass_context
+async def run(ctx, **kwargs):
     """Run executable(s)"""
-    make = Make(**kwargs)
-    rc = await make.run()
+    ctx(**kwargs)
+    rc = await ctx.make.run()
     sys.exit(rc)
 
 
 @cli.command()
 @common_opts
-async def test(**kwargs):
+@click.argument('TARGETS', nargs=-1)
+@pass_context
+async def test(ctx, **kwargs):
     """Run tests"""
-    make = Make(**kwargs)
-    rc = await make.test()
+    ctx(**kwargs)
+    rc = await ctx.make.test()
     sys.exit(rc)
 
 
 @cli.command()
-@click.option('-s', '--script', help='Use a source script to resolve compilation environment')
-def scan_toolchains(script: str, **kwargs):
+@click.option('-s', '--script',
+              help='Use a source script to resolve compilation environment')
+@click.option('-p', '--path', 'paths',
+              help='Use given path for compilers lookup', multiple=True, type=click.Path(exists=True, file_okay=False))
+@click.option('--verbose', '-v', is_flag=True,
+              help='Pring debug informations.', envvar='DAN_VERBOSE')
+def scan_toolchains(script: str, paths: list[str], verbose, **kwargs):
     """Scan system toolchains"""
+    logging.getLogger().setLevel(logging.DEBUG if verbose else logging.INFO)
     from dan.cxx.detect import create_toolchains, load_env_toolchain
     if script:
         load_env_toolchain(script)
     else:
-        create_toolchains()
+        create_toolchains(paths if len(paths) else None)
 
 
 @cli.group()
 def code():
     """VS-Code specific commands"""
     pass
 
 
 @code.command()
 @common_opts
+@click.argument('TARGETS', nargs=-1)
 @pass_context
 async def get_targets(ctx: CommandsContext, **kwargs):
-    kwargs['quiet'] = True
+    kwargs.update({'quiet': True, 'diags': True})
     ctx(**kwargs)
     await ctx.make.initialize()
-    from dan.core.include import context
     out = []
-    targets = context.root.all_targets
+    targets = ctx.make.context.root.all_targets
     for target in targets:
         out.append({
             'name': target.name,
             'fullname': target.fullname,
             'buildPath': str(target.build_path),
             'output': str(target.output),
             'executable': isinstance(target, Executable),
             'type': type(target).__name__
         })
     import json
     click.echo(json.dumps(out))
 
 @code.command()
 @common_opts
+@click.argument('TARGETS', nargs=-1)
 @pass_context
 async def get_tests(ctx: CommandsContext, **kwargs):
-    kwargs['quiet'] = True
+    kwargs.update({'quiet': True, 'diags': True})
     ctx(**kwargs)
     await ctx.make.initialize()
-    from dan.core.include import context
     import json
     out = list()
-    for t in context.root.all_tests:
+    for t in ctx.make.context.root.all_tests:
         out.append(t.fullname)
         if len(t) > 1:
             for c in t.cases:
                 out.append(f'{t.fullname}:{c.name}')
     click.echo(json.dumps(out))
 
 
 @code.command()
 @common_opts
 @click.option('--pretty', is_flag=True)
+@click.argument('TARGETS', nargs=-1)
 @pass_context
 async def get_test_suites(ctx: CommandsContext, pretty, **kwargs):
-    kwargs['quiet'] = True
+    kwargs.update({'quiet': True, 'diags': True})
     ctx(**kwargs)
     await ctx.make.initialize()
     code = Code(ctx.make)
     click.echo(code.get_test_suites(pretty))
 
 
 @code.command()
 def get_toolchains(**kwargs):
     import json
     click.echo(json.dumps(list(Make.toolchains()['toolchains'].keys())))
 
 
 @code.command()
+@click.option('--for-install', is_flag=True, help='Build for install purpose (will update rpaths [posix only])')
+@common_opts
+@click.option('--force', '-f', is_flag=True,
+              help='Clean before building')
+@click.argument('TARGETS', nargs=-1)
+@pass_context
+async def build(ctx: CommandsContext, force=False, **kwds):
+    """Build targets (vscode version)"""
+    ctx(**kwds, diags=True)  # update kwds
+    if force:
+        await ctx.make.clean()
+    await ctx.make.build()
+
+
+@code.command()
 @minimal_options
 @click.argument('SOURCES', nargs=-1)
 @pass_context
 async def get_source_configuration(ctx: CommandsContext, sources, **kwargs):
-    kwargs['quiet'] = True
+    kwargs.update({'quiet': True, 'diags': True})
     ctx(**kwargs)
     await ctx.make.initialize()
     code = Code(ctx.make)
     click.echo(await code.get_sources_configuration(sources))
 
 
 @code.command()
 @minimal_options
 @pass_context
 async def get_workspace_browse_configuration(ctx: CommandsContext, **kwargs):
-    kwargs['quiet'] = True
+    kwargs.update({'quiet': True, 'diags': True})
     ctx(**kwargs)
     await ctx.make.initialize()
     code = Code(ctx.make)
     click.echo(await code.get_workspace_browse_configuration())
 
-
 @cli.result_callback()
-def process_result(result, **kwargs):
-    asyncio.run(Cache.save_all())
+@pass_context
+async def process_result(ctx, result, **kwargs):
+    await Cache.save_all()
 
 
 def main():
     import sys
     try:
         cli(auto_envvar_prefix='DAN')
     except Exception as err:
```

### Comparing `dan-build-0.2.3/dan/cli/vscode.py` & `dan-build-0.2.4/dan/cli/vscode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import json
 import os
+from pathlib import Path
+
+from dan.core.asyncio import ExceptionGroup
 from dan.core.pm import re_match
-from dan.cxx.toolchain import Toolchain
+from dan.cxx.toolchain import CompilationFailure, LinkageFailure, Toolchain
 
 from dan.make import Make
 from dan.cxx.targets import CXXObject
-
+from dan.logging import Logging
 
 def get_intellisense_mode(toolchain : Toolchain):
     mode = list()
     if toolchain.system is not None:
         mode.append(toolchain.system)
     mode.append(toolchain.type)
     mode.append(toolchain.arch)
     return '-'.join(mode)
 
-class Code:
+class Code(Logging):
     def __init__(self, make: Make) -> None:
         self.make = make
-    
+        super().__init__('code')
+
     def get_test_suites(self, pretty):
-        from dan.core.include import context, MakeFile
+        from dan.core.include import MakeFile
         from dan.core.test import Test, Case
         from dan.cxx import Executable
 
         def make_inner_test_info(test: Test, case: Case):
             basename = test.basename(case)
             out, err = test.outs(case)
             ident = f'{test.fullname}:{case.name}' if case.name is not None else test.fullname
@@ -93,28 +97,28 @@
                 return {
                     'type': 'suite',
                     'id': mf.fullname,
                     'label': mf.name,
                     'children': children
                 }
 
-        return json.dumps(make_suite_info(context.root), indent=2 if pretty else None)
+        return json.dumps(make_suite_info(self.make.context.root), indent=2 if pretty else None)
         
     async def _make_source_configuration(self, target: CXXObject):
             # interface:
             #   - includePath: string[]
             #   - defines: string[]
             #   - intelliSenseMode?: "linux-clang-x86" | "linux-clang-x64" | "linux-clang-arm" | "linux-clang-arm64" | "linux-gcc-x86" | "linux-gcc-x64" | "linux-gcc-arm" | "linux-gcc-arm64" | "macos-clang-x86" | "macos-clang-x64" | "macos-clang-arm" | "macos-clang-arm64" | "macos-gcc-x86" | "macos-gcc-x64" | "macos-gcc-arm" | "macos-gcc-arm64" | "windows-clang-x86" | "windows-clang-x64" | "windows-clang-arm" | "windows-clang-arm64" | "windows-gcc-x86" | "windows-gcc-x64" | "windows-gcc-arm" | "windows-gcc-arm64" | "windows-msvc-x86" | "windows-msvc-x64" | "windows-msvc-arm" | "windows-msvc-arm64" | "msvc-x86" | "msvc-x64" | "msvc-arm" | "msvc-arm64" | "gcc-x86" | "gcc-x64" | "gcc-arm" | "gcc-arm64" | "clang-x86" | "clang-x64" | "clang-arm" | "clang-arm64";
             #   - standard?: "c89" | "c99" | "c11" | "c17" | "c++98" | "c++03" | "c++11" | "c++14" | "c++17" | "c++20" | "gnu89" | "gnu99" | "gnu11" | "gnu17" | "gnu++98" | "gnu++03" | "gnu++11" | "gnu++14" | "gnu++17" | "gnu++20";
             #   - forcedInclude?: string[];
             #   - compilerPath?: string;
             #   - compilerArgs?: string[];
             #   - windowsSdkVersion?: string;
-            includes = []
-            defines = []
+            includes = await target.toolchain.get_default_include_paths()
+            defines = [f'{k}={v}' for k, v in (await target.toolchain.get_default_defines()).items()]
             await target.initialize()
             for flag in target.private_cxx_flags:
                 match re_match(flag):
                     case r'[/-]I:?(.+)' as m:
                         includes.append(os.path.normcase(m[1]))
                     case r'[/-]D:?(.+)' as m:
                         defines.append(m[1])
```

### Comparing `dan-build-0.2.3/dan/cmake/configure_file.py` & `dan-build-0.2.4/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/conan/requirements.py` & `dan-build-0.2.4/dan/conan/requirements.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,36 +50,37 @@
             self.output = self.output.with_suffix('.bat')
         else:
             self.output = self.output.with_suffix('.sh')
 
         self.conanfile = ConanFile(makefile=makefile)
         self.preload_dependencies.add(self.conanfile)
 
+        self.toolchain = self.context.get('cxx_target_toolchain')
+
     def _get_version(self, toolchain):
         from dan.cxx.msvc_toolchain import MSVCToolchain
         match toolchain:
             case MSVCToolchain():
                 return f'{toolchain.version.major}{str(toolchain.version.minor)[0]}'
             case _:
                 return str(toolchain.version.major)
             
     def add(self, pkg: 'Package'):
         self.conanfile.add(pkg)
 
     async def __build__(self):
-        from dan.cxx import target_toolchain
         dest = self.output.parent
         dest.mkdir(exist_ok=True, parents=True)
         await async_run([
             'conan', 'install', '.',
             f'--output-folder={dest}',
-            '-s', f'build_type={target_toolchain.build_type.name.title()}',
-            '-s', f'compiler={target_toolchain.type}',
-            '-s', f'compiler.version={self._get_version(target_toolchain)}',
-            '-s', f'compiler.cppstd={target_toolchain.cpp_std}',
+            '-s', f'build_type={self.toolchain.build_type.name.title()}',
+            '-s', f'compiler={self.toolchain.type}',
+            '-s', f'compiler.version={self._get_version(self.toolchain)}',
+            '-s', f'compiler.cppstd={self.toolchain.cpp_std}',
             '--build=missing'],
             logger=self._logger, cwd=self.build_path)
 
 class Package(Target, internal=True):
     def __get_requirements(self) -> Requirements:
         if not hasattr(self.makefile, '__conan_requirements__'):
             setattr(self.makefile, '__conan_requirements__', Requirements(makefile=self.makefile))
```

### Comparing `dan-build-0.2.3/dan/core/asyncio.py` & `dan-build-0.2.4/dan/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/core/cache.py` & `dan-build-0.2.4/dan/core/cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,77 @@
+import dataclasses
 import functools
 import json
+import pickle
 import aiofiles
 import typing as t
 
 
 from dan.core.pathlib import Path
 from dan.core import asyncio
 
 T = t.TypeVar('T', bound=dict)
 
 class Cache(t.Generic[T]):
     dataclass: T = dict
-    indent = 0
+    indent = None
     __caches: dict[str, 'Cache'] = dict()
 
     def __init_subclass__(cls) -> None:
         cls.dataclass = t.get_args(cls.__orig_bases__[0])[0]
         return super().__init_subclass__()
 
-    def __init__(self, path: Path|str, *args, cache_name:str = None, **kwargs):
+    def __init__(self, path: Path|str, *args, cache_name:str = None, binary=False, **kwargs):
         self.__path = Path(path)     
         self.__name = cache_name or path.stem   
-        assert not self.name in self.__caches, 'a cache type should be unique'
+        self.__serializer = json if not binary else pickle
+        if self.name in self.__caches:
+            other = Cache.get(self.name)
+            if other.path == self.path:
+                raise RuntimeError(f'Cache {self.name} already created, use Cache.instance')
+            else:
+                raise RuntimeError(f'Cache {self.name} is not unique, use cache_name to distinguish {other.path} from {self.path}')
+        assert not self.name in self.__caches, 'a cache should be unique'
         if self.path.exists():
-            with open(self.path, 'r') as f:
-                if self.dataclass == dict:
-                    self.__data = json.load(f)
-                else:
+            with open(self.path, 'rb') as f:
+                if dataclasses.is_dataclass(self.dataclass):
                     self.__data = self.dataclass.from_json(f.read())
+                else:
+                    self.__data = self.__serializer.load(f)
                 if not isinstance(self.__data, self.dataclass):
                     self.__data = self.dataclass(**self.__data)
                 self.__modification_date = self.path.modification_time
         else:
             self.__data = self.dataclass(*args, **kwargs)
             self.__modification_date = 0.0
         
         self.__initial_state = self._dump()
         self.__dirty = False
         self.__caches[self.name] = self
     
-    def _dump(self):
-        if self.dataclass == dict:
-            return json.dumps(self.data, indent=self.indent)
+    @classmethod
+    def instance(cls, path: Path|str, *args, cache_name:str = None, **kwargs):
+        cache_name = cache_name or path.stem
+        if cache_name in cls.__caches:
+            return cls.__caches[cache_name]
+        return cls(path, *args, cache_name=cache_name, **kwargs)
+
+    @classmethod
+    def clear_all(cls):
+        del cls.__caches
+        cls.__caches = dict()
+    
+    def _dump(self):        
+        if self.__serializer is pickle:
+            return self.__serializer.dumps(self.data)
         else:
-            return self.data.to_json(indent=self.indent)
+            if self.dataclass == dict:
+                return self.__serializer.dumps(self.data).encode()
+            else:
+                return self.data.to_json(indent=self.indent).encode()
 
     
     @property
     def path(self):
         return self.__path
     
     @property
@@ -65,16 +89,17 @@
             self.__dirty = self.__initial_state != self.__state
         return self.__dirty
     
     async def save(self, force=False):
         if self.path and (self.dirty or force):
             if self.__state:
                 self.path.parent.mkdir(exist_ok=True, parents=True)
-                async with aiofiles.open(self.path, 'w') as f:
+                async with aiofiles.open(self.path, 'wb') as f:
                     await f.write(self.__state)
+                self.__dirty = False
 
     @classmethod
     async def save_all(cls):
         async with asyncio.TaskGroup('saving caches') as group:
             for c in cls.__caches.values():
                 if c.dirty:
                     group.create_task(c.save())
```

### Comparing `dan-build-0.2.3/dan/core/find.py` & `dan-build-0.2.4/dan/core/find.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import os
 from dan.core.pathlib import Path
 import re
+import typing as t
 
 include_paths_lookup = [
     '~/.local/include',
     '/usr/local/include',
     '/usr/include',
 ]
 
@@ -28,46 +29,49 @@
     r = re.compile(expr)
     for path in paths:
         for root, _, files in os.walk(os.path.expandvars(os.path.expanduser(path))):
             for file in files:
                 if r.match(file):
                     return Path(root) / file
 
-def find_files(expr, paths) -> list[Path]:
+
+def find_files(expr, paths) -> t.Generator[Path, None, None]:
     r = re.compile(expr)
-    files = list()
     for path in paths:
         for root, _, _files in os.walk(os.path.expandvars(os.path.expanduser(path))):
             for file in _files:
                 if r.match(file):
-                    files.append(Path(root) / file)
-    return files
+                    yield (Path(root) / file)
 
 
-def find_include_path(name, paths=list()) -> Path:
+def find_include_path(name, paths: list[str|Path] = None) -> Path:
+    paths = paths or list()
     return find_file(name, [*paths, *include_paths_lookup])
 
 
-def find_library(name, paths=list()) -> Path:
+def find_library(name, paths: list[str|Path] = None) -> Path:
+    paths = paths or list()
     if os.name == 'posix':
         expr = fr'lib{name}\.(so|a)'
     elif os.name == 'nt':
         expr = fr'lib{name}\.(lib|dll)'
     return find_file(expr, [*paths, *library_paths_lookup])
 
-def find_executable(name, paths=list(), default_paths=True) -> Path:
+def find_executable(name, paths: list[str|Path] = None, default_paths=True) -> Path:
+    paths = paths or list()
     if os.name == 'posix':
         expr = name + '$'
     elif os.name == 'nt':
         expr = f'{name}.exe$'
     if default_paths:
         paths.extend(programs_paths_lookup)
     return find_file(expr, paths)
 
-def find_executables(name, paths=list(), default_paths=True) -> list[Path]:
+def find_executables(name, paths: list[str|Path] = None, default_paths=True) -> t.Generator[Path, None, None]:
+    paths = paths or list()
     if os.name == 'posix':
         expr = name + '$'
     elif os.name == 'nt':
         expr = f'{name}.exe$'
     if default_paths:
         paths.extend(programs_paths_lookup)
-    return find_files(expr, paths)
+    yield from find_files(expr, paths)
```

### Comparing `dan-build-0.2.3/dan/core/functools.py` & `dan-build-0.2.4/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/core/include.py` & `dan-build-0.2.4/dan/core/include.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import contextmanager
 import importlib.util
 import os
 
 from dan.core.asyncio import sync_wait
 from dan.core.makefile import MakeFile
 from dan.core.pathlib import Path
 from dan.core.requirements import load_requirements
@@ -32,14 +33,16 @@
 
 
 class Context(Logging):
     def __init__(self) -> None:
         self.__root: MakeFile = None
         self.__current: MakeFile = None
         self.__all_makefiles: set[MakeFile] = set()
+        self.imported_makefiles: dict[Path, MakeFile] = dict()
+        self.__prev_ctx: Context = None
         super().__init__('context')
 
     @property
     def root(self):
         return self.__root
 
     @property
@@ -71,28 +74,32 @@
         if default is not None:
             setattr(self, name, default)
             return default
 
     def set(self, name, value):
         setattr(self, name, value)
 
-
-context = Context()
-
-
-def context_reset():
-    """Reset whole context
-
-    Mainly used for test purpose
-    """
-    global context
-    for m in context.all_makefiles:
-        del m
-    del context
-    context = Context()
+    def __enter__(self):
+        global context
+        self.__prev_ctx = context
+        context = self
+        return self
+
+    def __exit__(self, *exc):
+        global context
+        context = self.__prev_ctx
+        self.__prev_ctx = None
+
+
+context: Context = Context()
+
+class MakeFileError(RuntimeError):
+    def __init__(self, path) -> None:
+        self.path = Path(path)
+        super().__init__(f'failed to load {self.path}')
 
 
 def _init_makefile(module, name: str = 'root', build_path: Path = None, requirements: MakeFile = None, parent: MakeFile = None):
     global context
     source_path = Path(module.__file__).parent
     if parent is None and context.current is not None:
         parent = context.current
@@ -106,27 +113,29 @@
     module._setup(
         name,
         source_path,
         build_path,
         requirements,
         parent)
 
-_imported_makefiles: dict[Path, MakeFile] = dict()
-
 def load_makefile(module_path: Path, name: str = None, module_name: str = None, build_path: Path = None, requirements: MakeFile = None, parent: MakeFile = None) -> MakeFile:
     name = name or module_path.stem
     module_name = module_name or name
-    if module_path in _imported_makefiles:
-        return _imported_makefiles[module_path]
+    if module_path in context.imported_makefiles:
+        return context.imported_makefiles[module_path]
     spec = importlib.util.spec_from_file_location(
         module_name, module_path)
     module = importlib.util.module_from_spec(spec)
-    _imported_makefiles[module_path] = module
+    context.imported_makefiles[module_path] = module
     _init_makefile(module, name, build_path, requirements, parent)
-    spec.loader.exec_module(module)
+    try:
+        spec.loader.exec_module(module)
+    except Exception as err:
+        context.error('makefile error while loading \'%s\': %s', module_path, err)
+        raise MakeFileError(module_path) from err
     context.up()
     return module
 
 
 def include_makefile(name: str | Path, build_path: Path = None) -> set[Target]:
     ''' Include a sub-directory (or a sub-makefile).
     :returns: The set of exported targets.
@@ -149,31 +158,34 @@
                 spec = importlib.util.spec_from_file_location(
                     f'{context.current.name}.{name}', module_path)
                 break
         else:
             raise RuntimeError(
                 f'Cannot find anything to include for "{name}" (looked for: {", ".join(lookups)})')
         
-    if module_path in _imported_makefiles:
-        return _imported_makefiles[module_path]
+    if module_path in context.imported_makefiles:
+        return context.imported_makefiles[module_path]
 
     module = importlib.util.module_from_spec(spec)
-    _imported_makefiles[module_path] = module
+    context.imported_makefiles[module_path] = module
     _init_makefile(module, name, build_path)
 
     requirements_file = module_path.with_stem('dan-requires')
     if module_path.stem == 'dan-build' and requirements_file.exists():
         context.current.requirements = load_makefile(
             requirements_file, name='dan-requires', module_name=f'{name}.requirements')
 
     try:
         spec.loader.exec_module(module)
     except TargetNotFound as err:
         if len(context.missing) == 0:
             raise err
+    except Exception as err:
+        context.error('makefile error while including \'%s\': %s', module_path, err)
+        raise MakeFileError(module_path) from err
     context.up()
 
 
 def include(*names: str | Path) -> list[Target]:
     """Include one (or more) subdirectory (or named makefile).
 
     :param names: One (or more) subdirectory or makefile to include.
```

### Comparing `dan-build-0.2.3/dan/core/makefile.py` & `dan-build-0.2.4/dan/core/makefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,26 @@
         self.children: list[MakeFile] = list()
         if self.name != 'dan-requires' and self.parent:
             self.parent.children.append(self)
         self.options = Options(self)
         self.__targets: set[Target] = set()
         self.__tests: set[Test] = set()
 
+        from dan.core.include import context
+        self.context = context
+
     @property
     def fullname(self):
         return f'{self.parent.fullname}.{self.name}' if self.parent else self.name
 
     @property
     def cache(self) -> Cache:
         if not self.__cache:
             self.__cache = Cache(
-                self.build_path / f'{self.name}.cache.json', cache_name=self.fullname)
+                self.build_path / f'{self.name}.cache', cache_name=self.fullname, binary=True)
         return self.__cache
 
     def register(self, cls: type[Target | Test]):
         """Register Target/Test class"""
         if issubclass(cls, Target):
             self.__targets.add(cls())
         if issubclass(cls, Test):
@@ -50,15 +53,15 @@
         return cls
 
     def wraps(self, cls: type[Target]):
         def decorator(new_cls: type[Target]):
             assert issubclass(
                 new_cls, cls), 'Target wrapper must inherit from original target'
             for t in self.__targets:
-                if isinstance(t, cls):
+                if type(t) == cls:
                     self.__targets.remove(t)
                     return cls
             assert False, 'Original target has not been registered'
         return decorator
 
     def find(self, name_or_class) -> Target:
         """Find a target.
```

### Comparing `dan-build-0.2.3/dan/core/osinfo.py` & `dan-build-0.2.4/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/core/pathlib.py` & `dan-build-0.2.4/dan/core/pathlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
     def younger_than(self, other):
         time = other if isinstance(other, float) else other.modification_time
         assert isinstance(time, float)
         return self.modification_time > time
 
     def older_than(self, other):
-        return not self.younger_than(other)
+        time = other if isinstance(other, float) else other.modification_time
+        assert isinstance(time, float)
+        return self.modification_time < time
 
     def utime(self, *args, **kw_args):
         os.utime(self, *args, **kw_args)
 
     @property
     def is_empty(self):
         if os.path.exists(self) and not os.path.isfile(self):
```

### Comparing `dan-build-0.2.3/dan/core/pm.py` & `dan-build-0.2.4/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/core/register.py` & `dan-build-0.2.4/dan/core/register.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,11 +12,15 @@
     def get_static_makefile(cls):
         return cls.__makefile
 
     @property
     def makefile(self):
         return self.__makefile
     
+    @property
+    def context(self):
+        return self.__makefile.context
+    
     @makefile.setter
     def makefile(self, value) -> 'MakeFile':
         assert self.__makefile is None, 'makefile should be set once'
         self.__makefile = value
```

### Comparing `dan-build-0.2.3/dan/core/requirements.py` & `dan-build-0.2.4/dan/core/requirements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 
 import functools
-import re
 import typing as t
 from dan.core import asyncio
 from dan.core.pm import re_match
 from dan.core.settings import InstallMode, InstallSettings
 
-from dan.core.version import Version, VersionSpec
+from dan.core.version import VersionSpec
 from dan.logging import Logging
 
 def parse_package(name: str) -> tuple[str, str, str]:
     """Parse package name
     
     :returns: package, library, repository"""
     match re_match(name):
@@ -83,15 +82,14 @@
     else:
         return RequiredPackage(req)
 
 async def load_requirements(requirements: t.Iterable[RequiredPackage], makefile, logger = None, install = True):
 
     from dan.pkgconfig.package import find_package
     from dan.logging import _get_makefile_logger
-    from dan.core.include import context
     from dan.io import Package
 
     if logger is None:
         logger = _get_makefile_logger()
 
     deps_install_path = makefile.pkgs_path
     deps_settings = InstallSettings(deps_install_path)
@@ -105,15 +103,15 @@
 
     async with asyncio.TaskGroup('requirement loading') as group:
         for req in requirements:
             if req.found:
                 resolved.append(req)
                 continue
 
-            t = context.root.find(req.name)
+            t = makefile.context.root.find(req.name)
             if t and not t.is_requirement and req.is_compatible(t):
                 logger.debug('%s: already fullfilled by %s', req, t.fullname)
                 req.target = t
                 resolved.append(req)
                 continue
 
             t = find_package(req.name, req.version_spec, search_paths=pkgs_search_paths, makefile=makefile)
@@ -125,15 +123,16 @@
                 if makefile.requirements:
                     # install requirement from dan-requires.py
                     t = makefile.requirements.find(req.name)
                     if not t:
                         raise RuntimeError(f'Unresolved requirement {req}, it should have been defined in {makefile.requirements.__file__}')
                     logger.debug('%s using requirements\' target %s', req, t.fullname)
                 else:
-                    t = Package(req.name, req.version_spec, package=req.package, repository=req.repository, makefile=makefile)
+                    with makefile.context:
+                        t = Package(req.name, req.version_spec, package=req.package, repository=req.repository, makefile=makefile)
                     logger.debug('%s: adding package %s', req, t.fullname)
                 unresolved.append(req)
                 group.create_task(t.install(deps_settings, InstallMode.dev))
 
 
 
     if install:
```

### Comparing `dan-build-0.2.3/dan/core/runners.py` & `dan-build-0.2.4/dan/core/runners.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,22 +18,64 @@
         self.stderr = stderr
 
 
 _encoding = 'cp1252' if os.name == 'nt' else 'utf-8'
 
 
 async def log_stream(stream, *files):
-    while not stream.at_eof():
-        data = await stream.readline()
-        line = data.decode(_encoding)
-        for file in files:
-            if file in [sys.stdout, sys.stderr]:
-                tqdm.tqdm.write(line, end='', file=file)
-            else:
-                file.write(line)
+    with stream as lines:
+        async for line in lines:
+            for file in files:
+                if file in [sys.stdout, sys.stderr]:
+                    tqdm.tqdm.write(line, end='', file=file)
+                else:
+                    file.write(line)
+
+
+class AsyncStreamProducer:
+    
+    class Iterator:
+        def __init__(self) -> None:
+            self.q = asyncio.Queue()
+
+        async def __aiter__(self):
+            while True:
+                line = await self.q.get()
+                if line is None:
+                    self.q.task_done()
+                    return
+                yield line
+                self.q.task_done()
+
+    def __init__(self, stream) -> None:
+        self.stream = stream
+        self.__iterators: list[AsyncStreamProducer.Iterator] = list()
+
+    async def __notify(self, data):
+        asyncio.gather(*[it.q.put(data) for it in self.__iterators])
+        asyncio.gather(*[it.q.join() for it in self.__iterators])
+    
+    async def consume(self):
+        while not self.stream.at_eof():
+            data = await self.stream.readline()
+            if len(data) == 0:
+                continue
+            line = data.decode(_encoding)
+            await self.__notify(line)
+
+        await self.__notify(None)
+    
+    def __enter__(self):
+        it = self.Iterator()
+        self.__iterators.append(it)
+        return it
+
+    def __exit__(self, *exc):
+        pass
+
 
 _jobs_sem: asyncio.Semaphore = None
 
 
 def max_jobs(count=1):
     global _jobs_sem
     if count > 0:
@@ -103,44 +145,73 @@
                 escaped = False
 
     if current:
         result.append(''.join(current))
 
     return result
 
-async def async_run(command, log=True, logger: logging.Logger = None, no_raise=False, env=None, cwd=None):
+async def async_run(command, log=True, logger: logging.Logger = None, no_raise=False, env=None, cwd=None, out_capture=None, err_capture=None, all_capture=None, input: str = None) -> tuple[str, str, int]:
     if _jobs_sem is not None:
         await _jobs_sem.acquire()
     try:
         if not isinstance(command, str):
             command = subprocess.list2cmdline(command)
-        if env:
+        if env is not None:
             e = dict(os.environ)
             for k, v in env.items():
                 e[k] = v
             env = e
-        if logger:
-            logger.debug(f'executing: {command}')
+        if input is not None:
+            stdin = asyncio.subprocess.PIPE
+        else:
+            stdin = None
+        if logger is not None:
+            logger.debug('executing: %s', command)
         proc = await asyncio.subprocess.create_subprocess_shell(command,
                                                                 stdout=asyncio.subprocess.PIPE,
                                                                 stderr=asyncio.subprocess.PIPE,
+                                                                stdin=stdin,
                                                                 env=env,
                                                                 cwd=cwd)
-
         out = io.StringIO()
         err = io.StringIO()
         outs = [out]
         errs = [err]
         if log:
             outs.append(sys.stdout)
             errs.append(sys.stderr)
 
+        out_iter = AsyncStreamProducer(proc.stdout)
+        err_iter = AsyncStreamProducer(proc.stderr)
+
+        futures = [
+            log_stream(out_iter, *outs),
+            log_stream(err_iter, *errs),
+        ]
+
+        if all_capture is not None:
+            out_capture = err_capture = all_capture
+
+        if out_capture is not None:
+            futures.append(out_capture(out_iter))
+
+        if err_capture is not None:
+            futures.append(out_capture(err_iter))
+
+        futures.extend([
+            out_iter.consume(),
+            err_iter.consume(),
+        ])
+        
+        if input is not None:
+            proc.stdin.write(input.encode())
+            proc.stdin.write_eof()
+    
         await asyncio.gather(
-            log_stream(proc.stdout, *outs),
-            log_stream(proc.stderr, *errs),
+            *futures,
             proc.wait())
         # make sure return code is available
         await proc.communicate()
         out = out.getvalue()
         err = err.getvalue()
         if proc.returncode != 0 and not no_raise:
             message = f'command returned {proc.returncode}: {command}\n{out}\n{err}'
@@ -158,14 +229,19 @@
         command = subprocess.list2cmdline(command)
     if pipe:
         stdout = subprocess.PIPE
     else:
         stdout = None
     if logger:
         logger.debug(f'executing: {command}')
+    if env:
+        e = dict(os.environ)
+        for k, v in env.items():
+            e[k] = v
+        env = e
     proc = subprocess.Popen(command,
                             stdout=stdout,
                             stderr=stdout,
                             shell=shell,
                             env=env,
                             cwd=cwd,
                             universal_newlines=True)
```

### Comparing `dan-build-0.2.3/dan/core/settings.py` & `dan-build-0.2.4/dan/core/settings.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/core/target.py` & `dan-build-0.2.4/dan/core/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from functools import cached_property
 import functools
 from dan.core.register import MakefileRegister
 from dan.core.pathlib import Path
 from typing import Any, Callable, Iterable, Union, TypeAlias
 import inspect
 
-from dan.core import asyncio, aiofiles, utils
+from dan.core import asyncio, aiofiles, utils, diagnostics as diags
+from dan.core.cache import Cache
 from dan.core.requirements import load_requirements
 from dan.core.settings import InstallMode, InstallSettings, safe_load
 from dan.core.version import Version
 from dan.logging import Logging
 
 
 class Dependencies:
@@ -159,21 +160,21 @@
                 cache[parent.name] = dict()
             cache = cache[parent.name]
         else:
             cache = parent.cache.data
         if not 'options' in cache:
             cache['options'] = dict()
         self._cache = cache['options']
-        self.__items: set[Option] = set()
+        self.__items: list[Option] = list()
         self.update(default)
 
     def add(self, name: str, default_value, help=None):
         opt = Option(self, f'{self.__parent.fullname}.{name}',
                      default_value, help=help)
-        self.__items.add(opt)
+        self.__items.append(opt)
         return opt
 
     def get(self, name: str):
         for o in self.__items:
             if name in {o.name, o.fullname}:
                 return o
 
@@ -189,14 +190,22 @@
                     v = v[0]
                 case _:
                     pass
             if self[k]:
                 self[k] = v
             else:
                 self.add(k, v, help)
+    
+    @property
+    def sha1(self):
+        import hashlib
+        sha1 = hashlib.sha1()
+        for o in self.__items:
+            sha1.update(o.fullname.encode() + str(o.value).encode())
+        return sha1.hexdigest()
 
     def items(self):
         for o in self.__items:
             yield o.name, o.value
 
     def __getattr__(self, name):
         opt = self.get(name)
@@ -279,15 +288,16 @@
 
         if type(self).output != Target.output:
             # hack class-defined output
             #   transform it to classproperty for build_path resolution
             output = self.output
             type(self).output = utils.classproperty(lambda: self.build_path / output)
 
-    
+        self.diagnostics = diags.DiagnosticCollection()
+
     @property
     def output(self):
         if self._output is None:
             return None
         return self.build_path / self._output
     
     @property
@@ -377,24 +387,28 @@
         res = self.__initialize__()
         if inspect.iscoroutine(res):
             res = await res
         return res
 
     @property
     def modification_time(self):
-        return self.output.stat().st_mtime if self.output.exists() else 0.0
+        output = self.build_path / f'{self.name}.stamp' if self.output is None else self.output  
+        return output.stat().st_mtime if output.exists() else 0.0
 
     @property
     def up_to_date(self):
-        if self.output and not self.output.exists():
+        output = self.build_path / f'{self.name}.stamp' if self.output is None else self.output
+        if output and not output.exists():
             return False
         elif not self.dependencies.up_to_date:
             return False
         elif self.dependencies.modification_time > self.modification_time:
             return False
+        elif 'options_sha1' in self.cache and self.cache['options_sha1'] != self.options.sha1:
+            return False
         return True
 
     async def _build_dependencies(self):
         async with asyncio.TaskGroup(f'building {self.name}\'s target dependencies') as group:
             for dep in self.target_dependencies:
                 group.create_task(dep.build())
 
@@ -407,42 +421,48 @@
         result = self.__prebuild__()
         if inspect.iscoroutine(result):
             await result
 
         if self.up_to_date:
             self.info('up to date !')
             return
-        elif self.output.exists():
+        elif self.output is not None and self.output.exists():
             self.info('outdated !')
 
         with utils.chdir(self.build_path):
             self.info('building...')
+            if diags.enabled:
+                self.diagnostics.clear()
             result = self.__build__()
             if inspect.iscoroutine(result):
-                return await result
+                result = await result
+            if self.output is None:
+                (self.build_path / f'{self.name}.stamp').touch()
+            self.cache['options_sha1'] = self.options.sha1
             return result
 
     @property
     def target_dependencies(self):
         return [t for t in {*self.dependencies, *self.preload_dependencies} if isinstance(t, Target)]
 
     @property
     def file_dependencies(self):
         return [t for t in self.dependencies if isinstance(t, FileDependency)]
 
     @asyncio.cached
     async def clean(self):
         await self.initialize()
         async with asyncio.TaskGroup(f'cleaning {self.name} outputs') as group:
-            if self.output and self.output.exists():
+            output = self.build_path / f'{self.name}.stamp' if self.output is None else self.output
+            if output and output.exists():
                 self.info('cleaning...')
-                if self.output.is_dir():
-                    group.create_task(aiofiles.rmtree(self.output))
+                if output.is_dir():
+                    group.create_task(aiofiles.rmtree(output, force=True))
                 else:
-                    group.create_task(aiofiles.os.remove(self.output))
+                    group.create_task(aiofiles.os.remove(output))
             for f in self.other_generated_files:
                 if f.exists():
                     group.create_task(aiofiles.os.remove(f))
             res = self.__clean__()
             if inspect.iscoroutine(res):
                 group.create_task(res)
```

### Comparing `dan-build-0.2.3/dan/core/test.py` & `dan-build-0.2.4/dan/core/test.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/core/utils.py` & `dan-build-0.2.4/dan/core/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import inspect
 from dan.core.pathlib import Path
 import os
 
 
 class chdir:
-    def __init__(self, path: Path, create=True):
+    def __init__(self, path: Path, create=True, strict=False):
         self.path = path
+        self.strict = strict
         if create:
             self.path.mkdir(parents=True, exist_ok=True)
         self.prev = None
 
     def __enter__(self):
         self.prev = Path.cwd()
         os.chdir(self.path)
         return None
 
     def __exit__(self, *args):
-        os.chdir(self.prev)
+        try:
+            os.chdir(self.prev)
+        except OSError:
+            if self.strict:
+                raise
 
 
 def unique(*seqs):
     seen = set()
     full = list()
     for seq in seqs:
         full.extend(seq)
```

### Comparing `dan-build-0.2.3/dan/core/version.py` & `dan-build-0.2.4/dan/core/version.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/core/win.py` & `dan-build-0.2.4/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/cxx/__init__.py` & `dan-build-0.2.4/dan/cxx/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,33 @@
 
 from dan.core.errors import InvalidConfiguration
 from dan.core.settings import Settings
 from dan.cxx.toolchain import Toolchain
 from dan.cxx.detect import get_toolchains
 
 target_toolchain: Toolchain = None
+"""The target toolchain.
+"""
+
 host_toolchain: Toolchain = None
+"""The host toolchain.
+"""
 
 class __LazyContext(sys.__class__):
+    """Base class for the cxx module.
+
+    It overloads some context dependent properties exposed by this module, eg.: target and host toolchains.
+    """
     @property
-    def target_toolchain(__):
+    def target_toolchain(__) -> Toolchain:
         from dan.core.include import context
         return context.get('cxx_target_toolchain')
 
     @property
-    def host_toolchain(__):
+    def host_toolchain(__) -> Toolchain:
         from dan.core.include import context
         return context.get('cxx_host_toolchain')
     
 
 sys.modules[__name__].__class__ = __LazyContext
 
 
@@ -45,15 +54,15 @@
             tc_type = UnixToolchain
         case 'msvc':
             from .msvc_toolchain import MSVCToolchain
             tc_type = MSVCToolchain
         case _:
             raise InvalidConfiguration(f'Unhandeld toolchain type: {tc_type}')
     target_settings = settings.target
-    cache = Cache.get('dan.cache').data
+    cache = Cache.get('dan').data
     if not 'toolchains' in cache:
         cache['toolchains'] = {
             'host': dict(),
             'target': dict(),
         }
     target_toolchain = tc_type(toolchain_data, data['tools'], settings=target_settings, cache=cache['toolchains']['target'])
     target_toolchain.init()
@@ -64,28 +73,10 @@
         logging.warning(f'Cross compilation is currently not tested !')
         host_toolchain = None
 
     from dan.core.include import context
     context.set('cxx_target_toolchain', target_toolchain)
     context.set('cxx_host_toolchain', host_toolchain)
 
-def __pick_arg(*names, env=None, default=None):
-    import sys
-    import os
-    if env:
-        value = os.getenv(env, None)
-        if value:
-            return value
-    for name in names:
-        try:
-            return sys.argv[sys.argv.index(name) + 1]
-        except ValueError:
-            continue
-    return default
-
-#def __init_toolchains():
-#    init_toolchains(__pick_arg('-t', '--toolchain', env='DAN_TOOLCHAIN'))
-
-#__init_toolchains()
 
 from .targets import Executable, Library, LibraryType, Module
 from .targets import CXXObjectsTarget as Objects
```

### Comparing `dan-build-0.2.3/dan/cxx/compile_commands.py` & `dan-build-0.2.4/dan/cxx/compile_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 import json
 from dan.core.pathlib import Path
 import subprocess
 
 
 class CompileCommands:
-    def __init__(self) -> None:
-        from dan.core.include import context
-        self.cc_path: Path = context.root.build_path / 'compile_commands.json'
+    def __init__(self, path) -> None:
+        self.cc_path: Path = path / 'compile_commands.json'
         if self.cc_path.exists():
             with open(self.cc_path, 'r') as cc_f:
                 try:
                     self.data = json.load(cc_f)
                 except json.JSONDecodeError:
                     self.data = list()
         else:
```

### Comparing `dan-build-0.2.3/dan/cxx/detect.py` & `dan-build-0.2.4/dan/cxx/detect.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-import logging
 import os
 from dan.core.pathlib import Path
 import subprocess
 import sys
 import tempfile
 import functools
 
-import yaml
+import json
+import pickle
 from dan.core.find import find_executable
 
-from dan.core.osinfo import info as osinfo
+from dan import logging
 from dan.core.runners import sync_run
 from dan.core.version import Version
 from dan.core.win import vswhere
 
 
 class CompilerId:
     def __init__(self, name: str, version: Version, arch: str, system: str) -> None:
         self.name = name
         self.version = version
         self.arch = arch
         self.system = system
 
     def __str__(self) -> str:
         return f'{self.name}-{self.version}'
-
+    
+    @property
+    def is_unix(self):
+        return self.system not in ('windows', )
 
 GCC = "gcc"
 LLVM_GCC = "llvm-gcc"  # GCC frontend with LLVM backend
 CLANG = "clang"
 APPLE_CLANG = "apple-clang"
 SUNCC = "suncc"
 VISUAL_STUDIO = "Visual Studio"
@@ -88,15 +91,22 @@
     for d in defs:
         if d in defines:
             return True
     return False
 
 def get_target_system(defines: dict[str, str]) -> str:
     system = None
-    if dict_contains(defines, '_WIN32', '_WIN64'):
+    if dict_contains(defines, '__MSYS__', '__MINGW32__'):
+        if dict_contains(defines, '__MINGW64__'):
+            system = 'msys-mingw64'
+        elif dict_contains(defines, '__MINGW32__'):
+            system = 'msys-mingw32'
+        else:
+            system = 'msys'
+    elif dict_contains(defines, '_WIN32', '_WIN64'):
         system = 'windows'
     elif dict_contains(defines, '__ANDROID__'):
         system = 'android'
     elif dict_contains(defines, '__linux__'):
         system = 'linux'
     elif dict_contains(defines, '__sun'):
         system = 'sun'
@@ -221,15 +231,15 @@
     # "-dM" generate list of #define directives
     # "-E" run only preprocessor
     # "-x c" compiler as C code
     # the output is of lines in form of "#define name value"
     'gcc': ['-dM', '-E', '-x', 'c'],
     'clang': ['-dM', '-E', '-x', 'c'],
     'clang-cl': ['--driver-mode=g++', '-dM', '-E', '-x', 'c'],
-    'sun-cc': ['-c', '-xdumpmacros'], 
+    'sun-cc': ['-c', '-xdumpmacros'],
     # cl (Visual Studio, MSVC)
     # "/nologo" Suppress Startup Banner
     # "/E" Preprocess to stdout
     # "/B1" C front-end
     # "/c" Compile Without Linking
     # "/TC" Specify Source File Type
     'msvc': ['/nologo', '/E', '/B1', str(__detect_cmd), '/c', '/TC'],
@@ -256,40 +266,50 @@
                         name, value = token.split('=', 2)
                     else:
                         name, value = token, '1'
                     defines[name] = value
             break
     return defines
 
-def get_compiler_defines(executable: str, compiler_type: str, options: list[str], env=None):
+def get_compiler_defines(executable: str, compiler_type: str, options: list[str], env=None) -> dict[str, str]:
+    if env is None:
+        env = dict()
+    env['LC_LOCAL'] = 'C'
     with tempfile.TemporaryDirectory(prefix='dan-dci-') as tmpdir:
         output, _, rc = sync_run(
                 [executable, *detectors[compiler_type], *options, str(__empty_source)], env=env, cwd=tmpdir)
         return parse_compiler_defines(output)
 
 
-def detect_compiler_id(executable, env=None):
+def detect_compiler_id(executable, env=None, logger=None):
     # use a temporary file, as /dev/null might not be available on all platforms
     with tempfile.TemporaryDirectory(prefix='dan-dci-') as tmpdir:
         for name, detector in detectors.items():
             output, _, rc = sync_run(
-                [executable, *detector, str(__empty_source)], no_raise=True, env=env, cwd=tmpdir)
+                [executable, *detector, str(__empty_source)], no_raise=True, env=env, cwd=tmpdir, logger=logger)
             if 0 == rc:
                 defines = parse_compiler_defines(output)
                 compiler = _parse_compiler_version(defines)
                 if compiler is None:
                     continue
                 return compiler
         return None
 
 
 class Compiler:
-    def __init__(self, path: Path, env: dict[str, str] = None, tools: dict[str, Path] = dict()) -> None:
+    def __init__(self, path: Path, env: dict[str, str] = None, tools: dict[str, Path] = dict(), logger=None) -> None:
         self.path = path
-        self.compiler_id = detect_compiler_id(path, env=env)
+        if env is None:
+            env = dict()
+        env['LC_LOCAL'] = 'C'
+        epath = env.get('PATH', os.environ['PATH']).split(os.pathsep)
+        if not str(path.parent) in epath:
+            epath.insert(0, str(path.parent))
+        env['PATH'] = os.pathsep.join(epath)
+        self.compiler_id = detect_compiler_id(path, env=env, logger=logger)
         if self.compiler_id is None:
             raise RuntimeError(f'Cannot detect compiler ID of {self.path}')
         self.name = self.compiler_id.name
         self.env = env
         self.tools = tools
 
     @property
@@ -372,65 +392,81 @@
             value = line[pos + 1:].strip()
             # if os.getenv(name) != value:
             #    result[name] = value
             result[name] = value
     return result
 
 
-def get_compilers(logger: logging.Logger):
+def get_compilers(logger: logging.Logger, paths = None):
+    if paths is None:
+        default_paths = True
+    else:
+        default_paths = False
     from dan.core.find import find_executables, find_executable, find_file
     compilers: set[Compiler] = set()
-    if os.name == 'nt':
+    if paths is None and os.name == 'nt':
         infos = vswhere()
         for info in infos:
             logger.info(f'Loading Visual Studio: {info["displayName"]}')
             paths = [info['installationPath']]
             vcvars = find_file(r'vcvarsall.bat$', paths=paths)
             archs = [('x86_64', 'x64'), ('x86', 'x86')]
             for arch, vc_arch in archs:
+                logger.debug('Loading Visual Studio environment: %s (%s)', vcvars, vc_arch)
                 env = get_environment_from_batch_command([vcvars, vc_arch])
-                paths = env['PATH'].split(';')
+                logger.debug('Visual Studio environment: %s', env)
+                paths = env.get('PATH', env.get('Path', None))
+                if paths is None:
+                    raise RuntimeError('Cannot get PATH in Visual Studio environment')
+                paths = paths.split(os.pathsep)
                 cl = find_executable('cl', paths=paths, default_paths=False)
                 link = find_executable(
                     'link', paths=[cl.parent], default_paths=False)
                 lib = find_executable(
                     'lib', paths=[cl.parent], default_paths=False)
                 if env:
                     cc = Compiler(cl, env=env,
-                                  tools={'link': link, 'lib': lib})
+                                  tools={'link': link, 'lib': lib}, logger=logger)
                     assert cc.arch == vc_arch
                     compilers.add(cc)
                 else:
                     logger.warning(
                         f'Cannot load msvc with {arch} architecture')
     else:
-        for gcc in find_executables(r'gcc(-\d+)?'):
+        logger.debug('looking for gcc%s', logging.lazy_fmt(lambda: '' if paths is None else ' in' + ', '.join(paths)))
+        for gcc in find_executables(r'gcc(-\d+)?(\.exe)?', paths, default_paths):
             gcc = gcc.resolve()
-            compilers.add(Compiler(gcc))
-        for clang in find_executables(r'clang(-\d+)?'):
+            compilers.add(Compiler(gcc, logger=logger))
+        logger.debug('looking for clang%s', logging.lazy_fmt(lambda: '' if paths is None else ' in' + ', '.join(paths)))
+        for clang in find_executables(r'clang(-\d+)?(\.exe)?', paths, default_paths):
             clang = clang.resolve()
-            compilers.add(Compiler(clang))
+            compilers.add(Compiler(clang, logger=logger))
     return compilers
 
+unix_tools = [
+    'nm', 'ranlib', 'strip', 'readelf', 'ar', 'ranlib'
+]
 
 if os.name != 'nt':
-    _required_tools = [
-        'nm', 'ranlib', 'strip', 'readelf', 'ar', 'ranlib'
-    ]
+    _required_tools = unix_tools
 else:
     _required_tools = list()
 
 
 def create_toolchain(compiler: Compiler, logger=logging.getLogger('toolchain')):
-    logger.info(f'scanning {compiler.compiler_id} toolchain')
+    logger.info('scanning %s toolchain (%s-%s)', compiler.compiler_id, compiler.system, compiler.arch)
     data = {
         'type': compiler.name,
         'version': str(compiler.version),
         'cc': str(compiler.path),
     }
+    if len(compiler.path.suffixes):
+        extension = compiler.path.suffixes[-1]
+    else:
+        extension = ''
     pos = compiler.path.stem.rfind(compiler.name)
     if pos >= 0:
         prefix = None if pos == 0 else compiler.path.stem[:pos]
         base_name = compiler.name
         suffix = compiler.path.stem[pos + len(compiler.name):]
     else:
         prefix = None
@@ -447,31 +483,32 @@
     def get_compiler_tool(tool, toolname=None):
         if not toolname:
             toolname = f'{base_name}-{tool}'
         if prefix:
             toolname = f'{prefix}{toolname}'
         if suffix:
             toolname = f'{toolname}{suffix}'
-        tool_path = base_path / toolname
+        tool_path = (base_path / toolname).with_suffix(extension)
         if tool_path.exists():
             logger.debug(f'found {tool} tool: {tool_path}')
             data[tool] = str(tool_path)
         else:
             logger.debug(f'{tool} tool not found: {tool_path}')
     if compiler.name == 'gcc':
         get_compiler_tool('cxx', 'g++')
         get_compiler_tool('as')
     elif compiler.name == 'clang':
         get_compiler_tool('cxx', 'clang++')
     elif compiler.name == 'msvc':
         data['link'] = str(compiler.tools['link'])
         data['lib'] = str(compiler.tools['lib'])
 
-    for tool in _required_tools:
-        get_compiler_tool(tool)
+    if compiler.compiler_id.is_unix:
+        for tool in unix_tools:
+            get_compiler_tool(tool)
 
     name = str(compiler.compiler_id)
     if prefix:
         name = f'{prefix}{name}'
     if suffix:
         name = f'{name}{suffix}'
     return name, data
@@ -484,15 +521,15 @@
 def get_dan_path():
     path = Path(os.getenv('DAN_DATA', os.getenv(_home_var))) / '.dan'
     path.mkdir(exist_ok=True, parents=False)
     return path
 
 
 def get_toolchain_path():
-    return get_dan_path() / 'toolchains.yaml'
+    return get_dan_path() / 'toolchains.dat'
 
 
 def load_env_toolchain(script: Path = None, name: str = None):
     logger = logging.getLogger('toolchain')
     env = get_environment_from_batch_command(script)
     arch = env['ARCH'] if 'ARCH' in env else None
     paths = env['PATH'].split(os.pathsep)
@@ -516,77 +553,116 @@
     tname, toolchain = create_toolchain(cc, logger)
     save_toolchain(name or tname, toolchain)
 
 
 def save_toolchain(name, toolchain):
     toolchains_path = get_toolchain_path()
     logger = logging.getLogger('toolchain')
-    logger.setLevel(logging.INFO)
     if toolchains_path.exists():
-        with open(toolchains_path, 'r+') as f:
+        with open(toolchains_path, 'rb+') as f:
             logger.info(f'updating toolchains file {toolchains_path}')
-            data = yaml.load(f.read(), Loader=yaml.FullLoader)
+            data = pickle.load(f)
             toolchains = data['toolchains']
             toolchains[name] = toolchain
             f.seek(0)
             f.truncate()
-            f.write(yaml.dump(data))
+            pickle.dump(data, f)
 
 
-def create_toolchains():
-    import yaml
+def create_toolchains(paths = None):
+    if paths is None:
+        default_paths = True
+    else:
+        default_paths = False
     from dan.core.find import find_executable
     toolchains_path = get_toolchain_path()
     logger = logging.getLogger('toolchain')
-    logger.setLevel(logging.INFO)
     data = None
     if toolchains_path.exists():
-        with open(toolchains_path, 'r') as f:
+        with open(toolchains_path, 'rb') as f:
             logger.info(f'updating toolchains file {toolchains_path}')
-            data = yaml.load(f.read(), Loader=yaml.FullLoader)
+            data = pickle.load(f)
             if data:
                 toolchains = data['toolchains']
                 tools = data['tools']
     if not data:
         data = dict()
         toolchains = dict()
         tools = dict()
 
-    compilers = get_compilers(logger)
+    compilers = get_compilers(logger, paths)
+    if len(compilers) == 0:
+        logger.warning('no toolchain found')
+        return data
     for cc in compilers:
         k, v = create_toolchain(cc, logger)
+        arch_k = f'{k}-{v["arch"]}'
+        if arch_k in toolchains.keys():
+            k = arch_k
         if not k in toolchains.keys():
             logger.info(f'new toolchain \'{k}\' found')
         elif toolchains[k] != v:
             if toolchains[k]['type'] == v['type'] and toolchains[k]['arch'] != v['arch']:                
                 # add arch suffix
                 old_arch = toolchains[k]['arch']
                 logger.info(f'renaming \'{k}\' -> \'{k}-{old_arch}\'')
                 toolchains[f'{k}-{old_arch}'] = toolchains.pop(k)
-                logger.info(f'new toolchain \'{k}-{v["arch"]}\' found')
-                toolchains[f'{k}-{v["arch"]}'] = v
+                logger.info(f'new toolchain \'{arch_k}\' found')
+                toolchains[f'{arch_k}'] = v
+                continue
             else:
                 logger.info(f'updating toolchain \'{k}\'')
         else:
             logger.info(f'toolchain \'{k}\' unchanged')
             continue
         toolchains[k] = v
     for tool in _required_tools:
-        tools[tool] = str(find_executable(tool))
+        tools[tool] = str(find_executable(tool, paths, default_paths))
     data['tools'] = tools
     data['toolchains'] = toolchains
     if not 'default' in data:
-        data['default'] = list(toolchains.keys())[0]
-    with open(toolchains_path, 'w') as f:
-        f.write(yaml.dump(data))
+        from dan.core.osinfo import OSInfo
+        osi = OSInfo()
+        default_toolchain = None
+        for name, toolchain in toolchains.items():
+            if toolchain['system'] == osi.name and toolchain['arch'] == osi.arch:
+                default_toolchain = name
+                break
+        if default_toolchain is None:
+            default_toolchain = list(toolchains.keys())[0]
+        logger.debug('selected default toolchain: %s', default_toolchain)
+        data['default'] = default_toolchain
+
+    json_toolchain_path = toolchains_path.with_suffix('.json')
+    with open(json_toolchain_path, 'w') as jf, open(toolchains_path, 'wb') as pf:
+        pickle.dump(data, pf)
+        json.dump(data, jf, indent=4)
     return data
 
 
-def get_toolchains():
-    import yaml
+def get_toolchains(create = True):
     toolchains_path = get_toolchain_path()
     if not toolchains_path.exists():
+        if not create:
+            return {'toolchains': dict()}
         return create_toolchains()
+    
+    json_toolchain_path = toolchains_path.with_suffix('.json')
 
-    with open(toolchains_path) as f:
-        data = yaml.load(f, yaml.FullLoader)
-        return data if data else create_toolchains()
+    with open(toolchains_path, 'rb') as f:
+        data = pickle.load(f)
+    
+    # pickle/json synchronization
+    if not json_toolchain_path.exists() or json_toolchain_path.older_than(toolchains_path):
+        logger = logging.getLogger('toolchain')
+        logger.info(f'Updating {json_toolchain_path.name}')
+        with open(json_toolchain_path, 'w') as f:
+            json.dump(data, f, indent=4)
+            toolchains_path.touch()
+    elif json_toolchain_path.exists() and json_toolchain_path.younger_than(toolchains_path):
+        logger = logging.getLogger('toolchain')
+        logger.info(f'Updating {toolchains_path.name} ({json_toolchain_path.name} changed)')
+        with open(json_toolchain_path, 'r') as jf, open(toolchains_path, 'wb') as pf:
+            data = json.load(jf)
+            pickle.dump(data, pf)
+
+    return data
```

### Comparing `dan-build-0.2.3/dan/cxx/msvc_toolchain.py` & `dan-build-0.2.4/dan/cxx/msvc_toolchain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from functools import cached_property
 import json
+import typing as t
 
 import aiofiles
 from dan.core.runners import sync_run
 from dan.core.settings import BuildType
 from dan.core.utils import unique
 from dan.cxx.toolchain import CommandArgsList, RuntimeType, Toolchain, Path, FileDependency
+from dan.core import diagnostics as diag
 from dan.core.pm import re_match
+import os
 
 
 class MSVCToolchain(Toolchain):
     def __init__(self, data, *args, **kwargs):
         Toolchain.__init__(self, data, *args, **kwargs)
         self.cc = Path(data['cc'])
         self.cxx = self.cc
         self.lnk = Path(data['link'])
         self.lib = Path(data['lib'])
-        self.env = data['env']
+        self.env: dict[str, str] = data['env']
+        if 'INCLUDE' in self.env:
+            self._default_include_paths = self.env['INCLUDE'].split(os.pathsep)
+        else:
+            self._default_include_paths = list()
     
     @cached_property
     def common_flags(self):
         flags = [
             '/nologo',
         ]
         if self.build_type.is_debug_mode:
@@ -50,14 +57,17 @@
                 flags.extend((rt, '/O2', '/DNDEBUG'))
 
         return flags
 
     @property
     def default_cxxflags(self):
         return [f'/std:c++{self.cpp_std}', *self.settings.cxx_flags]
+    
+    async def get_default_include_paths(self, lang = 'c++') -> list[str]:
+        return self._default_include_paths
 
     def has_cxx_compile_options(self, *opts) -> bool:
         _, err, _ = sync_run([self.cxx, *opts], no_raise=True)
         # D9002 => unknown option
         return err.splitlines()[0].find('D9002') == 0
 
     def make_include_options(self, include_paths: set[Path]) -> list[str]:
@@ -157,7 +167,32 @@
     def make_shared_lib_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
         objects = list(objects)
         objs = [objects[0].name]
         for obj in objects[1:]:
             objs.append(obj.name)
         return [[self.lnk, *self.common_flags,
                 f'/IMPLIB:{output.with_suffix(".lib")}', '/DLL', *options, *objs, f'/OUT:{output.with_suffix(".dll")}']]
+
+    async def _handle_compile_output(self, lines) -> t.Iterable[diag.Diagnostic]:
+        async for line in lines:
+            line = line.strip()
+            match re_match(line):
+                case r'(.+)\((\d+)\):\s+(?:fatal\s+)?(error|warning)\s(\w+\d+):\s(.+)$' as m:
+                    yield diag.Diagnostic(
+                        message=m[5].strip(),
+                        range=diag.Range(start=diag.Position(line=int(m[2])-1)),
+                        code=m[4],
+                        severity=diag.Severity[m[3].upper()],
+                        source=self.type,
+                        filename=m[1])
+                case _:
+                    self._logger.debug('Unhandled line: %s', line)
+
+    async def _handle_link_output(self, lines) -> t.Iterable[diag.Diagnostic]:
+        async for line in lines:
+            match re_match(line):
+                case r'(.+?)\s?:\serror\s(\w+\d+):\s(.+)$' as m:
+                    yield diag.Diagnostic(message=m[3].strip(), code=m[2], source=self.type, filename=m[1])
+                case r'LINK\s?:\s?fatal\s+error\s+(\w+\d+):\s+(.+)$' as m:
+                    yield diag.Diagnostic(message=m[2].strip(), code=m[1], source=self.type)
+                case _:
+                    self._logger.debug('Unhandled line: %s', line)
```

### Comparing `dan-build-0.2.3/dan/cxx/support/qt.py` & `dan-build-0.2.4/dan/cxx/support/qt.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,48 +22,46 @@
         self.includes.private.append(self.build_path)
 
         for module in self.qt_modules:
             pkg = Package(f'Qt5{module}', makefile=self.makefile)
             await pkg.initialize()
             self.dependencies.add(pkg)
 
-        mocs = self.cache.get('mocs', list())
-        for moc_name in mocs:
+        self.mocs = self.cache.get('mocs', list())
+        for moc_name in self.mocs:
             moc_path = self.build_path / moc_name
             self.objs.append(
                 CXXObject(moc_path, self))
             self.other_generated_files.add(moc_path)
 
         await super().__initialize__()
 
     async def __clean__(self):
         await super().__clean__()
-        self.cache.reset('mocs')
+        self.cache['mocs'] = list()
 
     async def __build__(self):
-
-        mocs = list()
         moc_objs = list()
 
         async def do_moc(file: Path):
             moc_name = file.with_suffix('.moc.cpp').name
             moc_file_path = self.build_path / moc_name
             if not moc_file_path.exists() or file.younger_than(moc_file_path):
                 if moc_file_path.exists():
                     self.info(f'updating {moc_file_path}')
                 else:
                     self.info(f'generating {moc_file_path}')
                 out, err, rc = await async_run([self.moc, *self.includes.private, *self.compile_definitions.private, file], logger=self, log=False)
                 if rc == 0 and len(out):
                     async with aiofiles.open(moc_file_path, 'w') as f:
                         await f.write(out)
-                        if not moc_name in mocs:
+                        if not moc_name in self.mocs:
                             moc_objs.append(
                                 CXXObject(moc_file_path, self))
-                            mocs.append(moc_name)
+                            self.mocs.append(moc_name)
 
         # we have to generate objects first in order to get files dependencies,
         # which are used later to moc those dependencies (whenever they are within the same source directory)
 
         # build existing objects
         await CXXObjectsTarget.__build__(self)
 
@@ -77,15 +75,15 @@
             for source in sources:
                 g.create_task(do_moc(source))
         
         # add moc sources to objects dependencies
         self.objs.extend(moc_objs)
 
         # update cache
-        self.cache['mocs'] = mocs
+        self.cache['mocs'] = self.mocs
 
         # continue parent build process
         await super().__build__()
 
 
 def moc(modules: list[str]):
     def decorator(cls):
```

### Comparing `dan-build-0.2.3/dan/cxx/targets.py` & `dan-build-0.2.4/dan/cxx/targets.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 from dan.core.pathlib import Path
 from dan.core import aiofiles, cache
 from dan.core.settings import InstallMode, InstallSettings
 from dan.core.target import Target
 from dan.core.utils import chunks, unique
 from dan.core.runners import async_run
 from dan.core import asyncio
+from dan.cxx.toolchain import CompilationFailure, LinkageFailure, Toolchain
 
 
 class CXXObject(Target, internal=True):
     def __init__(self, source:Path, parent: 'CXXTarget') -> None:
         super().__init__(source.stem, parent=parent, default=False)
         self.parent = parent
         self.source = self.source_path / source
-        from . import target_toolchain
-        self.toolchain = target_toolchain
+        self.toolchain: Toolchain = self.context.get('cxx_target_toolchain')
         self.__dirty = False
 
     @property
     def cxx_flags(self):
         return self.parent.cxx_flags
 
     @property
     def private_cxx_flags(self):
         return self.parent.private_cxx_flags
     
     @property
     def includes(self):
         return self.parent.includes
-    
+
     @property
     def compile_definitions(self):
         return self.parent.compile_definitions
 
     async def __initialize__(self):
         await self.parent.preload()
 
@@ -69,18 +69,24 @@
     def up_to_date(self):
         res = super().up_to_date
         if res and self.__dirty:
             res = False
         return res
 
     async def __build__(self):
-        self.info(f'generating {self.output}...')
-        commands = await self.toolchain.compile(self.source, self.output, self.private_cxx_flags)
+        self.info('generating %s...', self.output.name)
+        try:
+            commands, diags = await self.toolchain.compile(self.source, self.output, self.private_cxx_flags)
+            self.parent.diagnostics.insert(diags, str(self.source))
+        except CompilationFailure as err:
+            self.parent.diagnostics.insert(err.diags, str(self.source))
+            err.target = self
+            raise
         self.cache['compile_args'] = [str(a) for a in commands[0]]
-        self.info(f'scanning dependencies of {self.source}')
+        self.debug('scanning dependencies of %s', self.source.name)
         deps = await self.toolchain.scan_dependencies(self.source, self.private_cxx_flags, self.build_path)
         deps = [d for d in deps
                 if self.makefile.root.source_path in Path(d).parents
                 or self.build_path in Path(d).parents]
         self.cache['deps'] = deps
 
 
@@ -163,16 +169,15 @@
     public_link_options: set[str] = set()
     private_link_options: set[str] = set()
 
     def __init__(self,
                  *args,
                  **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        from . import target_toolchain
-        self.toolchain = target_toolchain
+        self.toolchain : Toolchain = self.context.get('cxx_target_toolchain')
 
         self.includes = OptionSet(self, 'includes',
                                 #   self.public_includes, self.private_includes,
                                   transform=self.toolchain.make_include_options)
 
         self.compile_options = OptionSet(self, 'compile_options',
                                          self.public_compile_options, self.private_compile_options)
@@ -245,20 +250,24 @@
     @cache.once_method
     def _init_sources(self):
         if callable(self.sources):
             self.sources = set(self.sources())
         if not isinstance(self.sources, Iterable):
             assert callable(
                 self.sources), f'{self.name} sources parameter should be an iterable or a callable returning an iterable'
+        sources = list()
         for source in self.sources:
             source = Path(source)
             if not source.is_absolute():
                 source = self.source_path / source
+            sources.append(source)
             self.objs.append(
                 CXXObject(Path(source), self))
+        self.sources = sources
+            
 
     @property
     def file_dependencies(self):
         return unique(super().file_dependencies, *[o.file_dependencies for o in self.objs])
     
     @property
     def up_to_date(self):
@@ -280,20 +289,26 @@
 
     async def __build__(self):
         # compile objects
         async with asyncio.TaskGroup(f'building {self.name}\'s objects') as group:
             for dep in self.objs:
                 group.create_task(dep.build())
 
+    async def __clean__(self):
+        async with asyncio.TaskGroup(f'cleaning {self.name}\'s objects') as group:
+            for dep in self.objs:
+                group.create_task(dep.clean())
+        return await super().__clean__()
 
-class LibraryType(Enum):
-    AUTO = 0
-    STATIC = 1
-    SHARED = 2
-    INTERFACE = 3
+
+class LibraryType(str, Enum):
+    AUTO = 'auto'
+    STATIC = 'static'
+    SHARED = 'shared'
+    INTERFACE = 'interface'
 
 
 class Library(CXXObjectsTarget, internal=True):
 
     header_match = r'.+'
     library_type: LibraryType = LibraryType.AUTO
 
@@ -326,15 +341,14 @@
                 self.library_type = LibraryType.STATIC
 
         from .msvc_toolchain import MSVCToolchain
         if self.shared and isinstance(self.toolchain, MSVCToolchain):
             self.compile_definitions.add(f'{self.name.upper()}_EXPORT=1')
 
         if self.library_type != LibraryType.INTERFACE:
-            self.dependencies.update(self.objs)
             self.output = self.toolchain.make_library_name(self.name, self.shared)
         else:
             self.output = f"lib{self.name}.stamp"
         await super().__initialize__()
 
         previous_args = self.cache.get('generate_args')
         generate = None
@@ -342,15 +356,15 @@
             case LibraryType.STATIC:
                 generate = self.toolchain.static_lib
             case LibraryType.SHARED:
                 generate = self.toolchain.shared_lib
         if generate is not None:
             if previous_args and \
                     previous_args != await generate(
-                        [str(obj.output) for obj in self.objs], self.output, self.libs, dry_run=True):
+                        [obj.output for obj in self.objs], self.output, self.libs, dry_run=True):
                 self.__dirty = True
             else:
                 self.__dirty = False
         else:
             self.__dirty = False
 
     @property
@@ -359,34 +373,29 @@
             return False
         return super().up_to_date
 
     async def __build__(self):
         await super().__build__()
 
         self.info(
-            f'creating {self.library_type.name.lower()} library {self.output}...')
-
-        objs = self.objs
-        for dep in self.cxx_dependencies:
-            if isinstance(dep, CXXObjectsTarget) and not isinstance(dep, Library):
-                objs.update(dep.objs)
+            'creating %s library %s...', self.library_type.name.lower(), self.output.name)
 
         if self.static:
             await self.toolchain.static_lib([obj.output for obj in self.objs], self.output, self.libs)
         elif self.shared:
             await self.toolchain.shared_lib([obj.output for obj in self.objs], self.output, {*self.private_cxx_flags, *self.libs})
             from .msvc_toolchain import MSVCToolchain
             if isinstance(self.toolchain, MSVCToolchain):
                 self.compile_definitions.add(
                     f'{self.name.upper()}_IMPORT=1', public=True)
         else:
             assert self.interface
             self.output.touch()
 
-        self.debug(f'done')
+        self.debug('done')
 
     @asyncio.cached
     async def install(self, settings: InstallSettings, mode: InstallMode) -> list[Path]:
         if mode == InstallMode.user and not self.shared:
             return list()
 
         await self.build()
@@ -395,29 +404,28 @@
 
         if settings.create_pkg_config:
             from dan.pkgconfig.package import create_pkg_config
             tasks.append(create_pkg_config(self, settings))
 
         async def do_install(src: Path, dest: Path):
             if dest.exists() and dest.younger_than(src):
-                self.info(f'{dest} is up-to-date')
+                self.info('%s is up-to-date', dest)
             else:
-                self.info(f'installing {dest}')
+                self.debug('installing %s', dest)
                 dest.parent.mkdir(parents=True, exist_ok=True)
                 await aiofiles.copy(src, dest)
             return dest
 
         dest = settings.libraries_destination / self.output.name
+        self.info('installing %s to %s', self.name, dest)
+
         if not self.interface:
             tasks.append(do_install(self.output, dest))
 
         if mode == InstallMode.dev:
-            for dependency in self.library_dependencies:
-                tasks.append(dependency.install(settings, mode))
-
             header_expr = re.compile(self.header_match)
             includes_dest = settings.includes_destination
             for public_include_dir in self.includes.public_raw:
                 headers = public_include_dir.rglob('*.h*')
                 for header in headers:
                     if header_expr.match(str(header)):
                         dest = includes_dest / \
@@ -445,26 +453,28 @@
         return {*self.toolchain.cxxmodules_flags, *super().cxx_flags}
 
     async def __build__(self):
         return await super().__build__()
 
 class Executable(CXXObjectsTarget, internal=True):
 
+    installed = True
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.output = self.toolchain.make_executable_name(self.name)
         self.__dirty = False
 
     async def __initialize__(self):
         await super().__initialize__()
 
         previous_args = self.cache.get('link_args')
         if previous_args:
-            args = self.toolchain.make_link_commands([str(obj.output) for obj in self.objs], self.output,
+            args = self.toolchain.make_link_commands([obj.output for obj in self.objs], self.output,
                                                      [*self.libs, *self.link_options.public, *self.link_options.private])[0]
             args = [str(a) for a in args]
             if sorted(previous_args) != sorted(args):
                 self.__dirty = True
 
     @property
     def up_to_date(self):
@@ -472,27 +482,34 @@
             return False
         return super().up_to_date
 
     async def __build__(self):
         await super().__build__()
 
         # link
-        self.info(f'linking {self.output}...')
-        commands = await self.toolchain.link([str(obj.output) for obj in self.objs], self.output,
-                                             [*self.libs, *self.link_options.public, *self.link_options.private])
+        self.info('linking %s...', self.output.name)
+        try:
+            commands, diags = await self.toolchain.link([obj.output for obj in self.objs], self.output,
+                                                        [*self.libs, *self.link_options.public, *self.link_options.private])
+            self.diagnostics.insert(diags, str(self.output))
+        except LinkageFailure as err:
+            self.diagnostics.insert(err.diags, str(self.output))
+            err.target = self
+            raise
         self.cache['link_args'] = [str(a) for a in commands[0]]
-        self.debug(f'done')
+        self.debug('done')
 
     @asyncio.cached
     async def install(self, settings: InstallSettings, mode: InstallMode) -> list[Path]:
         dest = settings.runtime_destination / self.output.name
         if dest.exists() and dest.younger_than(self.output):
-            self.info(f'{dest} is up-to-date')
+            self.info('%s is up-to-date', dest)
         else:
-            self.info(f'installing {dest}')
+            self.info('installing %s', dest)
             dest.parent.mkdir(parents=True, exist_ok=True)
             await aiofiles.copy(self.output, dest)
         return [dest]
 
-    async def execute(self, *args, **kwargs):
-        await self.build()
+    async def execute(self, *args, build=True, **kwargs):
+        if build:
+            await self.build()
         return await async_run([self.output, *args], logger=self, env=self.toolchain.env, **kwargs)
```

### Comparing `dan-build-0.2.3/dan/cxx/toolchain.py` & `dan-build-0.2.4/dan/cxx/toolchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,53 @@
 from enum import Enum
-from dan.core.asyncio import sync_wait
-from dan.core.cache import Cache
+import dan.core.diagnostics as diag
 from dan.core.pathlib import Path
 from dan.core.settings import BuildType, ToolchainSettings
 from dan.core.target import FileDependency
 from dan.core.runners import async_run, sync_run, CommandError
 from dan.core.version import Version
 from dan.logging import Logging
 from dan.cxx.compile_commands import CompileCommands
 
+import typing as t
+
 import tempfile
 
 CommandArgs = list[str|Path]
 CommandArgsList = list[CommandArgs]
 
 class RuntimeType(Enum):
     static = 0
     dynamic = 1
 
+
+class BaseFailure(RuntimeError):
+    def __init__(self, msg: str, err: CommandError, options: set[str], command: str, toolchain: 'Toolchain', diags: list[diag.Diagnostic], target = None) -> None:
+        super().__init__(msg)
+        self.options = options
+        self.command = command
+        self.toolchain = toolchain
+        self.stdout = err.stdout
+        self.stderr = err.stderr
+        self.diags = diags
+        self.target = target
+    
+
+class CompilationFailure(BaseFailure):
+    def __init__(self, err: CommandError, sourcefile: Path, options: set[str], command: str, toolchain: 'Toolchain', diags: list[diag.Diagnostic] = [], target = None) -> None:
+        super().__init__(f'failed to compile {sourcefile}: {err.stdout}{err.stderr}', err, options, command, toolchain, diags, target)
+        self.sourcefile = sourcefile
+
+
+class LinkageFailure(BaseFailure):
+    def __init__(self, err: CommandError, objects: set[Path], options: set[str], command: str, toolchain: 'Toolchain', diags: list[diag.Diagnostic] = [], target = None) -> None:
+        super().__init__(f'failed to link {", ".join([str(o) for o in objects])}: {err.stdout}{err.stderr}', err, options, command, toolchain, diags, target)
+        self.objects = objects
+
+
 class Toolchain(Logging):
     def __init__(self, data: dict[str,str], tools: dict, settings: ToolchainSettings, cache: dict = None) -> None:
         self.cc : Path = None
         self.cxx : Path = None
         self.tools = tools
         self._compile_commands: CompileCommands = None
         self.cxx_flags = set()
@@ -71,20 +97,23 @@
         self.cache['defines'] = defines
         self.cache['arch'] = arch
         self.cache['arch_detect_flags'] = self.settings.cxx_flags
         
         from dan.core.osinfo import OSInfo
         osi = OSInfo()
         self.cache['is_host'] = self.system == osi.name and self.arch == osi.arch
-    
-    @property
-    def compile_commands(self):
-        if not self._compile_commands:
-            self._compile_commands = CompileCommands()
-        return self._compile_commands
+
+    async def get_default_defines(self) -> dict[str, str]:
+        return self.cache['defines']
+
+    # @property
+    # def compile_commands(self):
+    #     if not self._compile_commands:
+    #         self._compile_commands = CompileCommands()
+    #     return self._compile_commands
 
     def init(self):
         self.__update_cache()
 
     def has_cxx_compile_options(*opts) -> bool:
         raise NotImplementedError()
 
@@ -98,15 +127,21 @@
         raise NotImplementedError()
 
     def make_library_name(self, basename: str, shared: bool) -> str:
         raise NotImplementedError()
 
     def make_executable_name(self, basename: str) -> str:
         raise NotImplementedError()
+
+    async def _handle_compile_output(self, lines) -> t.Iterable[diag.Diagnostic]:
+        raise NotImplementedError()
     
+    async def _handle_link_output(self, lines) -> t.Iterable[diag.Diagnostic]:
+        raise NotImplementedError()
+
     async def scan_dependencies(self, file: Path, options: set[str], build_path: Path) -> set[FileDependency]:
         raise NotImplementedError()
 
     def compile_generated_files(self, output: Path) -> set[Path]:
         return set()
     
     def debug_files(self, output: Path) -> set[Path]:
@@ -121,48 +156,70 @@
     
     def to_unix_flags(self, flags: list[str]) -> list[str]:
         """Convert flags from target-compiler-style to unix-style"""
         return flags
 
     async def compile(self, sourcefile: Path, output: Path, options: set[str], **kwds):
         commands = self.make_compile_commands(sourcefile, output, options)
-        self.compile_commands.insert(sourcefile, output.parent, commands[0])
+        diags = []
+        if diag.enabled:
+            async def capture(stream):
+                with stream as lines:
+                    async for diag in self._handle_compile_output(lines):
+                        diags.append(diag)
+            kwds['all_capture'] = capture
         for index, command in enumerate(commands):
-            await self.run(f'compile{index}', output, command, **kwds, cwd=output.parent)
-        return commands
+            try:
+                await self.run(f'compile{index}', output, command, **kwds, cwd=output.parent)
+            except CommandError as err:
+                raise CompilationFailure(err, sourcefile, options, command, self, diags) from None
+        return commands, diags
 
     def make_link_commands(self, objects: set[Path], output: Path, options: set[str]) -> CommandArgsList:
         raise NotImplementedError()
 
     async def link(self, objects: set[Path], output: Path, options: set[str], **kwds):
         commands = self.make_link_commands(objects, output, options)
+        diags = []
+        if diag.enabled:
+            async def capture(stream):
+                with stream as lines:
+                    async for diag in self._handle_link_output(lines):
+                        diags.append(diag)
+            kwds['all_capture'] = capture
         for index, command in enumerate(commands):
-            await self.run(f'link{index}', output, command, **kwds, cwd=output.parent)
-        return commands
+            try:
+                await self.run(f'link{index}', output, command, **kwds, cwd=output.parent)
+            except CommandError as err:
+                raise LinkageFailure(err, objects, options, command, self, diags) from None
+        return commands, diags
 
     def make_static_lib_commands(self, objects: set[Path], output: Path, options: set[str]) -> CommandArgsList:
         raise NotImplementedError()
 
     async def static_lib(self, objects: set[Path], output: Path, options: set[str], **kwds):
         commands = self.make_static_lib_commands(objects, output, options)
         for index, command in enumerate(commands):
-            await self.run(f'static_lib{index}', output, command, **kwds, cwd=output.parent)
+            try:
+                await self.run(f'static_lib{index}', output, command, **kwds, cwd=output.parent)
+            except CommandError as err:
+                raise LinkageFailure(err, objects, options, command, self) from None
         return commands
 
     def make_static_lib_commands(self, objects: set[Path], output: Path, options: set[str]) -> CommandArgsList:
         raise NotImplementedError()
 
     async def shared_lib(self, objects: set[Path], output: Path, options: set[str], **kwds):
         commands = self.make_static_lib_commands(objects, output, options)
         for index, command in enumerate(commands):
             await self.run(f'shared_lib{index}', output, command, **kwds, cwd=output.parent)
         return commands
 
-    async def run(self, name: str, output: Path, args, quiet=False, **kwds):
-        return await async_run(args, env=self.env, logger=self if not quiet else None, **kwds)
+    async def run(self, name: str, output: Path, args, quiet=False, **kwds) -> tuple[str, str, int]:
+        return await async_run(args, env={**(self.env or dict()), 'LC_ALL': 'C'}, logger=self if not quiet else None, **kwds)
 
     @property
     def cxxmodules_flags(self) -> list[str]:
         ...
 
     def can_compile(self, source: str, options: set[str] = set(), extension='.cpp'):
         with tempfile.NamedTemporaryFile('w', suffix=extension) as f:
@@ -180,7 +237,10 @@
         return self.can_compile(source, options, extension)
 
     def has_definition(self, *definitions, options: set[str] = set(), extension='.cpp'):
         source = '\n'.join([f'''#ifndef {d}
         #error "{d} is not defined"
         #endif''' for d in definitions])
         return self.can_compile(source, options, extension)
+    
+    async def get_default_include_paths(self, lang = 'c++') -> list[str]:
+        return []
```

### Comparing `dan-build-0.2.3/dan/cxx/unix_toolchain.py` & `dan-build-0.2.4/dan/cxx/unix_toolchain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from functools import cached_property
-from dan.core.settings import BuildType, ToolchainSettings
+from dan.core import diagnostics as diag
+from dan.core.pm import re_match
+from dan.core.settings import BuildType
 from dan.core.utils import unique
 from dan.cxx.toolchain import CommandArgsList, Toolchain, Path, FileDependency
 from dan.cxx import auto_fpic
 from dan.core.runners import sync_run
 
+import typing as t
+
 cxx_extensions = ['.cpp', '.cxx', '.C', '.cc']
 c_extensions = ['.c']
 
 
 class UnixToolchain(Toolchain):
     def __init__(self, data, tools, *args, **kwargs):
         Toolchain.__init__(self, data, tools, *args, **kwargs)
         self.cc = data['cc']
         self.cxx = data['cxx']
         self.ar = data['ar'] if 'ar' in data else tools['ar']
         self.ranlib = data['ranlib'] if 'ranlib' in data else tools['ranlib']
-        self.as_ = data['readelf'] if 'readelf' in data else tools['readelf']
-        self.strip = data['env']['STRIP'] if 'env' in data and 'STRIP' in data['env'] else tools['strip']
+        # self.as_ = data['as'] if 'as' in data else tools['as']
+        # self.strip = data['env']['STRIP'] if 'env' in data and 'STRIP' in data['env'] else tools['strip']
         self.env = data['env'] if 'env' in data else None
-        self.debug(f'cc compiler is {self.type} {self.version} ({self.cc})')
-        self.debug(f'cxx compiler is {self.type} {self.version} ({self.cxx})')
+        self.debug('cxx compiler is %s %s (%s)', self.type, self.version, self.cc)
+        self.debug('cxx compiler is %s %s (%s)', self.type, self.version, self.cxx)
 
     @cached_property
     def default_cflags(self):
         flags = list()
         match self.build_type:
             case BuildType.debug:
                 flags.extend(('-g', ))
@@ -83,15 +87,15 @@
     def make_compile_definitions(self, definitions: set[str]) -> list[str]:
         return unique([f'-D{d}' for d in definitions])
 
     def make_library_name(self, basename: str, shared: bool) -> str:
         return f'lib{basename}.{"so" if shared else "a"}'
 
     def make_executable_name(self, basename: str) -> str:
-        return basename
+        return f'{basename}.exe' if self.system.startswith('msys') else basename
 
     def get_base_compile_args(self, sourcefile: Path) -> list[str]:
         match sourcefile.suffix:
             case _ if sourcefile.suffix in cxx_extensions:
                 return [self.cxx, *self.default_cxxflags]
             case _ if sourcefile.suffix in c_extensions:
                 return [self.cc, *self.default_cflags]
@@ -130,27 +134,94 @@
         args.extend([*self.compile_options, *options, '-MD', '-MT', str(output),
                     '-MF', f'{output}.d', '-o', str(output), '-c', str(sourcefile)])
         if auto_fpic:
             args.insert(1, '-fPIC')
         return [args]
 
     def make_link_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
-        args = [self.cxx, *objects, '-o', str(output), *unique(
+        args = [self.cxx, *[o.name for o in objects], '-o', str(output), *unique(
             self.default_ldflags, self.default_cflags, self.default_cxxflags, self.link_options, options)]
         commands = [args]
         if self._build_type in [BuildType.release, BuildType.release_min_size]:
             commands.append([self.strip, output])
         return commands
 
     def make_static_lib_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
         return [
-            [self.ar, 'cr', output, *objects], # *options],
+            [self.ar, 'cr', output, *[o.name for o in objects]], # *options],
             [self.ranlib, output],
         ]
 
     def make_shared_lib_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
         args = [self.cxx, '-shared', *
                 unique(self.default_ldflags, options), *objects, '-o', output]
         commands = [args]
         if self._build_type in [BuildType.release, BuildType.release_min_size]:
             commands.append([self.strip, output])
         return commands
+    
+    async def get_default_include_paths(self, lang = 'c++') -> list[Path]:
+        cache_key = f'default_{lang}_includes'
+        includes = self.cache.get(cache_key, None)
+        if includes is None:
+            args = [self.cc, '-x', lang, '-E', '-Wp,-v', '-']
+            out, err, rc = await self.run(f'get default {lang} includes', None, args, quiet=True, log=False, input='')
+            if rc != 0:
+                self.error('failed to get default %s includes: %s', lang, err)
+                return []
+            includes = []
+            for line in [*out.splitlines(), *err.splitlines()]:
+                match re_match(line):
+                    case r'^ (.+)$' as m:
+                        includes.append(str(Path(m[1]).resolve()))
+            self.cache[cache_key] = includes
+        return includes
+
+    async def _gen_gcc_compile_diags(self, lines) -> t.Iterable[diag.Diagnostic]:
+        async for line in lines:
+            match re_match(line):
+                case r'(.+):(\d+):(\d+):\s(error|warning):\s(.+)$' as m:
+                    yield diag.Diagnostic(
+                        message=m[5],
+                        range=diag.Range(start=diag.Position(line=int(m[2])-1, character=int(m[3]))),
+                        severity=diag.Severity[m[4].upper()],
+                        source=self.type,
+                        filename=m[1]
+                    )
+
+    async def _handle_compile_output(self, lines) -> t.Iterable[diag.Diagnostic]:
+        match self.type:
+            case 'gcc'|'clang':
+                async for d in self._gen_gcc_compile_diags(lines):
+                    yield d
+            case _:
+                raise NotImplementedError(f'handle_compile_output errors not implemented for {self.type}')
+    
+    async def _gen_ld_link_diags(self, lines) -> t.Iterable[diag.Diagnostic]:
+        function = None
+        object = None
+        async for line in lines:
+            match re_match(line):
+                case r'(.+): in function `(.+)\':$' as m:
+                    object = m[1]
+                    function = m[2]
+                case r'(?:.+: )?(?:(.+):)?\((.+)\+(.+)\): (.+)$' as m:
+                    # link error may not be associated to a source file,
+                    # in which case the associated file is the object
+                    filename = m[1] or object
+                    section = m[2]
+                    section_offset = int(m[3], 0)
+                    message = m[4]
+                    yield diag.Diagnostic(
+                        message=message,
+                        source=self.type
+                    )
+                case _:
+                    self._logger.debug('unhandled line: %s', line)
+
+    async def _handle_link_output(self, lines) -> t.Iterable[diag.Diagnostic]:
+        match self.type:
+            case 'gcc'|'clang':
+                async for d in self._gen_ld_link_diags(lines):
+                    yield d
+            case _:
+                raise NotImplementedError(f'handle_link_output not implemented for {self.type}')
```

### Comparing `dan-build-0.2.3/dan/io/package.py` & `dan-build-0.2.4/dan/io/package.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     if self.spec.is_compatible(version):
                         self.debug(f'using version {version} to match {self.spec}')
                         self.version = version
                         break
 
         packages_path = get_packages_path()
         
-        from dan.cxx import target_toolchain as toolchain
+        toolchain = self.context.get('cxx_target_toolchain')
         self._build_path = packages_path / toolchain.system / toolchain.arch / toolchain.build_type.name / self.package / str(self.version)
         self.install_settings = InstallSettings(self.build_path)
         
         # update package build-path
         makefile = self.package_makefile
         makefile.build_path = self.build_path / 'build'
 
@@ -87,30 +87,37 @@
             self.debug(f'{ident} already built by {self._all_builds[ident].fullname}')
             await self._all_builds[ident].build()
             return
 
         self._all_builds[ident] = self
 
         makefile = self.package_makefile
+        build_path = makefile.build_path
 
+        # FIXME: shall a makefile have an associated toolchain ?
+        toolchain = None
         async with asyncio.TaskGroup(f'installing {self.package}\'s targets') as group:
             for target in makefile.all_installed:
+                if hasattr(target, 'toolchain'):
+                    if toolchain is None:
+                        toolchain = target.toolchain
+                    else:
+                        assert toolchain == target.toolchain, 'Toolchain missmatch'
                 group.create_task(target.install(self.install_settings, InstallMode.dev))
 
         makefile.cache.ignore()
         del makefile
 
         os.chdir(self.build_path.parent)
 
         self.debug('cleaning')
         async with asyncio.TaskGroup(f'cleanup {self.package}') as group:
-            from dan.cxx import target_toolchain as toolchain
-            if not toolchain.build_type.is_debug_mode:
+            if toolchain is not None and not toolchain.build_type.is_debug_mode:
                 group.create_task(aiofiles.rmtree(self.output / 'src'))
-            # group.create_task(aiofiles.rmtree(self.build_path))
+            group.create_task(aiofiles.rmtree(build_path, force=True))
 
 
 class Package(Target, internal=True):
 
     def __init__(self,
                  name: str = None,
                  version: str = None,
@@ -169,11 +176,13 @@
                 self.debug('copying %s to %s', pkg, self.build_path / self.dan_path)
                 group.create_task(aiofiles.copy(pkg, self.build_path / self.dan_path))
         
         if self.output.exists():
             from dan.pkgconfig.package import Data, find_package
             data = Data(self.output)
             async with asyncio.TaskGroup(f'importing {self.name} package requirements') as group:
+                toolchain = self.context.get('cxx_target_toolchain')
+                search_path = get_packages_path() / toolchain.system / toolchain.arch / toolchain.build_type.name
                 for pkg in data.requires:
-                    pkg = find_package(pkg.name, spec=pkg.version_spec, search_paths=[get_packages_path()])
+                    pkg = find_package(pkg.name, spec=pkg.version_spec, search_paths=[search_path], makefile=self.makefile)
                     self.debug('copying %s to %s', pkg.config_path, self.build_path / self.pkgconfig_path)
                     group.create_task(aiofiles.copy(pkg.config_path, self.build_path / self.pkgconfig_path))
```

### Comparing `dan-build-0.2.3/dan/io/repositories.py` & `dan-build-0.2.4/dan/io/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 @dataclass
 class GitHubConfig:
     api_token: str = None
 
 @dataclass_json
 @dataclass
 class RepositoriesSettings:
-    github: GitHubConfig = field(default_factory=lambda: GitHubConfig())
+    github: t.Optional[GitHubConfig] = field(default_factory = GitHubConfig)
     repositories: list[RepositoryConfig] = field(default_factory=lambda: [
         RepositoryConfig('dan.io', 'https://github.com/Garcia6l20/dan.io.git'),
     ])
 
     def get(self, name):
         for config in self.repositories:
             if config.name == name:
@@ -84,15 +84,16 @@
 
     @property
     def pkgs_makefile(self) -> MakeFile:
         if self._package_makefile is None:
             from dan.core.include import load_makefile
             root = self.output / 'packages'
             requirements = None
-            self._package_makefile = load_makefile(root / 'dan-build.py', f'{self.name}.packages', requirements=requirements, build_path=self.build_path / self.name, parent=self.makefile)
+            with self.makefile.context:
+                self._package_makefile = load_makefile(root / 'dan-build.py', f'{self.name}.packages', requirements=requirements, build_path=self.build_path / self.name, parent=self.makefile)
 
         return self._package_makefile
 
     @property
     def installed(self) -> dict[str, Target]:
         pkgs = self.pkgs_makefile
         return {f'{lib.makefile.name}:{lib.name}@{self.name}' : lib for lib in pkgs.all_installed}
```

### Comparing `dan-build-0.2.3/dan/jinja.py` & `dan-build-0.2.4/dan/jinja.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import aiofiles
 from dan.core.pathlib import Path
-from dan.core import asyncio
 from dan.core.target import Target, TargetDependencyLike
 from typing import Callable
 import inspect
 
 
 class generator:
-    def __init__(self, output: str, template: str, dependencies: TargetDependencyLike = list(), name=None):
+    def __init__(self, output: str, template: str, dependencies: TargetDependencyLike = None, options: dict = None):
         self.output = Path(output)
-        self.dependencies = dependencies
+        self.dependencies = list() if dependencies is None else dependencies
         self.template = template
+        self.options = dict() if options is None else options
 
     def __call__(self, fn: Callable):
         class JinjaGenerator(Target):
             name = self.output.stem
             output = self.output
             template = self.template
             dependencies = [*self.dependencies, self.template]
+            options = self.options
 
             async def __build__(self):
                 import jinja2
                 arg_spec = inspect.getfullargspec(fn)
                 if 'self' in arg_spec.args:
                     data = fn(self)
                 elif not arg_spec.args:
```

### Comparing `dan-build-0.2.3/dan/logging.py` & `dan-build-0.2.4/dan/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import tqdm
 from logging import *
 from termcolor import colored
 
+# default level
+getLogger().setLevel(INFO)
 
 def merge(lhs, rhs):
     if type(lhs) != type(rhs):
         raise RuntimeError(f'cannot merge {type(lhs)} with {rhs}')
     if type(lhs) == dict:
         for k in rhs:
             if k in lhs:
@@ -137,7 +139,14 @@
 
 def error(*args, **kwds):
     return _get_makefile_logger().error(*args, **kwds)
 
 
 def critical(*args, **kwds):
     return _get_makefile_logger().critical(*args, **kwds)
+
+
+class lazy_fmt():    
+    def __init__(self, fn):
+        self.__fn=fn
+    def __str__(self):
+        return self.__fn()
```

### Comparing `dan-build-0.2.3/dan/make.py` & `dan-build-0.2.4/dan/make.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 
 from dataclasses import dataclass, field
 from enum import Enum
 import functools
+import itertools
 import logging
 import os
 import fnmatch
 import re
 
 from dataclasses_json import dataclass_json
-from dan.core.pathlib import Path
 import sys
 import tqdm
 import typing as t
+from collections.abc import Iterable
 
+from dan.core import diagnostics as diag
 from dan.core.cache import Cache
-from dan.core.include import include_makefile
+from dan.core.makefile import MakeFile
+from dan.core.pathlib import Path
+from dan.core.include import MakeFileError, include_makefile, Context
 from dan.core import aiofiles, asyncio
 from dan.core.settings import InstallMode, Settings
 from dan.core.test import Test
 from dan.core.utils import unique
 from dan.cxx import init_toolchains
 from dan.logging import Logging
 from dan.core.target import Option, Target
 from dan.cxx.targets import Executable
 from dan.core.runners import max_jobs
-from collections.abc import Iterable
-
-
-def make_target_name(name: str):
-    return name.replace('_', '-')
 
 
 def flatten(list_of_lists):
     if len(list_of_lists) == 0:
         return list_of_lists
     if isinstance(list_of_lists[0], Iterable):
         return flatten(list_of_lists[0]) + flatten(list_of_lists[1:])
@@ -45,23 +44,94 @@
     build_path: Path = None
     toolchain: str = None
     settings: Settings = field(default_factory=lambda: Settings())
 
 class ConfigCache(Cache[Config]):
     indent = 4
 
+def _get_code_position(code, instruction_index):
+    if instruction_index < 0 \
+        or not hasattr(code, 'co_positions'): # Python <= 3.10 does not have co_position
+        return (None, 0, 0, 0)
+    positions_gen = code.co_positions()
+    return next(itertools.islice(positions_gen, instruction_index // 2, None))
+
+def _tb_entries(tb):
+    entries = list()
+    while tb is not None:
+        entries.append(tb)
+        tb = tb.tb_next
+    return entries
+
+
+def _walk_tb(tb, reverse=True):
+    if isinstance(tb, Exception):
+        tb = tb.__traceback__
+
+    entries = _tb_entries(tb)
+    
+    if reverse:
+        entries = reversed(entries)
+    
+    for tb in entries:
+        positions = _get_code_position(tb.tb_frame.f_code, tb.tb_lasti)
+        # Yield tb_lineno when co_positions does not have a line number to
+        # maintain behavior with walk_tb.
+        if positions[0] is None:
+            yield tb.tb_frame.f_code.co_filename, (tb.tb_lineno, ) + positions[1:]
+        else:
+            yield tb.tb_frame.f_code.co_filename, positions
+
+
+def gen_python_diags(err: Exception):
+    diagnostics = diag.DiagnosticCollection()
+    if not diag.enabled:
+        return diagnostics
+    match err:
+        case MakeFileError():
+            cause = err.__cause__
+            related = None
+            if isinstance(cause, MakeFileError):
+                related = list()
+                cause_diags = gen_python_diags(cause)
+                for filename, diagns in cause_diags.items():
+                    for d in diagns:
+                        related.append(diag.RelatedInformation(diag.Location(diag.Uri(filename), d.range), d.message))
+                diagnostics.update(cause_diags)
+                err_filename = str(err.path)
+                for filename, (lineno, end_lineno, colno, end_colno) in _walk_tb(cause):
+                    if filename == err_filename:
+                        break
+            else:
+                for filename, (lineno, end_lineno, colno, end_colno) in _walk_tb(cause):
+                    break
+            diagnostics[filename] = diag.Diagnostic(
+                message=str(cause),
+                range=diag.Range(start=diag.Position(lineno - 1, colno), end=diag.Position(end_lineno - 1, end_colno)),
+                code=cause.__class__.__name__,
+                source='dan.make',
+                related_information=related
+            )
+        case _:
+            for filename, (lineno, end_lineno, colno, end_colno) in _walk_tb(err):
+                break
+            diagnostics[filename] = diag.Diagnostic(
+                message=str(err),
+                range=diag.Range(start=diag.Position(lineno - 1, colno), end=diag.Position(end_lineno - 1, end_colno)),
+                code=err.__class__.__name__,
+                source='dan.make'
+            )
+
+    return diagnostics
 
 class Make(Logging):
     _config_name = 'dan.config.json'
-    _cache_name = 'dan.cache.json'
-
-    def __init__(self, path: str, targets: list[str] = None, verbose: bool = False, quiet: bool = False, for_install: bool = False, jobs: int = None, no_progress=False):
+    _cache_name = 'dan.cache'
 
-        from dan.core.include import context_reset
-        context_reset()
+    def __init__(self, build_path: str, targets: list[str] = None, verbose: bool = False, quiet: bool = False, for_install: bool = False, jobs: int = None, no_progress=False, diags=False):
 
         jobs = jobs or os.cpu_count()
         max_jobs(jobs)
 
         if quiet:
             assert not verbose, "'quiet' cannot be combined with 'verbose'"
             log_level = logging.ERROR
@@ -69,82 +139,88 @@
             log_level = logging.DEBUG
         else:
             log_level = logging.INFO
         logging.getLogger().setLevel(log_level)
 
         super().__init__('make')
 
+        if diags:
+            diag.enabled = True
+
         self.no_progress = no_progress
         self.for_install = for_install
-        path = Path(path)
-        if not path.exists() or not (path / 'dan-build.py').exists():
-            self.source_path = Path.cwd().absolute()
-            self.build_path = path.absolute().resolve()
-        else:
-            self.source_path = path.absolute().resolve()
-            self.build_path = Path.cwd().absolute()
-
-        self.config_path = self.build_path / self._config_name
-        self.cache_path = self.build_path / self._cache_name
+        
+        self.build_path = Path(build_path)
+        self.config_path = build_path / self._config_name
+        self.cache_path = build_path / self._cache_name
 
         self.required_targets = targets
-        self.build_path.mkdir(exist_ok=True, parents=True)
-        sys.pycache_prefix = str(self.build_path / '__pycache__')
-        self._config = ConfigCache(self.config_path)
-        self.cache = Cache(self.cache_path)
-
-        # self.settings: Settings = self.config.get('settings', Settings())
-
-        # self.source_path = Path(self.config.get(
-        #     'source_path', self.source_path))
-
-        self.debug(f'source path: {self.source_path}')
-        self.debug(f'build path: {self.build_path}')
+        sys.pycache_prefix = str(build_path / '__pycache__')
+        self._config = ConfigCache.instance(self.config_path)
+        self.cache = Cache.instance(self.cache_path, binary=True)
+        
         self.debug(f'jobs: {jobs}')
 
-        assert (self.source_path /
-                'dan-build.py').exists(), f'no makefile in {self.source_path}'
-        assert (self.source_path !=
-                self.build_path), f'in-source build are not allowed'
+        self._diagnostics = diag.DiagnosticCollection()
+
+        self.context = Context()
         
     @property
     def config(self) -> Config:
         return self._config.data
     
     @property
     def settings(self) -> Settings:
         return self._config.data.settings
+    
+    @property
+    def source_path(self):
+        return Path(self.config.source_path)
+        
+    @property
+    def toolchain(self):
+        return self.context.get('cxx_target_toolchain')
+    
+    @property
+    def root(self) -> MakeFile:
+        return self.context.root
 
-    def configure(self, toolchain):
-        self.config.source_path = str(self.source_path)
+    async def configure(self, source_path: str, toolchain: str = None):
+        self.config.source_path = str(source_path)
         self.config.build_path = str(self.build_path)
-        self.config.toolchain = toolchain
+        self.info(f'source path: {self.config.source_path}')
+        self.info(f'build path: {self.config.build_path}')
+        if toolchain:
+            self.config.toolchain = toolchain
+        if not self.config.toolchain:
+            self.warning('no toolchain configured')
+        await self._config.save()
 
     @asyncio.cached
     async def initialize(self):
-        assert self.source_path and self.config_path.exists(), 'configure first'
+        assert self.config_path.exists(), 'configure first'
+
+        self.debug(f'source path: {self.source_path}')
+        self.debug(f'build path: {self.build_path}')
 
         toolchain = self.config.toolchain
         build_type = self.settings.build_type
 
         self.info(
             f'using \'{toolchain}\' toolchain in \'{build_type.name}\' mode')
 
-        from dan.core.include import context_reset
-        import gc
-
-        # for test purpose
-        context_reset()
-        gc.collect()
+        with self.context:
+            init_toolchains(toolchain, self.settings)
+            try:
+                include_makefile(self.source_path, self.build_path)
+            except MakeFileError as err:
+                self._diagnostics.update(gen_python_diags(err))
+                raise
 
-        init_toolchains(toolchain, self.settings)
-
-        include_makefile(self.source_path, self.build_path)
-
-        from dan.cxx import target_toolchain
+        target_toolchain = self.context.get('cxx_target_toolchain')
         target_toolchain.build_type = build_type
         if self.for_install:
             library_dest = Path(self.settings.install.destination) / \
                 self.settings.install.libraries_prefix
             target_toolchain.rpath = str(library_dest.absolute())
 
         self.debug(f'targets: {[t.name for t in self.targets]}')
@@ -153,71 +229,90 @@
         for required in self.required_targets:
             if fnmatch.fnmatch(target.fullname, f'*{required}*'):
                 return True
         return False
 
     @functools.cached_property
     def targets(self) -> list[Target]:
-        from dan.core.include import context
         items = list()
         if self.required_targets and len(self.required_targets) > 0:
-            for target in context.root.all_targets:
+            for target in self.root.all_targets:
                 if self.__matches(target):
                     items.append(target)
         else:
-            items = context.root.all_default
+            items = self.root.all_default
         return items
 
     @functools.cached_property
     def tests(self) -> list[Test]:
-        from dan.core.include import context
         items = list()
         if self.required_targets and len(self.required_targets) > 0:
             for required in self.required_targets:
                 test_name, *test_case = required.split(':')
                 test_case = test_case[0] if len(test_case) else None
 
-                for test in context.root.all_tests:
+                for test in self.root.all_tests:
                     
                     if fnmatch.fnmatch(test.fullname, f'*{test_name}*'):
                         if len(test) > 1 and test_case is not None:
                             cases = list()
                             for case in test.cases:
                                 if fnmatch.fnmatch(case.name, test_case):
                                     cases.append(case)
                             test.cases = cases
                         
                         items.append(test)
         else:
-            for test in context.root.all_tests:
+            for test in self.root.all_tests:
                 items.append(test)
         return items
 
     @property
     def all_options(self) -> list[Option]:
-        from dan.core.include import context
         opts = []
         for target in self.targets:
             for o in target.options:
                 opts.append(o)
-        for makefile in context.all_makefiles:
+        for makefile in self.context.all_makefiles:
             for o in makefile.options:
                 opts.append(o)
         return opts
+    
+    @property
+    def diagnostics(self):
+        result: diag.DiagnosticCollection = diag.DiagnosticCollection()
+        if self.root:
+            for target in self.root.all_targets:
+                result.update(target.diagnostics)
+        result.update(self._diagnostics)
+        return result
+
 
-    async def target_of(self, source):
-        from dan.core.include import context
+    async def target_of(self, source: Path):
         from dan.cxx.targets import CXXObjectsTarget
 
         source = Path(source)
-        for target in [target for target in context.root.all_targets if isinstance(target, CXXObjectsTarget)]:            
+        if source.suffix[1].lower() == 'h':
+            def check(t: CXXObjectsTarget):
+                for p in [*t.includes.private_raw, *t.includes.public_raw]:
+                    p: Path = p
+                    if p not in source.parents:
+                        continue
+                    return True
+                return False
+        else:
+            def check(t: CXXObjectsTarget):
+                t._init_sources()
+                if source.name in [Path(s).name for s in target.sources]:
+                    return True
+                return False
+        for target in [target for target in self.root.all_targets if isinstance(target, CXXObjectsTarget)]:            
             if target.source_path not in source.parents:
                 continue
-            target._init_sources()
-            if source.name in target.sources:
+            if check(target):
                 return target
 
 
     @classmethod
     def _parse_str_value(cls, name, value: str, orig: type, tp: type = None):
         if issubclass(orig, Enum):
             names = [n.lower()
@@ -229,14 +324,16 @@
                 raise RuntimeError(f'{name} should be one of {names}')
         elif issubclass(orig, (set, list)):
             assert tp is not None
             result = list()
             for sub in value.split(';'):
                 result.append(cls._parse_str_value(name, sub, tp))
             return orig(result)
+        elif orig == bool:
+            return value.lower() in ('true', 'yes', 'on', '1')
         else:
             if tp is not None:
                 raise TypeError(f'unhandled type {orig}[{tp}]')
             return orig(value)
 
     
     @classmethod
@@ -267,17 +364,17 @@
                 match (out_value, op, in_value):
                     case (list()|set(), '-', list()|set()) if len(in_value) == 1 and list(in_value)[0] == '*':
                         out_value.clear()
                     case (set(), '+', set()):
                         out_value.update(in_value)
                     case (set(), '-', set()):
                         out_value = out_value - in_value
-                    case (list(), '+', set()):
-                        out_value.insert(in_value)
-                    case (list(), '-', set()):
+                    case (list(), '+', set()|list()):
+                        out_value.extend(in_value)
+                    case (list(), '-', set()|list()):
                         for v in in_value:
                             out_value.remove(v)
                     case (_, '+' | '-', _):
                         raise TypeError(f'unhandled "{op}=" operator on type {type(out_value)} ({name})')
                     case _:
                         out_value = in_value
                 if isinstance(input, dict):
@@ -294,40 +391,39 @@
         def get_option(name):
             for opt in all_opts:
                 if opt.fullname == name:
                     return opt.cache, opt.value, opt.type
         self._apply_inputs(options, get_option, lambda k, v: self.info(f'option: {k} = {v}'))
 
     async def apply_settings(self, *settings):
-        await self.initialize()
+        # dont init for settings
         def get_setting(name):
             parts = name.split('.')
             setting = self.settings
             for part in parts[:-1]:
                 if not hasattr(setting, part):
                     raise RuntimeError(f'no such setting: {name}')
                 setting = getattr(setting, part)
             if not hasattr(setting, parts[-1]):
                 raise RuntimeError(f'no such setting: {name}')
             value = getattr(setting, parts[-1])
             return setting, value, type(setting)
         self._apply_inputs(settings, get_setting, lambda k, v: self.info(f'setting: {k} = {v}'))
-        pass
 
 
     @staticmethod
     def toolchains():
         from dan.cxx.detect import get_toolchains
         return get_toolchains()
 
     class progress:
 
         def __init__(self, desc, targets, task_builder, disable) -> None:
             self.desc = desc
-            self.targets = targets
+            self.targets = list(targets) # NOTE: need to take a copy of the list
             self.builder = task_builder
             import shutil
             term_cols = shutil.get_terminal_size().columns
             self.max_desc_width = int(term_cols * 0.25)
             self.pbar = tqdm.tqdm(total=len(targets),
                                   desc='building', disable=disable)
             self.pbar.unit = ' targets'
@@ -355,46 +451,69 @@
 
             return tasks
 
         def __exit__(self, *args):
             self.pbar.set_description_str(self.desc + ' done')
             self.pbar.refresh()
             return
+        
+    async def _build_target(self, t: Target):
+        try:
+            await t.build()
+        except Exception as err:
+            self._diagnostics.update(gen_python_diags(err))
+            raise
 
-    async def build(self):
+    async def build(self, targets: list[Target] = None):
         await self.initialize()
 
-        with self.progress('building', self.targets, lambda t: t.build(), self.no_progress) as tasks:
+        if targets is None:
+            targets = self.targets
+
+        with self.context, \
+             self.progress('building', targets, self._build_target, self.no_progress) as tasks:
             results = await asyncio.gather(*tasks, return_exceptions=True)
             errors = list()
             for result in results:
                 if isinstance(result, Exception):
-                    self._logger.exception(result)
+                    self._logger.error(str(result))
                     errors.append(result)
             err_count = len(errors)
             if err_count == 1:
                 raise errors[0]
             elif err_count > 1:
-                raise RuntimeError('One or more targets failed, check log...')
+                raise asyncio.ExceptionGroup('Multiple errors occured while building the project', errors=errors)
+
+    async def _install_target(self, t: Target, mode: InstallMode):
+        try:
+            return await t.install(self.settings.install, mode)
+        except Exception as err:
+            self._diagnostics.update(gen_python_diags(err))
+            raise
 
     async def install(self, mode: InstallMode = InstallMode.user):
         await self.initialize()
-        from dan.core.include import context
 
         self.for_install = True
         await self.initialize()
-        targets = context.root.all_installed
+        targets = []
+        for t in self.targets:
+            if t.installed:
+                targets.append(t)
+            else:
+                self.debug('skipping %s (not marked as installed)', t.fullname)
 
-        await self.build()
+        await self.build(targets)
 
-        with self.progress('installing', targets, lambda t: t.install(self.settings.install, mode), self.no_progress) as tasks:
+        with self.context, \
+             self.progress('installing', targets, functools.partial(self._install_target, mode=mode), self.no_progress) as tasks:
             installed_files = await asyncio.gather(*tasks)
             installed_files = unique(flatten(installed_files))
             manifest_path = self.settings.install.data_destination / \
-                'dan' / f'{context.root.name}-manifest.txt'
+                'dan' / f'{self.root.name}-manifest.txt'
             manifest_path.parent.mkdir(parents=True, exist_ok=True)
 
             async with aiofiles.open(manifest_path, 'w') as f:
                 await f.writelines([os.path.relpath(p, manifest_path.parent) + '\n' for p in installed_files])
 
     @property
     def executable_targets(self) -> list[Executable]:
@@ -405,29 +524,39 @@
         if script:
             load_env_toolchain(script)
         else:
             create_toolchains()
 
     async def run(self):
         await self.initialize()
-        results = await asyncio.gather(*[t.execute(log=True) for t in self.executable_targets])
-        for result in results:
-            if result[2] != 0:
-                return result[2]
+        with self.context:
+            results = await asyncio.gather(*[t.execute(log=True) for t in self.executable_targets])
+            for result in results:
+                if result[2] != 0:
+                    return result[2]
         return 0
 
+    async def _test_target(self, t: Test):
+        try:
+            return await t.run_test()
+        except Exception as err:
+            self._diagnostics.update(gen_python_diags(err))
+            raise
+
     async def test(self):
         await self.initialize()
-        with self.progress('testing', self.tests, lambda t: t.run_test(), self.no_progress) as tasks:
-            results = await asyncio.gather(*tasks)
-            if all(results):
-                self.info('Success !')
-                return 0
-            else:
-                self.error('Failed !')
-                return 255
+        with self.context:
+            with self.progress('testing', self.tests, self._test_target, self.no_progress) as tasks:
+                results = await asyncio.gather(*tasks)
+                if all(results):
+                    self.info('Success !')
+                    return 0
+                else:
+                    self.error('Failed !')
+                    return 255
 
     async def clean(self):
         await self.initialize()
-        await asyncio.gather(*[t.clean() for t in self.targets])
-        from dan.cxx import target_toolchain
-        target_toolchain.compile_commands.clear()
+        with self.context:
+            await asyncio.gather(*[t.clean() for t in self.targets])
+            # from dan.cxx import target_toolchain
+            # target_toolchain.compile_commands.clear()
```

### Comparing `dan-build-0.2.3/dan/pkgconfig/package.py` & `dan-build-0.2.4/dan/pkgconfig/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 from dan.core.requirements import RequiredPackage, parse_requirement
 from dan.core.runners import cmdline2list
 from dan.core.settings import InstallMode, InstallSettings
 from dan.core.utils import unique
 from dan.core.version import Version, VersionSpec
 from dan.cxx.targets import CXXTarget, Library
 
+import typing as t
+
 
 class MissingPackage(RuntimeError):
     def __init__(self, name) -> None:
         super().__init__(f'package {name} not found')
 
 
 def find_pkg_config(name, paths=list()) -> Path:
-    return find_file(fr'.*{name}\.pc$', ['$PKG_CONFIG_PATH', *paths, *library_paths_lookup])
+    return find_file(fr'.*{name}\.pc$', [*paths, '$PKG_CONFIG_PATH', *library_paths_lookup])
+
 
-def find_pkg_configs(name, paths=list()) -> Path:
-    return find_files(fr'.*{name}\.pc$', ['$PKG_CONFIG_PATH', *paths, *library_paths_lookup])
+def find_pkg_configs(name, paths=list()) -> t.Generator[Path, None, None]:
+    yield from find_files(fr'.*{name}\.pc$', [*paths, '$PKG_CONFIG_PATH', *library_paths_lookup])
 
 
 def has_package(name,  paths=list()):
     return find_pkg_config(name,  paths) is not None
 
 
 
@@ -157,39 +160,37 @@
                     deps.add(dep)
         self.includes.public.append(self.data.get('includedir'))
         self.dependencies.update(deps)
 
     @property
     def cxx_flags(self):
         if self.__cflags is None:
-            from dan.cxx import target_toolchain
             cflags = self.data.get('cflags')
             if cflags is not None:
                 cflags = cmdline2list(cflags)
-                cflags = target_toolchain.from_unix_flags(cflags)
+                cflags = self.toolchain.from_unix_flags(cflags)
             else:
                 cflags = list()
             for dep in self.cxx_dependencies:
                 cflags.extend(dep.cxx_flags)
             self.__cflags = unique(cflags)
         return self.__cflags
 
     @property
     def package_dependencies(self):
         return [pkg for pkg in self.dependencies if isinstance(pkg, Package)]
 
     @property
     def libs(self):
         if self.__libs is None:
-            from dan.cxx import target_toolchain
             tmp = list()
             libs = self.data.get('libs')
             if libs is not None:
                 libs = cmdline2list(libs)
-                libs = target_toolchain.from_unix_flags(libs)
+                libs = self.toolchain.from_unix_flags(libs)
                 tmp.extend(libs)
             for pkg in self.package_dependencies:
                 tmp.extend(pkg.libs)
             self.__libs = unique(tmp)
         return self.__libs
 
     @asyncio.cached
@@ -202,15 +203,15 @@
     def up_to_date(self):
         return True
 
     @property
     def modification_time(self):
         return self.config_path.modification_time
 
-    def __getattr__(self, name):        
+    def __getattr__(self, name):
         value = self.data.get(name) if self.data is not None else None
         if value is None:
             raise AttributeError(name)
         return value
 
 
 _jinja_env: jinja2.Environment = None
@@ -235,34 +236,33 @@
     if _jinja_env is None:
         _jinja_env = jinja2.Environment(
             loader=jinja2.PackageLoader('dan.pkgconfig'))
     return _jinja_env
 
 
 async def create_pkg_config(lib: Library, settings: InstallSettings) -> Path:
-    from dan.cxx import target_toolchain
     dest = settings.libraries_destination / 'pkgconfig' / f'{lib.name}.pc'
     lib.info(f'creating pkgconfig: {dest}')
 
     requires = list()
     for req in lib.requires:
         if req.version_spec:
             requires.append(f'{req.name} {req.version_spec.op} {req.version_spec.version}')
         else:
             requires.append(req.name)
 
-    libs = target_toolchain.make_link_options(
+    libs = lib.toolchain.make_link_options(
         [Path(f'${{libdir}}/{lib.name}')]) if not lib.interface else []
     libs.extend(lib.link_libraries.public)
     libs.extend(lib.link_options.public)
-    libs = target_toolchain.to_unix_flags(libs)
+    libs = lib.toolchain.to_unix_flags(libs)
 
     cflags = lib.compile_definitions.public
-    cflags.extend(target_toolchain.make_include_options(['${includedir}']))
-    cflags = target_toolchain.to_unix_flags(cflags)
+    cflags.extend(lib.toolchain.make_include_options(['${includedir}']))
+    cflags = lib.toolchain.to_unix_flags(cflags)
 
     data = _get_jinja_env()\
         .get_template('pkg.pc.jinja2')\
         .render({
             'lib': lib,
             'libs': libs,
             'cflags': cflags,
```

### Comparing `dan-build-0.2.3/dan/src/git.py` & `dan-build-0.2.4/dan/src/git.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/src/github.py` & `dan-build-0.2.4/dan/src/github.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan/src/tar.py` & `dan-build-0.2.4/dan/src/tar.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/dan_build.egg-info/PKG-INFO` & `dan-build-0.2.4/dan_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.3/dan_build.egg-info/SOURCES.txt` & `dan-build-0.2.4/dan_build.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 dan/conan/__init__.py
 dan/conan/requirements.py
 dan/core/__init__.py
 dan/core/aiofiles.py
 dan/core/asyncio.py
 dan/core/cache.py
 dan/core/detect.py
+dan/core/diagnostics.py
 dan/core/errors.py
 dan/core/find.py
 dan/core/functools.py
 dan/core/generator.py
 dan/core/include.py
 dan/core/makefile.py
 dan/core/osinfo.py
@@ -68,10 +69,12 @@
 dan/src/tar.py
 dan_build.egg-info/PKG-INFO
 dan_build.egg-info/SOURCES.txt
 dan_build.egg-info/dependency_links.txt
 dan_build.egg-info/entry_points.txt
 dan_build.egg-info/requires.txt
 dan_build.egg-info/top_level.txt
+tests/test_cxx_errors.py
 tests/test_cxx_libraries.py
 tests/test_cxx_simple.py
-tests/test_cxx_smc_catch2.py
+tests/test_cxx_src_catch2.py
+tests/test_python_errors.py
```

### Comparing `dan-build-0.2.3/pyproject.toml` & `dan-build-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.3/tests/test_cxx_libraries.py` & `dan-build-0.2.4/tests/test_cxx_libraries.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,75 +4,68 @@
 
 
 class CXXSimpleLibTest(PyMakeBaseTest):
     def __init__(self, methodName: str = None) -> None:
         super().__init__('cxx/libraries', methodName)
 
     async def test_build(self):
-        target_name = 'dan-simple-lib'
+        target_name = 'simplelib'
 
         ########################################
         async with self.section("base build", clean=True) as make:
-            target, = make.get(target_name)
+            target = make.root.find(target_name)
             await target.initialize()
             self.assertFalse(target.output.exists())
             await target.build()
             self.assertTrue(target.output.exists())
             self.modified_at = target.output.modification_time
 
-            del make, target
+        # ########################################
+        # async with self.section("no-modification => no-rebuild") as make:
+        #     target = make.root.find(target_name)
+        #     await target.build()
+        #     self.assertTrue(target.output.exists())
+        #     self.assertEqual(self.modified_at, target.output.modification_time,
+        #                     "no modifications should NOT trigger a re-build")
+
+        #     # update source
+        #     src: Path = target.source_path / list(target.sources)[0]
+        #     src.utime()
+
+        # async with self.section("source modification => rebuild") as make:
+        #     target = make.root.find(target_name)
+        #     await target.build()
+        #     self.assertTrue(target.output.younger_than(self.modified_at),
+        #                     "a source modification should trigger a re-build")
+        #     self.modified_at = target.output.modification_time
+
+
+    # async def test_install(self):
+    #     target_name = 'simplelib'
+
+    #     ########################################
+    #     async with self.section("base build",
+    #                             options=[
+    #                                 'root.library_type=shared'
+    #                             ],
+    #                             settings=[
+    #                                 f'install.destination={self.build_path}/dist'
+    #                             ],
+    #                             clean=True) as make:
+    #         self.assertEqual(make.settings.install.runtime_destination, self.build_path / 'dist/bin')
+    #         target = make.root.find(target_name)
+    #         await target.initialize()
+    #         self.assertFalse(target.output.exists())
+    #         await target.build()
+    #         self.assertTrue(target.output.exists())
+    #         modified_at = target.output.modification_time
+
+
+    #     ########################################
+    #     async with self.section("install", init=False) as make:
+    #         await make.install(InstallMode.user)
+    #         target = make.root.find(target_name)
+    #         # should be re-linked with new rpath
+    #         self.assertTrue(target.output.younger_than(modified_at))
+    #         self.assertTrue(
+    #             (self.build_path / f'dist/bin/{target_name}').exists())
 
-        ########################################
-        async with self.section("no-modification => no-rebuild") as make:
-            target, = make.get(target_name)
-            await target.build()
-            self.assertTrue(target.output.exists())
-            self.assertEqual(self.modified_at, target.output.modification_time,
-                            "no modifications should NOT trigger a re-build")
-
-            # update source
-            src: Path = target.source_path / list(target.sources)[0]
-            src.utime()
-
-            del make, target
-
-        async with self.section("source modification => rebuild") as make:
-            target, = make.get(target_name)
-            await target.build()
-            self.assertTrue(target.output.younger_than(self.modified_at),
-                            "a source modification should trigger a re-build")
-            self.modified_at = target.output.modification_time
-
-            del make, target
-
-    async def test_install(self):
-        target_name = 'dan-simple-lib'
-
-        ########################################
-        async with self.section("base build",
-                                options=[
-                                    'root.library_type=shared'
-                                ],
-                                settings=[
-                                    f'install.destination={self.build_path}/dist'
-                                ],
-                                clean=True) as make:
-            self.assertEqual(make.settings.install.runtime_destination, self.build_path / 'dist/bin')
-            target, = make.get(target_name)
-            await target.initialize()
-            self.assertFalse(target.output.exists())
-            await target.build()
-            self.assertTrue(target.output.exists())
-            modified_at = target.output.modification_time
-
-            del make, target
-
-        ########################################
-        async with self.section("install", init=False) as make:
-            await make.install(InstallMode.user)
-            target, = make.get(target_name)
-            # should be re-linked with new rpath
-            self.assertTrue(target.output.younger_than(modified_at))
-            self.assertTrue(
-                (self.build_path / f'dist/bin/{target_name}').exists())
-
-            del make, target
```

### Comparing `dan-build-0.2.3/tests/test_cxx_simple.py` & `dan-build-0.2.4/tests/test_cxx_simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,68 +7,75 @@
     def __init__(self, methodName: str = None) -> None:
         super().__init__('cxx/simple', methodName)
 
     async def test_build(self):
 
         ########################################
         async with self.section("base build", clean=True) as make:
-            target, = make.get('dan-simple')
+            target = make.root.find('simple')
             await target.initialize()
             self.assertFalse(target.output.exists())
             await target.build()
             self.assertTrue(target.output.exists())
-            self.modified_at = target.output.modification_time
-            del make, target
+            modified_at = target.output.modification_time
 
 
         ########################################
         async with self.section("no-modification => no-rebuild") as make:
-            target, = make.get('dan-simple')
+            target = make.root.find('simple')
             await target.build()
             self.assertTrue(target.output.exists())
-            self.assertEqual(self.modified_at, target.output.modification_time,
+            self.assertEqual(modified_at, target.output.modification_time,
                             "no modifications should NOT trigger a re-build")
 
             # update source
             src: Path = target.source_path / list(target.sources)[0]
             src.utime()
-            del make, target
 
         ########################################
         async with self.section("source modification => rebuild") as make:
-            target, = make.get('dan-simple')
+            target = make.root.find('simple')
             await target.build()
-            self.assertTrue(target.output.younger_than(self.modified_at),
+            self.assertTrue(target.output.younger_than(modified_at),
                             "a source modification should trigger a re-build")
-            self.modified_at = target.output.modification_time
 
+
+    async def test_option_change(self):
+
+        ########################################
+        async with self.section("base build", clean=True) as make:
+            target = make.root.find('simple')
+            await target.initialize()
+            self.assertFalse(target.output.exists())
+            await target.build()
+            self.assertTrue(target.output.exists())
+            modified_at = target.output.modification_time
+            sha1 = target.options.sha1
+            
             # change option
             greater = target.options.get('greater')
             expected_output = '=== test ==='
             greater.value = expected_output
-            await target.makefile.cache.save()
-            del make, target, greater
+            self.assertNotEqual(sha1, target.options.sha1)
 
         ########################################
         async with self.section("option modification => rebuild") as make:
-            target, = make.get('dan-simple')
+            target = make.root.find('simple')
             await target.build()
-            self.assertTrue(target.output.younger_than(self.modified_at),
+            self.assertTrue(target.output.younger_than(modified_at),
                             "an option change should trigger a re-build")
-            self.modified_at = target.output.modification_time
+            modified_at = target.output.modification_time
             out, err, rc = await target.execute()
             self.assertEqual(rc, 0)
-            self.assertEqual(out, f'{expected_output} !\n')
-
-            del make, target
-
+            self.assertEqual(out.strip(), f'{expected_output} !')
 
     async def test_install(self):
 
         ########################################
-        async with self.section("install") as make:
-            make.apply_settings(f"install.destination={self.build_path}/dist")
+        async with self.section("install",
+                                settings=[f"install.destination={self.build_path}/dist"]
+                                ) as make:
             await make.initialize()
             await make.install(InstallMode.user)
-            self.assertTrue((self.build_path / 'dist/bin/dan-simple').exists())
-
-            del make
+            bins = list((self.build_path / 'dist/bin').glob('*'))
+            self.assertEqual(len(bins), 1)
+            self.assertEqual(bins[0].stem, 'simple')
```

