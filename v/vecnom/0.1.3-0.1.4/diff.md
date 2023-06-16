# Comparing `tmp/vecnom-0.1.3.tar.gz` & `tmp/vecnom-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecnom-0.1.3.tar", max compression
+gzip compressed data, was "vecnom-0.1.4.tar", max compression
```

## Comparing `vecnom-0.1.3.tar` & `vecnom-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0     6148 2023-06-16 18:02:47.819081 vecnom-0.1.3/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253579 vecnom-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-16 18:39:39.929770 vecnom-0.1.3/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-10 10:14:19.937272 vecnom-0.1.3/data_types.py
--rw-r--r--   0        0        0     6148 2023-06-16 10:05:46.030654 vecnom-0.1.3/dist/.DS_Store
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.3/dist/vecnom-0.1.0/PKG-INFO
--rw-r--r--   0        0        0      292 2023-06-16 09:45:09.205407 vecnom-0.1.3/dist/vecnom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.3/dist/vecnom-0.1.0/vecnom.py
--rw-r--r--   0        0        0     1217 2023-06-16 09:57:54.791790 vecnom-0.1.3/dist/vecnom-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0      805 2023-06-16 09:57:54.737629 vecnom-0.1.3/dist/vecnom-0.1.0.tar.gz
--rw-r--r--   0        0        0     1216 2023-06-16 09:58:47.459517 vecnom-0.1.3/dist/vecnom-0.1.1-py3-none-any.whl
--rw-r--r--   0        0        0      805 2023-06-16 09:58:47.420965 vecnom-0.1.3/dist/vecnom-0.1.1.tar.gz
--rw-r--r--   0        0        0     6148 2023-06-16 10:05:46.032648 vecnom-0.1.3/dist/vecnom-0.1.2/.DS_Store
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.3/dist/vecnom-0.1.2/PKG-INFO
--rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253579 vecnom-0.1.3/dist/vecnom-0.1.2/README.md
--rw-r--r--   0        0        0     1182 2023-06-10 10:14:19.937272 vecnom-0.1.3/dist/vecnom-0.1.2/data_types.py
--rw-r--r--   0        0        0     6148 2023-06-16 09:59:20.236332 vecnom-0.1.3/dist/vecnom-0.1.2/dist/.DS_Store
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.0/PKG-INFO
--rw-r--r--   0        0        0      292 2023-06-16 09:45:09.205407 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.0/vecnom.py
--rw-r--r--   0        0        0     1217 2023-06-16 09:57:54.791790 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0      805 2023-06-16 09:57:54.737629 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.0.tar.gz
--rw-r--r--   0        0        0     1216 2023-06-16 09:58:47.459517 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.1-py3-none-any.whl
--rw-r--r--   0        0        0      805 2023-06-16 09:58:47.420965 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.1.tar.gz
--rw-r--r--   0        0        0     3202 2023-06-16 10:05:11.495380 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.2-py3-none-any.whl
--rw-r--r--   0        0        0        0 2023-06-16 10:05:20.076700 vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.2.tar.gz
--rw-r--r--   0        0        0      310 2023-06-16 10:05:02.757433 vecnom-0.1.3/dist/vecnom-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      460 2023-06-16 09:39:27.658274 vecnom-0.1.3/dist/vecnom-0.1.2/test.py
--rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253656 vecnom-0.1.3/dist/vecnom-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.3/dist/vecnom-0.1.2/vecnom.py
--rw-r--r--   0        0        0     6148 2023-06-16 09:20:41.063109 vecnom-0.1.3/dist/vecnom-0.1.2/vecnom_/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253531 vecnom-0.1.3/dist/vecnom-0.1.2/vecnom_/__init__.py
--rw-r--r--   0        0        0     3204 2023-06-16 18:39:22.903454 vecnom-0.1.3/dist/vecnom-0.1.2-py3-none-any.whl
--rw-r--r--   0        0        0    13393 2023-06-16 18:39:22.869112 vecnom-0.1.3/dist/vecnom-0.1.2.tar.gz
--rw-r--r--   0        0        0     3314 2023-06-16 18:39:56.068540 vecnom-0.1.3/dist/vecnom-0.1.3-py3-none-any.whl
--rw-r--r--   0        0        0    18863 2023-06-16 18:40:06.891220 vecnom-0.1.3/dist/vecnom-0.1.3.tar.gz
--rw-r--r--   0        0        0      310 2023-06-16 18:39:47.309143 vecnom-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      460 2023-06-16 09:39:27.658274 vecnom-0.1.3/test.py
--rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253656 vecnom-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.3/vecnom.py
--rw-r--r--   0        0        0     6148 2023-06-16 09:20:41.063109 vecnom-0.1.3/vecnom_/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253531 vecnom-0.1.3/vecnom_/__init__.py
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2023-06-16 18:02:47.819081 vecnom-0.1.4/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253579 vecnom-0.1.4/README.md
+-rw-r--r--   0        0        0       25 2023-06-16 18:43:33.225695 vecnom-0.1.4/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-10 10:14:19.937272 vecnom-0.1.4/data_types.py
+-rw-r--r--   0        0        0     6148 2023-06-16 10:05:46.030654 vecnom-0.1.4/dist/.DS_Store
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.4/dist/vecnom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-06-16 09:45:09.205407 vecnom-0.1.4/dist/vecnom-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.4/dist/vecnom-0.1.0/vecnom.py
+-rw-r--r--   0        0        0     1217 2023-06-16 09:57:54.791790 vecnom-0.1.4/dist/vecnom-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0      805 2023-06-16 09:57:54.737629 vecnom-0.1.4/dist/vecnom-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1216 2023-06-16 09:58:47.459517 vecnom-0.1.4/dist/vecnom-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0      805 2023-06-16 09:58:47.420965 vecnom-0.1.4/dist/vecnom-0.1.1.tar.gz
+-rw-r--r--   0        0        0     6148 2023-06-16 10:05:46.032648 vecnom-0.1.4/dist/vecnom-0.1.2/.DS_Store
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.4/dist/vecnom-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253579 vecnom-0.1.4/dist/vecnom-0.1.2/README.md
+-rw-r--r--   0        0        0     1182 2023-06-10 10:14:19.937272 vecnom-0.1.4/dist/vecnom-0.1.2/data_types.py
+-rw-r--r--   0        0        0     6148 2023-06-16 09:59:20.236332 vecnom-0.1.4/dist/vecnom-0.1.2/dist/.DS_Store
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-06-16 09:45:09.205407 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.0/vecnom.py
+-rw-r--r--   0        0        0     1217 2023-06-16 09:57:54.791790 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0      805 2023-06-16 09:57:54.737629 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1216 2023-06-16 09:58:47.459517 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0      805 2023-06-16 09:58:47.420965 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.1.tar.gz
+-rw-r--r--   0        0        0     3202 2023-06-16 10:05:11.495380 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0        0 2023-06-16 10:05:20.076700 vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.2.tar.gz
+-rw-r--r--   0        0        0      310 2023-06-16 10:05:02.757433 vecnom-0.1.4/dist/vecnom-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      460 2023-06-16 09:39:27.658274 vecnom-0.1.4/dist/vecnom-0.1.2/test.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253656 vecnom-0.1.4/dist/vecnom-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.4/dist/vecnom-0.1.2/vecnom.py
+-rw-r--r--   0        0        0     6148 2023-06-16 09:20:41.063109 vecnom-0.1.4/dist/vecnom-0.1.2/vecnom_/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253531 vecnom-0.1.4/dist/vecnom-0.1.2/vecnom_/__init__.py
+-rw-r--r--   0        0        0     3204 2023-06-16 18:39:22.903454 vecnom-0.1.4/dist/vecnom-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0    13393 2023-06-16 18:39:22.869112 vecnom-0.1.4/dist/vecnom-0.1.2.tar.gz
+-rw-r--r--   0        0        0     3373 2023-06-16 18:43:10.810464 vecnom-0.1.4/dist/vecnom-0.1.3-py3-none-any.whl
+-rw-r--r--   0        0        0    47695 2023-06-16 18:43:10.773541 vecnom-0.1.4/dist/vecnom-0.1.3.tar.gz
+-rw-r--r--   0        0        0     3372 2023-06-16 18:43:48.375196 vecnom-0.1.4/dist/vecnom-0.1.4-py3-none-any.whl
+-rw-r--r--   0        0        0    68521 2023-06-16 18:43:54.792947 vecnom-0.1.4/dist/vecnom-0.1.4.tar.gz
+-rw-r--r--   0        0        0      310 2023-06-16 18:43:38.752287 vecnom-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      460 2023-06-16 09:39:27.658274 vecnom-0.1.4/test.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253656 vecnom-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-16 09:39:11.208693 vecnom-0.1.4/vecnom.py
+-rw-r--r--   0        0        0     6148 2023-06-16 09:20:41.063109 vecnom-0.1.4/vecnom_/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-16 08:46:59.253531 vecnom-0.1.4/vecnom_/__init__.py
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 vecnom-0.1.4/PKG-INFO
```

### Comparing `vecnom-0.1.3/.DS_Store` & `vecnom-0.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/data_types.py` & `vecnom-0.1.4/data_types.py`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/.DS_Store` & `vecnom-0.1.4/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.0-py3-none-any.whl` & `vecnom-0.1.4/dist/vecnom-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.0.tar.gz` & `vecnom-0.1.4/dist/vecnom-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.1-py3-none-any.whl` & `vecnom-0.1.4/dist/vecnom-0.1.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.1.tar.gz` & `vecnom-0.1.4/dist/vecnom-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/.DS_Store` & `vecnom-0.1.4/dist/vecnom-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/data_types.py` & `vecnom-0.1.4/dist/vecnom-0.1.2/data_types.py`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/dist/.DS_Store` & `vecnom-0.1.4/dist/vecnom-0.1.2/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.0-py3-none-any.whl` & `vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.0.tar.gz` & `vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.1-py3-none-any.whl` & `vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.1.tar.gz` & `vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/dist/vecnom-0.1.2-py3-none-any.whl` & `vecnom-0.1.4/dist/vecnom-0.1.2/dist/vecnom-0.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2/vecnom_/.DS_Store` & `vecnom-0.1.4/dist/vecnom-0.1.2/vecnom_/.DS_Store`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2-py3-none-any.whl` & `vecnom-0.1.4/dist/vecnom-0.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.2.tar.gz` & `vecnom-0.1.4/dist/vecnom-0.1.2.tar.gz`

 * *Files identical despite different names*

