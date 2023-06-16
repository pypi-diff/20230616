# Comparing `tmp/ipycrawl-0.0.0.tar.gz` & `tmp/ipycrawl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipycrawl-0.0.0.tar", last modified: Fri Jun 16 04:52:13 2023, max compression
+gzip compressed data, was "ipycrawl-0.0.2.tar", last modified: Fri Jun 16 05:47:22 2023, max compression
```

## Comparing `ipycrawl-0.0.0.tar` & `ipycrawl-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 04:52:13.778294 ipycrawl-0.0.0/
--rw-rw-rw-   0        0        0     1085 2023-06-16 04:39:36.000000 ipycrawl-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      667 2023-06-16 04:52:13.777293 ipycrawl-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-16 04:41:55.000000 ipycrawl-0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 04:52:13.778294 ipycrawl-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-16 04:51:20.000000 ipycrawl-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 04:52:13.747287 ipycrawl-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 04:52:13.756289 ipycrawl-0.0.0/src/ipycrawl/
--rw-rw-rw-   0        0        0        0 2023-06-16 04:44:28.000000 ipycrawl-0.0.0/src/ipycrawl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 04:52:13.774293 ipycrawl-0.0.0/src/ipycrawl.egg-info/
--rw-rw-rw-   0        0        0      667 2023-06-16 04:52:13.000000 ipycrawl-0.0.0/src/ipycrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-16 04:52:13.000000 ipycrawl-0.0.0/src/ipycrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 04:52:13.000000 ipycrawl-0.0.0/src/ipycrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 04:52:13.000000 ipycrawl-0.0.0/src/ipycrawl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 05:47:22.364467 ipycrawl-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-06-16 04:39:36.000000 ipycrawl-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      667 2023-06-16 05:47:22.363467 ipycrawl-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-16 04:41:55.000000 ipycrawl-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 05:47:22.365467 ipycrawl-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-06-16 05:45:57.000000 ipycrawl-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 05:47:22.328459 ipycrawl-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 05:47:22.340462 ipycrawl-0.0.2/src/ipycrawl/
+-rw-rw-rw-   0        0        0        0 2023-06-16 04:44:28.000000 ipycrawl-0.0.2/src/ipycrawl/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-06-16 05:37:23.000000 ipycrawl-0.0.2/src/ipycrawl/file.py
+drwxrwxrwx   0        0        0        0 2023-06-16 05:47:22.360467 ipycrawl-0.0.2/src/ipycrawl.egg-info/
+-rw-rw-rw-   0        0        0      667 2023-06-16 05:47:22.000000 ipycrawl-0.0.2/src/ipycrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-16 05:47:22.000000 ipycrawl-0.0.2/src/ipycrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 05:47:22.000000 ipycrawl-0.0.2/src/ipycrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 05:47:22.000000 ipycrawl-0.0.2/src/ipycrawl.egg-info/top_level.txt
```

### Comparing `ipycrawl-0.0.0/LICENSE` & `ipycrawl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipycrawl-0.0.0/PKG-INFO` & `ipycrawl-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipycrawl
-Version: 0.0.0
+Version: 0.0.2
 Summary: 파일 다운로드 및 각종 RESTful OpenAPI 를 사용하여 데이타를 수집하는 Innovata Web Crawler 라이브러리 패키지
 Home-page: https://github.com/innovata/iCrawler
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ipycrawl-0.0.0/setup.py` & `ipycrawl-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipycrawl",
-    version="0.0.0",
+    version="0.0.2",
     author="innovata",
     author_email="iinnovata@gmail.com",
     description='파일 다운로드 및 각종 RESTful OpenAPI 를 사용하여 데이타를 수집하는 Innovata Web Crawler 라이브러리 패키지',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/innovata/iCrawler",
     classifiers=[
```

### Comparing `ipycrawl-0.0.0/src/ipycrawl.egg-info/PKG-INFO` & `ipycrawl-0.0.2/src/ipycrawl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipycrawl
-Version: 0.0.0
+Version: 0.0.2
 Summary: 파일 다운로드 및 각종 RESTful OpenAPI 를 사용하여 데이타를 수집하는 Innovata Web Crawler 라이브러리 패키지
 Home-page: https://github.com/innovata/iCrawler
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

