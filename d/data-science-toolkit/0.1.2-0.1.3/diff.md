# Comparing `tmp/data-science-toolkit-0.1.2.tar.gz` & `tmp/data-science-toolkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-science-toolkit-0.1.2.tar", last modified: Wed Jun 14 15:43:28 2023, max compression
+gzip compressed data, was "data-science-toolkit-0.1.3.tar", last modified: Fri Jun 16 11:02:33 2023, max compression
```

## Comparing `data-science-toolkit-0.1.2.tar` & `data-science-toolkit-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 15:43:28.465578 data-science-toolkit-0.1.2/
--rw-rw-rw-   0        0        0     1096 2021-12-07 14:10:07.000000 data-science-toolkit-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2004 2023-06-14 15:43:28.464581 data-science-toolkit-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2022-11-21 14:02:51.000000 data-science-toolkit-0.1.2/README.md
--rw-rw-rw-   0        0        0      387 2022-03-11 14:47:10.000000 data-science-toolkit-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 15:43:28.465578 data-science-toolkit-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1434 2023-06-14 15:42:44.000000 data-science-toolkit-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:43:28.387786 data-science-toolkit-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 15:43:28.423690 data-science-toolkit-0.1.2/src/data_science_toolkit/
--rw-rw-rw-   0        0        0        0 2022-03-09 14:14:26.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/__init__.py
--rw-rw-rw-   0        0        0    10268 2022-03-09 14:14:26.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/chart.py
--rw-rw-rw-   0        0        0     6375 2022-11-21 14:02:51.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/csm.py
--rw-rw-rw-   0        0        0    76997 2023-06-14 15:42:16.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/dataframe.py
--rw-rw-rw-   0        0        0    12467 2022-11-21 14:02:51.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/gis.py
--rw-rw-rw-   0        0        0     8456 2022-03-09 14:14:26.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/imagefactory.py
--rw-rw-rw-   0        0        0    25115 2023-06-08 11:04:49.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/lib.py
--rw-rw-rw-   0        0        0    28669 2023-06-08 11:04:49.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/model.py
--rw-rw-rw-   0        0        0     7636 2022-11-21 14:02:51.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/r3.py
--rw-rw-rw-   0        0        0     4983 2022-11-21 14:02:51.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/rl.py
--rw-rw-rw-   0        0        0     1445 2022-11-21 14:02:51.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/rl_dqn.py
--rw-rw-rw-   0        0        0     5488 2023-06-08 11:04:49.000000 data-science-toolkit-0.1.2/src/data_science_toolkit/vectorizer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:43:28.461590 data-science-toolkit-0.1.2/src/data_science_toolkit.egg-info/
--rw-rw-rw-   0        0        0     2004 2023-06-14 15:43:28.000000 data-science-toolkit-0.1.2/src/data_science_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      709 2023-06-14 15:43:28.000000 data-science-toolkit-0.1.2/src/data_science_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 15:43:28.000000 data-science-toolkit-0.1.2/src/data_science_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2023-06-14 15:43:28.000000 data-science-toolkit-0.1.2/src/data_science_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 15:43:28.000000 data-science-toolkit-0.1.2/src/data_science_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 15:43:28.462586 data-science-toolkit-0.1.2/test/
--rw-rw-rw-   0        0        0       85 2022-03-09 14:14:26.000000 data-science-toolkit-0.1.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:02:33.077655 data-science-toolkit-0.1.3/
+-rw-rw-rw-   0        0        0     1096 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1963 2023-06-16 11:02:33.076655 data-science-toolkit-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2022-04-14 01:06:21.000000 data-science-toolkit-0.1.3/README.md
+-rw-rw-rw-   0        0        0      387 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 11:02:33.078654 data-science-toolkit-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1434 2023-06-16 10:57:42.000000 data-science-toolkit-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:02:32.878657 data-science-toolkit-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:02:32.962655 data-science-toolkit-0.1.3/src/data_science_toolkit/
+-rw-rw-rw-   0        0        0        0 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/__init__.py
+-rw-rw-rw-   0        0        0    10268 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/chart.py
+-rw-rw-rw-   0        0        0     6375 2022-05-20 00:30:43.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/csm.py
+-rw-rw-rw-   0        0        0    77033 2023-06-16 10:57:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/dataframe.py
+-rw-rw-rw-   0        0        0    12467 2022-05-20 00:36:43.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/gis.py
+-rw-rw-rw-   0        0        0     8456 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/imagefactory.py
+-rw-rw-rw-   0        0        0    25115 2023-05-13 00:40:51.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/lib.py
+-rw-rw-rw-   0        0        0    28669 2023-03-15 23:27:50.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/model.py
+-rw-rw-rw-   0        0        0     7636 2022-05-20 00:33:21.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/r3.py
+-rw-rw-rw-   0        0        0     4983 2021-02-01 01:53:23.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/rl.py
+-rw-rw-rw-   0        0        0     1445 2022-05-19 23:54:12.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/rl_dqn.py
+-rw-rw-rw-   0        0        0     5488 2023-03-15 23:28:40.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/vectorizer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:02:33.060655 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1963 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      709 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:02:33.073655 data-science-toolkit-0.1.3/test/
+-rw-rw-rw-   0        0        0       85 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/test/test.py
```

### Comparing `data-science-toolkit-0.1.2/LICENSE` & `data-science-toolkit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/PKG-INFO` & `data-science-toolkit-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: data-science-toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.
 Home-page: https://github.com/elhachimi-ch/dst
 Author: EL HACHIMI CHOUAIB
 Author-email: elhachimi.ch@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/elhachimi-ch/dst/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -59,9 +57,7 @@
 
 ### Maintainership
 
 We're actively enhacing the repo with new algorithms.
 
 ### How to cite
 
-
-
```

### Comparing `data-science-toolkit-0.1.2/README.md` & `data-science-toolkit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/setup.py` & `data-science-toolkit-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
     
 setuptools.setup(
     name="data-science-toolkit",
-    version="0.1.02",
+    version="0.1.03",
     author="EL HACHIMI CHOUAIB",
     author_email="elhachimi.ch@gmail.com",
     description="Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elhachimi-ch/dst",
     project_urls={
```

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/chart.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/chart.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/csm.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/csm.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/dataframe.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from tensorflow.keras.preprocessing.sequence import TimeseriesGenerator as SG
 from sklearn.datasets import load_iris
 from collections import Counter
 from .chart import Chart
 import numpy as np
 import nltk
 from nltk.tokenize import sent_tokenize, word_tokenize
+from numpy import exp, power, sqrt
 
 
 class DataFrame:
     """
     """
     __vectorizer = None
     __generator = None
```

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/gis.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/gis.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/imagefactory.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/imagefactory.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/lib.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/lib.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/model.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/model.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/r3.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/r3.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/rl.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/rl.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/rl_dqn.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/rl_dqn.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit/vectorizer.py` & `data-science-toolkit-0.1.3/src/data_science_toolkit/vectorizer.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit.egg-info/PKG-INFO` & `data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: data-science-toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.
 Home-page: https://github.com/elhachimi-ch/dst
 Author: EL HACHIMI CHOUAIB
 Author-email: elhachimi.ch@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/elhachimi-ch/dst/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -59,9 +57,7 @@
 
 ### Maintainership
 
 We're actively enhacing the repo with new algorithms.
 
 ### How to cite
 
-
-
```

### Comparing `data-science-toolkit-0.1.2/src/data_science_toolkit.egg-info/SOURCES.txt` & `data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

