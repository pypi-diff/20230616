# Comparing `tmp/msl-loadlib-0.8.0.tar.gz` & `tmp/msl-loadlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\msl-loadlib-0.8.0.tar", last modified: Sat Feb 20 04:10:07 2021, max compression
+gzip compressed data, was "msl-loadlib-0.9.0.tar", last modified: Thu May 13 04:52:33 2021, max compression
```

## Comparing `msl-loadlib-0.8.0.tar` & `msl-loadlib-0.9.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.536199 msl-loadlib-0.8.0/
--rw-rw-rw-   0        0        0      212 2021-02-20 04:10:06.000000 msl-loadlib-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9636 2021-02-20 04:10:07.536199 msl-loadlib-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     6831 2021-02-19 21:53:54.000000 msl-loadlib-0.8.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.366255 msl-loadlib-0.8.0/msl/
--rw-rw-rw-   0        0        0      181 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.366255 msl-loadlib-0.8.0/msl/examples/
--rw-rw-rw-   0        0        0       26 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.476195 msl-loadlib-0.8.0/msl/examples/loadlib/
--rw-rw-rw-   0        0        0      816 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/Trig.class
--rw-rw-rw-   0        0        0     1512 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/Trig.java
--rw-rw-rw-   0        0        0      589 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/__init__.py
--rw-rw-rw-   0        0        0    12230 2021-01-20 04:24:44.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp32.py
--rw-rw-rw-   0        0        0     6822 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp64.py
--rw-rw-rw-   0        0        0     1658 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib.cpp
--rw-rw-rw-   0        0        0     1274 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib.h
--rw-rw-rw-   0        0        0   263824 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib32.dll
--rw-rw-rw-   0        0        0     7352 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib32.so
--rw-rw-rw-   0        0        0   268525 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib64.dll
--rw-rw-rw-   0        0        0     9064 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib64.dylib
--rw-rw-rw-   0        0        0    12624 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib64.so
--rw-rw-rw-   0        0        0    11830 2021-01-19 01:53:22.000000 msl-loadlib-0.8.0/msl/examples/loadlib/dotnet32.py
--rw-rw-rw-   0        0        0     6997 2020-11-12 07:42:25.000000 msl-loadlib-0.8.0/msl/examples/loadlib/dotnet64.py
--rw-rw-rw-   0        0        0     3019 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/dotnet_lib.cs
--rw-rw-rw-   0        0        0     6144 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/dotnet_lib32.dll
--rw-rw-rw-   0        0        0     5120 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/dotnet_lib64.dll
--rw-rw-rw-   0        0        0     2285 2021-01-19 01:53:22.000000 msl-loadlib-0.8.0/msl/examples/loadlib/echo32.py
--rw-rw-rw-   0        0        0     1667 2020-11-13 07:08:44.000000 msl-loadlib-0.8.0/msl/examples/loadlib/echo64.py
--rw-rw-rw-   0        0        0    20333 2021-01-19 01:53:22.000000 msl-loadlib-0.8.0/msl/examples/loadlib/fortran32.py
--rw-rw-rw-   0        0        0     8848 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/fortran64.py
--rw-rw-rw-   0        0        0     5119 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib.f90
--rw-rw-rw-   0        0        0   667339 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib32.dll
--rw-rw-rw-   0        0        0    11824 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib32.so
--rw-rw-rw-   0        0        0   643546 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib64.dll
--rw-rw-rw-   0        0        0   472904 2020-09-12 22:24:36.000000 msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib64.dylib
--rw-rw-rw-   0        0        0    13056 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib64.so
--rw-rw-rw-   0        0        0     4653 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/java_lib.jar
--rw-rw-rw-   0        0        0     3418 2021-01-19 01:53:22.000000 msl-loadlib-0.8.0/msl/examples/loadlib/kernel32.py
--rw-rw-rw-   0        0        0     2133 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/kernel64.py
--rw-rw-rw-   0        0        0     2845 2021-01-19 01:53:22.000000 msl-loadlib-0.8.0/msl/examples/loadlib/labview32.py
--rw-rw-rw-   0        0        0     2556 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/labview64.py
--rw-rw-rw-   0        0        0      474 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/labview_lib.h
--rw-rw-rw-   0        0        0    59904 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/labview_lib32.dll
--rw-rw-rw-   0        0        0    67584 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/labview_lib64.dll
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.356259 msl-loadlib-0.8.0/msl/examples/loadlib/nz/
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.356259 msl-loadlib-0.8.0/msl/examples/loadlib/nz/msl/
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.486223 msl-loadlib-0.8.0/msl/examples/loadlib/nz/msl/examples/
--rw-rw-rw-   0        0        0      305 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/nz/msl/examples/MathUtils.java
--rw-rw-rw-   0        0        0    13040 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/nz/msl/examples/Matrix.java
--rw-rw-rw-   0        0        0      168 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/examples/loadlib/nz/msl/examples/readme.txt
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.506181 msl-loadlib-0.8.0/msl/loadlib/
--rw-rw-rw-   0        0        0      772 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/loadlib/Py4JWrapper.java
--rw-rw-rw-   0        0        0     1916 2021-02-20 03:39:27.000000 msl-loadlib-0.8.0/msl/loadlib/__init__.py
--rw-rw-rw-   0        0        0    15305 2021-01-21 21:04:12.000000 msl-loadlib-0.8.0/msl/loadlib/client64.py
--rw-rw-rw-   0        0        0     1972 2021-01-18 21:56:50.000000 msl-loadlib-0.8.0/msl/loadlib/exceptions.py
--rw-rw-rw-   0        0        0     9105 2021-01-18 21:59:18.000000 msl-loadlib-0.8.0/msl/loadlib/freeze_server32.py
--rw-rw-rw-   0        0        0    15309 2021-01-21 19:48:58.000000 msl-loadlib-0.8.0/msl/loadlib/load_library.py
--rw-rw-rw-   0        0        0     1045 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/loadlib/py4j-wrapper.jar
--rw-rw-rw-   0        0        0     9440 2021-02-19 23:49:25.000000 msl-loadlib-0.8.0/msl/loadlib/server32.py
--rw-rw-rw-   0        0        0     9339 2021-01-19 21:09:54.000000 msl-loadlib-0.8.0/msl/loadlib/start_server32.py
--rw-rw-rw-   0        0        0    11936 2021-01-18 22:02:39.000000 msl-loadlib-0.8.0/msl/loadlib/utils.py
--rwxrwxrwx   0        0        0   117248 2020-07-18 05:06:31.000000 msl-loadlib-0.8.0/msl/loadlib/verpatch.exe
-drwxrwxrwx   0        0        0        0 2021-02-20 04:10:07.536199 msl-loadlib-0.8.0/msl_loadlib.egg-info/
--rw-rw-rw-   0        0        0     9636 2021-02-20 04:10:06.000000 msl-loadlib-0.8.0/msl_loadlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1911 2021-02-20 04:10:07.000000 msl-loadlib-0.8.0/msl_loadlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-20 04:10:06.000000 msl-loadlib-0.8.0/msl_loadlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      212 2021-02-20 04:10:06.000000 msl-loadlib-0.8.0/msl_loadlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2021-02-20 04:10:06.000000 msl-loadlib-0.8.0/msl_loadlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      504 2021-02-20 04:10:07.546159 msl-loadlib-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     9116 2021-02-20 04:09:48.000000 msl-loadlib-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:33.142178 msl-loadlib-0.9.0/
+-rw-rw-rw-   0        0        0      212 2021-05-13 04:52:32.000000 msl-loadlib-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9251 2021-05-13 04:52:33.142178 msl-loadlib-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6528 2021-05-06 00:02:57.000000 msl-loadlib-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:32.782656 msl-loadlib-0.9.0/msl/
+-rw-rw-rw-   0        0        0      181 2021-05-08 02:06:41.000000 msl-loadlib-0.9.0/msl/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:32.802326 msl-loadlib-0.9.0/msl/examples/
+-rw-rw-rw-   0        0        0       26 2021-05-08 02:06:41.000000 msl-loadlib-0.9.0/msl/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:33.077287 msl-loadlib-0.9.0/msl/examples/loadlib/
+-rw-rw-rw-   0        0        0      816 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/Trig.class
+-rw-rw-rw-   0        0        0     1512 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/Trig.java
+-rw-rw-rw-   0        0        0      589 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/__init__.py
+-rw-rw-rw-   0        0        0    12230 2021-04-11 21:55:43.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp32.py
+-rw-rw-rw-   0        0        0     6822 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp64.py
+-rw-rw-rw-   0        0        0     1658 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib.cpp
+-rw-rw-rw-   0        0        0     1274 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib.h
+-rw-rw-rw-   0        0        0   263824 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib32.dll
+-rw-rw-rw-   0        0        0     7352 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib32.so
+-rw-rw-rw-   0        0        0   268525 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib64.dll
+-rw-rw-rw-   0        0        0     9064 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib64.dylib
+-rw-rw-rw-   0        0        0    12624 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib64.so
+-rw-rw-rw-   0        0        0    11830 2021-04-11 21:55:43.000000 msl-loadlib-0.9.0/msl/examples/loadlib/dotnet32.py
+-rw-rw-rw-   0        0        0     6997 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/dotnet64.py
+-rw-rw-rw-   0        0        0     3019 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/dotnet_lib.cs
+-rw-rw-rw-   0        0        0     6144 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/dotnet_lib32.dll
+-rw-rw-rw-   0        0        0     5120 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/dotnet_lib64.dll
+-rw-rw-rw-   0        0        0     2285 2021-04-11 21:55:43.000000 msl-loadlib-0.9.0/msl/examples/loadlib/echo32.py
+-rw-rw-rw-   0        0        0     1667 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/echo64.py
+-rw-rw-rw-   0        0        0    20333 2021-04-11 21:55:43.000000 msl-loadlib-0.9.0/msl/examples/loadlib/fortran32.py
+-rw-rw-rw-   0        0        0     8848 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/fortran64.py
+-rw-rw-rw-   0        0        0     5119 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib.f90
+-rw-rw-rw-   0        0        0   667339 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib32.dll
+-rw-rw-rw-   0        0        0    11824 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib32.so
+-rw-rw-rw-   0        0        0   643546 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib64.dll
+-rw-rw-rw-   0        0        0   472904 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib64.dylib
+-rw-rw-rw-   0        0        0    13056 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib64.so
+-rw-rw-rw-   0        0        0     4653 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/java_lib.jar
+-rw-rw-rw-   0        0        0     3418 2021-04-11 21:55:43.000000 msl-loadlib-0.9.0/msl/examples/loadlib/kernel32.py
+-rw-rw-rw-   0        0        0     2133 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/kernel64.py
+-rw-rw-rw-   0        0        0     2845 2021-04-11 21:55:43.000000 msl-loadlib-0.9.0/msl/examples/loadlib/labview32.py
+-rw-rw-rw-   0        0        0     2556 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/labview64.py
+-rw-rw-rw-   0        0        0      474 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/labview_lib.h
+-rw-rw-rw-   0        0        0    59904 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/labview_lib32.dll
+-rw-rw-rw-   0        0        0    67584 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/labview_lib64.dll
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:32.776557 msl-loadlib-0.9.0/msl/examples/loadlib/nz/
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:32.776557 msl-loadlib-0.9.0/msl/examples/loadlib/nz/msl/
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:33.082334 msl-loadlib-0.9.0/msl/examples/loadlib/nz/msl/examples/
+-rw-rw-rw-   0        0        0      305 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/nz/msl/examples/MathUtils.java
+-rw-rw-rw-   0        0        0    13040 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/nz/msl/examples/Matrix.java
+-rw-rw-rw-   0        0        0      168 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/examples/loadlib/nz/msl/examples/readme.txt
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:33.112439 msl-loadlib-0.9.0/msl/loadlib/
+-rw-rw-rw-   0        0        0      772 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/loadlib/Py4JWrapper.java
+-rw-rw-rw-   0        0        0     2195 2021-05-13 04:41:56.000000 msl-loadlib-0.9.0/msl/loadlib/__init__.py
+-rw-rw-rw-   0        0        0     8858 2021-05-13 03:33:47.000000 msl-loadlib-0.9.0/msl/loadlib/activex.py
+-rw-rw-rw-   0        0        0    15429 2021-05-10 04:36:58.000000 msl-loadlib-0.9.0/msl/loadlib/client64.py
+-rw-rw-rw-   0        0        0     1972 2021-04-11 21:55:43.000000 msl-loadlib-0.9.0/msl/loadlib/exceptions.py
+-rw-rw-rw-   0        0        0     9105 2021-04-11 21:55:43.000000 msl-loadlib-0.9.0/msl/loadlib/freeze_server32.py
+-rw-rw-rw-   0        0        0    16576 2021-05-07 00:18:47.000000 msl-loadlib-0.9.0/msl/loadlib/load_library.py
+-rw-rw-rw-   0        0        0     1045 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/loadlib/py4j-wrapper.jar
+-rw-rw-rw-   0        0        0    12192 2021-05-10 04:23:35.000000 msl-loadlib-0.9.0/msl/loadlib/server32.py
+-rw-rw-rw-   0        0        0     9484 2021-05-13 00:28:57.000000 msl-loadlib-0.9.0/msl/loadlib/start_server32.py
+-rw-rw-rw-   0        0        0    14461 2021-05-12 23:24:50.000000 msl-loadlib-0.9.0/msl/loadlib/utils.py
+-rwxrwxrwx   0        0        0   117248 2020-12-23 21:00:22.000000 msl-loadlib-0.9.0/msl/loadlib/verpatch.exe
+drwxrwxrwx   0        0        0        0 2021-05-13 04:52:33.142178 msl-loadlib-0.9.0/msl_loadlib.egg-info/
+-rw-rw-rw-   0        0        0     9251 2021-05-13 04:52:32.000000 msl-loadlib-0.9.0/msl_loadlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1934 2021-05-13 04:52:32.000000 msl-loadlib-0.9.0/msl_loadlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-13 04:52:32.000000 msl-loadlib-0.9.0/msl_loadlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      244 2021-05-13 04:52:32.000000 msl-loadlib-0.9.0/msl_loadlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2021-05-13 04:52:32.000000 msl-loadlib-0.9.0/msl_loadlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      556 2021-05-13 04:52:33.142178 msl-loadlib-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     8673 2021-05-03 02:06:40.000000 msl-loadlib-0.9.0/setup.py
```

### Comparing `msl-loadlib-0.8.0/PKG-INFO` & `msl-loadlib-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msl-loadlib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Load a shared library (and access a 32-bit library from 64-bit Python)
 Home-page: https://github.com/MSLNZ/msl-loadlib
 Author: Measurement Standards Laboratory of New Zealand
 Author-email: info@measurement.govt.nz
 License: MIT
 Description: ===========
         MSL-LoadLib
