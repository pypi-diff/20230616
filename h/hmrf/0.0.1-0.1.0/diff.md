# Comparing `tmp/hmrf-0.0.1.tar.gz` & `tmp/hmrf-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hmrf-0.0.1.tar", last modified: Thu Jun 15 21:51:14 2023, max compression
+gzip compressed data, was "dist/hmrf-0.1.0.tar", last modified: Thu Jun 15 22:31:08 2023, max compression
```

## Comparing `hmrf-0.0.1.tar` & `hmrf-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gretel    (1000) gretel    (1000)        0 2023-06-15 21:51:14.000000 hmrf-0.0.1/
--rw-rw-r--   0 gretel    (1000) gretel    (1000)     4410 2023-06-15 21:51:14.000000 hmrf-0.0.1/PKG-INFO
--rw-rw-r--   0 gretel    (1000) gretel    (1000)      861 2023-06-15 21:51:09.000000 hmrf-0.0.1/setup.py
--rw-rw-r--   0 gretel    (1000) gretel    (1000)       38 2023-06-15 21:51:14.000000 hmrf-0.0.1/setup.cfg
--rw-rw-r--   0 gretel    (1000) gretel    (1000)     1061 2023-06-15 19:31:16.000000 hmrf-0.0.1/LICENSE.txt
--rw-rw-r--   0 gretel    (1000) gretel    (1000)     3986 2023-06-15 21:39:49.000000 hmrf-0.0.1/README.md
-drwxrwxr-x   0 gretel    (1000) gretel    (1000)        0 2023-06-15 21:51:14.000000 hmrf-0.0.1/hmrf/
-drwxrwxr-x   0 gretel    (1000) gretel    (1000)        0 2023-06-15 21:51:14.000000 hmrf-0.0.1/hmrf/src/
-drwxrwxr-x   0 gretel    (1000) gretel    (1000)        0 2023-06-15 21:51:14.000000 hmrf-0.0.1/hmrf/src/hmrf.egg-info/
--rw-rw-r--   0 gretel    (1000) gretel    (1000)      231 2023-06-15 21:51:14.000000 hmrf-0.0.1/hmrf/src/hmrf.egg-info/SOURCES.txt
--rw-rw-r--   0 gretel    (1000) gretel    (1000)     4410 2023-06-15 21:51:14.000000 hmrf-0.0.1/hmrf/src/hmrf.egg-info/PKG-INFO
--rw-rw-r--   0 gretel    (1000) gretel    (1000)       49 2023-06-15 21:51:14.000000 hmrf-0.0.1/hmrf/src/hmrf.egg-info/requires.txt
--rw-rw-r--   0 gretel    (1000) gretel    (1000)        1 2023-06-15 21:51:14.000000 hmrf-0.0.1/hmrf/src/hmrf.egg-info/dependency_links.txt
--rw-rw-r--   0 gretel    (1000) gretel    (1000)        5 2023-06-15 21:51:14.000000 hmrf-0.0.1/hmrf/src/hmrf.egg-info/top_level.txt
--rw-rw-r--   0 gretel    (1000) gretel    (1000)     5426 2023-06-15 21:40:39.000000 hmrf-0.0.1/hmrf/src/hmrf.py
+drwxrwxr-x   0 gretel    (1000) gretel    (1000)        0 2023-06-15 22:31:08.000000 hmrf-0.1.0/
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)     4392 2023-06-15 22:31:08.000000 hmrf-0.1.0/PKG-INFO
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)      861 2023-06-15 22:29:50.000000 hmrf-0.1.0/setup.py
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)       38 2023-06-15 22:31:08.000000 hmrf-0.1.0/setup.cfg
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)     1061 2023-06-15 19:31:16.000000 hmrf-0.1.0/LICENSE.txt
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)     3968 2023-06-15 22:20:53.000000 hmrf-0.1.0/README.md
+drwxrwxr-x   0 gretel    (1000) gretel    (1000)        0 2023-06-15 22:31:08.000000 hmrf-0.1.0/hmrf/
+drwxrwxr-x   0 gretel    (1000) gretel    (1000)        0 2023-06-15 22:31:08.000000 hmrf-0.1.0/hmrf/src/
+drwxrwxr-x   0 gretel    (1000) gretel    (1000)        0 2023-06-15 22:31:08.000000 hmrf-0.1.0/hmrf/src/hmrf.egg-info/
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)      231 2023-06-15 22:31:02.000000 hmrf-0.1.0/hmrf/src/hmrf.egg-info/SOURCES.txt
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)     4392 2023-06-15 22:31:02.000000 hmrf-0.1.0/hmrf/src/hmrf.egg-info/PKG-INFO
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)       49 2023-06-15 22:31:02.000000 hmrf-0.1.0/hmrf/src/hmrf.egg-info/requires.txt
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)        1 2023-06-15 22:31:02.000000 hmrf-0.1.0/hmrf/src/hmrf.egg-info/dependency_links.txt
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)        5 2023-06-15 22:31:02.000000 hmrf-0.1.0/hmrf/src/hmrf.egg-info/top_level.txt
+-rw-rw-r--   0 gretel    (1000) gretel    (1000)     5426 2023-06-15 21:40:39.000000 hmrf-0.1.0/hmrf/src/hmrf.py
```

### Comparing `hmrf-0.0.1/PKG-INFO` & `hmrf-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmrf
-Version: 0.0.1
+Version: 0.1.0
 Summary: Package to extract keywords in one of the classes of a dataset
 Home-page: UNKNOWN
 Author: UPV
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,35 +15,25 @@
 
 # Harmonic Mean of Relative Frequencies (HMRF)
 
 HMRF is a method for automatic keyword extraction from a text corpus. This method favors words that maximize the difference between their frequency in one class (positive class) and their frequency in the rest of the classes.
 
 ## Parameters
 
