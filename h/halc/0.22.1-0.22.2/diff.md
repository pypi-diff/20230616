# Comparing `tmp/halc-0.22.1.tar.gz` & `tmp/halc-0.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halc-0.22.1.tar", last modified: Fri Jun 16 05:05:03 2023, max compression
+gzip compressed data, was "halc-0.22.2.tar", last modified: Fri Jun 16 14:02:09 2023, max compression
```

## Comparing `halc-0.22.1.tar` & `halc-0.22.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 05:05:03.636515 halc-0.22.1/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1061 2023-06-14 16:42:42.000000 halc-0.22.1/LICENSE
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-16 05:05:03.636515 halc-0.22.1/PKG-INFO
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      328 2023-06-14 16:36:58.000000 halc-0.22.1/README.md
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 05:05:03.636515 halc-0.22.1/halc/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      227 2023-06-16 05:05:01.000000 halc-0.22.1/halc/__about__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       95 2023-06-16 02:01:38.000000 halc-0.22.1/halc/__init__.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 05:05:03.636515 halc-0.22.1/halc/images/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       27 2023-06-16 03:45:31.000000 halc-0.22.1/halc/images/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      487 2023-06-16 03:44:51.000000 halc-0.22.1/halc/images/get.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     5143 2023-06-16 02:05:42.000000 halc-0.22.1/halc/initialize.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 05:05:03.636515 halc-0.22.1/halc/projects/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       28 2023-06-16 01:55:40.000000 halc-0.22.1/halc/projects/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      507 2023-06-16 04:57:49.000000 halc-0.22.1/halc/projects/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 05:05:03.636515 halc-0.22.1/halc/upload/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      101 2023-06-16 03:33:09.000000 halc-0.22.1/halc/upload/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     4633 2023-06-16 04:59:32.000000 halc-0.22.1/halc/upload/images.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     6447 2023-06-16 04:54:54.000000 halc-0.22.1/halc/upload/labels.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      987 2023-06-16 04:34:06.000000 halc-0.22.1/halc/utils.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 05:05:03.636515 halc-0.22.1/halc/versions/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       42 2023-06-16 01:53:27.000000 halc-0.22.1/halc/versions/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      934 2023-06-16 02:12:02.000000 halc-0.22.1/halc/versions/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 05:05:03.636515 halc-0.22.1/halc.egg-info/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-16 05:05:03.000000 halc-0.22.1/halc.egg-info/PKG-INFO
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      448 2023-06-16 05:05:03.000000 halc-0.22.1/halc.egg-info/SOURCES.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        1 2023-06-16 05:05:03.000000 halc-0.22.1/halc.egg-info/dependency_links.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       88 2023-06-16 05:05:03.000000 halc-0.22.1/halc.egg-info/requires.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        5 2023-06-16 05:05:03.000000 halc-0.22.1/halc.egg-info/top_level.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       79 2023-06-16 05:05:03.636515 halc-0.22.1/setup.cfg
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1383 2023-06-16 03:56:22.000000 halc-0.22.1/setup.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1061 2023-06-14 16:42:42.000000 halc-0.22.2/LICENSE
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-16 14:02:09.283882 halc-0.22.2/PKG-INFO
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      328 2023-06-14 16:36:58.000000 halc-0.22.2/README.md
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      227 2023-06-16 14:02:07.000000 halc-0.22.2/halc/__about__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       95 2023-06-16 02:01:38.000000 halc-0.22.2/halc/__init__.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/images/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       27 2023-06-16 03:45:31.000000 halc-0.22.2/halc/images/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      487 2023-06-16 03:44:51.000000 halc-0.22.2/halc/images/get.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     5167 2023-06-16 13:59:13.000000 halc-0.22.2/halc/initialize.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/projects/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       28 2023-06-16 01:55:40.000000 halc-0.22.2/halc/projects/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      507 2023-06-16 04:57:49.000000 halc-0.22.2/halc/projects/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/upload/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      101 2023-06-16 03:33:09.000000 halc-0.22.2/halc/upload/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     4633 2023-06-16 04:59:32.000000 halc-0.22.2/halc/upload/images.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     6447 2023-06-16 04:54:54.000000 halc-0.22.2/halc/upload/labels.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      987 2023-06-16 04:34:06.000000 halc-0.22.2/halc/utils.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/versions/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       42 2023-06-16 01:53:27.000000 halc-0.22.2/halc/versions/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      934 2023-06-16 02:12:02.000000 halc-0.22.2/halc/versions/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc.egg-info/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/PKG-INFO
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      448 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        1 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       88 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/requires.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        5 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/top_level.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       79 2023-06-16 14:02:09.283882 halc-0.22.2/setup.cfg
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1383 2023-06-16 03:56:22.000000 halc-0.22.2/setup.py
```

### Comparing `halc-0.22.1/LICENSE` & `halc-0.22.2/LICENSE`

 * *Files identical despite different names*

### Comparing `halc-0.22.1/PKG-INFO` & `halc-0.22.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halc
-Version: 0.22.1
+Version: 0.22.2
 Summary: Python SDK for Happyrobot's HALC
 Home-page: https://happyrobot.ai
 Author: Happyrobot
 Author-email: luis.paarup@happyrobot.ai
 License: MIT
 Keywords: happyrobot computer vision artificial intelligence foundation models large vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `halc-0.22.1/halc/initialize.py` & `halc-0.22.2/halc/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     hr_file: Path = hr_dir / "config.yaml"
 
     endpoint: str = "https://app.happyrobot.ai"
     hrid: str = None
     hrinfo: str = None
     token: str = None
     storage: dict = None
+    backend: Any = None
 
     def is_valid(self) -> bool:
         return self.endpoint and self.hrid and self.hrinfo and self.token
 
     @classmethod
     def from_json(cls, **kwargs) -> "HRConfig":
         return cls(**kwargs)
```

### Comparing `halc-0.22.1/halc/upload/images.py` & `halc-0.22.2/halc/upload/images.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.1/halc/upload/labels.py` & `halc-0.22.2/halc/upload/labels.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.1/halc/utils.py` & `halc-0.22.2/halc/utils.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.1/halc/versions/get.py` & `halc-0.22.2/halc/versions/get.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.1/halc.egg-info/PKG-INFO` & `halc-0.22.2/halc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halc
-Version: 0.22.1
+Version: 0.22.2
 Summary: Python SDK for Happyrobot's HALC
 Home-page: https://happyrobot.ai
 Author: Happyrobot
 Author-email: luis.paarup@happyrobot.ai
 License: MIT
 Keywords: happyrobot computer vision artificial intelligence foundation models large vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `halc-0.22.1/setup.py` & `halc-0.22.2/setup.py`

 * *Files identical despite different names*