@@ -67,28 +67,28 @@
         
            >>> from msl.loadlib import LoadLibrary
            >>> from msl.examples.loadlib import EXAMPLES_DIR
         
         If the file extension is not included then a default extension,
         ``.dll`` (Windows) or ``.so`` (Linux), is used.
         
-        Load a `C++ <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/cpp_lib.cpp>`_
+        Load a `C++ <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/cpp_lib.cpp>`_
         library and call the ``add`` function
         
         .. invisible-code-block: pycon
         
            >>> SKIP_IF_32BIT()
         
         .. code-block:: pycon
         
            >>> cpp = LoadLibrary(EXAMPLES_DIR + '/cpp_lib64')
            >>> cpp.lib.add(1, 2)
            3
         
-        Load a `FORTRAN <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/fortran_lib.f90>`_
+        Load a `FORTRAN <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/fortran_lib.f90>`_
         library and call the ``factorial`` function
         
         .. code-block:: pycon
         
            >>> fortran = LoadLibrary(EXAMPLES_DIR + '/fortran_lib64')
         
         With a FORTRAN library you must pass values by reference using ctypes_, and, since
@@ -98,25 +98,25 @@
         .. code-block:: pycon
         
            >>> from ctypes import byref, c_int, c_double
            >>> fortran.lib.factorial.restype = c_double
            >>> fortran.lib.factorial(byref(c_int(37)))
            1.3763753091226343e+43
         
-        Load a `.NET <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/dotnet_lib.cs>`_
+        Load a `.NET <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/dotnet_lib.cs>`_
         library and call the ``reverse_string`` function, we must specify that the library
         type is a .NET library by passing in the ``'net'`` argument
         
         .. code-block:: pycon
         
            >>> net = LoadLibrary(EXAMPLES_DIR + '/dotnet_lib64.dll', 'net')
            >>> net.lib.StringManipulation().reverse_string('abcdefghijklmnopqrstuvwxyz')
            'zyxwvutsrqponmlkjihgfedcba'
         
-        Load `Java <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/Trig.java>`_
+        Load `Java <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/Trig.java>`_
         byte code and call the ``cos`` function
         
         .. code-block:: pycon
         
            >>> java = LoadLibrary(EXAMPLES_DIR + '/Trig.class')
            >>> java.lib.Trig.cos(1.234)
            0.33046510807172985
@@ -138,27 +138,14 @@
         
            >>> SKIP_IF_NOT_WINDOWS()
         
         .. code-block:: pycon
         
            >>> com = LoadLibrary('Scripting.FileSystemObject', 'com')
         
-        If creating the `com` object in the previous command raises
-        
-        .. code-block:: console
-        
-           OSError: [WinError -2147417850] Cannot change thread mode after it is set
-        
-        then perform the following and try again
-        
-        .. code-block:: pycon
-        
-           >>> import sys
-           >>> sys.coinit_flags = 0
-        
         We then use the library to create, edit and close a text file
         
         .. code-block:: pycon
         
            >>> fp = com.lib.CreateTextFile('a_new_file.txt')
            >>> fp.WriteLine('This is a test')
            0
@@ -186,19 +173,19 @@
         .. |docs| image:: https://readthedocs.org/projects/msl-loadlib/badge/?version=stable
            :target: https://msl-loadlib.readthedocs.io/en/stable/
            :alt: Documentation Status
         
         .. |pypi| image:: https://badge.fury.io/py/msl-loadlib.svg
            :target: https://badge.fury.io/py/msl-loadlib
         
-        .. |travis| image:: https://img.shields.io/travis/MSLNZ/msl-loadlib/master.svg?label=Travis-CI
+        .. |travis| image:: https://img.shields.io/travis/MSLNZ/msl-loadlib/main.svg?label=Travis-CI
            :target: https://travis-ci.org/MSLNZ/msl-loadlib
         
-        .. |appveyor| image:: https://img.shields.io/appveyor/ci/jborbely/msl-loadlib/master.svg?label=AppVeyor
-           :target: https://ci.appveyor.com/project/jborbely/msl-loadlib/branch/master
+        .. |appveyor| image:: https://img.shields.io/appveyor/ci/jborbely/msl-loadlib/main.svg?label=AppVeyor
+           :target: https://ci.appveyor.com/project/jborbely/msl-loadlib/branch/main
         
         .. _ctypes: https://docs.python.org/3/library/ctypes.html
         .. _Python for .NET: https://pythonnet.github.io/
         .. _Py4J: https://www.py4j.org/
         .. _ipc: https://en.wikipedia.org/wiki/Inter-process_communication
         .. _Java Virtual Machine: https://en.wikipedia.org/wiki/Java_virtual_machine
         .. _MSL Package Manager: https://msl-package-manager.readthedocs.io/en/latest/
@@ -224,7 +211,8 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: clr
 Provides-Extra: java
 Provides-Extra: com
 Provides-Extra: all
 Provides-Extra: tests
