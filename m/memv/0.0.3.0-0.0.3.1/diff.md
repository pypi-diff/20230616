# Comparing `tmp/memv-0.0.3.0.tar.gz` & `tmp/memv-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.3.0.tar", last modified: Fri Jun 16 10:07:33 2023, max compression
+gzip compressed data, was "memv-0.0.3.1.tar", last modified: Fri Jun 16 10:09:11 2023, max compression
```

## Comparing `memv-0.0.3.0.tar` & `memv-0.0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:07:33.284877 memv-0.0.3.0/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.3.0/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:07:33.284703 memv-0.0.3.0/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:06:11.000000 memv-0.0.3.0/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:07:33.282734 memv-0.0.3.0/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.3.0/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     3746 2023-06-16 10:07:17.000000 memv-0.0.3.0/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      969 2023-06-16 09:12:50.000000 memv-0.0.3.0/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:07:33.284451 memv-0.0.3.0/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:07:33.000000 memv-0.0.3.0/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:07:33.000000 memv-0.0.3.0/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:07:33.000000 memv-0.0.3.0/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:07:33.000000 memv-0.0.3.0/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:07:33.000000 memv-0.0.3.0/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:07:33.000000 memv-0.0.3.0/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:07:33.284915 memv-0.0.3.0/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:07:29.000000 memv-0.0.3.0/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:09:11.556878 memv-0.0.3.1/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.3.1/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:09:11.556666 memv-0.0.3.1/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:06:11.000000 memv-0.0.3.1/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:09:11.554326 memv-0.0.3.1/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.3.1/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     3746 2023-06-16 10:07:17.000000 memv-0.0.3.1/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      965 2023-06-16 10:08:52.000000 memv-0.0.3.1/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:09:11.556384 memv-0.0.3.1/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:09:11.000000 memv-0.0.3.1/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:09:11.000000 memv-0.0.3.1/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:09:11.000000 memv-0.0.3.1/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:09:11.000000 memv-0.0.3.1/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:09:11.000000 memv-0.0.3.1/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:09:11.000000 memv-0.0.3.1/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:09:11.556920 memv-0.0.3.1/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:09:08.000000 memv-0.0.3.1/setup.py
```

### Comparing `memv-0.0.3.0/LICENSE` & `memv-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.3.0/memv/memv.py` & `memv-0.0.3.1/memv/memv.py`

 * *Files identical despite different names*

### Comparing `memv-0.0.3.0/memv/utils.py` & `memv-0.0.3.1/memv/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 def parseDurationToSecond(duration_str):
     duration_unit = duration_str[-1]
     duration_value_str = duration_str[:-1]
     try:
         duration_value = int(duration_value_str)
     except ValueError:
-        print(f'Invalid duration format: "{duration_str}". Supported 30s | 30m | 8h | 3d')
+        print(f'Invalid duration format: {duration_str}. Supported 30s | 30m | 8h | 3d')
         return None
     
     if duration_unit == 's':
         return duration_value
     elif duration_unit == 'm':
         return duration_value * 60
     elif duration_unit == 'h':
         return duration_value * 60 * 60
     elif duration_unit == 'd':
         return duration_value * 60 * 60 * 24
     else:
-        print(f'Invalid duration format: "{duration_str}". Supported 30s | 30m | 8h | 3d')
+        print(f'Invalid duration format: {duration_str}. Supported 30s | 30m | 8h | 3d')
         return None
```

