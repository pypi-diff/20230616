# Comparing `tmp/EssaySummarizer-0.0.1.tar.gz` & `tmp/EssaySummarizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EssaySummarizer-0.0.1.tar", last modified: Fri Jun 16 07:27:04 2023, max compression
+gzip compressed data, was "EssaySummarizer-0.0.2.tar", last modified: Fri Jun 16 07:29:11 2023, max compression
```

## Comparing `EssaySummarizer-0.0.1.tar` & `EssaySummarizer-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-16 07:27:04.682867 EssaySummarizer-0.0.1/
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1073 2023-06-07 01:00:16.000000 EssaySummarizer-0.0.1/LICENSE
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1791 2023-06-16 07:27:04.682520 EssaySummarizer-0.0.1/PKG-INFO
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1360 2023-06-16 07:26:05.000000 EssaySummarizer-0.0.1/README.md
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       38 2023-06-16 07:27:04.682990 EssaySummarizer-0.0.1/setup.cfg
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      728 2023-06-16 07:21:04.000000 EssaySummarizer-0.0.1/setup.py
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-16 07:27:04.678737 EssaySummarizer-0.0.1/src/
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-16 07:27:04.681583 EssaySummarizer-0.0.1/src/EssaySummarizer.egg-info/
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1791 2023-06-16 07:27:04.000000 EssaySummarizer-0.0.1/src/EssaySummarizer.egg-info/PKG-INFO
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      263 2023-06-16 07:27:04.000000 EssaySummarizer-0.0.1/src/EssaySummarizer.egg-info/SOURCES.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        1 2023-06-16 07:27:04.000000 EssaySummarizer-0.0.1/src/EssaySummarizer.egg-info/dependency_links.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        5 2023-06-16 07:27:04.000000 EssaySummarizer-0.0.1/src/EssaySummarizer.egg-info/requires.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       16 2023-06-16 07:27:04.000000 EssaySummarizer-0.0.1/src/EssaySummarizer.egg-info/top_level.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1858 2023-06-16 07:22:40.000000 EssaySummarizer-0.0.1/src/EssaySummarizer.py
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-16 07:29:11.008940 EssaySummarizer-0.0.2/
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1073 2023-06-07 01:00:16.000000 EssaySummarizer-0.0.2/LICENSE
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1797 2023-06-16 07:29:11.007722 EssaySummarizer-0.0.2/PKG-INFO
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1366 2023-06-16 07:28:52.000000 EssaySummarizer-0.0.2/README.md
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       38 2023-06-16 07:29:11.009408 EssaySummarizer-0.0.2/setup.cfg
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      728 2023-06-16 07:28:59.000000 EssaySummarizer-0.0.2/setup.py
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-16 07:29:11.002838 EssaySummarizer-0.0.2/src/
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-16 07:29:11.006684 EssaySummarizer-0.0.2/src/EssaySummarizer.egg-info/
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1797 2023-06-16 07:29:10.000000 EssaySummarizer-0.0.2/src/EssaySummarizer.egg-info/PKG-INFO
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      263 2023-06-16 07:29:10.000000 EssaySummarizer-0.0.2/src/EssaySummarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        1 2023-06-16 07:29:10.000000 EssaySummarizer-0.0.2/src/EssaySummarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        5 2023-06-16 07:29:10.000000 EssaySummarizer-0.0.2/src/EssaySummarizer.egg-info/requires.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       16 2023-06-16 07:29:10.000000 EssaySummarizer-0.0.2/src/EssaySummarizer.egg-info/top_level.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1858 2023-06-16 07:22:40.000000 EssaySummarizer-0.0.2/src/EssaySummarizer.py
```

### Comparing `EssaySummarizer-0.0.1/LICENSE` & `EssaySummarizer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EssaySummarizer-0.0.1/PKG-INFO` & `EssaySummarizer-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EssaySummarizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Essay Summarizer.
 Home-page: UNKNOWN
 Author: Ujjwal Reddy K S
 License: UNKNOWN
 Keywords: Essay,Summarizer,nltk
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -32,15 +32,15 @@
 
  ```
 # test.py
 import EssaySummarizer
 
 ## To run
 
-sentence = EssaySummarizer.play_game(essay,num_sentences) # default num_sentences=3
+sentence = EssaySummarizer.summarize_essay(essay,num_sentences) # default num_sentences=3
 
 print(sentence)
 ```
 
 ## Run the following Script.
  ```
   python test.py
```

### Comparing `EssaySummarizer-0.0.1/README.md` & `EssaySummarizer-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
  ```
 # test.py
 import EssaySummarizer
 
 ## To run
 
-sentence = EssaySummarizer.play_game(essay,num_sentences) # default num_sentences=3
+sentence = EssaySummarizer.summarize_essay(essay,num_sentences) # default num_sentences=3
 
 print(sentence)
 ```
 
 ## Run the following Script.
  ```
   python test.py
```

### Comparing `EssaySummarizer-0.0.1/setup.py` & `EssaySummarizer-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EssaySummarizer',
-    version='0.0.1',
+    version='0.0.2',
     description='Essay Summarizer.',
     author= 'Ujjwal Reddy K S',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['Essay', 'Summarizer', 'nltk'],
     classifiers=[
```

### Comparing `EssaySummarizer-0.0.1/src/EssaySummarizer.egg-info/PKG-INFO` & `EssaySummarizer-0.0.2/src/EssaySummarizer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EssaySummarizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Essay Summarizer.
 Home-page: UNKNOWN
 Author: Ujjwal Reddy K S
 License: UNKNOWN
 Keywords: Essay,Summarizer,nltk
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -32,15 +32,15 @@
 
  ```
 # test.py
 import EssaySummarizer
 
 ## To run
 
-sentence = EssaySummarizer.play_game(essay,num_sentences) # default num_sentences=3
+sentence = EssaySummarizer.summarize_essay(essay,num_sentences) # default num_sentences=3
 
 print(sentence)
 ```
 
 ## Run the following Script.
  ```
   python test.py
```

### Comparing `EssaySummarizer-0.0.1/src/EssaySummarizer.py` & `EssaySummarizer-0.0.2/src/EssaySummarizer.py`

 * *Files identical despite different names*