-- lang: str, default = 'english'
-
-Language of the texts.
+- lang: str, default = 'english'. Language of the texts.
 
 - positive_class: str or int, default = 1
 
-- n: int, default = 50
-
-Amount of keywords to extract.
-
-- phrases: bool, default = False
+- n: int, default = 50. Amount of keywords to extract.
 
-If phrases will be extracted.
+- phrases: bool, default = False. If phrases will be extracted.
 
-- n_phrases: int, default = 20
+- n_phrases: int, default = 20. Amount of key phrases to extract.
 
-Amount of key phrases to extract.
-
-- phrases_by: {'Freq', 'PMI', 'TTEST', 'CHI'}, default = 'PMI'
-
-Strategy to extract key phrases.
+- phrases_by: {'Freq', 'PMI', 'TTEST', 'CHI'}, default = 'PMI'. Strategy to extract key phrases.
 
 ## Usage (Python)
 
 ### Example 1
 
 ```
 import hmrf
@@ -69,31 +59,22 @@
 
 ```
 
 ### Output
 
 ```
 purchase
-
 notch
-
 kept
-
 room
-
 impeccable
-
 hotel
-
 hooked
-
 recommend
-
 spacious
-
 stay
 ```
 
 
 ### Example 2
 
 ```
@@ -120,29 +101,20 @@
 
 ```
 
 ### Output
 
 ```
 healthcare
-
 government
-
 policy
-
 reform
-
 global
-
 generations
-
 income
-
 future
-
 inequality
-
 accessible
 ```