+Provides-Extra: docs
```

### Comparing `msl-loadlib-0.8.0/README.rst` & `msl-loadlib-0.9.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -59,28 +59,28 @@
 
    >>> from msl.loadlib import LoadLibrary
    >>> from msl.examples.loadlib import EXAMPLES_DIR
 
 If the file extension is not included then a default extension,
 ``.dll`` (Windows) or ``.so`` (Linux), is used.
 
-Load a `C++ <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/cpp_lib.cpp>`_
+Load a `C++ <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/cpp_lib.cpp>`_
 library and call the ``add`` function
 
 .. invisible-code-block: pycon
 
    >>> SKIP_IF_32BIT()
 
 .. code-block:: pycon
 
    >>> cpp = LoadLibrary(EXAMPLES_DIR + '/cpp_lib64')
    >>> cpp.lib.add(1, 2)
    3
 
-Load a `FORTRAN <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/fortran_lib.f90>`_
+Load a `FORTRAN <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/fortran_lib.f90>`_
 library and call the ``factorial`` function
 
 .. code-block:: pycon
 
    >>> fortran = LoadLibrary(EXAMPLES_DIR + '/fortran_lib64')
 
 With a FORTRAN library you must pass values by reference using ctypes_, and, since
@@ -90,25 +90,25 @@
 .. code-block:: pycon
 
    >>> from ctypes import byref, c_int, c_double
    >>> fortran.lib.factorial.restype = c_double
    >>> fortran.lib.factorial(byref(c_int(37)))
    1.3763753091226343e+43
 
-Load a `.NET <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/dotnet_lib.cs>`_
+Load a `.NET <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/dotnet_lib.cs>`_
 library and call the ``reverse_string`` function, we must specify that the library
 type is a .NET library by passing in the ``'net'`` argument
 
 .. code-block:: pycon
 
    >>> net = LoadLibrary(EXAMPLES_DIR + '/dotnet_lib64.dll', 'net')
    >>> net.lib.StringManipulation().reverse_string('abcdefghijklmnopqrstuvwxyz')
    'zyxwvutsrqponmlkjihgfedcba'
 
-Load `Java <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/Trig.java>`_
+Load `Java <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/Trig.java>`_
 byte code and call the ``cos`` function
 
 .. code-block:: pycon
 
    >>> java = LoadLibrary(EXAMPLES_DIR + '/Trig.class')
    >>> java.lib.Trig.cos(1.234)
    0.33046510807172985
@@ -130,27 +130,14 @@
 
    >>> SKIP_IF_NOT_WINDOWS()
 
 .. code-block:: pycon
 
    >>> com = LoadLibrary('Scripting.FileSystemObject', 'com')
 
-If creating the `com` object in the previous command raises
-
-.. code-block:: console
-
-   OSError: [WinError -2147417850] Cannot change thread mode after it is set
-
-then perform the following and try again
-
-.. code-block:: pycon
-
-   >>> import sys
-   >>> sys.coinit_flags = 0
-
 We then use the library to create, edit and close a text file
 
 .. code-block:: pycon
 
    >>> fp = com.lib.CreateTextFile('a_new_file.txt')
    >>> fp.WriteLine('This is a test')
    0
@@ -178,19 +165,19 @@
 .. |docs| image:: https://readthedocs.org/projects/msl-loadlib/badge/?version=stable
    :target: https://msl-loadlib.readthedocs.io/en/stable/
    :alt: Documentation Status
 
 .. |pypi| image:: https://badge.fury.io/py/msl-loadlib.svg
    :target: https://badge.fury.io/py/msl-loadlib
 
-.. |travis| image:: https://img.shields.io/travis/MSLNZ/msl-loadlib/master.svg?label=Travis-CI
+.. |travis| image:: https://img.shields.io/travis/MSLNZ/msl-loadlib/main.svg?label=Travis-CI
    :target: https://travis-ci.org/MSLNZ/msl-loadlib
 
-.. |appveyor| image:: https://img.shields.io/appveyor/ci/jborbely/msl-loadlib/master.svg?label=AppVeyor
-   :target: https://ci.appveyor.com/project/jborbely/msl-loadlib/branch/master
+.. |appveyor| image:: https://img.shields.io/appveyor/ci/jborbely/msl-loadlib/main.svg?label=AppVeyor
+   :target: https://ci.appveyor.com/project/jborbely/msl-loadlib/branch/main
 
 .. _ctypes: https://docs.python.org/3/library/ctypes.html
 .. _Python for .NET: https://pythonnet.github.io/
 .. _Py4J: https://www.py4j.org/
 .. _ipc: https://en.wikipedia.org/wiki/Inter-process_communication
 .. _Java Virtual Machine: https://en.wikipedia.org/wiki/Java_virtual_machine
 .. _MSL Package Manager: https://msl-package-manager.readthedocs.io/en/latest/
```

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/Trig.class` & `msl-loadlib-0.9.0/msl/examples/loadlib/Trig.class`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/Trig.java` & `msl-loadlib-0.9.0/msl/examples/loadlib/Trig.java`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/__init__.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/__init__.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp32.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp32.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp64.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp64.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib.cpp` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib.cpp`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib.h` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib.h`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib32.dll` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib32.dll`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib32.so` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib32.so`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib64.dll` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib64.dll`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib64.dylib` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib64.dylib`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/cpp_lib64.so` & `msl-loadlib-0.9.0/msl/examples/loadlib/cpp_lib64.so`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/dotnet32.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/dotnet32.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/dotnet64.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/dotnet64.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/dotnet_lib.cs` & `msl-loadlib-0.9.0/msl/examples/loadlib/dotnet_lib.cs`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/dotnet_lib32.dll` & `msl-loadlib-0.9.0/msl/examples/loadlib/dotnet_lib32.dll`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/dotnet_lib64.dll` & `msl-loadlib-0.9.0/msl/examples/loadlib/dotnet_lib64.dll`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/echo32.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/echo32.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/echo64.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/echo64.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/fortran32.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/fortran32.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/fortran64.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/fortran64.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib.f90` & `msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib.f90`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib32.dll` & `msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib32.dll`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib32.so` & `msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib32.so`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib64.dll` & `msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib64.dll`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib64.dylib` & `msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib64.dylib`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/fortran_lib64.so` & `msl-loadlib-0.9.0/msl/examples/loadlib/fortran_lib64.so`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/java_lib.jar` & `msl-loadlib-0.9.0/msl/examples/loadlib/java_lib.jar`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/kernel32.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/kernel32.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/kernel64.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/kernel64.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/labview32.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/labview32.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/labview64.py` & `msl-loadlib-0.9.0/msl/examples/loadlib/labview64.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/labview_lib32.dll` & `msl-loadlib-0.9.0/msl/examples/loadlib/labview_lib32.dll`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/labview_lib64.dll` & `msl-loadlib-0.9.0/msl/examples/loadlib/labview_lib64.dll`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/examples/loadlib/nz/msl/examples/Matrix.java` & `msl-loadlib-0.9.0/msl/examples/loadlib/nz/msl/examples/Matrix.java`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/loadlib/Py4JWrapper.java` & `msl-loadlib-0.9.0/msl/loadlib/Py4JWrapper.java`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/loadlib/__init__.py` & `msl-loadlib-0.9.0/msl/loadlib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,27 @@
 """
 import re
 import sys
 from collections import namedtuple
 
 __author__ = 'Measurement Standards Laboratory of New Zealand'
 __copyright__ = '\xa9 2017 - 2021, ' + __author__
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 _v = re.search(r'(\d+)\.(\d+)\.(\d+)[.-]?(.*)', __version__).groups()
 
 version_info = namedtuple('version_info', 'major minor micro releaselevel')(int(_v[0]), int(_v[1]), int(_v[2]), 'final')
 """:obj:`~collections.namedtuple`: Contains the version information as a (major, minor, micro, releaselevel) tuple."""
 
+if not hasattr(sys, 'coinit_flags'):
+    # Configure comtypes to use COINIT_MULTITHREADED when it is imported.
+    # This avoids the following exception from being raised:
+    #   [WinError -2147417850] Cannot change thread mode after it is set
+    sys.coinit_flags = 0x0
+
 IS_WINDOWS = sys.platform == 'win32'
 """:class:`bool`: Whether the operating system is Windows."""
 
 IS_LINUX = sys.platform.startswith('linux')
 """:class:`bool`: Whether the operating system is Linux."""
 
 IS_MAC = sys.platform == 'darwin'
```

### Comparing `msl-loadlib-0.8.0/msl/loadlib/client64.py` & `msl-loadlib-0.9.0/msl/loadlib/client64.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         in :data:`sys.path` so that those modules can be imported when `module32`
         is imported.
 
         Raises
         ------
         ~msl.loadlib.exceptions.ConnectionTimeoutError
             If the connection to the 32-bit server cannot be established.
-        IOError
+        OSError
             If the frozen executable cannot be found.
         TypeError
             If the data type of `append_sys_path` or `append_environ_path` is invalid.
         """
         self._meta32 = None
         self._conn = None
 
@@ -140,15 +140,15 @@
                 self._pickle_protocol = 4
         else:
             self._pickle_protocol = protocol
 
         # make sure that the server32 executable exists
         server_exe = os.path.join(os.path.dirname(__file__), SERVER_FILENAME)
         if not os.path.isfile(server_exe):
-            raise IOError('Cannot find ' + server_exe)
+            raise OSError('Cannot find ' + server_exe)
 
         cmd = [
             server_exe,
             '--module', module32,
             '--host', host,
             '--port', str(port)
         ]
@@ -244,21 +244,22 @@
         Returns
         -------
         :class:`str`
             The path to the 32-bit shared-library file.
         """
         return self._meta32['path']
 
-    def request32(self, method32, *args, **kwargs):
+    def request32(self, name, *args, **kwargs):
         """Send a request to the 32-bit server.
 
         Parameters
         ----------
