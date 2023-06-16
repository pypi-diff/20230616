# Comparing `tmp/saa-0.0.1.tar.gz` & `tmp/saa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saa-0.0.1.tar", max compression
+gzip compressed data, was "saa-0.0.2.tar", max compression
```

## Comparing `saa-0.0.1.tar` & `saa-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1079 2023-06-16 12:35:59.730267 saa-0.0.1/LICENSE
--rw-r--r--   0        0        0     3222 2023-06-16 12:35:59.730267 saa-0.0.1/README.md
--rw-r--r--   0        0        0      441 2023-06-16 12:35:59.730267 saa-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-16 12:35:59.730267 saa-0.0.1/saa/__init__.py
--rw-r--r--   0        0        0     1149 2023-06-16 12:35:59.730267 saa-0.0.1/saa/clock.py
--rw-r--r--   0        0        0        0 2023-06-16 12:35:59.730267 saa-0.0.1/saa/core/__init__.py
--rw-r--r--   0        0        0      575 2023-06-16 12:35:59.730267 saa-0.0.1/saa/core/language.py
--rw-r--r--   0        0        0      837 2023-06-16 12:35:59.730267 saa-0.0.1/saa/core/numbers.py
--rw-r--r--   0        0        0      308 2023-06-16 12:35:59.730267 saa-0.0.1/saa/core/plugins.py
--rw-r--r--   0        0        0      620 2023-06-16 12:35:59.730267 saa-0.0.1/saa/core/template.py
--rw-r--r--   0        0        0      775 2023-06-16 12:35:59.730267 saa-0.0.1/saa/core/watch.py
--rw-r--r--   0        0        0     1546 2023-06-16 12:35:59.730267 saa-0.0.1/saa/luga/da/__init__.py
--rw-r--r--   0        0        0     1422 2023-06-16 12:35:59.730267 saa-0.0.1/saa/luga/en/__init__.py
--rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 saa-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-16 14:10:52.143833 saa-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3248 2023-06-16 14:10:52.143833 saa-0.0.2/README.md
+-rw-r--r--   0        0        0      441 2023-06-16 14:10:52.143833 saa-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-16 14:10:52.143833 saa-0.0.2/saa/__init__.py
+-rw-r--r--   0        0        0     1149 2023-06-16 14:10:52.143833 saa-0.0.2/saa/clock.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:10:52.143833 saa-0.0.2/saa/core/__init__.py
+-rw-r--r--   0        0        0      575 2023-06-16 14:10:52.143833 saa-0.0.2/saa/core/language.py
+-rw-r--r--   0        0        0      837 2023-06-16 14:10:52.143833 saa-0.0.2/saa/core/numbers.py
+-rw-r--r--   0        0        0      308 2023-06-16 14:10:52.143833 saa-0.0.2/saa/core/plugins.py
+-rw-r--r--   0        0        0      620 2023-06-16 14:10:52.143833 saa-0.0.2/saa/core/template.py
+-rw-r--r--   0        0        0      775 2023-06-16 14:10:52.143833 saa-0.0.2/saa/core/watch.py
+-rw-r--r--   0        0        0     1534 2023-06-16 14:10:52.143833 saa-0.0.2/saa/luga/da/__init__.py
+-rw-r--r--   0        0        0     1422 2023-06-16 14:10:52.143833 saa-0.0.2/saa/luga/en/__init__.py
+-rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 saa-0.0.2/PKG-INFO
```

### Comparing `saa-0.0.1/LICENSE` & `saa-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saa-0.0.1/README.md` & `saa-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Saa
+> _Making Time Speak!_ 🎙️
 Translating time into human-friendly spoken expressions
 
 ![Saa OpenJourny](watch.png)
 
-**Saa** allows you to effortlessly translate time into human-friendly spoken expressions. The word `saa` means `hour` in Swahili, and this package aims to humanify time expression across languages. It is build using pure Python standard libraries. 
+**Saa** allows you to effortlessly translate time into human-friendly spoken expressions. The word `saa` means `hour` in Swahili, and this package aims to humanify time expression across languages. It is build using pure Python standard libraries.
 
 ```python
 from datetime import time
 from saa import Clock
 
 clock = Clock("en")
 clock("11:15") # 'quarter past eleven'
@@ -40,18 +41,18 @@
 ```python
 from saa import Clock
 
 # Create a Clock instance with the desired language (e.g., "en" for English)
 clock = Clock("en")
 
 # Translate time into a human-friendly spoken expression
-# supports also datetime and time. .e.g. time(hour=11, minute=45) 
-spoken_time = clock("11:45") 
+# supports also datetime and time. .e.g. time(hour=11, minute=45)
+spoken_time = clock("11:45")
 
-print(spoken_time)  
+print(spoken_time)
 # Output: "quarter to twelve"
 ```
 
 ## Supported Languages
 
 **Saa** currently supports the following languages:
```

### Comparing `saa-0.0.1/saa/clock.py` & `saa-0.0.2/saa/clock.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.1/saa/core/language.py` & `saa-0.0.2/saa/core/language.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.1/saa/core/numbers.py` & `saa-0.0.2/saa/core/numbers.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.1/saa/core/template.py` & `saa-0.0.2/saa/core/template.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.1/saa/core/watch.py` & `saa-0.0.2/saa/core/watch.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.1/saa/luga/da/__init__.py` & `saa-0.0.2/saa/luga/da/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,16 +55,15 @@
             minute = 60 - minute
 
         return hour, minute, is_to, is_minutes
 
     @staticmethod
     def post_logic(text):
         text = " ".join(
-            "et" if word == "en" else word.replace("en", "et")
+            word if ("enog" in word or "kken" in word) else word.replace("en", "et")
             for word in text.split()
-            if "enog" not in word
         )
         return text
 
 
 class Language(Danish):
     pass
```

### Comparing `saa-0.0.1/saa/luga/en/__init__.py` & `saa-0.0.2/saa/luga/en/__init__.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.1/PKG-INFO` & `saa-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: saa
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converting time into natural language phrases
 License: MIT
 Author: Prayson W. Daniel
 Author-email: praysonpi@gmail.com
 Requires-Python: >3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Saa
+> _Making Time Speak!_ 🎙️
 Translating time into human-friendly spoken expressions
 
 ![Saa OpenJourny](watch.png)
 
-**Saa** allows you to effortlessly translate time into human-friendly spoken expressions. The word `saa` means `hour` in Swahili, and this package aims to humanify time expression across languages. It is build using pure Python standard libraries. 
+**Saa** allows you to effortlessly translate time into human-friendly spoken expressions. The word `saa` means `hour` in Swahili, and this package aims to humanify time expression across languages. It is build using pure Python standard libraries.
 
 ```python
 from datetime import time
 from saa import Clock
 
 clock = Clock("en")
 clock("11:15") # 'quarter past eleven'
@@ -55,18 +56,18 @@
 ```python
 from saa import Clock
 
 # Create a Clock instance with the desired language (e.g., "en" for English)
 clock = Clock("en")
 
 # Translate time into a human-friendly spoken expression
-# supports also datetime and time. .e.g. time(hour=11, minute=45) 
-spoken_time = clock("11:45") 
+# supports also datetime and time. .e.g. time(hour=11, minute=45)
+spoken_time = clock("11:45")
 
-print(spoken_time)  
+print(spoken_time)
 # Output: "quarter to twelve"
 ```
 
 ## Supported Languages
 
 **Saa** currently supports the following languages:
```

