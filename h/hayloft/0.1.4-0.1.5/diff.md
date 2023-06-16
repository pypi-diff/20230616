# Comparing `tmp/hayloft-0.1.4.tar.gz` & `tmp/hayloft-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.1.4.tar", max compression
+gzip compressed data, was "hayloft-0.1.5.tar", max compression
```

## Comparing `hayloft-0.1.4.tar` & `hayloft-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.4/LICENSE
--rw-r--r--   0        0        0      295 2023-06-14 14:43:21.952821 hayloft-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.4/hayloft/__init__.py
--rw-r--r--   0        0        0     3139 2023-06-14 14:51:34.732443 hayloft-0.1.4/hayloft/app.py
--rw-r--r--   0        0        0      457 2023-06-14 14:43:49.279652 hayloft-0.1.4/hayloft/logger.py
--rw-r--r--   0        0        0    18046 2023-06-14 14:46:56.924111 hayloft-0.1.4/hayloft/public/assets/index-144454fa.css
--rw-r--r--   0        0        0   174556 2023-06-14 14:46:56.924111 hayloft-0.1.4/hayloft/public/assets/index-ad0b845f.js
--rw-r--r--   0        0        0      382 2023-06-14 14:48:21.944620 hayloft-0.1.4/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.4/hayloft/schema.py
--rw-r--r--   0        0        0      430 2023-06-14 14:54:01.546657 hayloft-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 hayloft-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.5/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-14 14:43:21.952821 hayloft-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.5/hayloft/__init__.py
+-rw-r--r--   0        0        0     3139 2023-06-14 14:51:34.732443 hayloft-0.1.5/hayloft/app.py
+-rw-r--r--   0        0        0      466 2023-06-16 09:26:59.182198 hayloft-0.1.5/hayloft/logger.py
+-rw-r--r--   0        0        0    18046 2023-06-14 14:46:56.924111 hayloft-0.1.5/hayloft/public/assets/index-144454fa.css
+-rw-r--r--   0        0        0   174556 2023-06-14 14:46:56.924111 hayloft-0.1.5/hayloft/public/assets/index-ad0b845f.js
+-rw-r--r--   0        0        0      382 2023-06-14 14:48:21.944620 hayloft-0.1.5/hayloft/public/index.html
+-rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.5/hayloft/schema.py
+-rw-r--r--   0        0        0      430 2023-06-16 09:28:40.988722 hayloft-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 hayloft-0.1.5/PKG-INFO
```

### Comparing `hayloft-0.1.4/LICENSE` & `hayloft-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.4/hayloft/app.py` & `hayloft-0.1.5/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.4/hayloft/public/assets/index-144454fa.css` & `hayloft-0.1.5/hayloft/public/assets/index-144454fa.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.4/hayloft/public/assets/index-ad0b845f.js` & `hayloft-0.1.5/hayloft/public/assets/index-ad0b845f.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.4/hayloft/schema.py` & `hayloft-0.1.5/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.4/PKG-INFO` & `hayloft-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.1.4
+Version: 0.1.5
 Summary: UI tool for LLM frameworks
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