-        method32 : :class:`str`
-            The name of the method to call in the :class:`~.server32.Server32` subclass.
+        name : :class:`str`
+            The name of an attribute of the :class:`~.server32.Server32` subclass.
+            The name can be a method, property or any attribute.
         *args
             The arguments that the method in the :class:`~.server32.Server32` subclass requires.
         **kwargs
             The keyword arguments that the method in the :class:`~.server32.Server32` subclass requires.
 
         Returns
         -------
@@ -270,31 +271,33 @@
             If there was an error processing the request on the 32-bit server.
         ~msl.loadlib.exceptions.ResponseTimeoutError
             If a timeout occurs while waiting for the response from the 32-bit server.
         """
         if self._conn is None:
             raise Server32Error('The 32-bit server is not active')
 
-        with open(self._pickle_path, 'wb') as f:
+        with open(self._pickle_path, mode='wb') as f:
             pickle.dump(args, f, protocol=self._pickle_protocol)
             pickle.dump(kwargs, f, protocol=self._pickle_protocol)
 
-        self._conn.request('GET', method32)
+        self._conn.request('GET', name)
 
         try:
             response = self._conn.getresponse()
         except socket.timeout:
             response = None
 
         if response is None:
-            raise ResponseTimeoutError('Waiting for the response from the {!r} request timed '
-                                       'out after {} seconds'.format(method32, self._rpc_timeout))
+            raise ResponseTimeoutError(
+                'Waiting for the response from the {!r} request timed '
+                'out after {} seconds'.format(name, self._rpc_timeout)
+            )
 
         if response.status == OK:
-            with open(self._pickle_path, 'rb') as f:
+            with open(self._pickle_path, mode='rb') as f:
                 result = pickle.load(f)
             return result
 
         raise Server32Error(**json.loads(response.read().decode(encoding='utf-8', errors='replace')))
 
     def shutdown_server32(self, kill_timeout=10):
         """Shutdown the 32-bit server.
@@ -361,9 +364,11 @@
             os.remove(self._pickle_path)
 
         self._conn.close()
         self._conn = None
         return self._proc.stdout, self._proc.stderr
 
     def __del__(self):