```

### Comparing `hmrf-0.0.1/setup.py` & `hmrf-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hmrf",                     
-    version="0.0.1",                       
+    version="0.1.0",                       
     author="UPV",                    
     description="Package to extract keywords in one of the classes of a dataset",
     long_description=long_description,     
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `hmrf-0.0.1/LICENSE.txt` & `hmrf-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hmrf-0.0.1/README.md` & `hmrf-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 # Harmonic Mean of Relative Frequencies (HMRF)
 
 HMRF is a method for automatic keyword extraction from a text corpus. This method favors words that maximize the difference between their frequency in one class (positive class) and their frequency in the rest of the classes.
 
 ## Parameters
 
-- lang: str, default = 'english'
-
-Language of the texts.
+- lang: str, default = 'english'. Language of the texts.
 
 - positive_class: str or int, default = 1
 
-- n: int, default = 50
-
-Amount of keywords to extract.
-
-- phrases: bool, default = False
+- n: int, default = 50. Amount of keywords to extract.
 
-If phrases will be extracted.
+- phrases: bool, default = False. If phrases will be extracted.
 
-- n_phrases: int, default = 20
+- n_phrases: int, default = 20. Amount of key phrases to extract.
 
-Amount of key phrases to extract.
-
-- phrases_by: {'Freq', 'PMI', 'TTEST', 'CHI'}, default = 'PMI'
-
-Strategy to extract key phrases.
+- phrases_by: {'Freq', 'PMI', 'TTEST', 'CHI'}, default = 'PMI'. Strategy to extract key phrases.
 
 ## Usage (Python)
 
 ### Example 1
 
 ```
 import hmrf
@@ -54,31 +44,22 @@
 
 ```
 
 ### Output
 
 ```
 purchase
-
 notch
-
 kept
-
 room
-
 impeccable
-
 hotel
-
 hooked
-
 recommend
-
 spacious
-
 stay
 ```
 
 
 ### Example 2
 
 ```
@@ -105,27 +86,18 @@
 
 ```
 
 ### Output
 
 ```
 healthcare
-
 government
-
 policy
-
 reform
-
 global
-
 generations
-
 income
-
 future
-
 inequality
-
 accessible
 ```
```

### Comparing `hmrf-0.0.1/hmrf/src/hmrf.egg-info/PKG-INFO` & `hmrf-0.1.0/hmrf/src/hmrf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmrf
-Version: 0.0.1
+Version: 0.1.0
 Summary: Package to extract keywords in one of the classes of a dataset
 Home-page: UNKNOWN
 Author: UPV
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,35 +15,25 @@
 
 # Harmonic Mean of Relative Frequencies (HMRF)
 
 HMRF is a method for automatic keyword extraction from a text corpus. This method favors words that maximize the difference between their frequency in one class (positive class) and their frequency in the rest of the classes.
 
 ## Parameters
 
-- lang: str, default = 'english'
-
-Language of the texts.
+- lang: str, default = 'english'. Language of the texts.
 
 - positive_class: str or int, default = 1
 
-- n: int, default = 50
-
-Amount of keywords to extract.
-
-- phrases: bool, default = False
+- n: int, default = 50. Amount of keywords to extract.
 
-If phrases will be extracted.
+- phrases: bool, default = False. If phrases will be extracted.
 
-- n_phrases: int, default = 20
+- n_phrases: int, default = 20. Amount of key phrases to extract.
 
-Amount of key phrases to extract.
-
-- phrases_by: {'Freq', 'PMI', 'TTEST', 'CHI'}, default = 'PMI'
-
-Strategy to extract key phrases.
+- phrases_by: {'Freq', 'PMI', 'TTEST', 'CHI'}, default = 'PMI'. Strategy to extract key phrases.
 
 ## Usage (Python)
 
 ### Example 1
 
 ```
 import hmrf
@@ -69,31 +59,22 @@
 
 ```
 
 ### Output
 
 ```
 purchase
-
 notch
-
 kept
-
 room
-
 impeccable
-
 hotel
-
 hooked
-
 recommend
-
 spacious
-
 stay
 ```
 
 
 ### Example 2
 
 ```
@@ -120,29 +101,20 @@
 
 ```
 
 ### Output
 
 ```
 healthcare
-
 government
-
 policy
-
 reform
-
 global
-
 generations
-
 income
-
 future
-
 inequality
-
 accessible
 ```
```

### Comparing `hmrf-0.0.1/hmrf/src/hmrf.py` & `hmrf-0.1.0/hmrf/src/hmrf.py`

 * *Files identical despite different names*