### Comparing `vecnom-0.1.3/dist/vecnom-0.1.3-py3-none-any.whl` & `vecnom-0.1.4/dist/vecnom-0.1.4-py3-none-any.whl`

 * *Files 24% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3314 bytes, number of entries: 10
+Zip file size: 3372 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 .DS_Store
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 README.md
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 __init__.py
+-rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 __init__.py
 -rw-r--r--  2.0 unx     1182 b- defN 80-Jan-01 00:00 data_types.py
 -rw-r--r--  2.0 unx      310 b- defN 80-Jan-01 00:00 pyproject.toml
 -rw-r--r--  2.0 unx      460 b- defN 80-Jan-01 00:00 test.py
 -rw-r--r--  2.0 unx      435 b- defN 80-Jan-01 00:00 vecnom.py
--rw-r--r--  2.0 unx      456 b- defN 80-Jan-01 00:00 vecnom-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 vecnom-0.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx      664 b- defN 16-Jan-01 00:00 vecnom-0.1.3.dist-info/RECORD
-10 files, 9743 bytes uncompressed, 2212 bytes compressed:  77.3%
+-rw-r--r--  2.0 unx      456 b- defN 80-Jan-01 00:00 vecnom-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 vecnom-0.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 vecnom-0.1.4.dist-info/RECORD
+10 files, 9769 bytes uncompressed, 2270 bytes compressed:  76.8%
```

#### zipnote «TEMP»/diffoscope_g2p92i07_/tmph9wxttgq_.zip

```diff
@@ -15,17 +15,17 @@
 
 Filename: test.py
 Comment: 
 
 Filename: vecnom.py
 Comment: 
 