-        if self._conn is not None:
-            self.shutdown_server32()
+        if hasattr(self, '_conn'):
+            out, err = self.shutdown_server32()
+            out.close()
+            err.close()
```

### Comparing `msl-loadlib-0.8.0/msl/loadlib/exceptions.py` & `msl-loadlib-0.9.0/msl/loadlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/loadlib/freeze_server32.py` & `msl-loadlib-0.9.0/msl/loadlib/freeze_server32.py`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/loadlib/load_library.py` & `msl-loadlib-0.9.0/msl/loadlib/load_library.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,81 +14,89 @@
 )
 
 _encoding = sys.getfilesystemencoding()
 
 
 class LoadLibrary(object):
 
+    LIBTYPES = ['cdll', 'windll', 'oledll', 'net', 'clr', 'java', 'com', 'activex']
+    """The library types that are supported."""
+
     def __init__(self, path, libtype=None, **kwargs):
         """Load a shared library.
 
         For example, a C/C++, FORTRAN, C#, Java, Delphi, LabVIEW, ActiveX, ... library.
 
-        Based on the value of `libtype` this class will load the shared library as a:
-
-            * :class:`~ctypes.CDLL` if `libtype` is ``'cdll'``,
-            * :class:`~ctypes.WinDLL` if `libtype` is ``'windll'``,
-            * :class:`~ctypes.OleDLL` if `libtype` is ``'oledll'``,
-            * `System.Reflection.Assembly <Assembly_>`_ if `libtype` is ``'net'`` or ``'clr'`` ,
-            * :class:`~.py4j.java_gateway.JavaGateway` if `libtype` is ``'java'``, or
-            * comtypes.CreateObject_ if `libtype` is ``'com'``.
-
         .. versionchanged:: 0.4
            Added support for Java archives.
 
         .. versionchanged:: 0.5
            Added support for COM_ libraries.
 
-        .. _Assembly: https://msdn.microsoft.com/en-us/library/system.reflection.assembly(v=vs.110).aspx
+        .. versionchanged:: 0.9
+           Added support for ActiveX_ libraries.
+
+        .. _Assembly: https://docs.microsoft.com/en-us/dotnet/api/system.reflection.assembly
         .. _comtypes.CreateObject: https://pythonhosted.org/comtypes/#creating-and-accessing-com-objects
         .. _COM: https://en.wikipedia.org/wiki/Component_Object_Model
+        .. _ActiveX: https://en.wikipedia.org/wiki/ActiveX
 
         Parameters
         ----------
         path : :class:`str`
             The path to the shared library.
 
             The search order for finding the shared library is:
 
                 1. assume that a full or a relative (to the current working directory)
                    path is specified,
                 2. use :func:`ctypes.util.find_library` to find the shared library file,
                 3. search :data:`sys.path`, then
                 4. search :data:`os.environ['PATH'] <os.environ>` to find the shared library.
 
-            If loading a COM_ library then `path` represents the `progid <comtypes.CreateObject_>`_
-            argument.
+            If loading a COM_ library then `path` is either the `ProgID`, e.g.
+            ``"InternetExplorer.Application"``, or the `CLSID`, e.g.
+            ``"{2F7860A2-1473-4D75-827D-6C4E27600CAC}"``.
 
         libtype : :class:`str`, optional
             The library type. The following values are currently supported:
 
             * ``'cdll'`` -- for a library that uses the __cdecl calling convention
             * ``'windll'`` or ``'oledll'`` -- for a __stdcall calling convention
             * ``'net'`` or ``'clr'`` -- for Microsoft's .NET Framework (Common Language Runtime)
             * ``'java'`` -- for a Java archive, ``.jar``, or Java byte code, ``.class``, file
-            * ``'com'`` -- for a COM_ library.
+            * ``'com'`` -- for a COM_ library
+            * ``'activex'`` -- for an ActiveX_ library
 
             Default is ``'cdll'``.
 
             .. tip::
                Since the ``.jar`` or ``.class`` extension uniquely defines a Java library,
                the `libtype` will be automatically set to ``'java'`` if `path` ends with
-               ``.jar`` or ``.class``. If `path` starts with ``'{'`` and ends with ``'}'``
-               then this uniquely defines the Class ID for a COM_ library and so `libtype`
-               will be automatically set to ``'com'``.
+               ``.jar`` or ``.class``.
 
         **kwargs
-            Keyword arguments that are passed to the object that loads the library.
+            All additional keyword arguments are passed to the object that loads the library.
+
+            If `libtype` is
+
+                * ``'cdll'`` then :class:`~ctypes.CDLL`
+                * ``'windll'`` then :class:`~ctypes.WinDLL`
+                * ``'oledll'`` then :class:`~ctypes.OleDLL`
+                * ``'net'`` or ``'clr'`` then all keyword arguments are ignored
+                * ``'java'`` then :class:`~.py4j.java_gateway.JavaGateway`
+                * ``'com'`` then comtypes.CreateObject_
+                * ``'activex'`` then :meth:`Application.load <msl.loadlib.activex.Application.load>`
 
         Raises
         ------
-        IOError
+        OSError
             If the shared library cannot be loaded.
-        TypeError
-            If `libtype` is not a supported library type.
+        ValueError
+            If the value of `libtype` is not supported.
         """
         # a reference to the shared library
         self._lib = None
 
         # a reference to the .NET Runtime Assembly
         self._assembly = None
 
@@ -100,38 +108,42 @@
 
         # fixes Issue #8, if `path` is a <class 'pathlib.Path'> object
         if hasattr(path, 'as_posix'):
             path = path.as_posix()
 
         # try to automatically determine the libtype
         if libtype is None:
-            if path.startswith('{') and path.endswith('}'):
-                libtype = 'com'
-            elif path.endswith('.jar') or path.endswith('.class'):
+            if path.endswith('.jar') or path.endswith('.class'):
                 libtype = 'java'
             else:
                 libtype = 'cdll'
         else:
             libtype = libtype.lower()
 
+        if libtype not in LoadLibrary.LIBTYPES:
+            raise ValueError(
+                'Cannot load libtype={!r}.\n'
+                'Must be one of: {}'.format(libtype, ', '.join(LoadLibrary.LIBTYPES))
+            )
+
         # create a new reference to `path` just in case the
         # DEFAULT_EXTENSION is appended below so that the
         # ctypes.util.find_library function call will use the
         # unmodified value of `path`
         _path = path
 
         # assume a default extension if no extension was provided
         ext = os.path.splitext(path)[1]
-        if libtype != 'java' and libtype != 'com' and not ext:
+        if not ext and libtype not in ['java', 'com', 'activex']:
             _path += DEFAULT_EXTENSION
 
         if IS_PYTHON2:
             _path = _path.encode(_encoding)
 
-        if libtype != 'com':
+        if libtype not in ['com', 'activex']:
             self._path = os.path.abspath(_path)
             if not os.path.isfile(self._path):
                 # for find_library use the original 'path' value since it may be a library name
                 # without any prefix like 'lib', suffix like '.so', '.dylib' or version number
                 self._path = ctypes.util.find_library(path)
                 if self._path is None:  # then search sys.path and os.environ['PATH']
                     success = False
@@ -139,34 +151,54 @@
                     for directory in search_dirs:
                         p = os.path.join(directory, _path)
                         if os.path.isfile(p):
                             self._path = p
                             success = True
                             break
                     if not success:
-                        raise IOError('Cannot find the shared library {!r}'.format(path))
+                        raise OSError("Cannot find '{}' for libtype='{}'".format(path, libtype))
         else:
             self._path = _path
 
         if libtype == 'cdll':
             self._lib = ctypes.CDLL(self._path, **kwargs)
         elif libtype == 'windll':
             self._lib = ctypes.WinDLL(self._path, **kwargs)
         elif libtype == 'oledll':
             self._lib = ctypes.OleDLL(self._path, **kwargs)
         elif libtype == 'com':
             if not utils.is_comtypes_installed():
-                raise IOError('Cannot load a COM library because comtypes is not installed.\n'
-                              'To install comtypes run: pip install comtypes')
+                raise OSError(
+                    'Cannot load a COM library because comtypes is not installed.\n'
+                    'Run: pip install comtypes'
+                )
+
+            from comtypes import GUID
             from comtypes.client import CreateObject
-            self._lib = CreateObject(self._path, **kwargs)
+
+            try:
+                clsid = GUID.from_progid(self._path)
+            except (TypeError, OSError):
+                clsid = None
+
+            if clsid is None:
+                raise OSError("Cannot find '{}' for libtype='com'".format(path))
+
+            self._lib = CreateObject(clsid, **kwargs)
+
+        elif libtype == 'activex':
+            from .activex import Application
+            self._lib = Application.load(self._path, **kwargs)
+
         elif libtype == 'java':
             if not utils.is_py4j_installed():
-                raise IOError('Cannot load a Java file because Py4J is not installed.\n'
-                              'To install Py4J run: pip install py4j')
+                raise OSError(
+                    'Cannot load a Java file because Py4J is not installed.\n'
+                    'Run: pip install py4j'
+                )
 
             from py4j.version import __version__
             from py4j.java_gateway import JavaGateway, GatewayParameters
 
             # the address and port to use to host the py4j.GatewayServer
             address = kwargs.pop('address', '127.0.0.1')
             port = kwargs.pop('port', utils.get_available_port())
@@ -177,16 +209,18 @@
             py4j_jar = os.path.join(root, 'share', 'py4j', filename)
             if not os.path.isfile(py4j_jar):
                 root = os.path.dirname(root)  # then check one folder up (for unix or venv)
                 py4j_jar = os.path.join(root, 'share', 'py4j', filename)
                 if not os.path.isfile(py4j_jar):
                     py4j_jar = os.environ.get('PY4J_JAR', '')  # then check the environment variable
                     if not os.path.isfile(py4j_jar):
-                        raise IOError('Cannot find {0}\nCreate a PY4J_JAR environment '
-                                      'variable to be equal to the full path to {0}'.format(filename))
+                        raise OSError(
+                            'Cannot find {0}\nCreate a PY4J_JAR environment '
+                            'variable to be equal to the full path to {0}'.format(filename)
+                        )
 
             # build the java command
             wrapper = os.path.join(os.path.dirname(__file__), 'py4j-wrapper.jar')
             cmd = ['java', '-cp', py4j_jar + os.pathsep + wrapper, 'Py4JWrapper', str(port)]
 
             # from the URLClassLoader documentation:
             #   Any URL that ends with a '/' is assumed to refer to a directory. Otherwise, the URL
@@ -196,47 +230,55 @@
             else:  # it is a .class file
                 cmd.append(os.path.dirname(self._path) + '/')
 
             try:
                 # start the py4j.GatewayServer
                 subprocess.Popen(cmd, stderr=subprocess.PIPE, stdout=subprocess.PIPE)
                 err = None
-            except IOError as e:
+            except OSError as e:
                 err = str(e) + '\nYou must have a Java Runtime Environment installed and available on PATH'
 
             if err:
-                raise IOError(err)
+                raise OSError(err)
 
             utils.wait_for_server(address, port, 5.0)
 
             self._gateway = JavaGateway(
                 gateway_parameters=GatewayParameters(address=address, port=port, **kwargs)
             )
 
             self._lib = self._gateway.jvm
 
         elif libtype == 'net' or libtype == 'clr':
             if not utils.is_pythonnet_installed():
-                raise IOError('Cannot load a .NET Assembly because pythonnet is not installed.\n'
-                              'To install pythonnet run: pip install pythonnet')
+                raise OSError(
+                    'Cannot load a .NET Assembly because pythonnet is not installed.\n'
+                    'Run: pip install pythonnet'
+                )
 
             import clr
+            import System
+            dotnet = {'System': System}
 
             # the shared library must be available in sys.path
             head, tail = os.path.split(self._path)
             sys.path.insert(0, head)
 
-            # don't include the library extension
-            clr.AddReference(os.path.splitext(tail)[0])
-
-            import System
-            dotnet = {'System': System}
+            try:
+                # don't include the library extension
+                clr.AddReference(os.path.splitext(tail)[0])
+            except System.IO.FileNotFoundException:
+                # The file must exist since its existence is checked above.
+                # There must be another reason why loading the DLL raises this
+                # error. Calling LoadFile (below) provides more information
+                # in the error message.
+                pass
 
             try:
-                # By default, pythonnet can only load libraries that are for .NET 4.0+.3.9
+                # By default, pythonnet can only load libraries that are for .NET 4.0+
                 #
                 # In order to allow pythonnet to load a library from .NET <4.0 the
                 # useLegacyV2RuntimeActivationPolicy property needs to be enabled
                 # in a <python-executable>.config file. If the following statement
                 # raises a FileLoadException then attempt to create the configuration
                 # file that has the property enabled and then notify the user why
                 # loading the library failed and ask them to re-run their Python
@@ -246,24 +288,24 @@
             except System.IO.FileLoadException as err:
                 # Example error message that can occur if the library is for .NET <4.0,
                 # and the useLegacyV2RuntimeActivationPolicy is not enabled:
                 #
                 # " Mixed mode assembly is built against version 'v2.0.50727' of the
                 #  runtime and cannot be loaded in the 4.0 runtime without additional
                 #  configuration information. "
-                if str(err).startswith('Mixed mode assembly'):
+                if str(err).startswith('Mixed mode assembly is built against version'):
                     status, msg = utils.check_dot_net_config(sys.executable)
                     if not status == 0:
-                        raise IOError(msg)
+                        raise OSError(msg)
                     else:
                         update_msg = 'Checking .NET config returned "{}" '.format(msg)
                         update_msg += 'and still cannot load library.\n'
                         update_msg += str(err)
-                        raise IOError(update_msg)
-                raise IOError('The above "System.IO.FileLoadException" is not handled.\n')
+                        raise OSError(update_msg)
+                raise OSError('The above "System.IO.FileLoadException" is not handled.\n')
 
             try:
                 types = self._assembly.GetTypes()
             except Exception as e:
                 utils.logger.error(e)
                 utils.logger.error('The LoaderExceptions are:')
                 for item in e.LoaderExceptions:
@@ -281,15 +323,15 @@
 
                     if obj.__name__ not in dotnet:
                         dotnet[obj.__name__] = obj
 
             self._lib = DotNet(dotnet, self._path)
 
         else:
-            raise TypeError('Cannot load libtype={}'.format(libtype))
+            assert False, 'Should not get here -- contact developers'
 
         if IS_PYTHON2:
             self._path = self._path.decode(_encoding)
 
         utils.logger.debug('Loaded ' + self._path)
 
     def __repr__(self):
@@ -300,20 +342,20 @@
         if self._gateway is not None:
             self._gateway.shutdown()
             utils.logger.debug('shutdown py4j.GatewayServer')
 
     @property
     def assembly(self):
         """
-        Returns a reference to the `.NET Runtime Assembly <Assembly_>`_ object, only if
-        the shared library is a .NET Framework, otherwise returns :data:`None`.
+        Returns a reference to the `.NET Runtime Assembly <Assembly_>`_ object if
+        the shared library is a .NET Framework otherwise returns :data:`None`.
 
         .. tip::
            The `JetBrains dotPeek`_ program can be used to reliably decompile any
-           .NET Assembly in to the equivalent source code.
+           .NET Assembly into the equivalent source code.
 
         .. _JetBrains dotPeek: https://www.jetbrains.com/decompiler/
         """
         return self._assembly
 
     @property
     def gateway(self):
@@ -330,15 +372,15 @@
         For example, if `libtype` is
 
             * ``'cdll'`` then a :class:`~ctypes.CDLL` object
             * ``'windll'`` then a :class:`~ctypes.WinDLL` object
             * ``'oledll'`` then a :class:`~ctypes.OleDLL` object
             * ``'net'`` or ``'clr'`` then a :class:`~.load_library.DotNet` object
             * ``'java'`` then a :class:`~py4j.java_gateway.JVMView` object
-            * ``'com'`` then the interface pointer returned by comtypes.CreateObject_
+            * ``'com'`` or ``'activex'`` then an interface pointer to the COM_ object
         """
         return self._lib
 
     @property
     def path(self):
         """:class:`str`: The path to the shared library file."""
         return self._path
@@ -348,14 +390,14 @@
 
     def __init__(self, dot_net_dict, path):
         """Contains the namespace_ modules, classes and `System.Type`_ objects of a .NET Assembly.
 
         Do not instantiate this class directly.
 
         .. _namespace: https://msdn.microsoft.com/en-us/library/z2kcy19k.aspx
-        .. _System.Type: https://msdn.microsoft.com/en-us/library/system.type(v=vs.110).aspx
+        .. _System.Type: https://docs.microsoft.com/en-us/dotnet/api/system.type
         """
         self.__dict__.update(dot_net_dict)
         self._path = path
 
     def __repr__(self):
         return '<{} path={}>'.format(self.__class__.__name__, self._path)
```

### Comparing `msl-loadlib-0.8.0/msl/loadlib/py4j-wrapper.jar` & `msl-loadlib-0.9.0/msl/loadlib/py4j-wrapper.jar`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl/loadlib/server32.py` & `msl-loadlib-0.9.0/msl/loadlib/server32.py`

 * *Files 24% similar despite different names*

```diff
@@ -48,81 +48,72 @@
 
         .. _standard: https://docs.python.org/3/py-modindex.html
         .. _JVM: https://en.wikipedia.org/wiki/Java_virtual_machine
 
         Parameters
         ----------
         path : :class:`str`
-            The path to the 32-bit library.
+            The path to the 32-bit library. See :class:`.LoadLibrary` for more details.
         libtype : :class:`str`
-            The library type to use for the calling convention. One of the following:
-
-                * ``'cdll'`` -- for a __cdecl library
-                * ``'windll'`` or ``'oledll'`` -- for a __stdcall library (Windows only)
-                * ``'net'`` or ``'clr'`` -- for Microsoft's .NET Framework (Common Language Runtime)
-                * ``'com'`` -- for a `COM <https://en.wikipedia.org/wiki/Component_Object_Model>`_ library.
+            The library type. See :class:`.LoadLibrary` for more details.
 
             .. note::
                Since Java byte code is executed on the JVM_ it does not make sense to
                use :class:`Server32` for a Java ``.jar`` or ``.class`` file.
 
         host : :class:`str`
             The IP address of the server.
         port : :class:`int`
-            The port to open on the server.
+            The port to run the server on.
         *args
             All additional arguments are currently ignored.
         **kwargs
             All keyword arguments are passed to :class:`.LoadLibrary`.
-
-        Raises
-        ------
-        IOError
-            If the shared library cannot be loaded.
-        TypeError
-            If the value of `libtype` is not supported.
         """
         self._library = LoadLibrary(path, libtype=libtype, **kwargs)
+        self._assembly = self._library.assembly
+        self._lib = self._library.lib
+        self._path = self._library.path
         super(Server32, self).__init__((host, int(port)), _RequestHandler)
 
     @property
     def assembly(self):
         """
-        Returns a reference to the `.NET Runtime Assembly <NET_>`_ object, *only if
-        the shared library is a .NET Framework*, otherwise returns :data:`None`.
+        Returns a reference to the `.NET Runtime Assembly <NET_>`_ object if
+        the shared library is a .NET Framework otherwise returns :data:`None`.
 
         .. tip::
            The `JetBrains dotPeek`_ program can be used to reliably decompile any
-           .NET Assembly in to the equivalent source code.
+           .NET Assembly into the equivalent source code.
 
-        .. _NET: https://msdn.microsoft.com/en-us/library/system.reflection.assembly(v=vs.110).aspx
+        .. _NET: https://docs.microsoft.com/en-us/dotnet/api/system.reflection.assembly
         .. _JetBrains dotPeek: https://www.jetbrains.com/decompiler/
         """
-        return self._library.assembly
+        return self._assembly
 
     @property
     def lib(self):
-        """Returns the reference to the 32-bit, loaded library object.
+        """Returns the reference to the 32-bit, loaded-library object.
 
         For example, if `libtype` is
 
-        * ``'cdll'`` then a :class:`~ctypes.CDLL` object
-        * ``'windll'`` then a :class:`~ctypes.WinDLL` object
-        * ``'oledll'`` then a :class:`~ctypes.OleDLL` object
-        * ``'net'`` or ``'clr'`` then a :class:`~.load_library.DotNet` object
-        * ``'com'`` then the interface pointer returned by comtypes.CreateObject_
+            * ``'cdll'`` then a :class:`~ctypes.CDLL` object
+            * ``'windll'`` then a :class:`~ctypes.WinDLL` object
+            * ``'oledll'`` then a :class:`~ctypes.OleDLL` object
+            * ``'net'`` or ``'clr'`` then a :class:`~.load_library.DotNet` object
+            * ``'com'`` or ``'activex'`` then an interface pointer to the COM_ object
 
-        .. _comtypes.CreateObject: https://pythonhosted.org/comtypes/#creating-and-accessing-com-objects
+        .. _COM: https://en.wikipedia.org/wiki/Component_Object_Model
         """
-        return self._library.lib
+        return self._lib
 
     @property
     def path(self):
         """:class:`str`: The path to the shared library file."""
-        return self._library.path
+        return self._path
 
     @staticmethod
     def version():
         """Gets the version of the Python interpreter that the 32-bit server is running on.
 
         Returns
         -------
@@ -176,25 +167,118 @@
     def quiet(self):
         """This attribute is no longer used and it will be removed in a future release.
 
         Returns :data:`True`.
         """
         warnings.simplefilter('once', DeprecationWarning)
         warnings.warn(
-            'The `quiet` attribute for Server32 will be removed in version 0.9 -- attribute returns True',
+            'The `quiet` attribute for Server32 will be removed in a future release -- always returns True',
             DeprecationWarning,
             stacklevel=2
         )
         return True
 
+    @staticmethod
+    def remove_site_packages_64bit():
+        """Remove the site-packages directory from the 64-bit process.
+
+        By default the site-packages directory of the 64-bit process is
+        included in :data:`sys.path` of the 32-bit process. Having the
+        64-bit site-packages directory available can sometimes cause issues.
+        For example, comtypes imports numpy so if numpy is installed in the
+        64-bit process then comtypes will import the 64-bit version of numpy
+        in the 32-bit process. Depending on the version of Python and/or numpy
+        this can cause the 32-bit server to crash.
+
+        .. versionadded:: 0.9
+
+        Examples
+        --------
+        ::
+
+            import sys
+            from msl.loadlib import Server32
+
+            class FileSystem(Server32):
+
+                def __init__(self, host, port, **kwargs):
+
+                    # remove the site-packages directory that was passed from 64-bit Python
+                    # before calling the super() function to load the COM library
+                    path = Server32.remove_site_packages_64bit()
+
+                    super(FileSystem, self).__init__('Scripting.FileSystemObject', 'com', host, port)
+
+                    # optional: add the site-packages directory back into sys.path
+                    sys.path.append(path)
+
+        Returns
+        -------
+        :class:`str`
+            The path of the site-packages directory that was removed. Can be an
+            empty string if the directory was not found in :data:`sys.path`.
+        """
+        for index, path in enumerate(sys.path):
+            if path.endswith('site-packages'):
+                return sys.path.pop(index)
+        return ''
+
+    @staticmethod
+    def is_interpreter():
+        """Check if code is running on the 32-bit server.
+
+        If the same module is executed by both
+        :class:`~msl.loadlib.client64.Client64` and :class:`.Server32`
+        then there may be only parts of the code that should be executed
+        by the correct bitness of the Python interpreter.
+
+        .. versionadded:: 0.9
+
+        Returns
+        -------
+        :class:`bool`
+            Whether the code is running on the 32-bit server.
+
+        Examples
+        --------
+        ::
+
+            import sys
+            from msl.loadlib import Server32
+
+            if Server32.is_interpreter():
+                # this only gets executed on the 32-bit server
+                assert sys.maxsize < 2**32
+
+        """
+        return sys.executable.endswith(SERVER_FILENAME)
+
+    @staticmethod
+    def examples_dir():
+        """Get the directory where the example libraries are located.
+
+        .. versionadded:: 0.9
+
+        Returns
+        -------
+        :class:`str`
+            The directory where the example libraries are located.
+        """
+        if Server32.is_interpreter():
+            root = os.path.dirname(sys.executable)
+        else:
+            root = os.path.dirname(__file__)
+        path = os.path.join(root, os.pardir, 'examples', 'loadlib')
+        return os.path.abspath(path)
+
     def shutdown_handler(self):
         """Proxy function that is called immediately prior to the server shutting down.
 
         The intended use case is for the server to do any necessary cleanup, such as stopping