-Filename: vecnom-0.1.3.dist-info/METADATA
+Filename: vecnom-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: vecnom-0.1.3.dist-info/WHEEL
+Filename: vecnom-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: vecnom-0.1.3.dist-info/RECORD
+Filename: vecnom-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### __init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 6461 7461 5f74 7970 6573  from .data_types
+00000010: 2069 6d70 6f72 7420 2a                    import *
```

#### pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vecnom"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Ray <rejojer@gmail.com>"]
 include = ["*"]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

#### Comparing `vecnom-0.1.3.dist-info/RECORD` & `vecnom-0.1.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .DS_Store,sha256=DyXiRjjsxnolfu2SKlTPhfii_keh6JgcrabjteR3XXU,6148
 README.md,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+__init__.py,sha256=FmpNiG1vmXwXIJmGJFLXLD36pNWXopPwfIbWk1iVjww,25
 data_types.py,sha256=HZ-AOSS95jCbwxga19u0YBMHKm_2oHW7-Jq1flus8Vo,1182
-pyproject.toml,sha256=kLVFfq9rMPKDSl36kLB296ONv326o3pmt73NdKQVNSI,310
+pyproject.toml,sha256=Cv6W1rw48_Xs8G5Yf6G1NkDzrwLRndU_nbxM5KDjKos,310
 test.py,sha256=NZ0a6o7QtxK4XTQNUhQECh7JQMubXC0-DCqwYntLKgA,460
 vecnom.py,sha256=UXtzUqkNTYXsDCfN0rjYp3AqM9sjsgOeOA5IRTAmSGw,435
-vecnom-0.1.3.dist-info/METADATA,sha256=YwQ45pTOqLxWaAf78BptD0x7Cxcr-6Stl64sPgeJt-k,456
-vecnom-0.1.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-vecnom-0.1.3.dist-info/RECORD,,
+vecnom-0.1.4.dist-info/METADATA,sha256=tls7YpLngiFhLR9sImit4i0tgGSTQgIuH8wZCaNS_n4,456
+vecnom-0.1.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+vecnom-0.1.4.dist-info/RECORD,,
```

### Comparing `vecnom-0.1.3/vecnom_/.DS_Store` & `vecnom-0.1.4/vecnom_/.DS_Store`

 * *Files identical despite different names*