-        locally started threads, closing file-handles, etc. before it shuts down.
+        locally started threads or closing file handles before it shuts down.
 
         .. versionadded:: 0.6
         """
         pass
 
 
 class _RequestHandler(BaseHTTPRequestHandler):
@@ -202,25 +286,25 @@
 
     def do_GET(self):
         """Handle a GET request."""
         try:
             if self.path == METADATA:
                 response = {'path': self.server.path, 'pid': os.getpid()}
             else:
-                with open(self.server.pickle_path, 'rb') as f:
+                with open(self.server.pickle_path, mode='rb') as f:
                     args = pickle.load(f)
                     kwargs = pickle.load(f)
 
                 attr = getattr(self.server, self.path)
                 if callable(attr):
                     response = attr(*args, **kwargs)
                 else:
                     response = attr
 
-            with open(self.server.pickle_path, 'wb') as f:
+            with open(self.server.pickle_path, mode='wb') as f:
                 pickle.dump(response, f, protocol=self.server.pickle_protocol)
 
             self.send_response(OK)
             self.end_headers()
 
         except Exception as e:
             print('{}: {}'.format(e.__class__.__name__, e))
```

### Comparing `msl-loadlib-0.8.0/msl/loadlib/start_server32.py` & `msl-loadlib-0.9.0/msl/loadlib/start_server32.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     if args.quiet:
         print('DeprecationWarning: the --quiet flag is ignored and will be removed in a future release')
 
     # if you get to this point in the script that means you want to start a server for
     # inter-process communication and therefore args.module must have a value
     if not args.module:
         err = 'You must specify a Python module to run on the 32-bit server.\n' \
-              'For example: {} -m my_module.py\n' \
+              'For example: {} -m my_module\n' \
               'Cannot start the 32-bit server.'.format(SERVER_FILENAME)
         print(err, file=sys.stderr)
         return -1
 
     args.module = os.path.basename(args.module)
     if args.module.endswith('.py'):
         args.module = args.module[:-3]
@@ -165,39 +165,44 @@
     if cls is None:
         err = 'AttributeError: module {}.py\n' \
               'Module does not contain a class that is a subclass of Server32.\n' \
               'Cannot start the 32-bit server.'.format(args.module)
         print(err, file=sys.stderr)
         return -1
 
-    server, err = None, ''
+    server, error = None, None
     try:
         server = cls(args.host, args.port, **kwargs)
     except Exception as e:
-        err = '{}: {}\n'.format(e.__class__.__name__, e)
-        if e.__class__.__name__ == 'TypeError' and '__init__' in err:
-            # support the old syntax where the Server32 required a 'quiet' argument
-            if "missing 1 required positional argument: 'quiet'" in err:
-                try:
-                    server = cls(args.host, args.port, True, **kwargs)
-                except Exception as e:
-                    err = '{}: {}\n'.format(e.__class__.__name__, e)
-
-    if server is None:
-        err += 'The \'{0}\' class must be defined with the following syntax:\n\n' \
-               'class {0}(Server32):\n' \
-               '    def __init__(self, host, port, **kwargs):\n' \
-               '        super({0}, self).__init__(path, libtype, host, port, **kwargs)\n\n' \
-               'Cannot start the 32-bit server.'.format(cls.__name__)
+        # support the old syntax where the Server32 required a 'quiet' argument
+        if "missing 1 required positional argument: 'quiet'" in str(e):
+            try:
+                server = cls(args.host, args.port, True, **kwargs)
+            except Exception as e:
+                error = e
+        else:
+            error = e
+
+    if error is not None:
+        err = 'Instantiating the 32-bit server raised the following exception:\n' \
+              '  {}: {}\n'.format(error.__class__.__name__, error)
+
+        if error.__class__.__name__ == 'TypeError' and '__init__' in str(error):
+            err += 'Check that the \'{0}\' class is defined with the following syntax:\n\n' \
+                   'class {0}(Server32):\n' \
+                   '    def __init__(self, host, port, **kwargs):\n' \
+                   '        super({0}, self).__init__(path, libtype, host, port, **kwargs)\n\n'.format(cls.__name__)
+
+        err += 'Cannot start the 32-bit server.'
         print(err, file=sys.stderr)
         return -1
 
     if not hasattr(server, '_library'):
-        err = 'The super() method was never called.\n' \
-              'The \'{0}\' class must be defined with the following syntax:\n\n' \
+        err = 'The super() function was never called in the Server32 subclass.\n' \
+              'Check that the \'{0}\' class is defined with the following syntax:\n\n' \
               'class {0}(Server32):\n' \
               '    def __init__(self, host, port, **kwargs):\n' \
               '        super({0}, self).__init__(path, libtype, host, port, **kwargs)\n\n' \
               'Cannot start the 32-bit server.'.format(cls.__name__)
         print(err, file=sys.stderr)
         return -1
```

### Comparing `msl-loadlib-0.8.0/msl/loadlib/utils.py` & `msl-loadlib-0.9.0/msl/loadlib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -353,7 +353,84 @@
                         results[clsid][name] = None
             finally:
                 winreg.CloseKey(sub_key)
 
         winreg.CloseKey(key)
 
     return results
+
+
+def generate_com_wrapper(lib, out_dir=None):
+    """Generate a Python wrapper module around a COM library.
+
+    For more information see `Accessing type libraries`_.
+
+    .. versionadded:: 0.9
+
+    .. _Accessing type libraries: https://pythonhosted.org/comtypes/#accessing-type-libraries
+
+    Parameters
+    ----------
+    lib
+        Can be any of the following
+
+            * a :class:`~msl.loadlib.load_library.LoadLibrary` object
+            * the `ProgID` or `CLSID` of a registered COM library as a :class:`str`
+            * a COM pointer instance
+            * an ITypeLib COM pointer instance
+            * a path to a library file (.tlb, .exe or .dll) as a :class:`str`
+            * a :class:`tuple` or :class:`list` specifying the GUID of a library,
+              a major and a minor version number, plus optionally an LCID number,
+              e.g., (guid, major, minor, lcid=0)
+            * an object with ``_reg_libid_`` and ``_reg_version_`` attributes
+
+    out_dir : :class:`str`, optional
+        The output directory to save the wrapper to. If not specified then
+        saves it to the ``../site-packages/comtypes/gen`` directory.
+
+    Returns
+    -------
+    The wrapper module that was generated.
+    """
+    if not is_comtypes_installed():
+        raise OSError(
+            'Cannot create a COM wrapper because comtypes is not installed, run\n'
+            '  pip install comtypes'
+        )
+
+    import comtypes.client
+
+    mod = None
+
+    # cache the value of gen_dir to reset it later
+    cached_gen_dir = comtypes.client.gen_dir
+    if out_dir is not None:
+        gen_dir = os.path.abspath(out_dir)
+        if not os.path.isdir(gen_dir):
+            os.makedirs(gen_dir)
+        comtypes.client.gen_dir = gen_dir
+
+    def from_pointer(p):
+        info = p.GetTypeInfo(0)
+        type_lib, index = info.GetContainingTypeLib()
+        return comtypes.client.GetModule(type_lib)
+
+    try:
+        mod = comtypes.client.GetModule(lib)
+    except OSError:
+        pass
+    except AttributeError as e:
+        if str(e).startswith("'LoadLibrary'"):
+            mod = from_pointer(lib.lib)
+        elif hasattr(lib, '__com_interface__'):
+            mod = from_pointer(lib)
+        else:
+            raise
+
+    if not mod and isinstance(lib, str):
+        obj = comtypes.client.CreateObject(lib)
+        mod = from_pointer(obj)
+
+    if out_dir is not None:
+        comtypes.client.gen_dir = cached_gen_dir
+
+    return mod
```

### Comparing `msl-loadlib-0.8.0/msl/loadlib/verpatch.exe` & `msl-loadlib-0.9.0/msl/loadlib/verpatch.exe`

 * *Files identical despite different names*

### Comparing `msl-loadlib-0.8.0/msl_loadlib.egg-info/PKG-INFO` & `msl-loadlib-0.9.0/msl_loadlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msl-loadlib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Load a shared library (and access a 32-bit library from 64-bit Python)
 Home-page: https://github.com/MSLNZ/msl-loadlib
 Author: Measurement Standards Laboratory of New Zealand
 Author-email: info@measurement.govt.nz
 License: MIT
 Description: ===========
         MSL-LoadLib
@@ -67,28 +67,28 @@
         
            >>> from msl.loadlib import LoadLibrary
            >>> from msl.examples.loadlib import EXAMPLES_DIR
         
         If the file extension is not included then a default extension,
         ``.dll`` (Windows) or ``.so`` (Linux), is used.
         
-        Load a `C++ <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/cpp_lib.cpp>`_
+        Load a `C++ <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/cpp_lib.cpp>`_
         library and call the ``add`` function
         
         .. invisible-code-block: pycon
         
            >>> SKIP_IF_32BIT()
         
         .. code-block:: pycon
         
            >>> cpp = LoadLibrary(EXAMPLES_DIR + '/cpp_lib64')
            >>> cpp.lib.add(1, 2)
            3
         
-        Load a `FORTRAN <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/fortran_lib.f90>`_
+        Load a `FORTRAN <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/fortran_lib.f90>`_
         library and call the ``factorial`` function
         
         .. code-block:: pycon
         
            >>> fortran = LoadLibrary(EXAMPLES_DIR + '/fortran_lib64')
         
         With a FORTRAN library you must pass values by reference using ctypes_, and, since
@@ -98,25 +98,25 @@
         .. code-block:: pycon
         
            >>> from ctypes import byref, c_int, c_double
            >>> fortran.lib.factorial.restype = c_double
            >>> fortran.lib.factorial(byref(c_int(37)))
            1.3763753091226343e+43
         
-        Load a `.NET <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/dotnet_lib.cs>`_
+        Load a `.NET <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/dotnet_lib.cs>`_
         library and call the ``reverse_string`` function, we must specify that the library
         type is a .NET library by passing in the ``'net'`` argument
         
         .. code-block:: pycon
         
            >>> net = LoadLibrary(EXAMPLES_DIR + '/dotnet_lib64.dll', 'net')
            >>> net.lib.StringManipulation().reverse_string('abcdefghijklmnopqrstuvwxyz')
            'zyxwvutsrqponmlkjihgfedcba'
         
-        Load `Java <https://github.com/MSLNZ/msl-loadlib/blob/master/msl/examples/loadlib/Trig.java>`_
+        Load `Java <https://github.com/MSLNZ/msl-loadlib/blob/main/msl/examples/loadlib/Trig.java>`_
         byte code and call the ``cos`` function
         
         .. code-block:: pycon
         
            >>> java = LoadLibrary(EXAMPLES_DIR + '/Trig.class')
            >>> java.lib.Trig.cos(1.234)
            0.33046510807172985
@@ -138,27 +138,14 @@
         
            >>> SKIP_IF_NOT_WINDOWS()
         
         .. code-block:: pycon
         
            >>> com = LoadLibrary('Scripting.FileSystemObject', 'com')
         
-        If creating the `com` object in the previous command raises
-        
-        .. code-block:: console
-        
-           OSError: [WinError -2147417850] Cannot change thread mode after it is set
-        
-        then perform the following and try again
-        
-        .. code-block:: pycon
-        
-           >>> import sys
-           >>> sys.coinit_flags = 0
-        
         We then use the library to create, edit and close a text file
         
         .. code-block:: pycon
         
            >>> fp = com.lib.CreateTextFile('a_new_file.txt')
            >>> fp.WriteLine('This is a test')
            0
@@ -186,19 +173,19 @@
         .. |docs| image:: https://readthedocs.org/projects/msl-loadlib/badge/?version=stable
            :target: https://msl-loadlib.readthedocs.io/en/stable/
            :alt: Documentation Status
         
         .. |pypi| image:: https://badge.fury.io/py/msl-loadlib.svg
            :target: https://badge.fury.io/py/msl-loadlib
         
-        .. |travis| image:: https://img.shields.io/travis/MSLNZ/msl-loadlib/master.svg?label=Travis-CI
+        .. |travis| image:: https://img.shields.io/travis/MSLNZ/msl-loadlib/main.svg?label=Travis-CI
            :target: https://travis-ci.org/MSLNZ/msl-loadlib
         
-        .. |appveyor| image:: https://img.shields.io/appveyor/ci/jborbely/msl-loadlib/master.svg?label=AppVeyor
-           :target: https://ci.appveyor.com/project/jborbely/msl-loadlib/branch/master
+        .. |appveyor| image:: https://img.shields.io/appveyor/ci/jborbely/msl-loadlib/main.svg?label=AppVeyor
+           :target: https://ci.appveyor.com/project/jborbely/msl-loadlib/branch/main
         
         .. _ctypes: https://docs.python.org/3/library/ctypes.html
         .. _Python for .NET: https://pythonnet.github.io/
         .. _Py4J: https://www.py4j.org/
         .. _ipc: https://en.wikipedia.org/wiki/Inter-process_communication
         .. _Java Virtual Machine: https://en.wikipedia.org/wiki/Java_virtual_machine
         .. _MSL Package Manager: https://msl-package-manager.readthedocs.io/en/latest/
@@ -224,7 +211,8 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: clr
 Provides-Extra: java
 Provides-Extra: com
 Provides-Extra: all
 Provides-Extra: tests
+Provides-Extra: docs
```

### Comparing `msl-loadlib-0.8.0/msl_loadlib.egg-info/SOURCES.txt` & `msl-loadlib-0.9.0/msl_loadlib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 msl/examples/loadlib/labview_lib32.dll
 msl/examples/loadlib/labview_lib64.dll
 msl/examples/loadlib/nz/msl/examples/MathUtils.java
 msl/examples/loadlib/nz/msl/examples/Matrix.java
 msl/examples/loadlib/nz/msl/examples/readme.txt
 msl/loadlib/Py4JWrapper.java
 msl/loadlib/__init__.py
+msl/loadlib/activex.py
 msl/loadlib/client64.py
 msl/loadlib/exceptions.py
 msl/loadlib/freeze_server32.py
 msl/loadlib/load_library.py
 msl/loadlib/py4j-wrapper.jar
 msl/loadlib/server32.py
 msl/loadlib/start_server32.py
```

### Comparing `msl-loadlib-0.8.0/setup.py` & `msl-loadlib-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import re
 import sys
-import subprocess
+from subprocess import check_output
 from setuptools import (
     setup,
     find_packages,
     Command,
 )
 
 
 class ApiDocs(Command):
     """
     A custom command that calls sphinx-apidoc
-    see: https://www.sphinx-doc.org/en/latest/man/sphinx-apidoc.html
+    see: https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html
     """
     description = 'builds the api documentation using sphinx-apidoc'
     user_options = []
 
     def initialize_options(self):
         pass
 
@@ -33,107 +33,120 @@
             'msl',  # the path to the Python package to document
         ]
 
         import sphinx
         if sphinx.version_info[:2] < (1, 7):
             from sphinx.apidoc import main
         else:
-            from sphinx.ext.apidoc import main  # Sphinx also changed the location of apidoc.main
+            from sphinx.ext.apidoc import main
             command.pop(0)
 
         main(command)
-        sys.exit(0)
 
 
 class BuildDocs(Command):
     """
     A custom command that calls sphinx-build
-    see: https://www.sphinx-doc.org/en/latest/man/sphinx-build.html
+    see: https://www.sphinx-doc.org/en/master/man/sphinx-build.html
     """
     description = 'builds the documentation using sphinx-build'
     user_options = []
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
-        import sphinx
-
         command = [
             None,  # in Sphinx < 1.7.0 the first command-line argument was parsed, in 1.7.0 it became argv[1:]
             '-b', 'html',  # the builder to use, e.g., create a HTML version of the documentation
             '-a',  # generate output for all files
             '-E',  # ignore cached files, forces to re-read all source files from disk
             'docs',  # the source directory where the documentation files are located
             './docs/_build/html',  # where to save the output files
         ]
 
+        import sphinx
         if sphinx.version_info[:2] < (1, 7):
             from sphinx import build_main
         else:
-            from sphinx.cmd.build import build_main  # Sphinx also changed the location of build_main
+            from sphinx.cmd.build import build_main
             command.pop(0)
 
         build_main(command)
-        sys.exit(0)
 
 
 def read(filename):
     with open(filename) as fp:
         return fp.read()
 
 
 def fetch_init(key):
-    # open the __init__.py file to determine the value instead of importing the package to get the value
-    init_text = read('msl/loadlib/__init__.py')
-    return re.search(r'{}\s*=\s*(.*)'.format(key), init_text).group(1).strip('\'\"')
+    # open the __init__.py file to determine a value instead of importing the package
+    return re.search(r'{}\s*=\s*(.+)'.format(key), read(init_original)).group(1).strip('\'\"')
 
 
 def get_version():
     init_version = fetch_init('__version__')
-    if 'dev' not in init_version:
+    if 'dev' not in init_version or testing:
         return init_version
 
-    if ('develop' in sys.argv) or (os.path.join('msl-loadlib', 'setup.py') in sys.argv[0]):
+    if 'develop' in sys.argv:
         # then installing in editable (develop) mode
         #   python setup.py develop
         #   pip install -e .
-        suffix = 'editable'
-    else:
-        file_dir = os.path.dirname(os.path.abspath(__file__))
+        # following PEP-440, the local version identifier starts with '+'
+        return init_version + '+editable'
+
+    # append the commit hash to __version__
+    setup_dir = os.path.dirname(os.path.realpath(__file__))
+    try:
+        # write all error messages from git to devnull
+        with open(os.devnull, mode='w') as devnull:
+            out = check_output(['git', 'rev-parse', 'HEAD'], cwd=setup_dir, stderr=devnull)
+            sha1 = out.strip().decode()
+    except:
+        # the git executable is not available, manually parse .git directory
         try:
-            # write all error messages from git to devnull
-            with open(os.devnull, 'w') as devnull:
-                out = subprocess.check_output(['git', 'rev-parse', 'HEAD'], cwd=file_dir, stderr=devnull)
+            git_dir = os.path.join(setup_dir, '.git')
+            with open(os.path.join(git_dir, 'HEAD'), mode='rt') as fp1:
+                line = fp1.readline().strip()
+                if line.startswith('ref:'):
+                    _, ref_path = line.split()
+                    with open(os.path.join(git_dir, ref_path), mode='rt') as fp2:
+                        sha1 = fp2.readline().strip()
+                else:  # detached HEAD
+                    sha1 = line
         except:
-            try:
-                git_dir = os.path.join(file_dir, '.git')
-                with open(os.path.join(git_dir, 'HEAD'), mode='rt') as fp1:
-                    line = fp1.readline().strip()
-                    if line.startswith('ref:'):
-                        _, ref_path = line.split()
-                        with open(os.path.join(git_dir, ref_path), mode='rt') as fp2:
-                            sha1 = fp2.readline().strip()
-                    else:  # detached HEAD
-                        sha1 = line
-            except:
-                return init_version
-        else:
-            sha1 = out.strip().decode('ascii')
-
-        suffix = sha1[:7]
+            return init_version
 
-    if init_version.endswith(suffix):
+    suffix = sha1[:7]
+    if not suffix or init_version.endswith(suffix):
         return init_version
 
     # following PEP-440, the local version identifier starts with '+'
-    return init_version + '+' + suffix
+    dev_version = init_version + '+' + suffix
+
+    with open(init_original) as fp:
+        init_source = fp.read()
+
+    if os.path.isfile(init_backup):
+        os.remove(init_backup)
+    os.rename(init_original, init_backup)
+
+    with open(init_original, mode='wt') as fp:
+        fp.write(re.sub(
+            r'__version__\s*=.+',
+            "__version__ = '{}'".format(dev_version),
+            init_source
+        ))
+
+    return dev_version
 
 
 IS_WINDOWS = sys.platform == 'win32'
 
 # auto generate the MANIFEST.in file depending on the distribution that is being built
 if 'bdist_wheel' in sys.argv and 'sdist' in sys.argv:
     raise ValueError('cannot specify bdist_wheel and sdist in the same command, run one command at a time')
@@ -164,20 +177,24 @@
     'py4j',
     'numpy',  # needed for [doctest] tutorials_cpp_array.rst
     'pythonnet',
     'pathlib;python_version<"3.0"',
     'comtypes;sys_platform=="win32"',
 ]
 
+docs_require = ['sphinx', 'sphinx_rtd_theme']
+
 testing = {'test', 'tests', 'pytest'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if testing else []
 
 needs_sphinx = {'doc', 'docs', 'apidoc', 'apidocs', 'build_sphinx'}.intersection(sys.argv)
-sphinx = ['sphinx', 'sphinx_rtd_theme'] + install_requires if needs_sphinx else []
+sphinx = docs_require + install_requires if needs_sphinx else []
 
+init_original = 'msl/loadlib/__init__.py'
+init_backup = init_original + '.backup'
 version = get_version()
 
 setup(
     name='msl-loadlib',
     version=version,
     author=fetch_init('__author__'),
     author_email='info@measurement.govt.nz',
@@ -209,33 +226,17 @@
     install_requires=install_requires,
     extras_require={
         'clr': ['pythonnet'],
         'java': ['py4j'],
         'com': ['comtypes'],
         'all': ['pythonnet', 'py4j', 'comtypes'],
         'tests': tests_require,
+        'docs': docs_require,
     },
     cmdclass={'docs': BuildDocs, 'apidocs': ApiDocs},
     packages=find_packages(include=('msl*',)),
     include_package_data=True,
 )
 
-if 'dev' in version and not version.endswith('editable'):
-    # ensure that the value of __version__ is correct if installing the package from an unreleased code base
-    init_path = ''
-    if sys.argv[0] == 'setup.py' and 'install' in sys.argv and not {'--help', '-h'}.intersection(sys.argv):
-        # python setup.py install
-        try:
-            cmd = [sys.executable, '-c', 'import msl.loadlib as p; print(p.__file__)']
-            output = subprocess.check_output(cmd, cwd=os.path.dirname(sys.executable))
-            init_path = output.strip().decode()
-        except:
-            pass
-    elif 'egg_info' in sys.argv:
-        # pip install
-        init_path = os.path.dirname(sys.argv[0]) + '/msl/loadlib/__init__.py'
-
-    if init_path and os.path.isfile(init_path):
-        with open(init_path, mode='r+') as fp:
-            source = fp.read()
-            fp.seek(0)
-            fp.write(re.sub(r'__version__\s*=.*', "__version__ = '{}'".format(version), source))
+if os.path.isfile(init_backup):
+    os.remove(init_original)
+    os.rename(init_backup, init_original)
```

